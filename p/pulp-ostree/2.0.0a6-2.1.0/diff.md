# Comparing `tmp/pulp-ostree-2.0.0a6.tar.gz` & `tmp/pulp-ostree-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-ostree-2.0.0a6.tar", last modified: Fri Jun 24 16:40:14 2022, max compression
+gzip compressed data, was "pulp-ostree-2.1.0.tar", last modified: Sun May 28 21:25:08 2023, max compression
```

## Comparing `pulp-ostree-2.0.0a6.tar` & `pulp-ostree-2.1.0.tar`

### file list

```diff
@@ -1,64 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 16:40:14.424278 pulp-ostree-2.0.0a6/
--rw-r--r--   0 runner    (1001) docker     (121)     2629 2022-06-24 16:40:11.000000 pulp-ostree-2.0.0a6/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2095 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/COMMITMENT
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (121)    18046 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1137 2022-06-24 16:40:14.424278 pulp-ostree-2.0.0a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/functest_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 16:40:14.420278 pulp-ostree-2.0.0a6/pulp_ostree/
--rwxr-xr-x   0 runner    (1001) docker     (121)       65 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 16:40:14.420278 pulp-ostree-2.0.0a6/pulp_ostree/app/
--rwxr-xr-x   0 runner    (1001) docker     (121)      264 2022-06-24 16:40:13.000000 pulp-ostree-2.0.0a6/pulp_ostree/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 16:40:14.424278 pulp-ostree-2.0.0a6/pulp_ostree/app/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     5718 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     1929 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/app/migrations/0002_add_relative_path_uniqueness.py
--rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/app/migrations/0003_create_many_to_many_objs_commits.py
--rw-r--r--   0 runner    (1001) docker     (121)      787 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/app/migrations/0004_add_include_exclude_refs.py
--rwxr-xr-x   0 runner    (1001) docker     (121)        1 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/app/migrations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4322 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/app/models.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11247 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/app/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 16:40:14.424278 pulp-ostree-2.0.0a6/pulp_ostree/app/tasks/
--rwxr-xr-x   0 runner    (1001) docker     (121)      174 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/app/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10868 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/app/tasks/importing.py
--rw-r--r--   0 runner    (1001) docker     (121)     4942 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/app/tasks/modifying.py
--rw-r--r--   0 runner    (1001) docker     (121)     5462 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/app/tasks/stages.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10984 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/app/tasks/synchronizing.py
--rw-r--r--   0 runner    (1001) docker     (121)      956 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/app/tasks/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10267 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/app/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 16:40:14.424278 pulp-ostree-2.0.0a6/pulp_ostree/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 16:40:14.424278 pulp-ostree-2.0.0a6/pulp_ostree/tests/functional/
--rwxr-xr-x   0 runner    (1001) docker     (121)       31 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/tests/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 16:40:14.424278 pulp-ostree-2.0.0a6/pulp_ostree/tests/functional/api/
--rwxr-xr-x   0 runner    (1001) docker     (121)       64 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/tests/functional/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3847 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/tests/functional/api/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)    11726 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/tests/functional/api/test_import.py
--rw-r--r--   0 runner    (1001) docker     (121)    11729 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/tests/functional/api/test_modify.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6350 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/tests/functional/api/test_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1118 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/tests/functional/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3196 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/tests/functional/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 16:40:14.424278 pulp-ostree-2.0.0a6/pulp_ostree/tests/performance/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/tests/performance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 16:40:14.424278 pulp-ostree-2.0.0a6/pulp_ostree/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/tests/unit/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      229 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/tests/unit/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 16:40:14.424278 pulp-ostree-2.0.0a6/pulp_ostree/tests/upgrade/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/tests/upgrade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 16:40:14.424278 pulp-ostree-2.0.0a6/pulp_ostree/tests/upgrade/post/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/tests/upgrade/post/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 16:40:14.424278 pulp-ostree-2.0.0a6/pulp_ostree/tests/upgrade/pre/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pulp_ostree/tests/upgrade/pre/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 16:40:14.420278 pulp-ostree-2.0.0a6/pulp_ostree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1137 2022-06-24 16:40:14.000000 pulp-ostree-2.0.0a6/pulp_ostree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1608 2022-06-24 16:40:14.000000 pulp-ostree-2.0.0a6/pulp_ostree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-24 16:40:14.000000 pulp-ostree-2.0.0a6/pulp_ostree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-06-24 16:40:14.000000 pulp-ostree-2.0.0a6/pulp_ostree.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-06-24 16:40:14.000000 pulp-ostree-2.0.0a6/pulp_ostree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-06-24 16:40:14.000000 pulp-ostree-2.0.0a6/pulp_ostree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1506 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-24 16:40:14.424278 pulp-ostree-2.0.0a6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1210 2022-06-24 16:40:13.000000 pulp-ostree-2.0.0a6/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-06-24 16:40:03.000000 pulp-ostree-2.0.0a6/unittest_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:08.679677 pulp-ostree-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-05-28 21:25:05.000000 pulp-ostree-2.1.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/COMMITMENT
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-28 21:25:08.675676 pulp-ostree-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/functest_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:08.675676 pulp-ostree-2.1.0/pulp_ostree/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       65 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:08.675676 pulp-ostree-2.1.0/pulp_ostree/app/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      262 2023-05-28 21:25:07.000000 pulp-ostree-2.1.0/pulp_ostree/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:08.675676 pulp-ostree-2.1.0/pulp_ostree/app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/migrations/0002_add_relative_path_uniqueness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/migrations/0003_create_many_to_many_objs_commits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/migrations/0004_add_include_exclude_refs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/migrations/0005_add_static_delta_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/migrations/0006_alter_pointers_to_related_models_globally.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        1 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/migrations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4963 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7109 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:08.675676 pulp-ostree-2.1.0/pulp_ostree/app/tasks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      174 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13911 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/tasks/importing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/tasks/modifying.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/tasks/stages.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11608 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/tasks/synchronizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/tasks/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9455 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:08.675676 pulp-ostree-2.1.0/pulp_ostree/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:08.675676 pulp-ostree-2.1.0/pulp_ostree/tests/functional/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       31 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:08.675676 pulp-ostree-2.1.0/pulp_ostree/tests/functional/api/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       64 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/functional/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/functional/api/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13257 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/functional/api/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/functional/api/test_modify.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6565 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/functional/api/test_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1118 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/functional/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3196 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/functional/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:08.675676 pulp-ostree-2.1.0/pulp_ostree/tests/performance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/performance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:08.675676 pulp-ostree-2.1.0/pulp_ostree/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/unit/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      229 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/unit/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:08.675676 pulp-ostree-2.1.0/pulp_ostree/tests/upgrade/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/upgrade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:08.675676 pulp-ostree-2.1.0/pulp_ostree/tests/upgrade/post/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/upgrade/post/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:08.675676 pulp-ostree-2.1.0/pulp_ostree/tests/upgrade/pre/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/upgrade/pre/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:08.675676 pulp-ostree-2.1.0/pulp_ostree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-28 21:25:08.000000 pulp-ostree-2.1.0/pulp_ostree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-28 21:25:08.000000 pulp-ostree-2.1.0/pulp_ostree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 21:25:08.000000 pulp-ostree-2.1.0/pulp_ostree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-28 21:25:08.000000 pulp-ostree-2.1.0/pulp_ostree.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-28 21:25:08.000000 pulp-ostree-2.1.0/pulp_ostree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-28 21:25:08.000000 pulp-ostree-2.1.0/pulp_ostree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 21:25:08.679677 pulp-ostree-2.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1220 2023-05-28 21:25:07.000000 pulp-ostree-2.1.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/unittest_requirements.txt
```

### Comparing `pulp-ostree-2.0.0a6/CHANGES.rst` & `pulp-ostree-2.1.0/CHANGES.rst`

 * *Files 27% similar despite different names*

```diff
@@ -7,14 +7,56 @@
     file is managed by towncrier. You *may* edit previous change logs to
     fix problems like typo corrections or such.
 
     WARNING: Don't drop the next directive!
 
 .. towncrier release notes start
 
+2.1.0 (2023-05-28)
+==================
+
+Features
+--------
+
+- Made the plugin compatible with Django 4.2 and pulpcore 3.25.
+  `#258 <https://github.com/pulp/pulp_ostree/issues/258>`_
+
+
+Bugfixes
+--------
+
+- Fixed the path resolution when a user specifies absolute paths when importing repositories.
+  `#226 <https://github.com/pulp/pulp_ostree/issues/226>`_
+- Fixed a bug that disallowed users to pull re-synced content locally.
+  `#257 <https://github.com/pulp/pulp_ostree/issues/257>`_
+- Fixed a bug which prevented users from assigning remotes to repositories in advance.
+  `#262 <https://github.com/pulp/pulp_ostree/issues/262>`_
+
+
+----
+
+
+2.0.0 (2023-03-30)
+==================
+
+Features
+--------
+
+- Added support for third-party storage backends (i.e., S3, Azure).
+  `#172 <https://github.com/pulp/pulp_ostree/issues/172>`_
+- Added support for static deltas. The static deltas are automatically computed for synced and
+  imported repositories. This behaviour is enabled by default. Set ``compute_delta`` to ``False``
+  in a corresponding repository if there is no need to compute the static deltas between the last
+  two commits.
+  `#230 <https://github.com/pulp/pulp_ostree/issues/230>`_
+
+
+----
+
+
 2.0.0a6 (2022-06-24)
 ====================
 
 Features
 --------
 
 - Added support for filtering refs during synchronization. Users can now use the flags
```

### Comparing `pulp-ostree-2.0.0a6/COMMITMENT` & `pulp-ostree-2.1.0/COMMITMENT`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.0.0a6/COPYRIGHT` & `pulp-ostree-2.1.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.0.0a6/LICENSE` & `pulp-ostree-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.0.0a6/PKG-INFO` & `pulp-ostree-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-ostree
-Version: 2.0.0a6
+Version: 2.1.0
 Summary: OSTree plugin for the Pulp Project
 Home-page: http://www.pulpproject.org
 Author: Pulp Project Developers
 Author-email: pulp-list@redhat.com
 License: GPLv2+
 Description: ![Nightly CI/CD](https://github.com/pulp/pulp_ostree/actions/workflows/nightly.yml/badge.svg?branch=main)
         
@@ -14,15 +14,15 @@
         A Pulp plugin to support hosting your own OSTree content.
         
         For more information, please see the [documentation](https://docs.pulpproject.org/pulp_ostree/) or the [Pulp project page](https://pulpproject.org/).
         
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulp-ostree-2.0.0a6/pulp_ostree/app/migrations/0001_initial.py` & `pulp-ostree-2.1.0/pulp_ostree/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.0.0a6/pulp_ostree/app/migrations/0002_add_relative_path_uniqueness.py` & `pulp-ostree-2.1.0/pulp_ostree/app/migrations/0002_add_relative_path_uniqueness.py`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.0.0a6/pulp_ostree/app/migrations/0003_create_many_to_many_objs_commits.py` & `pulp-ostree-2.1.0/pulp_ostree/app/migrations/0003_create_many_to_many_objs_commits.py`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.0.0a6/pulp_ostree/app/migrations/0004_add_include_exclude_refs.py` & `pulp-ostree-2.1.0/pulp_ostree/app/migrations/0004_add_include_exclude_refs.py`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.0.0a6/pulp_ostree/app/models.py` & `pulp-ostree-2.1.0/pulp_ostree/app/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -78,31 +78,46 @@
     commit = models.ForeignKey(OstreeCommit, related_name="object_commit", on_delete=models.CASCADE)
     obj = models.ForeignKey(OstreeObject, related_name="commit_object", on_delete=models.CASCADE)
 
     class Meta:
         unique_together = [["commit", "obj"]]
 
 
+class OstreeContent(Content):
+    """Any type of content/object that is currently not tracked by separate means."""
+
+    repo_key_fields = ("relative_path",)
+
+    relative_path = models.TextField(null=False)
+    digest = models.CharField(max_length=64, null=False)
+
+    class Meta:
+        default_related_name = "%(app_label)s_%(model_name)s"
+        unique_together = ("relative_path", "digest")
+
+
 class OstreeConfig(Content):
     """A content model for an OSTree repository configuration file."""
 
     TYPE = "config"
+    repo_key_fields = ("relative_path",)
 
     sha256 = models.CharField(max_length=64, db_index=True)
     relative_path = models.TextField(null=False)
 
     class Meta:
         default_related_name = "%(app_label)s_%(model_name)s"
         unique_together = [["sha256", "relative_path"]]
 
 
 class OstreeSummary(Content):
     """A content model for an OSTree summary file."""
 
     TYPE = "summary"
+    repo_key_fields = ("relative_path",)
 
     sha256 = models.CharField(max_length=64, db_index=True)
     relative_path = models.TextField(null=False)
 
     class Meta:
         default_related_name = "%(app_label)s_%(model_name)s"
         unique_together = [["sha256", "relative_path"]]
@@ -122,15 +137,25 @@
 
 
 class OstreeRepository(Repository):
     """A repository model for OSTree content."""
 
     TYPE = "ostree"
 
-    CONTENT_TYPES = [OstreeCommit, OstreeRef, OstreeObject, OstreeConfig, OstreeSummary]
+    CONTENT_TYPES = [
+        OstreeCommit,
+        OstreeRef,
+        OstreeObject,
+        OstreeConfig,
+        OstreeSummary,
+        OstreeContent,
+    ]
+    REMOTE_TYPES = [OstreeRemote]
+
+    compute_delta = models.BooleanField(default=True)
 
     class Meta:
         default_related_name = "%(app_label)s_%(model_name)s"
 
     def finalize_new_version(self, new_version):
         """Handle repository duplicates."""
         remove_duplicates(new_version)
```

### Comparing `pulp-ostree-2.0.0a6/pulp_ostree/app/serializers.py` & `pulp-ostree-2.1.0/pulp_ostree/app/viewsets.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,326 +1,263 @@
 from gettext import gettext as _
-from tarfile import is_tarfile
 
-from django.urls import resolve
-from rest_framework import serializers
-from rest_framework_nested.relations import (
-    NestedHyperlinkedIdentityField,
-    NestedHyperlinkedRelatedField,
+from django_filters.filters import CharFilter
+from drf_spectacular.utils import extend_schema
+from rest_framework.decorators import action
+from rest_framework.serializers import ValidationError
+
+from pulpcore.plugin.viewsets import ReadOnlyContentViewSet, ContentFilter, NAME_FILTER_OPTIONS
+from pulpcore.plugin import viewsets as core
+from pulpcore.plugin.models import RepositoryVersion
+from pulpcore.plugin.actions import ModifyRepositoryActionMixin
+from pulpcore.plugin.serializers import (
+    AsyncOperationResponseSerializer,
+    RepositoryAddRemoveContentSerializer,
+    RepositorySyncURLSerializer,
 )
-from rest_framework.utils.field_mapping import get_nested_relation_kwargs
+from pulpcore.plugin.tasking import dispatch
 
-from pulpcore.plugin import serializers as platform
-from pulpcore.plugin.models import Artifact, Remote, RepositoryVersion
-from pulpcore.plugin.viewsets import NamedModelViewSet
+from . import models, serializers, tasks
 
-from . import models
 
+class OstreeRemoteViewSet(core.RemoteViewSet):
+    """A ViewSet class for OSTree remote repositories."""
 
-class OstreeImportAllSerializer(serializers.Serializer):
-    """A Serializer class for importing all refs and commits to a repository."""
+    endpoint_name = "ostree"
+    queryset = models.OstreeRemote.objects.all()
+    serializer_class = serializers.OstreeRemoteSerializer
 
-    artifact = platform.RelatedField(
-        many=False,
-        lookup_field="pk",
-        view_name="artifacts-detail",
-        queryset=Artifact.objects.all(),
-        help_text=_("An artifact representing OSTree content compressed as a tarball."),
-    )
-    repository_name = serializers.CharField(
-        help_text=_("The name of a repository that contains the compressed OSTree content.")
-    )
-
-    def validate(self, data):
-        """Validate the passed tarball and optional ref attributes."""
-        new_data = {}
-        new_data.update(self.initial_data)
-
-        self.validate_tarball(new_data)
-
-        return new_data
-
-    def validate_tarball(self, data):
-        """Check if the artifact is a tarball."""
-        artifact = NamedModelViewSet.get_resource(data["artifact"])
-        if not is_tarfile(artifact.file.path):
-            raise serializers.ValidationError(_("The artifact is not a tar archive file"))
-        data["artifact"] = artifact
 
+class OstreeRepositoryViewSet(core.RepositoryViewSet, ModifyRepositoryActionMixin):
+    """A ViewSet class for OSTree repositories."""
 
-class OstreeImportCommitsToRefSerializer(OstreeImportAllSerializer):
-    """A Serializer class for appending child commits to a repository."""
+    endpoint_name = "ostree"
+    queryset = models.OstreeRepository.objects.all()
+    serializer_class = serializers.OstreeRepositorySerializer
 
-    ref = serializers.CharField(
-        help_text=_("The name of a ref branch that holds the reference to the last commit."),
+    @extend_schema(
+        description="Trigger an asynchronous task to sync content.",
+        summary="Sync from remote",
+        responses={202: AsyncOperationResponseSerializer},
     )
+    @action(detail=True, methods=["post"], serializer_class=RepositorySyncURLSerializer)
+    def sync(self, request, pk):
+        """Dispatch a sync task."""
+        repository = self.get_object()
+        serializer = RepositorySyncURLSerializer(
+            data=request.data, context={"request": request, "repository_pk": pk}
+        )
+        serializer.is_valid(raise_exception=True)
+        remote = serializer.validated_data.get("remote", repository.remote)
+        mirror = serializer.validated_data.get("mirror")
+
+        result = dispatch(
+            tasks.synchronize,
+            shared_resources=[remote],
+            exclusive_resources=[repository],
+            kwargs={
+                "remote_pk": str(remote.pk),
+                "repository_pk": str(repository.pk),
+                "mirror": mirror,
+            },
+        )
+        return core.OperationPostponedResponse(result, request)
 
+    @extend_schema(
+        description="Trigger an asynchronous task to import all refs and commits to a repository.",
+        summary="Import refs and commits to a repository",
+        responses={202: AsyncOperationResponseSerializer},
+    )
+    @action(detail=True, methods=["post"], serializer_class=serializers.OstreeImportAllSerializer)
+    def import_all(self, request, pk):
+        """Import all refs and commits to a repository."""
+        repository = self.get_object()
 
-class OstreeCommitSerializer(platform.SingleArtifactContentSerializer):
-    """A Serializer class for OSTree commits."""
+        serializer = serializers.OstreeImportAllSerializer(
+            data=request.data, context={"request": request}
+        )
+        serializer.is_valid(raise_exception=True)
 
-    parent_commit = platform.DetailRelatedField(
-        many=False,
-        view_name="ostree-commits-detail",
-        queryset=models.OstreeCommit.objects.all(),
-        allow_null=True,
-        default=None,
-    )
-    checksum = serializers.CharField()
-    objs = platform.DetailRelatedField(
-        many=True,
-        view_name="ostree-objects-detail",
-        queryset=models.OstreeObject.objects.all(),
-    )
+        artifact = serializer.validated_data["artifact"]
+        repository_name = serializer.validated_data["repository_name"]
 
-    class Meta:
-        fields = platform.SingleArtifactContentSerializer.Meta.fields + (
-            "parent_commit",
-            "checksum",
-            "objs",
+        async_result = dispatch(
+            tasks.import_all_refs_and_commits,
+            exclusive_resources=[artifact, repository],
+            kwargs={
+                "artifact_pk": str(artifact.pk),
+                "repository_pk": str(repository.pk),
+                "repository_name": repository_name,
+            },
         )
-        model = models.OstreeCommit
+        return core.OperationPostponedResponse(async_result, request)
 
+    @extend_schema(
+        description="Trigger an asynchronous task to append child commits to a repository.",
+        summary="Append child commits to a repository",
+        responses={202: AsyncOperationResponseSerializer},
+    )
+    @action(
+        detail=True,
+        methods=["post"],
+        serializer_class=serializers.OstreeImportCommitsToRefSerializer,
+    )
+    def import_commits(self, request, pk):
+        """Append child commits to a repository."""
+        repository = self.get_object()
 
-class OstreeRefSerializer(platform.SingleArtifactContentSerializer):
-    """A Serializer class for OSTree head commits."""
+        serializer = serializers.OstreeImportCommitsToRefSerializer(
+            data=request.data, context={"request": request}
+        )
+        serializer.is_valid(raise_exception=True)
 
-    commit = platform.DetailRelatedField(
-        many=False,
-        view_name="ostree-commits-detail",
-        queryset=models.OstreeCommit.objects.all(),
-    )
-    name = serializers.CharField()
-    checksum = serializers.CharField(source="commit.checksum", read_only=True)
+        artifact = serializer.validated_data["artifact"]
+        repository_name = serializer.validated_data["repository_name"]
+        ref = serializer.validated_data["ref"]
+
+        async_result = dispatch(
+            tasks.import_child_commits,
+            exclusive_resources=[artifact, repository],
+            kwargs={
+                "artifact_pk": str(artifact.pk),
+                "repository_pk": str(repository.pk),
+                "repository_name": repository_name,
+                "ref": ref,
+            },
+        )
+        return core.OperationPostponedResponse(async_result, request)
 
-    class Meta:
-        fields = platform.SingleArtifactContentSerializer.Meta.fields + (
-            "commit",
-            "checksum",
-            "name",
+    @extend_schema(
+        description="Trigger an asynchronous task to modify content.",
+        summary="Modify repository",
+        responses={202: AsyncOperationResponseSerializer},
+    )
+    @action(
+        detail=True,
+        methods=["post"],
+        serializer_class=RepositoryAddRemoveContentSerializer,
+    )
+    def modify(self, request, pk):
+        """Queues a task that adds and remove content units within a repository."""
+        repository = self.get_object()
+        serializer = self.get_serializer(data=request.data, context={"request": request})
+        serializer.is_valid(raise_exception=True)
+
+        if "base_version" in request.data:
+            base_version_pk = self.get_resource(request.data["base_version"], RepositoryVersion).pk
+        else:
+            base_version_pk = None
+
+        task = dispatch(
+            tasks.modify_content,
+            exclusive_resources=[repository],
+            kwargs={
+                "repository_pk": pk,
+                "base_version_pk": base_version_pk,
+                "add_content_units": serializer.validated_data.get("add_content_units", []),
+                "remove_content_units": serializer.validated_data.get("remove_content_units", []),
+            },
         )
-        model = models.OstreeRef
+        return core.OperationPostponedResponse(task, request)
 
+    def verify_content_units(self, content_units, all_content_units):
+        """Verify referenced content units."""
+        existing_content_units_pks = content_units.values_list("pk", flat=True)
+        existing_content_units_pks = {str(pk) for pk in existing_content_units_pks}
 
-class OstreeObjectSerializer(platform.SingleArtifactContentSerializer):
-    """A Serializer class for OSTree objects (e.g., dirtree, dirmeta, file)."""
+        missing_pks = set(all_content_units.keys()) - existing_content_units_pks
+        if missing_pks:
+            missing_hrefs = [all_content_units[pk] for pk in missing_pks]
+            raise ValidationError(
+                _("Could not find the following content units: {}").format(missing_hrefs)
+            )
 
-    typ = serializers.IntegerField(
-        help_text=_(
-            """
-            The type of an object. All values are described by the mapping declared at
-            https://lazka.github.io/pgi-docs/OSTree-1.0/enums.html#OSTree.ObjectType
-            """
-        ),
-    )
-    checksum = serializers.CharField()
 
-    class Meta:
-        fields = platform.SingleArtifactContentSerializer.Meta.fields + (
-            "checksum",
-            "typ",
-        )
-        model = models.OstreeObject
+class OstreeRepositoryVersionViewSet(core.RepositoryVersionViewSet):
+    """A ViewSet class that represents a single OSTree repository version."""
 
+    parent_viewset = OstreeRepositoryViewSet
 
-class OstreeConfigSerializer(platform.SingleArtifactContentSerializer):
-    """A Serializer class for OSTree repository configuration files."""
 
-    class Meta:
-        fields = platform.SingleArtifactContentSerializer.Meta.fields
-        model = models.OstreeConfig
+class OstreeDistributionViewSet(core.DistributionViewSet):
+    """A ViewSet class for OSTree distributions."""
 
+    endpoint_name = "ostree"
+    queryset = models.OstreeDistribution.objects.all()
+    serializer_class = serializers.OstreeDistributionSerializer
 
-class OstreeSummarySerializer(platform.SingleArtifactContentSerializer):
-    """A Serializer class for an OSTree summary file."""
 
-    class Meta:
-        fields = platform.SingleArtifactContentSerializer.Meta.fields
-        model = models.OstreeSummary
+class OstreeRefFilter(ContentFilter):
+    """A filterset class for refs."""
 
+    checksum = CharFilter(field_name="commit__checksum")
 
-class OstreeRemoteSerializer(platform.RemoteSerializer):
-    """A Serializer class for a remote OSTree repository."""
+    class Meta:
+        model = models.OstreeRef
+        fields = {"name": NAME_FILTER_OPTIONS}
 
-    depth = serializers.IntegerField(
-        default=0,
-        min_value=0,
-        required=False,
-        help_text=_("An option to specify how many commits to traverse."),
-    )
-    policy = serializers.ChoiceField(
-        help_text="""
-        immediate - All OSTree objects are downloaded and saved during synchronization.
-        on_demand - Only commits, dirtrees, and refs are downloaded. Other OSTree objects are
-                    not downloaded until they are requested for the first time by a client.
-        """,
-        choices=[Remote.IMMEDIATE, Remote.ON_DEMAND],
-        default=Remote.IMMEDIATE,
-    )
-    include_refs = serializers.ListField(
-        child=serializers.CharField(max_length=255),
-        allow_null=True,
-        required=False,
-        help_text=_(
-            """
-            A list of refs to include during a sync.
-            The wildcards *, ? are recognized.
-            'include_refs' is evaluated before 'exclude_refs'.
-            """
-        ),
-    )
-    exclude_refs = serializers.ListField(
-        child=serializers.CharField(max_length=255),
-        allow_null=True,
-        required=False,
-        help_text=_(
-            """
-            A list of tags to exclude during a sync.
-            The wildcards *, ? are recognized.
-            'exclude_refs' is evaluated after 'include_refs'.
-            """
-        ),
-    )
 
-    class Meta:
-        fields = platform.RemoteSerializer.Meta.fields + ("depth", "include_refs", "exclude_refs")
-        model = models.OstreeRemote
+class OstreeRefViewSet(ReadOnlyContentViewSet):
+    """A ViewSet class for OSTree head commits."""
 
+    endpoint_name = "refs"
+    queryset = models.OstreeRef.objects.all()
+    serializer_class = serializers.OstreeRefSerializer
+    filterset_class = OstreeRefFilter
 
-class OstreeRepositorySerializer(platform.RepositorySerializer):
-    """A Serializer class for an OSTree repository."""
 
-    class Meta:
-        fields = platform.RepositorySerializer.Meta.fields
-        model = models.OstreeRepository
+class OstreeCommitFilter(ContentFilter):
+    """A filterset class for commits."""
 
+    class Meta:
+        model = models.OstreeCommit
+        fields = {"checksum": ["exact"]}
 
-class NestedHyperlinkedModelSerializer(serializers.HyperlinkedModelSerializer):
-    """
-    A type of `ModelSerializer` that uses hyperlinked relationships with compound keys instead
-    of primary key relationships.  Specifically:
 
-    * A 'url' field is included instead of the 'id' field.
-    * Relationships to other instances are hyperlinks, instead of primary keys.
+class OstreeCommitViewSet(ReadOnlyContentViewSet):
+    """A ViewSet class for OSTree commits."""
 
-    NOTE: this only works with DRF 3.1.0 and above.
-    """
+    endpoint_name = "commits"
+    queryset = models.OstreeCommit.objects.all()
+    serializer_class = serializers.OstreeCommitSerializer
+    filterset_class = OstreeCommitFilter
 
-    parent_lookup_kwargs = {"parent_pk": "parent__pk"}
 
-    serializer_url_field = NestedHyperlinkedIdentityField
-    serializer_related_field = NestedHyperlinkedRelatedField
+class OstreeObjectFilter(ContentFilter):
+    """A filterset class for objects."""
 
-    def __init__(self, *args, **kwargs):
-        """Initialize class-wide variables."""
-        self.parent_lookup_kwargs = kwargs.pop("parent_lookup_kwargs", self.parent_lookup_kwargs)
-        super(NestedHyperlinkedModelSerializer, self).__init__(*args, **kwargs)
+    class Meta:
+        model = models.OstreeObject
+        fields = {"checksum": ["exact"]}
 
-    def build_url_field(self, field_name, model_class):
-        """Return URL fields."""
-        field_class, field_kwargs = super(NestedHyperlinkedModelSerializer, self).build_url_field(
-            field_name, model_class
-        )
-        field_kwargs["parent_lookup_kwargs"] = self.parent_lookup_kwargs
 
-        return field_class, field_kwargs
+class OstreeObjectViewSet(ReadOnlyContentViewSet):
+    """A ViewSet class for OSTree objects (e.g., dirtree, dirmeta, file)."""
 
-    def build_nested_field(self, field_name, relation_info, nested_depth):
-        """
-        Create nested fields for forward and reverse relationships.
-        """
-
-        class NestedSerializer(NestedHyperlinkedModelSerializer):
-            class Meta:
-                model = relation_info.related_model
-                depth = nested_depth - 1
-                fields = "__all__"
-
-        field_class = NestedSerializer
-        field_kwargs = get_nested_relation_kwargs(relation_info)
-
-        return field_class, field_kwargs
-
-
-class RepositoryAddRemoveContentSerializer(
-    platform.ModelSerializer, NestedHyperlinkedModelSerializer
-):
-    """A serializer class for add/remove operations."""
-
-    add_content_units = serializers.ListField(
-        help_text=_(
-            "A list of content units to add to a new repository version. This content is "
-            "added after remove_content_units are removed."
-        ),
-        required=False,
-    )
-    remove_content_units = serializers.ListField(
-        help_text=_(
-            "A list of content units to remove from the latest repository version. "
-            "You may also specify '*' as an entry to remove all content. This content is "
-            "removed before add_content_units are added."
-        ),
-        required=False,
-    )
-    base_version = platform.RepositoryVersionRelatedField(
-        required=False,
-        help_text=_(
-            "A repository version whose content will be used as the initial set of content "
-            "for the new repository version"
-        ),
-    )
+    endpoint_name = "objects"
+    queryset = models.OstreeObject.objects.all()
+    serializer_class = serializers.OstreeObjectSerializer
+    filterset_class = OstreeObjectFilter
 
-    def validate_remove_content_units(self, value):
-        """Validate the passed content units."""
-        if len(value) > 1 and "*" in value:
-            raise serializers.ValidationError("Cannot supply content units and '*'.")
-        return value
 
-    class Meta:
-        model = RepositoryVersion
-        fields = ["add_content_units", "remove_content_units", "base_version"]
+class OstreeContentViewSet(ReadOnlyContentViewSet):
+    """A ViewSet class for uncategorized content units (e.g., static deltas)."""
 
+    endpoint_name = "content"
+    queryset = models.OstreeContent.objects.all()
+    serializer_class = serializers.OstreeContentSerializer
 
-class OstreeRepositoryAddRemoveContentSerializer(RepositoryAddRemoveContentSerializer):
-    """A Serializer class for modifying a repository from an existing repository."""
 
-    ALLOWED_ADD_REMOVE_CONTENT_UNITS = [
-        models.OstreeCommit,
-        models.OstreeRef,
-        models.OstreeConfig,
-        models.OstreeSummary,
-    ]
-
-    def validate(self, data):
-        """Validate content that will be added or removed from a repository."""
-        data = super().validate(data)
-
-        self.validate_units("add_content_units", data)
-        self.validate_units("remove_content_units", data)
-
-        return data
-
-    def validate_units(self, units_modify_type, content):
-        """Check if the content is in allowed content types (e.g., commit)."""
-        if units_modify_type in content:
-            for unit_href in content[units_modify_type]:
-                unit_model = resolve(unit_href).func.cls.queryset.model
-                if unit_model not in self.ALLOWED_ADD_REMOVE_CONTENT_UNITS:
-                    raise serializers.ValidationError(
-                        _(
-                            "The unit {} is not allowed to be used in this endpoint".format(
-                                unit_href
-                            )
-                        )
-                    )
+class OstreeConfigViewSet(ReadOnlyContentViewSet):
+    """A ViewSet class for OSTree repository configurations."""
 
+    endpoint_name = "configs"
+    queryset = models.OstreeConfig.objects.all()
+    serializer_class = serializers.OstreeConfigSerializer
 
-class OstreeDistributionSerializer(platform.DistributionSerializer):
-    """A Serializer class for an OSTree distribution."""
 
-    repository_version = platform.RepositoryVersionRelatedField(
-        required=False, help_text=_("RepositoryVersion to be served"), allow_null=True
-    )
+class OstreeSummaryViewSet(ReadOnlyContentViewSet):
+    """A ViewSet class for OSTree repository summary files."""
 
-    class Meta:
-        fields = platform.DistributionSerializer.Meta.fields + ("repository_version",)
-        model = models.OstreeDistribution
+    endpoint_name = "summaries"
+    queryset = models.OstreeSummary.objects.all()
+    serializer_class = serializers.OstreeSummarySerializer
```

### Comparing `pulp-ostree-2.0.0a6/pulp_ostree/app/tasks/importing.py` & `pulp-ostree-2.1.0/pulp_ostree/app/tasks/synchronizing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,288 +1,294 @@
 import os
-import tarfile
+import logging
 
-from gettext import gettext
+from fnmatch import fnmatch
+from gettext import gettext as _
+from pathlib import Path
+from urllib.parse import urljoin
 
-from asgiref.sync import sync_to_async
-
-from pulpcore.plugin.models import Artifact, Repository, ProgressReport
+from pulpcore.plugin.models import Repository, ProgressReport, Artifact, Remote
 from pulpcore.plugin.stages import (
     ArtifactSaver,
+    ArtifactDownloader,
     ContentSaver,
     DeclarativeVersion,
+    DeclarativeArtifact,
+    DeclarativeContent,
     QueryExistingArtifacts,
     QueryExistingContents,
+    RemoteArtifactSaver,
     ResolveContentFutures,
     Stage,
 )
 
 from pulp_ostree.app.models import (
+    OstreeRemote,
+    OstreeObjectType,
     OstreeCommit,
     OstreeConfig,
-    OstreeObjectType,
+    OstreeSummary,
 )
-from pulp_ostree.app.tasks.utils import get_checksum_filepath
 from pulp_ostree.app.tasks.stages import OstreeAssociateContent, DeclarativeContentCreatorMixin
+from pulp_ostree.app.tasks.utils import get_checksum_filepath, bytes_to_checksum
 
 import gi
 
 gi.require_version("OSTree", "1.0")
 from gi.repository import Gio, GLib, OSTree  # noqa: E402: module level not at top of file
 
+log = logging.getLogger(__name__)
 
-def import_all_refs_and_commits(artifact_pk, repository_pk, repository_name):
-    """Import all ref and commits to an OSTree repository.
 
-    Args:
-        artifact_pk (str): The PK of an artifact that identifies a tarball.
-        repository_pk (str): The repository PK.
-        repository_name (str): The name of an OSTree repository (e.g., "repo").
-
-    Raises:
-        ValueError: If an OSTree repository could not be properly parsed or the specified ref
-            does not exist.
+def synchronize(remote_pk, repository_pk, mirror):
     """
-    tarball_artifact = Artifact.objects.get(pk=artifact_pk)
-    repository = Repository.objects.get(pk=repository_pk)
-    first_stage = OstreeImportAllRefsFirstStage(tarball_artifact, repository_name)
-    dv = OstreeImportDeclarativeVersion(first_stage, repository)
-    return dv.create()
+    Sync content from the remote repository.
 
-
-def import_child_commits(artifact_pk, repository_pk, repository_name, ref):
-    """Import child commits to a specific ref.
+    Create a new version of the repository that is synchronized with the remote.
 
     Args:
-        artifact_pk (str): The PK of an artifact that identifies a tarball.
+        remote_pk (str): The remote PK.
         repository_pk (str): The repository PK.
-        repository_name (str): The name of an OSTree repository (e.g., "repo").
-        ref (str): The name of a ref object that points to the last commit.
+        mirror (bool): True for mirror mode, False for additive.
 
     Raises:
-        ValueError: If an OSTree repository could not be properly parsed or the specified ref
-            does not exist.
+        ValueError: If the remote does not specify a URL to sync
+
     """
-    tarball_artifact = Artifact.objects.get(pk=artifact_pk)
+    remote = OstreeRemote.objects.get(pk=remote_pk)
     repository = Repository.objects.get(pk=repository_pk)
-    first_stage = OstreeImportSingleRefFirstStage(tarball_artifact, repository_name, ref)
-    dv = OstreeImportDeclarativeVersion(first_stage, repository)
-    return dv.create()
 
+    if not remote.url:
+        raise ValueError(_("A remote must have a url specified to synchronize."))
 
-class OstreeSingleRefParserMixin:
-    """A mixin class that allows stages to share the same methods for parsing OSTree data."""
+    deferred_download = remote.policy != Remote.IMMEDIATE
+    compute_delta = repository.cast().compute_delta
+    first_stage = OstreeFirstStage(remote, deferred_download, compute_delta)
+    dv = OstreeSyncDeclarativeVersion(first_stage, repository, mirror=mirror)
+    return dv.create()
 
-    async def parse_ref(self, name, ref_commit_checksum, has_referenced_parent=False):
-        """Parse a single ref object with associated commits and other objects."""
-        _, ref_commit, _ = self.repo.load_commit(ref_commit_checksum)
-        relative_path = get_checksum_filepath(
-            ref_commit_checksum, OstreeObjectType.OSTREE_OBJECT_TYPE_COMMIT
-        )
-        ref_path = os.path.join("refs/", "heads/", name)
 
-        parent_checksum = OSTree.commit_get_parent(ref_commit)
-        if not parent_checksum:
-            # there are not any parent commits, return and continue parsing the next ref
-            commit = OstreeCommit(checksum=ref_commit_checksum)
-            commit_dc = self.create_dc(relative_path, commit)
-            await self.put(commit_dc)
-
-            await self.submit_related_objects(commit_dc)
-
-            self.init_ref_object(name, ref_path, commit_dc)
-
-            return
-
-        checksum = ref_commit_checksum
-        ref_commit = OstreeCommit(checksum=checksum)
-        ref_commit_dc = self.create_dc(relative_path, ref_commit)
-        self.commit_dcs.append(ref_commit_dc)
-
-        self.init_ref_object(name, ref_path, ref_commit_dc)
-
-        try:
-            _, parent_commit, _ = self.repo.load_commit(parent_checksum)
-        except GLib.Error:
-            if has_referenced_parent:
-                # the associated parent commit may not be present in the parsed tarball
-                # and this state is still considered valid
-                return parent_checksum, ref_commit_dc
-            else:
-                raise ValueError(
-                    gettext("The parent commit '{}' could not be loaded").format(parent_checksum)
-                )
+class OstreeFirstStage(DeclarativeContentCreatorMixin, Stage):
+    """A first stage of the OSTree syncing pipeline that handles creation of content units."""
 
-        return await self.load_next_commits(parent_commit, parent_checksum, has_referenced_parent)
+    def __init__(self, remote, deferred_download, compute_delta):
+        """Initialize class variables used for parsing OSTree objects."""
+        super().__init__()
+        self.remote = remote
+        self.deferred_download = deferred_download
+        self.compute_delta = compute_delta
 
-    async def load_next_commits(self, parent_commit, checksum, has_referenced_parent=False):
-        """Queue next parent commits if exist."""
-        relative_path = get_checksum_filepath(checksum, OstreeObjectType.OSTREE_OBJECT_TYPE_COMMIT)
+        self.repo_name = remote.name
+        self.repo = None
+        self.repo_path = None
 
-        parent_checksum = OSTree.commit_get_parent(parent_commit)
+        self.commit_dcs = []
+        self.refs_dcs = []
 
-        while parent_checksum:
-            commit = OstreeCommit(checksum=checksum)
-            commit_dc = self.create_dc(relative_path, commit)
-            self.commit_dcs.append(commit_dc)
+        self.create_object_dc_func = self.create_remote_artifact_dc
 
-            checksum = parent_checksum
-            relative_path = get_checksum_filepath(
-                checksum, OstreeObjectType.OSTREE_OBJECT_TYPE_COMMIT
-            )
-            try:
-                _, parent_commit, _ = self.repo.load_commit(parent_checksum)
-            except GLib.Error:
-                if has_referenced_parent:
-                    # the associated parent commit may not be present in the parsed tarball
-                    # and this state is still considered valid
-                    return parent_checksum, commit_dc
-                else:
-                    raise ValueError(
-                        gettext("The parent commit '{}' could not be loaded").format(
-                            parent_checksum
-                        )
-                    )
-            parent_checksum = OSTree.commit_get_parent(parent_commit)
+    async def run(self):
+        """Create OSTree content units and declare relations between them."""
+        async with ProgressReport(
+            message="Parsing Metadata", code="sync.parsing_metadata", total=1
+        ) as pb:
+            self.init_repository()
+
+            await self.submit_metafiles()
+
+            _, refs = self.repo.remote_list_refs(self.repo_name)
+            for name in self.filter_refs(refs.keys()):
+                ref_commit_checksum = refs[name]
+
+                ref_relative_path = os.path.join("refs/heads/", name)
+                local_ref_path = os.path.join(self.repo_path, ref_relative_path)
+
+                dirname = os.path.dirname(local_ref_path)
+                # create a directory to prevent IOError
+                os.makedirs(dirname, exist_ok=True)
+
+                with open(local_ref_path, "w") as f:
+                    f.write(ref_commit_checksum)
+                    f.flush()
 
-        commit = OstreeCommit(checksum=checksum)
-        commit_dc = self.create_dc(relative_path, commit)
-        self.commit_dcs.append(commit_dc)
+                relative_path = get_checksum_filepath(
+                    ref_commit_checksum, OstreeObjectType.OSTREE_OBJECT_TYPE_COMMIT
+                )
+                await self.download_remote_object(relative_path)
 
-        await self.put(commit_dc)
-        await self.submit_related_objects(commit_dc)
+                _, ref_commit, _ = self.repo.load_commit(ref_commit_checksum)
+                ref_parent_checksum = parent_checksum = OSTree.commit_get_parent(ref_commit)
+                if not parent_checksum or self.remote.depth == 0:
+                    # there are not any parent commits, continue parsing the next head branch
+                    commit = OstreeCommit(checksum=ref_commit_checksum)
+                    commit_dc = self.create_dc(relative_path, commit)
+                    await self.put(commit_dc)
 
-        await self.submit_previous_commits_and_related_objects()
+                    await self.submit_related_objects(commit_dc)
 
+                    self.init_ref_object(name, ref_relative_path, commit_dc)
 
-class OstreeImportStage(Stage):
-    """A stage generalizing the common methods for initializing an OSTree repository."""
+                    continue
 
-    def __init__(self, repo_name):
-        """Initialize class variables that are common for tasks that import OSTree content."""
-        super().__init__()
+                checksum = ref_commit_checksum
+                ref_commit = OstreeCommit(checksum=checksum)
+                ref_commit_dc = self.create_dc(relative_path, ref_commit)
+                self.commit_dcs.append(ref_commit_dc)
 
-        self.repo_name = repo_name
-        self.repo = None
-        self.repo_path = None
+                relative_path = get_checksum_filepath(
+                    parent_checksum, OstreeObjectType.OSTREE_OBJECT_TYPE_COMMIT
+                )
+                await self.download_remote_object(relative_path)
+                _, parent_commit, _ = self.repo.load_commit(parent_checksum)
+                parent_checksum = OSTree.commit_get_parent(parent_commit)
 
-        self.commit_dcs = []
-        self.refs_dcs = []
+                max_depth = self.remote.depth
 
-    def init_repository(self):
-        """Initialize new OSTree repository objects."""
-        self.repo_path = os.path.join(os.getcwd(), self.repo_name)
+                while parent_checksum and max_depth > 0:
+                    commit = OstreeCommit(checksum=checksum)
+                    commit_dc = self.create_dc(relative_path, commit)
+                    self.commit_dcs.append(commit_dc)
+
+                    checksum = parent_checksum
+                    relative_path = get_checksum_filepath(
+                        checksum, OstreeObjectType.OSTREE_OBJECT_TYPE_COMMIT
+                    )
+                    await self.download_remote_object(relative_path)
+                    _, parent_commit, _ = self.repo.load_commit(checksum)
+                    parent_checksum = OSTree.commit_get_parent(parent_commit)
+
+                    max_depth -= 1
+
+                commit = OstreeCommit(checksum=checksum)
+                commit_dc = self.create_dc(relative_path, commit)
+                self.commit_dcs.append(commit_dc)
 
-        self.repo = OSTree.Repo.new(Gio.File.new_for_path(self.repo_path))
+                await self.put(commit_dc)
+                await self.submit_related_objects(commit_dc)
 
-        try:
-            self.repo.open()
-        except GLib.Error:
-            raise ValueError(
-                gettext("An invalid path to the repository provided: {}").format(self.repo_name)
-            )
+                await self.submit_previous_commits_and_related_objects()
 
+                self.init_ref_object(name, ref_relative_path, ref_commit_dc)
 
-class OstreeImportSingleRefFirstStage(
-    DeclarativeContentCreatorMixin, OstreeSingleRefParserMixin, OstreeImportStage
-):
-    """A first stage of the OSTree importing pipeline that appends child commits to a repository."""
+                if self.compute_delta:
+                    await self.compute_static_delta(ref_commit_checksum, ref_parent_checksum)
 
-    def __init__(self, tarball_artifact, repo_name, ref):
-        """Initialize class variables used for parsing OSTree objects."""
-        super().__init__(repo_name)
-        self.tarball_artifact = tarball_artifact
-        self.ref = ref
+            await pb.aincrement()
 
-        self.create_object_dc_func = self.create_dc
+        await self.submit_ref_objects()
 
-    async def run(self):
-        """Create OSTree content units and associate them with the parent commit."""
-        with tarfile.open(self.tarball_artifact.file.path) as tar:
-            async with ProgressReport(
-                message="Adding the child commits", code="adding.commits", total=1
-            ) as pb:
-                tar.extractall(path=os.getcwd())
-                self.init_repository()
-
-                last_commit_dc = None
-                _, refs = self.repo.list_refs()
-                for name, ref_commit_checksum in refs.items():
-                    if self.ref == name:
-                        parent_checksum, last_commit_dc = await self.parse_ref(
-                            name, ref_commit_checksum, has_referenced_parent=True
-                        )
-                        break
-
-                if last_commit_dc is None:
-                    raise ValueError(
-                        gettext("An invalid ref name in the repository was specified: {}").format(
-                            self.ref
-                        )
-                    )
+    def filter_refs(self, refs):
+        """Filter refs by the list of include/exclude patterns."""
 
-                try:
-                    parent_commit = await sync_to_async(OstreeCommit.objects.get)(
-                        checksum=parent_checksum
-                    )
-                except OstreeCommit.DoesNotExist:
-                    pass
-                else:
-                    last_commit_dc.extra_data["parent_commit"] = parent_commit
-                    await self.put(last_commit_dc)
-                    await self.submit_related_objects(last_commit_dc)
+        def _pattern_matches(ref, patterns):
+            return any(fnmatch(ref, pattern) for pattern in patterns)
 
-                await self.submit_previous_commits_and_related_objects()
+        include_refs = self.remote.include_refs
+        if include_refs:
+            refs = [ref for ref in refs if _pattern_matches(ref, include_refs)]
 
-                await pb.aincrement()
+        exclude_refs = self.remote.exclude_refs
+        if exclude_refs:
+            refs = [ref for ref in refs if not _pattern_matches(ref, exclude_refs)]
 
-            await self.submit_ref_objects()
+        return refs
 
+    def init_repository(self):
+        """Initialize a new OSTree repository object."""
+        self.repo_path = os.path.join(os.getcwd(), "repo/")
 
-class OstreeImportAllRefsFirstStage(
-    DeclarativeContentCreatorMixin, OstreeSingleRefParserMixin, OstreeImportStage
-):
-    """A first stage of the OSTree importing pipeline that handles creation of content units."""
+        self.repo = OSTree.Repo.new(Gio.File.new_for_path(self.repo_path))
+        self.repo.create(OSTree.RepoMode.ARCHIVE)
 
-    def __init__(self, tarball_artifact, repo_name):
-        """Initialize class variables used for parsing OSTree objects."""
-        super().__init__(repo_name)
-        self.tarball_artifact = tarball_artifact
+        no_gpg_verify = {"gpg-verify": GLib.Variant.new_boolean(False)}
+        gpg_verify_variant = GLib.Variant("a{sv}", no_gpg_verify)
+        self.repo.remote_add(self.repo_name, self.remote.url, gpg_verify_variant)
+
+        # TODO: with this, we will no longer need to manually download ostree content because all
+        #   the content will be available in place; refactoring the code is necessary:
+        #   https://github.com/pulp/pulp_ostree/issues/169#issuecomment-1476232489
+        self.repo.pull(self.repo_name, None, OSTree.RepoPullFlags.MIRROR)
+
+    async def submit_metafiles(self):
+        """Download config and summary files and create DeclarativeContent objects for them."""
+        await self.download_remote_object("config")
+        await self.submit_metafile_object("config", OstreeConfig())
+
+        await self.download_remote_object("summary")
+        await self.submit_metafile_object("summary", OstreeSummary())
+
+    async def download_remote_object(self, relative_path):
+        """Download an object identified by the relative path with respect to the remote."""
+        url = urljoin(self.remote.url, relative_path)
+        downloader = self.remote.get_downloader(url=url)
+        await downloader.run()
+
+        full_path = Path(self.repo_path, relative_path)
+        full_path.parent.mkdir(parents=True, exist_ok=True)
+        os.rename(downloader.path, full_path)
+
+    def create_remote_artifact_dc(self, relative_path, content):
+        """Create a declarative artifact that will have associated a remote artifact with it."""
+        content_url = urljoin(self.remote.url, relative_path)
+
+        content.relative_path = relative_path
+
+        da = DeclarativeArtifact(
+            artifact=Artifact(),
+            remote=self.remote,
+            url=content_url,
+            relative_path=relative_path,
+            deferred_download=self.deferred_download,
+        )
 
-        self.create_object_dc_func = self.create_dc
+        return DeclarativeContent(content=content, d_artifacts=[da])
 
-    async def run(self):
-        """Create OSTree content units and declare relations between them."""
-        with tarfile.open(self.tarball_artifact.file.path) as tar:
-            async with ProgressReport(
-                message="Committing the tarball", code="committing.tarball", total=1
-            ) as pb:
-                tar.extractall(path=os.getcwd())
-                self.init_repository()
+    async def submit_related_objects(self, commit_dc):
+        """Queue related DeclarativeContent objects and additionally download dirtree metadata."""
+        _, loaded_commit, _ = self.repo.load_commit(commit_dc.content.checksum)
+
+        # it is necessary to download referenced dirtree objects; otherwise, the traversal cannot
+        # be executed without errors; the traversing allows us to read all referenced checksums,
+        # meaning that in the end we will have a list of all objects referenced by a single commit
+        dirtree_checksum = bytes_to_checksum(loaded_commit[6])
+        relative_path = get_checksum_filepath(
+            dirtree_checksum, OstreeObjectType.OSTREE_OBJECT_TYPE_DIR_TREE
+        )
+        await self.download_remote_object(relative_path)
 
-                await self.submit_metafile_object("config", OstreeConfig())
+        _, dirtree_obj = self.repo.load_variant(OSTree.ObjectType.DIR_TREE, dirtree_checksum)
+        subtree_checksums = {bytes_to_checksum(subtree[1]) for subtree in dirtree_obj[1]}
+        await self.download_dirtrees(subtree_checksums)
 
-                _, refs = self.repo.list_refs()
-                for name, ref_commit_checksum in refs.items():
-                    await self.parse_ref(name, ref_commit_checksum)
+        await super().submit_related_objects(commit_dc)
 
-                await pb.aincrement()
+    async def download_dirtrees(self, subtree_checksums):
+        """Recursively download dirtree objects and their sub-dirtree objects."""
+        for subtree_checksum in subtree_checksums:
+            relative_path = get_checksum_filepath(
+                subtree_checksum, OstreeObjectType.OSTREE_OBJECT_TYPE_DIR_TREE
+            )
+            await self.download_remote_object(relative_path)
 
-            await self.submit_ref_objects()
+            _, dirtree_obj = self.repo.load_variant(OSTree.ObjectType.DIR_TREE, subtree_checksum)
+            child_subtree_checksums = {bytes_to_checksum(subtree[1]) for subtree in dirtree_obj[1]}
+            await self.download_dirtrees(child_subtree_checksums)
 
 
-class OstreeImportDeclarativeVersion(DeclarativeVersion):
-    """A customized DeclarativeVersion class that creates a pipeline for the OSTree import."""
+class OstreeSyncDeclarativeVersion(DeclarativeVersion):
+    """A customized DeclarativeVersion class that creates a pipeline for the OSTree sync."""
 
     def pipeline_stages(self, new_version):
         """Build a list of stages."""
         pipeline = [
             self.first_stage,
             QueryExistingArtifacts(),
+            ArtifactDownloader(),
             ArtifactSaver(),
             QueryExistingContents(),
             ContentSaver(),
+            RemoteArtifactSaver(),
             ResolveContentFutures(),
             OstreeAssociateContent(),
         ]
 
         return pipeline
```

### Comparing `pulp-ostree-2.0.0a6/pulp_ostree/app/tasks/modifying.py` & `pulp-ostree-2.1.0/pulp_ostree/app/tasks/modifying.py`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.0.0a6/pulp_ostree/app/tasks/stages.py` & `pulp-ostree-2.1.0/pulp_ostree/app/tasks/stages.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,16 +6,27 @@
 from pulpcore.plugin.models import Artifact
 from pulpcore.plugin.stages import (
     DeclarativeArtifact,
     DeclarativeContent,
     Stage,
 )
 
-from pulp_ostree.app.models import OstreeCommit, OstreeObject, OstreeRef, OstreeCommitObject
-from pulp_ostree.app.tasks.utils import get_checksum_filepath
+from pulp_ostree.app.models import (
+    OstreeCommit,
+    OstreeContent,
+    OstreeObject,
+    OstreeRef,
+    OstreeCommitObject,
+)
+from pulp_ostree.app.tasks.utils import compute_hash, get_checksum_filepath
+
+import gi
+
+gi.require_version("OSTree", "1.0")
+from gi.repository import GLib, OSTree  # noqa: E402: module level not at top of file
 
 
 class DeclarativeContentCreatorMixin:
     """A mixin class that defines basic methods for creating declarative content."""
 
     async def submit_related_objects(self, commit_dc):
         """Queue DeclarativeContent objects describing standard OSTree objects (e.g., dirtree)."""
@@ -83,14 +94,39 @@
         # referenced by multiple content units at the same time; in particular, this means that
         # one OSTree object (e.g., dirmeta, filez) is referenced by two different commits
         filepath_copy = filepath + str(uuid.uuid4())
         os.link(filepath, filepath_copy)
 
         return Artifact.init_and_validate(filepath_copy)
 
+    async def compute_static_delta(self, ref_commit_checksum, parent_checksum=None):
+        if not self.commit_dcs:
+            return
+
+        if parent_checksum:
+            from_ = parent_checksum
+        else:
+            from_ = self.commit_dcs[0].content.checksum
+
+        # latest commit
+        to = ref_commit_checksum
+
+        self.repo.static_delta_generate(
+            OSTree.StaticDeltaGenerateOpt.MAJOR, from_, to, None, GLib.Variant("a{sv}", None)
+        )
+
+        for dirpath, dirnames, filenames in os.walk(os.path.join(self.repo_path, "deltas/")):
+            for filename in filenames:
+                full_path = os.path.join(dirpath, filename)
+                relative_path = os.path.relpath(full_path, self.repo_path)
+
+                content = OstreeContent(relative_path=relative_path, digest=compute_hash(full_path))
+                content_dc = self.create_dc(relative_path, content)
+                await self.put(content_dc)
+
 
 class OstreeAssociateContent(Stage):
     """A stage for creating associations between OSTree objects."""
 
     async def run(self):
         """Create relations between each OSTree object specified in DeclarativeContent objects."""
         async for batch in self.batches():
```

### Comparing `pulp-ostree-2.0.0a6/pulp_ostree/tests/functional/api/test_filter.py` & `pulp-ostree-2.1.0/pulp_ostree/tests/functional/api/test_filter.py`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.0.0a6/pulp_ostree/tests/functional/api/test_import.py` & `pulp-ostree-2.1.0/pulp_ostree/tests/functional/api/test_import.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import requests
 import shutil
 import subprocess
+import tempfile
 import unittest
 
+from urllib.parse import urljoin
 from pathlib import Path
 
 from pulp_smash import config, api
 from pulp_smash.pulp3.bindings import delete_orphans, monitor_task
 from pulp_smash.pulp3.utils import gen_repo, gen_distribution, utils
 
 from pulpcore.client.pulp_ostree import (
@@ -42,18 +44,24 @@
         client_api = gen_ostree_client()
         cls.repositories_api = RepositoriesOstreeApi(client_api)
         cls.versions_api = RepositoriesOstreeVersionsApi(client_api)
         cls.distributions_api = DistributionsOstreeApi(client_api)
         cls.commits_api = ContentCommitsApi(client_api)
         cls.refs_api = ContentRefsApi(client_api)
 
+        cls.original_dir = os.getcwd()
+        cls.tmpdir = tempfile.TemporaryDirectory()
+        os.chdir(cls.tmpdir.name)
+
     @classmethod
     def tearDownClass(cls):
         """Clean orphaned content after finishing the tests."""
         delete_orphans()
+        os.chdir(cls.original_dir)
+        cls.tmpdir.cleanup()
 
     def setUp(self):
         """Clean orphaned content before each test."""
         delete_orphans()
 
     def test_simple_tarball_import(self):
         """Import a repository consisting of three commit, publish it, and pull it from Pulp."""
@@ -141,40 +149,40 @@
 
         # 1. create a first file
         sample_dir1.mkdir()
         self.addCleanup(shutil.rmtree, sample_dir1)
         sample_file1.touch()
 
         # 2. initialize a local OSTree repository and commit the created file
-        subprocess.run(["ostree", f"--repo={self.repo_name1}", "init", "--mode=archive"])
-        subprocess.run(
+        subprocess.check_output(["ostree", f"--repo={self.repo_name1}", "init", "--mode=archive"])
+        subprocess.check_output(
             ["ostree", f"--repo={self.repo_name1}", "commit", "--branch=foo", f"{sample_dir1}/"]
         )
         with open(f"{self.repo_name1}/refs/heads/foo", "r") as ref:
             commits_to_check.append(ref.read().strip())
 
         # 3. create a tarball from the first repository
         subprocess.run(["tar", "-cvf", f"{self.repo_name1}1.tar", f"{self.repo_name1}/"])
         self.addCleanup(os.unlink, f"{self.repo_name1}1.tar")
         self.commit_repo1_artifact = gen_artifact(f"{self.repo_name1}1.tar")
 
         shutil.rmtree(self.repo_name1)
 
         # 4. initialize a second OSTree repository and commit the created file
-        subprocess.run(["ostree", f"--repo={self.repo_name1}", "init", "--mode=archive"])
+        subprocess.check_output(["ostree", f"--repo={self.repo_name1}", "init", "--mode=archive"])
 
         sample_dir2.mkdir()
         self.addCleanup(shutil.rmtree, sample_dir2)
 
         # 5. create new commits by submitting randomly generated files one by one
         for _ in range(number_of_commits):
             sample_file2 = sample_dir2 / Path(utils.uuid4())
             sample_file2.touch()
 
-            subprocess.run(
+            subprocess.check_output(
                 [
                     "ostree",
                     f"--repo={self.repo_name1}",
                     "commit",
                     "--branch=foo",
                     f"{sample_dir2}/",
                     f"--parent={commits_to_check[-1]}",
@@ -185,14 +193,35 @@
                 commits_to_check.append(ref.read().strip())
 
         # 6. create a tarball from the second repository
         subprocess.run(["tar", "-cvf", f"{self.repo_name1}2.tar", f"{self.repo_name1}/"])
         self.addCleanup(os.unlink, f"{self.repo_name1}2.tar")
         self.commit_repo2_artifact = gen_artifact(f"{self.repo_name1}2.tar")
 
+        # the latest parent commit is not accessible to this repository since it was removed;
+        # therefore, we need to unpack the old repository into the new one to mimic the
+        # behaviour that should occur in a real repository when computing static deltas
+        subprocess.run(["tar", "-xvf", f"{self.repo_name1}1.tar", f"{self.repo_name1}/"])
+        subprocess.check_output(
+            [
+                "ostree",
+                f"--repo={self.repo_name1}",
+                "static-delta",
+                "generate",
+                f"--from={commits_to_check[-2]}",
+                f"--to={commits_to_check[-1]}",
+            ]
+        )
+
+        deltas_paths = []
+        for dirpath, dirnames, filenames in os.walk(os.path.join(self.repo_name1, "deltas/")):
+            for filename in filenames:
+                full_path = os.path.join(dirpath, filename)
+                deltas_paths.append(os.path.relpath(full_path, self.repo_name1))
+
         shutil.rmtree(self.repo_name1)
 
         # 7. import the first repository
         repo = self.repositories_api.create(OstreeOstreeRepository(**gen_repo()))
         self.addCleanup(self.repositories_api.delete, repo.pulp_href)
         commit_data = OstreeImportAll(self.commit_repo1_artifact["pulp_href"], self.repo_name1)
         response = self.repositories_api.import_all(repo.pulp_href, commit_data)
@@ -240,14 +269,21 @@
         ostree_repo_path = self.distributions_api.read(distribution).base_url
 
         # 11. initialize a local OSTree repository and pull the content from Pulp
         remote_name = init_local_repo_with_remote(self.repo_name2, ostree_repo_path)
         self.addCleanup(shutil.rmtree, Path(self.repo_name2))
         validate_repo_integrity(self.repo_name2, f"{remote_name}:foo", set(commits_to_check))
 
+        # 12. check if static deltas are being published
+        for delta_path in deltas_paths:
+            response = self.client.using_handler(api.echo_handler).get(
+                urljoin(ostree_repo_path, delta_path)
+            )
+            self.assertEqual(response.status_code, 200)
+
     def test_version_removal(self):
         """Test the repository version removal functionality by removing two adjacent versions."""
         self.single_ref_import(1)
 
         repo_href = self.repositories_api.list().to_dict()["results"][0]["pulp_href"]
         repo_version1_href = self.versions_api.read(f"{repo_href}versions/1/").pulp_href
         repo_version2_href = self.versions_api.read(f"{repo_href}versions/2/").pulp_href
```

### Comparing `pulp-ostree-2.0.0a6/pulp_ostree/tests/functional/api/test_modify.py` & `pulp-ostree-2.1.0/pulp_ostree/tests/functional/api/test_modify.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+import os
 import shutil
+import tempfile
 import unittest
 
 from urllib.parse import urlparse
 
-from requests.exceptions import HTTPError
-
 from pulp_smash import config, api
 from pulp_smash.pulp3.bindings import delete_orphans, monitor_task
 from pulp_smash.pulp3.utils import get_content, gen_distribution, gen_repo, modify_repo
 
 from pulpcore.client.pulp_ostree import (
     DistributionsOstreeApi,
     OstreeOstreeDistribution,
@@ -53,18 +53,24 @@
         cls.distributions_api = DistributionsOstreeApi(client_api)
         cls.commits_api = ContentCommitsApi(client_api)
         cls.configs_api = ContentConfigsApi(client_api)
         cls.objs_api = ContentObjectsApi(client_api)
         cls.remotes_api = RemotesOstreeApi(client_api)
         cls.refs_api = ContentRefsApi(client_api)
 
+        cls.original_dir = os.getcwd()
+        cls.tmpdir = tempfile.TemporaryDirectory()
+        os.chdir(cls.tmpdir.name)
+
     @classmethod
     def tearDownClass(cls):
         """Clean orphaned content after finishing the tests."""
         delete_orphans()
+        os.chdir(cls.original_dir)
+        cls.tmpdir.cleanup()
 
     def setUp(self):
         """Clean orphaned content before each test and initialize a new repository."""
         delete_orphans()
 
         self.repo1 = self.repositories_api.create(gen_repo())
         self.addCleanup(self.repositories_api.delete, self.repo1.pulp_href)
@@ -223,19 +229,24 @@
         self.assertEqual(removed_content["ostree.object"]["count"], 3)
 
     def test_add_remove_obj(self):
         """Try to modify an object (e.g., dirtree, dirmeta, ...) in the existing repository."""
         created_objs = self.objs_api.list(repository_version_added=self.repo_version1.pulp_href)
         obj = created_objs.to_dict()["results"][0]
 
-        with self.assertRaises(HTTPError):
-            modify_repo(self.cfg, self.repo1.to_dict(), add_units=[obj])
+        version1 = self.repositories_api.read(self.repo1.pulp_href).latest_version_href
 
-        with self.assertRaises(HTTPError):
-            modify_repo(self.cfg, self.repo1.to_dict(), remove_units=[obj])
+        # objects should be ignored by the machinery
+        modify_repo(self.cfg, self.repo1.to_dict(), add_units=[obj])
+        version2 = self.repositories_api.read(self.repo1.pulp_href).latest_version_href
+        self.assertEqual(version1, version2)
+
+        modify_repo(self.cfg, self.repo1.to_dict(), remove_units=[obj])
+        version2 = self.repositories_api.read(self.repo1.pulp_href).latest_version_href
+        self.assertEqual(version1, version2)
 
 
 def normalize_content(repo_content):
     """Make the repository content to be ready for comparison purposes."""
     repo_commits = sorted(
         [remove_created_key(item) for item in repo_content[OSTREE_COMMITS_NAME]],
         key=lambda item: item["pulp_href"],
```

### Comparing `pulp-ostree-2.0.0a6/pulp_ostree/tests/functional/api/test_sync.py` & `pulp-ostree-2.1.0/pulp_ostree/tests/functional/api/test_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import os
 import shutil
+import tempfile
 import unittest
 
 from pulp_smash.pulp3.bindings import delete_orphans, monitor_task
 from pulp_smash.pulp3.utils import gen_repo, gen_distribution
 
 from pulp_ostree.tests.functional.utils import (
     gen_ostree_client,
@@ -31,18 +33,24 @@
         client_api = gen_ostree_client()
         cls.repositories_api = RepositoriesOstreeApi(client_api)
         cls.versions_api = RepositoriesOstreeVersionsApi(client_api)
         cls.remotes_api = RemotesOstreeApi(client_api)
         cls.distributions_api = DistributionsOstreeApi(client_api)
         cls.refs_api = ContentRefsApi(client_api)
 
+        cls.original_dir = os.getcwd()
+        cls.tmpdir = tempfile.TemporaryDirectory()
+        os.chdir(cls.tmpdir.name)
+
     @classmethod
     def tearDownClass(cls):
         """Clean orphaned content after finishing the tests."""
         delete_orphans()
+        os.chdir(cls.original_dir)
+        cls.tmpdir.cleanup()
 
     def setUp(self):
         """Clean orphaned content before each test."""
         delete_orphans()
 
     def test_on_demand_sync(self):
         """Test on_demand synchronization."""
```

### Comparing `pulp-ostree-2.0.0a6/pulp_ostree/tests/functional/constants.py` & `pulp-ostree-2.1.0/pulp_ostree/tests/functional/constants.py`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.0.0a6/pulp_ostree/tests/functional/utils.py` & `pulp-ostree-2.1.0/pulp_ostree/tests/functional/utils.py`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.0.0a6/pulp_ostree.egg-info/PKG-INFO` & `pulp-ostree-2.1.0/pulp_ostree.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-ostree
-Version: 2.0.0a6
+Version: 2.1.0
 Summary: OSTree plugin for the Pulp Project
 Home-page: http://www.pulpproject.org
 Author: Pulp Project Developers
 Author-email: pulp-list@redhat.com
 License: GPLv2+
 Description: ![Nightly CI/CD](https://github.com/pulp/pulp_ostree/actions/workflows/nightly.yml/badge.svg?branch=main)
         
@@ -14,15 +14,15 @@
         A Pulp plugin to support hosting your own OSTree content.
         
         For more information, please see the [documentation](https://docs.pulpproject.org/pulp_ostree/) or the [Pulp project page](https://pulpproject.org/).
         
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulp-ostree-2.0.0a6/pulp_ostree.egg-info/SOURCES.txt` & `pulp-ostree-2.1.0/pulp_ostree.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 pulp_ostree/app/models.py
 pulp_ostree/app/serializers.py
 pulp_ostree/app/viewsets.py
 pulp_ostree/app/migrations/0001_initial.py
 pulp_ostree/app/migrations/0002_add_relative_path_uniqueness.py
 pulp_ostree/app/migrations/0003_create_many_to_many_objs_commits.py
 pulp_ostree/app/migrations/0004_add_include_exclude_refs.py
+pulp_ostree/app/migrations/0005_add_static_delta_support.py
+pulp_ostree/app/migrations/0006_alter_pointers_to_related_models_globally.py
 pulp_ostree/app/migrations/__init__.py
 pulp_ostree/app/tasks/__init__.py
 pulp_ostree/app/tasks/importing.py
 pulp_ostree/app/tasks/modifying.py
 pulp_ostree/app/tasks/stages.py
 pulp_ostree/app/tasks/synchronizing.py
 pulp_ostree/app/tasks/utils.py
```

### Comparing `pulp-ostree-2.0.0a6/pyproject.toml` & `pulp-ostree-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -69,13 +69,14 @@
     ".bumpversion.cfg",
     "CHANGES/**",
     "CONTRIBUTING.rst",
     "HISTORY.rst",
     "dev_requirements.txt",
     "doc_requirements.txt",
     "docs/**",
-    "flake8.cfg",
     "template_config.yml",
     ".ci/**",
     ".github/**",
+    "lint_requirements.txt",
+    ".flake8",
 ]
```

### Comparing `pulp-ostree-2.0.0a6/setup.py` & `pulp-ostree-2.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,30 +6,30 @@
     requirements = requirements.readlines()
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="pulp-ostree",
-    version="2.0.0a6",
+    version="2.1.0",
     description="OSTree plugin for the Pulp Project",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="GPLv2+",
     author="Pulp Project Developers",
     author_email="pulp-list@redhat.com",
     url="http://www.pulpproject.org",
     python_requires=">=3.8",
     install_requires=requirements,
     include_package_data=True,
     packages=find_packages(exclude=["tests"]),
     classifiers=[
         "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
         "Operating System :: POSIX :: Linux",
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 5 - Production/Stable",
         "Framework :: Django",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
     entry_points={"pulpcore.plugin": ["pulp_ostree = pulp_ostree:default_app_config"]},
```

