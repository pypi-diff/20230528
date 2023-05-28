# Comparing `tmp/jupyter-lsp-2.1.0.tar.gz` & `tmp/jupyter-lsp-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-lsp-2.1.0.tar", last modified: Sun Apr 23 21:22:46 2023, max compression
+gzip compressed data, was "jupyter-lsp-2.2.0.tar", last modified: Sun May 28 13:17:54 2023, max compression
```

## Comparing `jupyter-lsp-2.1.0.tar` & `jupyter-lsp-2.2.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:22:46.203579 jupyter-lsp-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-23 21:22:46.203579 jupyter-lsp-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:22:46.195579 jupyter-lsp-2.1.0/jupyter_lsp/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:22:46.199579 jupyter-lsp-2.1.0/jupyter_lsp/etc/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/etc/jupyter-lsp-jupyter-server.json
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/etc/jupyter-lsp-notebook.json
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10505 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/non_blocking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:22:46.199579 jupyter-lsp-2.1.0/jupyter_lsp/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/schema/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/serverextension.py
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:22:46.199579 jupyter-lsp-2.1.0/jupyter_lsp/specs/
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/bash_language_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:22:46.199579 jupyter-lsp-2.1.0/jupyter_lsp/specs/config/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/config/bash-language-server.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/config/dockerfile-language-server-nodejs.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/config/julia-language-server.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/config/pyls.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/config/pylsp.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    23281 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/config/pyright.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/config/r-languageserver.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/config/sql-language-server.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/config/texlab.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/config/typescript-language-server.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/config/yaml-language-server.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/dockerfile_language_server_nodejs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/javascript_typescript_langserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/jedi_language_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/julia_language_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/pyls.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/pyright.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/python_lsp_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/r_languageserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/sql_language_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/texlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/typescript_language_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/unified_language_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/vscode_css_languageserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/vscode_html_languageserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/vscode_json_languageserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/yaml_language_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/stdio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:22:46.203579 jupyter-lsp-2.1.0/jupyter_lsp/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/tests/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/tests/test_bad_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/tests/test_conf_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/tests/test_detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/tests/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/tests/test_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/tests/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/tests/test_stdio.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/tests/test_virtual_documents_shadow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/trait_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/virtual_documents_shadow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:22:46.199579 jupyter-lsp-2.1.0/jupyter_lsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-23 21:22:46.000000 jupyter-lsp-2.1.0/jupyter_lsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-04-23 21:22:46.000000 jupyter-lsp-2.1.0/jupyter_lsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 21:22:46.000000 jupyter-lsp-2.1.0/jupyter_lsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-23 21:22:46.000000 jupyter-lsp-2.1.0/jupyter_lsp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 21:22:46.000000 jupyter-lsp-2.1.0/jupyter_lsp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-23 21:22:46.000000 jupyter-lsp-2.1.0/jupyter_lsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-23 21:22:46.000000 jupyter-lsp-2.1.0/jupyter_lsp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-23 21:22:46.203579 jupyter-lsp-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:17:54.381026 jupyter-lsp-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-28 13:17:54.381026 jupyter-lsp-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:17:54.373026 jupyter-lsp-2.2.0/jupyter_lsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:17:54.373026 jupyter-lsp-2.2.0/jupyter_lsp/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/etc/jupyter-lsp-jupyter-server.json
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/etc/jupyter-lsp-notebook.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10511 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/non_blocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:17:54.373026 jupyter-lsp-2.2.0/jupyter_lsp/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/schema/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/serverextension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:17:54.377026 jupyter-lsp-2.2.0/jupyter_lsp/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/bash_language_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:17:54.381026 jupyter-lsp-2.2.0/jupyter_lsp/specs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/config/bash-language-server.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/config/dockerfile-language-server-nodejs.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/config/julia-language-server.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/config/pyls.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/config/pylsp.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23281 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/config/pyright.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/config/r-languageserver.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/config/sql-language-server.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/config/texlab.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/config/typescript-language-server.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/config/yaml-language-server.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/dockerfile_language_server_nodejs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/javascript_typescript_langserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/jedi_language_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/julia_language_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/pyls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/pyright.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/python_lsp_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/r_languageserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/sql_language_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/texlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/typescript_language_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/unified_language_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/vscode_css_languageserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/vscode_html_languageserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/vscode_json_languageserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/specs/yaml_language_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/stdio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:17:54.381026 jupyter-lsp-2.2.0/jupyter_lsp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/tests/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/tests/test_bad_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/tests/test_conf_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/tests/test_detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/tests/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/tests/test_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/tests/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/tests/test_stdio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/tests/test_virtual_documents_shadow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/trait_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/jupyter_lsp/virtual_documents_shadow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:17:54.373026 jupyter-lsp-2.2.0/jupyter_lsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-28 13:17:54.000000 jupyter-lsp-2.2.0/jupyter_lsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-05-28 13:17:54.000000 jupyter-lsp-2.2.0/jupyter_lsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 13:17:54.000000 jupyter-lsp-2.2.0/jupyter_lsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-28 13:17:54.000000 jupyter-lsp-2.2.0/jupyter_lsp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 13:17:54.000000 jupyter-lsp-2.2.0/jupyter_lsp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-28 13:17:54.000000 jupyter-lsp-2.2.0/jupyter_lsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-28 13:17:54.000000 jupyter-lsp-2.2.0/jupyter_lsp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-28 13:17:54.385026 jupyter-lsp-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-28 13:14:40.000000 jupyter-lsp-2.2.0/setup.py
```

### Comparing `jupyter-lsp-2.1.0/LICENSE` & `jupyter-lsp-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/PKG-INFO` & `jupyter-lsp-2.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-lsp
-Version: 2.1.0
+Version: 2.2.0
 Summary: Multi-Language Server WebSocket proxy for Jupyter Notebook/Lab server
 Author: jupyter-lsp Contributors
 Author-email: project.jupyter@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/jupyter-lsp/jupyterlab-lsp/issues
 Project-URL: Documentation, https://jupyterlab-lsp.readthedocs.io/
 Project-URL: Source Code, https://github.com/jupyter-lsp/jupyterlab-lsp
```

### Comparing `jupyter-lsp-2.1.0/README.md` & `jupyter-lsp-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/handlers.py` & `jupyter-lsp-2.2.0/jupyter_lsp/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/manager.py` & `jupyter-lsp-2.2.0/jupyter_lsp/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         self.init_language_servers()
         self.init_listeners()
         self.init_sessions()
         self._ready = True
 
     async def ready(self):
         while not self._ready:  # pragma: no cover
-            asyncio.sleep(0.1)
+            await asyncio.sleep(0.1)
         return True
 
     def init_language_servers(self) -> None:
         """determine the final language server configuration."""
         # copy the language servers before anybody monkeys with them
         self._language_servers_from_config = dict(self.language_servers)
         self.language_servers = self._collect_language_servers(only_installed=True)
```

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/non_blocking.py` & `jupyter-lsp-2.2.0/jupyter_lsp/non_blocking.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/paths.py` & `jupyter-lsp-2.2.0/jupyter_lsp/paths.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/schema/__init__.py` & `jupyter-lsp-2.2.0/jupyter_lsp/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/schema/schema.json` & `jupyter-lsp-2.2.0/jupyter_lsp/schema/schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/serverextension.py` & `jupyter-lsp-2.2.0/jupyter_lsp/serverextension.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/session.py` & `jupyter-lsp-2.2.0/jupyter_lsp/session.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/specs/__init__.py` & `jupyter-lsp-2.2.0/jupyter_lsp/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/specs/bash_language_server.py` & `jupyter-lsp-2.2.0/jupyter_lsp/specs/pyright.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from .config import load_config_schema
 from .utils import NodeModuleSpec
 
 
-class BashLanguageServer(NodeModuleSpec):
-    node_module = key = "bash-language-server"
-    script = ["bin", "main.js"]
-    args = ["start"]
-    languages = ["bash", "sh"]
+class PyrightLanguageServer(NodeModuleSpec):
+    node_module = key = "pyright"
+    script = ["langserver.index.js"]
+    args = ["--stdio"]
+    languages = ["python"]
     spec = dict(
         display_name=key,
-        mime_types=["text/x-sh", "application/x-sh"],
+        mime_types=["text/python", "text/x-ipython"],
         urls=dict(
-            home="https://github.com/mads-hartmann/{}".format(key),
-            issues="https://github.com/mads-hartmann/{}/issues".format(key),
+            home="https://github.com/microsoft/pyright",
+            issues="https://github.com/microsoft/pyright/issues",
         ),
         install=dict(
             npm="npm install --save-dev {}".format(key),
             yarn="yarn add --dev {}".format(key),
             jlpm="jlpm add --dev {}".format(key),
         ),
         config_schema=load_config_schema(key),
+        requires_documents_on_disk=False,
     )
```

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/specs/config/dockerfile-language-server-nodejs.schema.json` & `jupyter-lsp-2.2.0/jupyter_lsp/specs/config/dockerfile-language-server-nodejs.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/specs/config/julia-language-server.schema.json` & `jupyter-lsp-2.2.0/jupyter_lsp/specs/config/julia-language-server.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/specs/config/pyls.schema.json` & `jupyter-lsp-2.2.0/jupyter_lsp/specs/config/pyls.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/specs/config/pylsp.schema.json` & `jupyter-lsp-2.2.0/jupyter_lsp/specs/config/pylsp.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/specs/config/pyright.schema.json` & `jupyter-lsp-2.2.0/jupyter_lsp/specs/config/pyright.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/specs/config/r-languageserver.schema.json` & `jupyter-lsp-2.2.0/jupyter_lsp/specs/config/r-languageserver.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/specs/config/sql-language-server.schema.json` & `jupyter-lsp-2.2.0/jupyter_lsp/specs/config/sql-language-server.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/specs/config/texlab.schema.json` & `jupyter-lsp-2.2.0/jupyter_lsp/specs/config/texlab.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/specs/config/typescript-language-server.schema.json` & `jupyter-lsp-2.2.0/jupyter_lsp/specs/config/typescript-language-server.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/specs/config/yaml-language-server.schema.json` & `jupyter-lsp-2.2.0/jupyter_lsp/specs/config/yaml-language-server.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/specs/dockerfile_language_server_nodejs.py` & `jupyter-lsp-2.2.0/jupyter_lsp/specs/dockerfile_language_server_nodejs.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/specs/javascript_typescript_langserver.py` & `jupyter-lsp-2.2.0/jupyter_lsp/specs/javascript_typescript_langserver.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/specs/jedi_language_server.py` & `jupyter-lsp-2.2.0/jupyter_lsp/specs/jedi_language_server.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/specs/julia_language_server.py` & `jupyter-lsp-2.2.0/jupyter_lsp/specs/julia_language_server.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/specs/pyls.py` & `jupyter-lsp-2.2.0/jupyter_lsp/specs/pyls.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/specs/pyright.py` & `jupyter-lsp-2.2.0/jupyter_lsp/specs/unified_language_server.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-from .config import load_config_schema
 from .utils import NodeModuleSpec
 
 
-class PyrightLanguageServer(NodeModuleSpec):
-    node_module = key = "pyright"
-    script = ["langserver.index.js"]
-    args = ["--stdio"]
-    languages = ["python"]
+class UnifiedLanguageServer(NodeModuleSpec):
+    node_module = key = "unified-language-server"
+    script = ["src", "server.js"]
+    args = ["--parser=remark-parse", "--stdio"]
+    languages = ["markdown", "ipythongfm", "gfm"]
     spec = dict(
         display_name=key,
-        mime_types=["text/python", "text/x-ipython"],
+        mime_types=["text/x-gfm", "text/x-ipythongfm", "text/x-markdown"],
         urls=dict(
-            home="https://github.com/microsoft/pyright",
-            issues="https://github.com/microsoft/pyright/issues",
+            home="https://github.com/unifiedjs/{}".format(key),
+            issues="https://github.com/unifiedjs/{}/issues".format(key),
         ),
         install=dict(
             npm="npm install --save-dev {}".format(key),
             yarn="yarn add --dev {}".format(key),
             jlpm="jlpm add --dev {}".format(key),
         ),
-        config_schema=load_config_schema(key),
-        requires_documents_on_disk=False,
     )
```

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/specs/python_lsp_server.py` & `jupyter-lsp-2.2.0/jupyter_lsp/specs/python_lsp_server.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/specs/r_languageserver.py` & `jupyter-lsp-2.2.0/jupyter_lsp/specs/r_languageserver.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/specs/sql_language_server.py` & `jupyter-lsp-2.2.0/jupyter_lsp/specs/sql_language_server.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/specs/texlab.py` & `jupyter-lsp-2.2.0/jupyter_lsp/specs/texlab.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/specs/typescript_language_server.py` & `jupyter-lsp-2.2.0/jupyter_lsp/specs/typescript_language_server.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/specs/utils.py` & `jupyter-lsp-2.2.0/jupyter_lsp/specs/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/specs/vscode_css_languageserver.py` & `jupyter-lsp-2.2.0/jupyter_lsp/specs/vscode_css_languageserver.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/specs/vscode_html_languageserver.py` & `jupyter-lsp-2.2.0/jupyter_lsp/specs/vscode_html_languageserver.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/specs/vscode_json_languageserver.py` & `jupyter-lsp-2.2.0/jupyter_lsp/specs/vscode_json_languageserver.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/specs/yaml_language_server.py` & `jupyter-lsp-2.2.0/jupyter_lsp/specs/yaml_language_server.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/stdio.py` & `jupyter-lsp-2.2.0/jupyter_lsp/stdio.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/tests/conftest.py` & `jupyter-lsp-2.2.0/jupyter_lsp/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/tests/test_detect.py` & `jupyter-lsp-2.2.0/jupyter_lsp/tests/test_detect.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/tests/test_extension.py` & `jupyter-lsp-2.2.0/jupyter_lsp/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/tests/test_listener.py` & `jupyter-lsp-2.2.0/jupyter_lsp/tests/test_listener.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/tests/test_paths.py` & `jupyter-lsp-2.2.0/jupyter_lsp/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/tests/test_session.py` & `jupyter-lsp-2.2.0/jupyter_lsp/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/tests/test_stdio.py` & `jupyter-lsp-2.2.0/jupyter_lsp/tests/test_stdio.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/tests/test_virtual_documents_shadow.py` & `jupyter-lsp-2.2.0/jupyter_lsp/tests/test_virtual_documents_shadow.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+import logging
 from pathlib import Path
 from types import SimpleNamespace
 from typing import List
 
 import pytest
 
+from jupyter_lsp import LanguageServerManager
+
 from ..virtual_documents_shadow import (
     EditableFile,
     ShadowFilesystemError,
     extract_or_none,
     setup_shadow_filesystem,
 )
 
@@ -89,17 +92,24 @@
 @pytest.fixture
 def shadow_path(tmpdir):
     return str(tmpdir.mkdir(".virtual_documents"))
 
 
 @pytest.fixture
 def manager():
-    return SimpleNamespace(
-        language_servers={"python-lsp-server": {"requires_documents_on_disk": True}}
-    )
+    manager = LanguageServerManager()
+    manager.language_servers = {
+        "python-lsp-server": {
+            "requires_documents_on_disk": True,
+            "argv": [],
+            "languages": ["python"],
+            "version": 2,
+        }
+    }
+    return manager
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
     "message_func, content, expected_content",
     [
         [did_open, "content\nof\nopened\nfile", "content\nof\nopened\nfile"],
@@ -194,7 +204,48 @@
     with pytest.raises(ShadowFilesystemError, match=".* is missing contentChanges"):
         await run_shadow(
             {
                 "method": "textDocument/didChange",
                 "params": {"textDocument": {"uri": ok_file_uri}},
             }
         )
+
+
+@pytest.fixture
+def forbidden_shadow_path(tmpdir):
+    path = Path(tmpdir) / "no_permission_dir"
+    path.mkdir()
+    path.chmod(0o000)
+
+    yield path
+
+    # re-adjust the permissions, see https://github.com/pytest-dev/pytest/issues/7821
+    path.chmod(0o755)
+
+
+@pytest.mark.asyncio
+async def test_io_failure(forbidden_shadow_path, manager, caplog):
+    file_uri = (forbidden_shadow_path / "test.py").as_uri()
+
+    shadow = setup_shadow_filesystem(forbidden_shadow_path.as_uri())
+
+    def send_change():
+        message = did_open(file_uri, "content")
+        return shadow("client", message, "python-lsp-server", manager)
+
+    with caplog.at_level(logging.WARNING):
+        assert await send_change() is None
+        assert await send_change() is None
+    # no message should be emitted during the first two attempts
+    assert caplog.text == ""
+
+    # a wargning should be emitted on third failure
+    with caplog.at_level(logging.WARNING):
+        assert await send_change() is None
+    assert "initialization of shadow filesystem failed three times" in caplog.text
+    assert "PermissionError" in caplog.text
+    caplog.clear()
+
+    # no message should be emitted in subsequent attempts
+    with caplog.at_level(logging.WARNING):
+        assert await send_change() is None
+    assert caplog.text == ""
```

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/trait_types.py` & `jupyter-lsp-2.2.0/jupyter_lsp/trait_types.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/types.py` & `jupyter-lsp-2.2.0/jupyter_lsp/types.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp/virtual_documents_shadow.py` & `jupyter-lsp-2.2.0/jupyter_lsp/virtual_documents_shadow.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # flake8: noqa: W503
 from concurrent.futures import ThreadPoolExecutor
 from pathlib import Path
 from shutil import rmtree
+from typing import List
 
 from tornado.concurrent import run_on_executor
 from tornado.gen import convert_yielded
 
 from .manager import lsp_message_listener
 from .paths import file_uri_to_path
 from .types import LanguageServerManagerAPI
@@ -107,14 +108,16 @@
     if not virtual_documents_uri.startswith("file:/"):
         raise ShadowFilesystemError(  # pragma: no cover
             'Virtual documents URI has to start with "file:/", got '
             + virtual_documents_uri
         )
 
     initialized = False
+    failures: List[Exception] = []
+
     shadow_filesystem = Path(file_uri_to_path(virtual_documents_uri))
 
     @lsp_message_listener("client")
     async def shadow_virtual_documents(scope, message, language_server, manager):
         """Intercept a message with document contents creating a shadow file for it.
 
         Only create the shadow file if the URI matches the virtual documents URI.
@@ -141,20 +144,35 @@
             raise ShadowFilesystemError("Could not get URI from: {}".format(message))
 
         if not uri.startswith(virtual_documents_uri):
             return
 
         # initialization (/any file system operations) delayed until needed
         if not initialized:
-            # create if does no exist (so that removal does not raise)
-            shadow_filesystem.mkdir(parents=True, exist_ok=True)
-            # remove with contents
-            rmtree(str(shadow_filesystem))
-            # create again
-            shadow_filesystem.mkdir(parents=True, exist_ok=True)
+            if len(failures) == 3:
+                return
+            try:
+                # create if does no exist (so that removal does not raise)
+                shadow_filesystem.mkdir(parents=True, exist_ok=True)
+                # remove with contents
+                rmtree(str(shadow_filesystem))
+                # create again
+                shadow_filesystem.mkdir(parents=True, exist_ok=True)
+            except (OSError, PermissionError, FileNotFoundError) as e:
+                failures.append(e)
+                if len(failures) == 3:
+                    manager.log.warn(
+                        "[lsp] initialization of shadow filesystem failed three times"
+                        " check if the path set by `LanguageServerManager.virtual_documents_dir`"
+                        " or `JP_LSP_VIRTUAL_DIR` is correct; if this is happening with a server"
+                        " for which which you control (or wish to override) jupyter-lsp specification"
+                        " you can try switching `requires_documents_on_disk` off. The errors were: %s",
+                        failures,
+                    )
+                return
             initialized = True
 
         path = file_uri_to_path(uri)
         editable_file = EditableFile(path)
 
         await editable_file.read()
```

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp.egg-info/PKG-INFO` & `jupyter-lsp-2.2.0/jupyter_lsp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-lsp
-Version: 2.1.0
+Version: 2.2.0
 Summary: Multi-Language Server WebSocket proxy for Jupyter Notebook/Lab server
 Author: jupyter-lsp Contributors
 Author-email: project.jupyter@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/jupyter-lsp/jupyterlab-lsp/issues
 Project-URL: Documentation, https://jupyterlab-lsp.readthedocs.io/
 Project-URL: Source Code, https://github.com/jupyter-lsp/jupyterlab-lsp
```

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp.egg-info/SOURCES.txt` & `jupyter-lsp-2.2.0/jupyter_lsp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/jupyter_lsp.egg-info/entry_points.txt` & `jupyter-lsp-2.2.0/jupyter_lsp.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/setup.cfg` & `jupyter-lsp-2.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.1.0/setup.py` & `jupyter-lsp-2.2.0/setup.py`

 * *Files identical despite different names*

