# Comparing `tmp/johnsnowlabs-4.4.5.tar.gz` & `tmp/johnsnowlabs-4.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "johnsnowlabs-4.4.5.tar", last modified: Wed May  3 11:42:03 2023, max compression
+gzip compressed data, was "johnsnowlabs-4.4.6.tar", last modified: Sun May 28 18:43:03 2023, max compression
```

## Comparing `johnsnowlabs-4.4.5.tar` & `johnsnowlabs-4.4.6.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-03 11:42:03.539852 johnsnowlabs-4.4.5/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    11356 2023-03-31 15:38:35.000000 johnsnowlabs-4.4.5/LICENSE
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9278 2023-05-03 11:42:03.539852 johnsnowlabs-4.4.5/PKG-INFO
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8307 2023-03-31 15:38:35.000000 johnsnowlabs-4.4.5/README.md
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-03 11:42:03.535852 johnsnowlabs-4.4.5/johnsnowlabs/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      932 2023-04-26 14:30:28.000000 johnsnowlabs-4.4.5/johnsnowlabs/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-03 11:42:03.535852 johnsnowlabs-4.4.5/johnsnowlabs/abstract_base/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.5/johnsnowlabs/abstract_base/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      395 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/abstract_base/base_enum.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9775 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/abstract_base/lib_resolver.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      733 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/abstract_base/pydantic_model.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9287 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/abstract_base/software_product.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-03 11:42:03.535852 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-03 11:42:03.535852 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/databricks/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/databricks/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2623 2023-03-26 01:30:02.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/databricks/dbfs.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12144 2023-03-26 01:30:02.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/databricks/install_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6612 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/databricks/work_utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-03 11:42:03.535852 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/health_checks/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/health_checks/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      973 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/health_checks/hc_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      884 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/health_checks/nlp_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2076 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/health_checks/ocr_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3496 2023-03-30 22:32:50.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/health_checks/report.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6935 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/install_flow.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    11362 2023-02-01 13:41:22.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/install_software.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12079 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/jsl_home.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-03 11:42:03.535852 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/lib_resolvers/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      124 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/lib_resolvers/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2061 2023-04-13 00:38:10.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3187 2023-04-26 21:13:04.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2105 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8828 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/offline_install.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9133 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/softwares.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4710 2023-04-26 14:30:28.000000 johnsnowlabs-4.4.5/johnsnowlabs/finance.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      212 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/lab.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4639 2023-04-26 14:30:28.000000 johnsnowlabs-4.4.5/johnsnowlabs/legal.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4526 2023-04-26 14:30:28.000000 johnsnowlabs-4.4.5/johnsnowlabs/medical.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1367 2023-04-13 01:03:52.000000 johnsnowlabs-4.4.5/johnsnowlabs/nlp.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-03 11:42:03.539852 johnsnowlabs-4.4.5/johnsnowlabs/py_models/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.5/johnsnowlabs/py_models/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4826 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/py_models/install_info.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    31165 2023-03-26 01:30:02.000000 johnsnowlabs-4.4.5/johnsnowlabs/py_models/jsl_secrets.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4168 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/py_models/lib_version.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        2 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/py_models/license_info.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      128 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/py_models/primitive.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2079 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/py_models/url_dependency.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2201 2023-05-03 11:36:35.000000 johnsnowlabs-4.4.5/johnsnowlabs/settings.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-03 11:42:03.539852 johnsnowlabs-4.4.5/johnsnowlabs/utils/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6657 2023-03-31 10:39:36.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/enums.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4253 2023-04-26 21:13:04.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/env_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      759 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/file_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1005 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/functional.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3326 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/modelhub_markdown.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10004 2023-03-19 17:22:02.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/my_jsl_api.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10654 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/notebooks.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5856 2023-01-31 09:04:19.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/pip_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      982 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/print_messages.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4371 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/py_process.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8019 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/sparksession_utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-03 11:42:03.539852 johnsnowlabs-4.4.5/johnsnowlabs/utils/testing/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:29:40.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/testing/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4050 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/testing/jsl_pre_processor.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1778 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/testing/nb_code_match.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1132 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/testing/nb_nodes.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3460 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/testing/test_settings.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4353 2023-04-26 21:13:04.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/venv_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1332 2023-04-26 14:30:28.000000 johnsnowlabs-4.4.5/johnsnowlabs/visual.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      408 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/viz.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-03 11:42:03.535852 johnsnowlabs-4.4.5/johnsnowlabs.egg-info/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9278 2023-05-03 11:42:03.000000 johnsnowlabs-4.4.5/johnsnowlabs.egg-info/PKG-INFO
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2466 2023-05-03 11:42:03.000000 johnsnowlabs-4.4.5/johnsnowlabs.egg-info/SOURCES.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2023-05-03 11:42:03.000000 johnsnowlabs-4.4.5/johnsnowlabs.egg-info/dependency_links.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      126 2023-05-03 11:42:03.000000 johnsnowlabs-4.4.5/johnsnowlabs.egg-info/requires.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       13 2023-05-03 11:42:03.000000 johnsnowlabs-4.4.5/johnsnowlabs.egg-info/top_level.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       38 2023-05-03 11:42:03.539852 johnsnowlabs-4.4.5/setup.cfg
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2054 2023-04-26 21:10:35.000000 johnsnowlabs-4.4.5/setup.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-28 18:43:03.662166 johnsnowlabs-4.4.6/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11356 2023-03-31 15:38:35.000000 johnsnowlabs-4.4.6/LICENSE
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9278 2023-05-28 18:43:03.662166 johnsnowlabs-4.4.6/PKG-INFO
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8307 2023-03-31 15:38:35.000000 johnsnowlabs-4.4.6/README.md
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-28 18:43:03.662166 johnsnowlabs-4.4.6/johnsnowlabs/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      932 2023-04-26 14:30:28.000000 johnsnowlabs-4.4.6/johnsnowlabs/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-28 18:43:03.662166 johnsnowlabs-4.4.6/johnsnowlabs/abstract_base/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.6/johnsnowlabs/abstract_base/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      395 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.6/johnsnowlabs/abstract_base/base_enum.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9794 2023-05-28 18:29:17.000000 johnsnowlabs-4.4.6/johnsnowlabs/abstract_base/lib_resolver.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      733 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.6/johnsnowlabs/abstract_base/pydantic_model.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9287 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.6/johnsnowlabs/abstract_base/software_product.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-28 18:43:03.662166 johnsnowlabs-4.4.6/johnsnowlabs/auto_install/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.6/johnsnowlabs/auto_install/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-28 18:43:03.662166 johnsnowlabs-4.4.6/johnsnowlabs/auto_install/databricks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.6/johnsnowlabs/auto_install/databricks/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2623 2023-03-26 01:30:02.000000 johnsnowlabs-4.4.6/johnsnowlabs/auto_install/databricks/dbfs.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12144 2023-03-26 01:30:02.000000 johnsnowlabs-4.4.6/johnsnowlabs/auto_install/databricks/install_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6612 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.6/johnsnowlabs/auto_install/databricks/work_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-28 18:43:03.662166 johnsnowlabs-4.4.6/johnsnowlabs/auto_install/health_checks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.6/johnsnowlabs/auto_install/health_checks/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      973 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.6/johnsnowlabs/auto_install/health_checks/hc_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      884 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.6/johnsnowlabs/auto_install/health_checks/nlp_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2076 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.6/johnsnowlabs/auto_install/health_checks/ocr_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3496 2023-03-30 22:32:50.000000 johnsnowlabs-4.4.6/johnsnowlabs/auto_install/health_checks/report.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6935 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.6/johnsnowlabs/auto_install/install_flow.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11362 2023-02-01 13:41:22.000000 johnsnowlabs-4.4.6/johnsnowlabs/auto_install/install_software.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12178 2023-05-26 21:55:38.000000 johnsnowlabs-4.4.6/johnsnowlabs/auto_install/jsl_home.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-28 18:43:03.662166 johnsnowlabs-4.4.6/johnsnowlabs/auto_install/lib_resolvers/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      124 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.6/johnsnowlabs/auto_install/lib_resolvers/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2061 2023-05-25 04:21:48.000000 johnsnowlabs-4.4.6/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3187 2023-05-25 02:23:06.000000 johnsnowlabs-4.4.6/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2105 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.6/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9118 2023-05-16 20:30:52.000000 johnsnowlabs-4.4.6/johnsnowlabs/auto_install/offline_install.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9133 2023-05-28 17:28:52.000000 johnsnowlabs-4.4.6/johnsnowlabs/auto_install/softwares.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4710 2023-04-26 14:30:28.000000 johnsnowlabs-4.4.6/johnsnowlabs/finance.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      212 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.6/johnsnowlabs/lab.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4639 2023-04-26 14:30:28.000000 johnsnowlabs-4.4.6/johnsnowlabs/legal.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4526 2023-05-28 17:25:36.000000 johnsnowlabs-4.4.6/johnsnowlabs/medical.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1367 2023-04-13 01:03:52.000000 johnsnowlabs-4.4.6/johnsnowlabs/nlp.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-28 18:43:03.662166 johnsnowlabs-4.4.6/johnsnowlabs/py_models/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.6/johnsnowlabs/py_models/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4925 2023-05-26 21:57:49.000000 johnsnowlabs-4.4.6/johnsnowlabs/py_models/install_info.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    31165 2023-03-26 01:30:02.000000 johnsnowlabs-4.4.6/johnsnowlabs/py_models/jsl_secrets.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4168 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.6/johnsnowlabs/py_models/lib_version.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        2 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.6/johnsnowlabs/py_models/license_info.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      128 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.6/johnsnowlabs/py_models/primitive.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2077 2023-05-16 20:23:18.000000 johnsnowlabs-4.4.6/johnsnowlabs/py_models/url_dependency.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2200 2023-05-28 18:42:02.000000 johnsnowlabs-4.4.6/johnsnowlabs/settings.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-28 18:43:03.662166 johnsnowlabs-4.4.6/johnsnowlabs/utils/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.6/johnsnowlabs/utils/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6657 2023-03-31 10:39:36.000000 johnsnowlabs-4.4.6/johnsnowlabs/utils/enums.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4409 2023-05-26 12:08:46.000000 johnsnowlabs-4.4.6/johnsnowlabs/utils/env_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      759 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.6/johnsnowlabs/utils/file_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1005 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.6/johnsnowlabs/utils/functional.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3326 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.6/johnsnowlabs/utils/modelhub_markdown.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10004 2023-03-19 17:22:02.000000 johnsnowlabs-4.4.6/johnsnowlabs/utils/my_jsl_api.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10654 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.6/johnsnowlabs/utils/notebooks.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5856 2023-01-31 09:04:19.000000 johnsnowlabs-4.4.6/johnsnowlabs/utils/pip_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      982 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.6/johnsnowlabs/utils/print_messages.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4371 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.6/johnsnowlabs/utils/py_process.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8127 2023-05-21 06:35:03.000000 johnsnowlabs-4.4.6/johnsnowlabs/utils/sparksession_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-28 18:43:03.662166 johnsnowlabs-4.4.6/johnsnowlabs/utils/testing/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:29:40.000000 johnsnowlabs-4.4.6/johnsnowlabs/utils/testing/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4050 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.6/johnsnowlabs/utils/testing/jsl_pre_processor.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1778 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.6/johnsnowlabs/utils/testing/nb_code_match.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1132 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.6/johnsnowlabs/utils/testing/nb_nodes.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3460 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.6/johnsnowlabs/utils/testing/test_settings.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4353 2023-04-26 21:13:04.000000 johnsnowlabs-4.4.6/johnsnowlabs/utils/venv_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1332 2023-04-26 14:30:28.000000 johnsnowlabs-4.4.6/johnsnowlabs/visual.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      408 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.6/johnsnowlabs/viz.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-28 18:43:03.662166 johnsnowlabs-4.4.6/johnsnowlabs.egg-info/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9278 2023-05-28 18:43:03.000000 johnsnowlabs-4.4.6/johnsnowlabs.egg-info/PKG-INFO
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2466 2023-05-28 18:43:03.000000 johnsnowlabs-4.4.6/johnsnowlabs.egg-info/SOURCES.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2023-05-28 18:43:03.000000 johnsnowlabs-4.4.6/johnsnowlabs.egg-info/dependency_links.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      126 2023-05-28 18:43:03.000000 johnsnowlabs-4.4.6/johnsnowlabs.egg-info/requires.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       13 2023-05-28 18:43:03.000000 johnsnowlabs-4.4.6/johnsnowlabs.egg-info/top_level.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       38 2023-05-28 18:43:03.662166 johnsnowlabs-4.4.6/setup.cfg
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2063 2023-05-28 17:28:52.000000 johnsnowlabs-4.4.6/setup.py
```

### Comparing `johnsnowlabs-4.4.5/LICENSE` & `johnsnowlabs-4.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/PKG-INFO` & `johnsnowlabs-4.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: johnsnowlabs
-Version: 4.4.5
+Version: 4.4.6
 Summary: The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for Finance, Legal and Medical domains. Easily scalable to Spark Cluster 
 Home-page: https://www.johnsnowlabs.com/
 Author: John Snow Labs
 Author-email: christian@johnsnowlabs.com
 Keywords: Spark NLP OCR Finance Legal Medical John Snow Labs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `johnsnowlabs-4.4.5/README.md` & `johnsnowlabs-4.4.6/README.md`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/__init__.py` & `johnsnowlabs-4.4.6/johnsnowlabs/__init__.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/abstract_base/lib_resolver.py` & `johnsnowlabs-4.4.6/johnsnowlabs/abstract_base/lib_resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,17 +112,17 @@
 
         if cls.has_secret:
             if settings.enforce_versions:
                 url = compat_map[matching_jsl_spark_release][install_type].url.format(
                     secret=secret, lib_version=cls.lib_version.as_str()
                 )
             else:
-                # Read Version from secret
+                # Parse Version from secret
                 url = compat_map[matching_jsl_spark_release][install_type].url.format(
-                    secret=secret, lib_version=secret.split("-")[0]
+                    secret=secret, lib_version=secret.split("-")[0].replace(".PR",'')
                 )
 
         else:
             if settings.enforce_versions:
                 url = compat_map[matching_jsl_spark_release][install_type].url.format(
                     lib_version=cls.lib_version.as_str()
                 )
```

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/abstract_base/pydantic_model.py` & `johnsnowlabs-4.4.6/johnsnowlabs/abstract_base/pydantic_model.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/abstract_base/software_product.py` & `johnsnowlabs-4.4.6/johnsnowlabs/abstract_base/software_product.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/databricks/dbfs.py` & `johnsnowlabs-4.4.6/johnsnowlabs/auto_install/databricks/dbfs.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/databricks/install_utils.py` & `johnsnowlabs-4.4.6/johnsnowlabs/auto_install/databricks/install_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/databricks/work_utils.py` & `johnsnowlabs-4.4.6/johnsnowlabs/auto_install/databricks/work_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/health_checks/hc_test.py` & `johnsnowlabs-4.4.6/johnsnowlabs/auto_install/health_checks/hc_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/health_checks/nlp_test.py` & `johnsnowlabs-4.4.6/johnsnowlabs/auto_install/health_checks/nlp_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/health_checks/ocr_test.py` & `johnsnowlabs-4.4.6/johnsnowlabs/auto_install/health_checks/ocr_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/health_checks/report.py` & `johnsnowlabs-4.4.6/johnsnowlabs/auto_install/health_checks/report.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/install_flow.py` & `johnsnowlabs-4.4.6/johnsnowlabs/auto_install/install_flow.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/install_software.py` & `johnsnowlabs-4.4.6/johnsnowlabs/auto_install/install_software.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/jsl_home.py` & `johnsnowlabs-4.4.6/johnsnowlabs/auto_install/jsl_home.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,16 @@
     aws_key_id: Optional[str] = None,
     fin_license: Optional[str] = None,
     leg_license: Optional[str] = None,
     store_in_jsl_home: bool = True,
     log: bool = True,
 ) -> InstallSuite:
     """Read all info files from JSL home if exists. If not exists, sets up JSL home"""
-
+    if not jsl_home_exist() and not create_jsl_home_if_missing:
+        return InstallSuite.empty()
     license_data: JslSecrets = JslSecrets.build_or_try_find_secrets(
         browser_login=browser_login,
         force_browser=force_browser,
         access_token=access_token,
         local_license_number=local_license_number,
         remote_license_number=remote_license_number,
         secrets_file=secrets_file,
```

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py` & `johnsnowlabs-4.4.6/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py` & `johnsnowlabs-4.4.6/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py` & `johnsnowlabs-4.4.6/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/offline_install.py` & `johnsnowlabs-4.4.6/johnsnowlabs/auto_install/offline_install.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,28 @@
+
+import requests
 from typing import List, Tuple
 
+from johnsnowlabs import settings
+
 from johnsnowlabs.auto_install.lib_resolvers import (
     OcrLibResolver,
     HcLibResolver,
     NlpLibResolver,
 )
 from johnsnowlabs.py_models.jsl_secrets import JslSecrets
 from johnsnowlabs.py_models.url_dependency import UrlDependency
 from johnsnowlabs.utils.enums import PyInstallTypes, ProductLogo, JvmHardwareTarget
 
 
 def get_printable_dependency_urls(
-    secrets: JslSecrets,
-    jvm_install_type: JvmHardwareTarget = JvmHardwareTarget.cpu,
-    py_install_type: PyInstallTypes = PyInstallTypes.wheel,
-    spark_version=None,
+        secrets: JslSecrets,
+        jvm_install_type: JvmHardwareTarget = JvmHardwareTarget.cpu,
+        py_install_type: PyInstallTypes = PyInstallTypes.wheel,
+        spark_version=None,
 ) -> Tuple[List[str], List[str]]:
     """
     Get URL for every dependency to which the found_secrets have access to with respect to CURRENT pyspark install.
     If no pyspark is installed, this fails because we need to know pyspark version to generate correct URL
     :param jvm_install_type:
     :param spark_version:
     :param secrets:
@@ -91,22 +95,22 @@
     print(
         f"Make sure all these dependencies are installed on your Spark Driver and Worker nodes"
     )
     return java_dependencies, py_dependencies
 
 
 def get_py4j_dependency_urls(
-    secrets: JslSecrets,
-    jvm_install_type: JvmHardwareTarget = JvmHardwareTarget.cpu,
-    py_install_type: PyInstallTypes = PyInstallTypes.wheel,
-    spark_version=None,
-    get_all_jvm_hardware_targets: bool = False,
-    visual=False,
-    nlp=True,
-    spark_nlp=True,
+        secrets: JslSecrets,
+        jvm_install_type: JvmHardwareTarget = JvmHardwareTarget.cpu,
+        py_install_type: PyInstallTypes = PyInstallTypes.wheel,
+        spark_version=None,
+        get_all_jvm_hardware_targets: bool = False,
+        visual=False,
+        nlp=True,
+        spark_nlp=True,
 ) -> Tuple[List[UrlDependency], List[UrlDependency]]:
     """
     Get URL for every dependency to which the found_secrets have access to with respect to CURRENT pyspark install.
     If no pyspark is installed, this fails because we need to know pyspark version to generate correct URL
     :param jvm_install_type:
     :param spark_version:
     :param get_all_jvm_hardware_targets:
@@ -138,25 +142,17 @@
                 NlpLibResolver.get_jar_urls(
                     hardware_target=jvm_install_type,
                     spark_version_to_match=spark_version,
                 )
             )
 
         if py_install_type == PyInstallTypes.wheel:
-            py_dependencies.append(
-                NlpLibResolver.get_py_urls(
-                    install_type=py_install_type, spark_version_to_match=spark_version
-                )
-            )
-        else:
-            py_dependencies.append(
-                NlpLibResolver.get_py_urls(
-                    install_type=py_install_type, spark_version_to_match=spark_version
-                )
-            )
+            url = NlpLibResolver.get_py_urls(install_type=py_install_type, spark_version_to_match=spark_version)
+            url.url = get_wheel_and_pypi('spark-nlp', settings.raw_version_nlp)[0]
+            py_dependencies.append(url)
 
     if secrets and secrets.HC_SECRET and nlp:
         java_dependencies.append(
             HcLibResolver.get_jar_urls(
                 secret=secrets.HC_SECRET, spark_version_to_match=spark_version
             )
         )
@@ -164,22 +160,14 @@
             py_dependencies.append(
                 HcLibResolver.get_py_urls(
                     secret=secrets.HC_SECRET,
                     install_type=py_install_type,
                     spark_version_to_match=spark_version,
                 )
             )
-        else:
-            py_dependencies.append(
-                HcLibResolver.get_py_urls(
-                    secret=secrets.HC_SECRET,
-                    install_type=py_install_type,
-                    spark_version_to_match=spark_version,
-                )
-            )
 
     if secrets and secrets.OCR_SECRET and visual:
         java_dependencies.append(
             OcrLibResolver.get_jar_urls(
                 secret=secrets.OCR_SECRET, spark_version_to_match=spark_version
             )
         )
@@ -187,17 +175,37 @@
             py_dependencies.append(
                 OcrLibResolver.get_py_urls(
                     secret=secrets.OCR_SECRET,
                     install_type=py_install_type,
                     spark_version_to_match=spark_version,
                 )
             )
-        else:
-            py_dependencies.append(
-                OcrLibResolver.get_py_urls(
-                    secret=secrets.OCR_SECRET,
-                    install_type=py_install_type,
-                    spark_version_to_match=spark_version,
-                )
-            )
 
     return java_dependencies, py_dependencies
+
+def get_wheel_and_pypi(pypi_name, version):
+    # Construct the API URL
+    api_url = f"https://pypi.org/pypi/{pypi_name}/{version}/json"
+
+    try:
+        # Send a GET request to the PyPI API
+        response = requests.get(api_url)
+        response.raise_for_status()  # Raise an exception for any HTTP errors
+
+        # Parse the JSON response
+        data = response.json()
+
+        wheel_url = None
+        tarball_url = None
+
+        # Extract the download URLs for wheels and tarballs
+        for release in data["urls"]:
+            if release["packagetype"] == "bdist_wheel":
+                wheel_url = release["url"]
+            elif release["packagetype"] == "sdist":
+                tarball_url = release["url"]
+
+        return wheel_url, tarball_url
+
+    except requests.exceptions.RequestException as e:
+        print(f"Could not find Pypi Wheel/Tar for {pypi_name}=={version}: {e}")
+        return None, None
```

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/softwares.py` & `johnsnowlabs-4.4.6/johnsnowlabs/auto_install/softwares.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/finance.py` & `johnsnowlabs-4.4.6/johnsnowlabs/finance.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/legal.py` & `johnsnowlabs-4.4.6/johnsnowlabs/legal.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/medical.py` & `johnsnowlabs-4.4.6/johnsnowlabs/medical.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/nlp.py` & `johnsnowlabs-4.4.6/johnsnowlabs/nlp.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/py_models/install_info.py` & `johnsnowlabs-4.4.6/johnsnowlabs/py_models/install_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,23 +100,26 @@
     def py_folder_from_home():
         if os.path.exists(settings.py_info_file):
             return InstallFolder.parse_file(settings.py_info_file)
         return False
 
 
 class InstallSuite(WritableBaseModel):
-    info: RootInfo
+    info: Optional[RootInfo] = None
     secrets: Optional[JslSecrets] = None
     # Py4J Libs
-    nlp: LocalPy4JLib
+    nlp: Optional[LocalPy4JLib] = None
     ocr: Optional[LocalPy4JLib] = None
     hc: Optional[LocalPy4JLib] = None
     # Pure Python Libs
     pure_py_jsl: Optional[LocalPyLib] = None
 
+    @staticmethod
+    def empty():
+        return InstallSuite()
     def get_missing_products(self, nlp, visual, spark_nlp):
         missing = []
         from johnsnowlabs.auto_install.softwares import Software
 
         if self.secrets.OCR_LICENSE and visual:
             if not self.ocr.java_lib or not self.ocr.get_java_path():
                 missing.append(Software.spark_ocr)
```

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/py_models/jsl_secrets.py` & `johnsnowlabs-4.4.6/johnsnowlabs/py_models/jsl_secrets.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/py_models/lib_version.py` & `johnsnowlabs-4.4.6/johnsnowlabs/py_models/lib_version.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/py_models/url_dependency.py` & `johnsnowlabs-4.4.6/johnsnowlabs/py_models/url_dependency.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,17 @@
             return False
 
     def download_url(
         self, save_path, name_print_prefix: str = "", keep_default_file_name=True
     ):
         if not UrlDependency.internet_on():
             print(
-                f"Warning! It looks like there is no active internet connection on this machine"
+                f"Warning! It looks like there is no active internet connection on this machine "
+                f"Trying to continue but might run into problems..."
             )
-            print(f"Trying to continue but might run into problems...")
 
         if not self.validate():
             raise ValueError(f"Trying to download Invalid URL! {self.url}")
         if keep_default_file_name:
             self.file_name = self.url.split("/")[-1]
         save_path = save_path + "/" + self.file_name
```

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/settings.py` & `johnsnowlabs-4.4.6/johnsnowlabs/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,28 +4,27 @@
 from johnsnowlabs.utils.env_utils import (
     is_running_in_databricks,
     set_py4j_logger_to_error_on_databricks,
     env_required_license,
 )
 
 # These versions are used for auto-installs and version  checks
-raw_version_jsl_lib = "4.4.5"
+raw_version_jsl_lib = "4.4.6"
 raw_version_nlp = "4.4.1"
 raw_version_nlu = "4.2.0"
 raw_version_pyspark = "3.1.2"
 raw_version_nlp_display = "4.1"
 
-raw_version_medical = "4.4.1"
-raw_version_secret_medical = "4.4.1"
+raw_version_medical = "4.4.2"
+raw_version_secret_medical = "4.4.2"
 
-raw_version_secret_ocr = "4.4.0"
-raw_version_ocr = "4.4.0"
+raw_version_secret_ocr = "4.4.1"
+raw_version_ocr = "4.4.1"
 
 pypi_page = "https://pypi.org/project/johnsnowlabs"
-
 json_indent = 4
 enforce_secret_on_version = False
 enforce_versions = True
 
 # Environment
 on_databricks = is_running_in_databricks()
 license_required = env_required_license()
```

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/utils/enums.py` & `johnsnowlabs-4.4.6/johnsnowlabs/utils/enums.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/utils/env_utils.py` & `johnsnowlabs-4.4.6/johnsnowlabs/utils/env_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,12 +117,16 @@
     ):
         return False
     return True
 
 
 def set_py4j_logger_to_error_on_databricks():
     # Only call this when in Databricks
-    import logging
-    from pyspark.sql import SparkSession
-
-    logger = SparkSession.builder.getOrCreate()._jvm.org.apache.log4j
-    logging.getLogger("py4j.java_gateway").setLevel(logging.ERROR)
+    try:
+        if 'SKIP_py4j_DISABLE' in os.environ and os.environ['SKIP_py4j_DISABLE'] == '1':
+            return
+        import logging
+        from pyspark.sql import SparkSession
+        logger = SparkSession.builder.getOrCreate()._jvm.org.apache.log4j
+        logging.getLogger("py4j.java_gateway").setLevel(logging.ERROR)
+    except:
+        pass
```

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/utils/file_utils.py` & `johnsnowlabs-4.4.6/johnsnowlabs/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/utils/functional.py` & `johnsnowlabs-4.4.6/johnsnowlabs/utils/functional.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/utils/modelhub_markdown.py` & `johnsnowlabs-4.4.6/johnsnowlabs/utils/modelhub_markdown.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/utils/my_jsl_api.py` & `johnsnowlabs-4.4.6/johnsnowlabs/utils/my_jsl_api.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/utils/notebooks.py` & `johnsnowlabs-4.4.6/johnsnowlabs/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/utils/pip_utils.py` & `johnsnowlabs-4.4.6/johnsnowlabs/utils/pip_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/utils/print_messages.py` & `johnsnowlabs-4.4.6/johnsnowlabs/utils/print_messages.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/utils/py_process.py` & `johnsnowlabs-4.4.6/johnsnowlabs/utils/py_process.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/utils/sparksession_utils.py` & `johnsnowlabs-4.4.6/johnsnowlabs/utils/sparksession_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,14 +69,15 @@
     jar_paths: List[str] = None,
     # spark_nlp corresponds to enterprise NLP jar
     spark_nlp: bool = True,
     nlp: bool = True,
     visual: bool = False,
     hardware_target: str = JvmHardwareTarget.cpu.value,
     model_cache_folder: str = None,
+    create_jsl_home_if_missing: bool = True,
 ) -> "pyspark.sql.SparkSession":
     from pyspark.sql import SparkSession
 
     already_launched = False
     if (
         "_instantiatedSession" in dir(SparkSession)
         and SparkSession._instantiatedSession is not None
@@ -89,14 +90,15 @@
             )
 
     launched_products: List[str] = []
     hardware_target = JvmHardwareTarget.from_str(hardware_target)
 
     # Get all Local Jar Paths, downloads them if missing
     suite = get_install_suite_from_jsl_home(
+        create_jsl_home_if_missing=create_jsl_home_if_missing,
         only_jars=True,
         jvm_hardware_target=hardware_target,
         force_browser=browser_login,
         browser_login=browser_login,
         access_token=access_token,
         local_license_number=local_license_number,
         remote_license_number=remote_license_number,
```

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/utils/testing/jsl_pre_processor.py` & `johnsnowlabs-4.4.6/johnsnowlabs/utils/testing/jsl_pre_processor.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/utils/testing/nb_code_match.py` & `johnsnowlabs-4.4.6/johnsnowlabs/utils/testing/nb_code_match.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/utils/testing/nb_nodes.py` & `johnsnowlabs-4.4.6/johnsnowlabs/utils/testing/nb_nodes.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/utils/testing/test_settings.py` & `johnsnowlabs-4.4.6/johnsnowlabs/utils/testing/test_settings.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/utils/venv_utils.py` & `johnsnowlabs-4.4.6/johnsnowlabs/utils/venv_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs/visual.py` & `johnsnowlabs-4.4.6/johnsnowlabs/visual.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs.egg-info/PKG-INFO` & `johnsnowlabs-4.4.6/johnsnowlabs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: johnsnowlabs
-Version: 4.4.5
+Version: 4.4.6
 Summary: The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for Finance, Legal and Medical domains. Easily scalable to Spark Cluster 
 Home-page: https://www.johnsnowlabs.com/
 Author: John Snow Labs
 Author-email: christian@johnsnowlabs.com
 Keywords: Spark NLP OCR Finance Legal Medical John Snow Labs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `johnsnowlabs-4.4.5/johnsnowlabs.egg-info/SOURCES.txt` & `johnsnowlabs-4.4.6/johnsnowlabs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.5/setup.py` & `johnsnowlabs-4.4.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 import johnsnowlabs.settings
-
 here = path.abspath(path.dirname(__file__))
 
-with open(path.join(here, "README.md"), encoding="utf-8") as f:
+with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 REQUIRED_PKGS = [
-    f"pyspark=={johnsnowlabs.settings.raw_version_pyspark}",
-    f"spark-nlp=={johnsnowlabs.settings.raw_version_nlp}",
-    f"nlu=={johnsnowlabs.settings.raw_version_nlu}",
-    f"spark-nlp-display=={johnsnowlabs.settings.raw_version_nlp_display}",
-    "numpy",
-    "dataclasses",
-    "requests",
-    "databricks-api",
-    "pydantic",
-    "colorama",
+    f'pyspark=={johnsnowlabs.settings.raw_version_pyspark}',
+    f'spark-nlp=={johnsnowlabs.settings.raw_version_nlp}',
+    f'nlu=={johnsnowlabs.settings.raw_version_nlu}',
+    f'spark-nlp-display=={johnsnowlabs.settings.raw_version_nlp_display}',
+    'numpy',
+    'dataclasses',
+    'requests',
+    'databricks-api',
+    'pydantic',
+    'colorama'
 ]
 
 setup(
     version=johnsnowlabs.settings.raw_version_jsl_lib,
-    # name="johnsnowlabs_for_databricks",
-    name="johnsnowlabs",
-    description="The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for "
-    "Finance, Legal and Medical domains. Easily scalable to Spark Cluster ",
+    # name='johnsnowlabs_for_databricks',
+    name='johnsnowlabs',
+    description='The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for '
+                'Finance, Legal and Medical domains. Easily scalable to Spark Cluster ',
     long_description=long_description,
     install_requires=REQUIRED_PKGS,
-    long_description_content_type="text/markdown",
-    url="https://www.johnsnowlabs.com/",
-    author="John Snow Labs",
-    author_email="christian@johnsnowlabs.com",
+    long_description_content_type='text/markdown',
+    url='https://www.johnsnowlabs.com/',
+    author='John Snow Labs',
+    author_email='christian@johnsnowlabs.com',
     classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Developers",
-        "Topic :: Software Development :: Build Tools",
-        "License :: OSI Approved :: Apache Software License",
+        'Development Status :: 5 - Production/Stable',
+        'Intended Audience :: Developers',
+        'Topic :: Software Development :: Build Tools',
+        'License :: OSI Approved :: Apache Software License',
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.4",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.4',
+        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
     ],
-    keywords="Spark NLP OCR Finance Legal Medical John Snow Labs  ",
-    packages=find_packages(exclude=["test*", "tmp*"]),  # exclude=['test']
-    include_package_data=True,
+    keywords='Spark NLP OCR Finance Legal Medical John Snow Labs  ',
+    packages=find_packages(exclude=['test*', 'tmp*']),  # exclude=['test']
+    include_package_data=True
 )
```

