# Comparing `tmp/cfn-stk-0.15.1.tar.gz` & `tmp/cfn-stk-0.15.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfn-stk-0.15.1.tar", last modified: Mon May  1 10:17:34 2023, max compression
+gzip compressed data, was "cfn-stk-0.15.2.tar", last modified: Sat May 27 23:18:39 2023, max compression
```

## Comparing `cfn-stk-0.15.1.tar` & `cfn-stk-0.15.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 johnw      (501) staff       (20)        0 2023-05-01 10:17:34.325677 cfn-stk-0.15.1/
--rw-r--r--   0 johnw      (501) staff       (20)     1080 2022-04-22 05:39:32.000000 cfn-stk-0.15.1/LICENSE.txt
--rw-r--r--   0 johnw      (501) staff       (20)    20877 2023-05-01 10:17:34.325980 cfn-stk-0.15.1/PKG-INFO
--rw-r--r--   0 johnw      (501) staff       (20)    20400 2023-04-21 22:10:37.000000 cfn-stk-0.15.1/README.md
--rw-r--r--   0 johnw      (501) staff       (20)      154 2023-04-21 09:38:32.000000 cfn-stk-0.15.1/pyproject.toml
--rw-r--r--   0 johnw      (501) staff       (20)      901 2023-05-01 10:17:34.326900 cfn-stk-0.15.1/setup.cfg
-drwxr-xr-x   0 johnw      (501) staff       (20)        0 2023-05-01 10:17:34.288703 cfn-stk-0.15.1/src/
-drwxr-xr-x   0 johnw      (501) staff       (20)        0 2023-05-01 10:17:34.295256 cfn-stk-0.15.1/src/cfn_stk.egg-info/
--rw-r--r--   0 johnw      (501) staff       (20)    20877 2023-05-01 10:17:34.000000 cfn-stk-0.15.1/src/cfn_stk.egg-info/PKG-INFO
--rw-r--r--   0 johnw      (501) staff       (20)     1303 2023-05-01 10:17:34.000000 cfn-stk-0.15.1/src/cfn_stk.egg-info/SOURCES.txt
--rw-r--r--   0 johnw      (501) staff       (20)        1 2023-05-01 10:17:34.000000 cfn-stk-0.15.1/src/cfn_stk.egg-info/dependency_links.txt
--rw-r--r--   0 johnw      (501) staff       (20)       54 2023-05-01 10:17:34.000000 cfn-stk-0.15.1/src/cfn_stk.egg-info/entry_points.txt
--rw-r--r--   0 johnw      (501) staff       (20)        1 2023-04-21 10:00:31.000000 cfn-stk-0.15.1/src/cfn_stk.egg-info/not-zip-safe
--rw-r--r--   0 johnw      (501) staff       (20)      134 2023-05-01 10:17:34.000000 cfn-stk-0.15.1/src/cfn_stk.egg-info/requires.txt
--rw-r--r--   0 johnw      (501) staff       (20)        4 2023-05-01 10:17:34.000000 cfn-stk-0.15.1/src/cfn_stk.egg-info/top_level.txt
-drwxr-xr-x   0 johnw      (501) staff       (20)        0 2023-05-01 10:17:34.312582 cfn-stk-0.15.1/src/stk/
--rw-r--r--   0 johnw      (501) staff       (20)     1049 2023-05-01 09:54:44.000000 cfn-stk-0.15.1/src/stk/__init__.py
--rw-r--r--   0 johnw      (501) staff       (20)     3884 2023-04-16 07:13:04.000000 cfn-stk-0.15.1/src/stk/aws_config.py
--rw-r--r--   0 johnw      (501) staff       (20)     2876 2023-01-30 23:26:06.000000 cfn-stk-0.15.1/src/stk/basic_stack.py
--rw-r--r--   0 johnw      (501) staff       (20)     1769 2022-06-09 21:19:18.000000 cfn-stk-0.15.1/src/stk/cfn_bucket.py
--rw-r--r--   0 johnw      (501) staff       (20)     5710 2023-01-31 00:05:56.000000 cfn-stk-0.15.1/src/stk/change_set.py
--rw-r--r--   0 johnw      (501) staff       (20)      186 2022-08-01 23:49:13.000000 cfn-stk-0.15.1/src/stk/chdir.py
--rw-r--r--   0 johnw      (501) staff       (20)    11502 2023-01-31 00:05:56.000000 cfn-stk-0.15.1/src/stk/cli.py
--rw-r--r--   0 johnw      (501) staff       (20)    11211 2023-04-16 07:13:04.000000 cfn-stk-0.15.1/src/stk/config.py
-drwxr-xr-x   0 johnw      (501) staff       (20)        0 2023-05-01 10:17:34.315026 cfn-stk-0.15.1/src/stk/config_cmd/
--rw-r--r--   0 johnw      (501) staff       (20)        0 2022-11-14 21:14:00.000000 cfn-stk-0.15.1/src/stk/config_cmd/__init__.py
--rw-r--r--   0 johnw      (501) staff       (20)     8947 2022-11-28 21:14:54.000000 cfn-stk-0.15.1/src/stk/config_cmd/add_template.py
--rw-r--r--   0 johnw      (501) staff       (20)     2061 2022-11-15 08:25:57.000000 cfn-stk-0.15.1/src/stk/config_cmd/cli.py
--rw-r--r--   0 johnw      (501) staff       (20)     9164 2022-12-13 09:20:13.000000 cfn-stk-0.15.1/src/stk/config_cmd/init.py
--rw-r--r--   0 johnw      (501) staff       (20)     7659 2023-04-16 07:13:04.000000 cfn-stk-0.15.1/src/stk/config_file.py
--rw-r--r--   0 johnw      (501) staff       (20)     2513 2022-05-16 08:31:28.000000 cfn-stk-0.15.1/src/stk/human_bytes.py
--rw-r--r--   0 johnw      (501) staff       (20)     6069 2022-04-22 02:04:14.000000 cfn-stk-0.15.1/src/stk/ignore_file.py
--rw-r--r--   0 johnw      (501) staff       (20)     1261 2022-12-13 05:38:00.000000 cfn-stk-0.15.1/src/stk/interpolated_dict.py
--rw-r--r--   0 johnw      (501) staff       (20)     1523 2022-05-10 10:04:13.000000 cfn-stk-0.15.1/src/stk/multipart_encoder.py
--rw-r--r--   0 johnw      (501) staff       (20)     8891 2023-01-31 00:05:56.000000 cfn-stk-0.15.1/src/stk/provider.py
--rw-r--r--   0 johnw      (501) staff       (20)     4531 2023-04-16 07:13:04.000000 cfn-stk-0.15.1/src/stk/stack.py
--rw-r--r--   0 johnw      (501) staff       (20)     2214 2023-01-30 23:30:53.000000 cfn-stk-0.15.1/src/stk/stack_delegated_command.py
--rw-r--r--   0 johnw      (501) staff       (20)     1016 2022-12-13 05:38:00.000000 cfn-stk-0.15.1/src/stk/stack_reference.py
--rw-r--r--   0 johnw      (501) staff       (20)     6733 2022-12-14 23:11:07.000000 cfn-stk-0.15.1/src/stk/stack_refs.py
--rw-r--r--   0 johnw      (501) staff       (20)     5589 2022-10-26 19:07:43.000000 cfn-stk-0.15.1/src/stk/stack_waiter.py
--rw-r--r--   0 johnw      (501) staff       (20)     7455 2023-01-09 20:17:20.000000 cfn-stk-0.15.1/src/stk/template.py
--rw-r--r--   0 johnw      (501) staff       (20)     1878 2023-03-13 03:43:19.000000 cfn-stk-0.15.1/src/stk/template_command.py
--rw-r--r--   0 johnw      (501) staff       (20)    12216 2023-03-13 22:07:59.000000 cfn-stk-0.15.1/src/stk/template_helpers.py
--rw-r--r--   0 johnw      (501) staff       (20)      773 2022-05-27 00:53:36.000000 cfn-stk-0.15.1/src/stk/template_source.py
-drwxr-xr-x   0 johnw      (501) staff       (20)        0 2023-05-01 10:17:34.325024 cfn-stk-0.15.1/src/stk/tests/
--rw-r--r--   0 johnw      (501) staff       (20)     1970 2023-04-16 07:13:04.000000 cfn-stk-0.15.1/src/stk/tests/__init__.py
--rw-r--r--   0 johnw      (501) staff       (20)      342 2023-04-16 07:13:04.000000 cfn-stk-0.15.1/src/stk/tests/test_aws_config.py
--rw-r--r--   0 johnw      (501) staff       (20)     2507 2023-04-16 07:13:04.000000 cfn-stk-0.15.1/src/stk/tests/test_cli.py
--rw-r--r--   0 johnw      (501) staff       (20)     5237 2023-04-16 07:13:04.000000 cfn-stk-0.15.1/src/stk/tests/test_config.py
--rw-r--r--   0 johnw      (501) staff       (20)      649 2023-04-16 07:13:04.000000 cfn-stk-0.15.1/src/stk/tests/test_config_file.py
--rw-r--r--   0 johnw      (501) staff       (20)      872 2023-04-14 21:42:08.000000 cfn-stk-0.15.1/src/stk/tests/test_deploy_metadata.py
--rw-r--r--   0 johnw      (501) staff       (20)      175 2023-04-16 07:13:04.000000 cfn-stk-0.15.1/src/stk/tests/test_provider.py
--rw-r--r--   0 johnw      (501) staff       (20)     5597 2023-04-16 07:13:04.000000 cfn-stk-0.15.1/src/stk/tests/test_refs.py
--rw-r--r--   0 johnw      (501) staff       (20)     1029 2023-04-16 07:13:04.000000 cfn-stk-0.15.1/src/stk/tests/test_stack.py
--rw-r--r--   0 johnw      (501) staff       (20)     2593 2022-05-20 01:16:56.000000 cfn-stk-0.15.1/src/stk/tests/test_template.py
--rw-r--r--   0 johnw      (501) staff       (20)     4323 2023-04-16 07:13:04.000000 cfn-stk-0.15.1/src/stk/tests/test_template_helpers.py
--rw-r--r--   0 johnw      (501) staff       (20)     1854 2023-01-09 23:51:50.000000 cfn-stk-0.15.1/src/stk/util.py
+drwxr-xr-x   0 johnw      (501) staff       (20)        0 2023-05-27 23:18:39.338263 cfn-stk-0.15.2/
+-rw-r--r--   0 johnw      (501) staff       (20)     1080 2022-04-22 05:39:32.000000 cfn-stk-0.15.2/LICENSE.txt
+-rw-r--r--   0 johnw      (501) staff       (20)    20877 2023-05-27 23:18:39.338352 cfn-stk-0.15.2/PKG-INFO
+-rw-r--r--   0 johnw      (501) staff       (20)    20400 2023-04-21 22:10:37.000000 cfn-stk-0.15.2/README.md
+-rw-r--r--   0 johnw      (501) staff       (20)      154 2023-04-21 09:38:32.000000 cfn-stk-0.15.2/pyproject.toml
+-rw-r--r--   0 johnw      (501) staff       (20)      901 2023-05-27 23:18:39.338747 cfn-stk-0.15.2/setup.cfg
+drwxr-xr-x   0 johnw      (501) staff       (20)        0 2023-05-27 23:17:41.213599 cfn-stk-0.15.2/src/
+drwxr-xr-x   0 johnw      (501) staff       (20)        0 2023-05-27 23:18:39.330416 cfn-stk-0.15.2/src/cfn_stk.egg-info/
+-rw-r--r--   0 johnw      (501) staff       (20)    20877 2023-05-27 23:18:39.000000 cfn-stk-0.15.2/src/cfn_stk.egg-info/PKG-INFO
+-rw-r--r--   0 johnw      (501) staff       (20)     1303 2023-05-27 23:18:39.000000 cfn-stk-0.15.2/src/cfn_stk.egg-info/SOURCES.txt
+-rw-r--r--   0 johnw      (501) staff       (20)        1 2023-05-27 23:18:39.000000 cfn-stk-0.15.2/src/cfn_stk.egg-info/dependency_links.txt
+-rw-r--r--   0 johnw      (501) staff       (20)       54 2023-05-27 23:18:39.000000 cfn-stk-0.15.2/src/cfn_stk.egg-info/entry_points.txt
+-rw-r--r--   0 johnw      (501) staff       (20)        1 2023-04-21 10:00:31.000000 cfn-stk-0.15.2/src/cfn_stk.egg-info/not-zip-safe
+-rw-r--r--   0 johnw      (501) staff       (20)      134 2023-05-27 23:18:39.000000 cfn-stk-0.15.2/src/cfn_stk.egg-info/requires.txt
+-rw-r--r--   0 johnw      (501) staff       (20)        4 2023-05-27 23:18:39.000000 cfn-stk-0.15.2/src/cfn_stk.egg-info/top_level.txt
+drwxr-xr-x   0 johnw      (501) staff       (20)        0 2023-05-27 23:18:39.335112 cfn-stk-0.15.2/src/stk/
+-rw-r--r--   0 johnw      (501) staff       (20)     1294 2023-05-27 23:09:43.000000 cfn-stk-0.15.2/src/stk/__init__.py
+-rw-r--r--   0 johnw      (501) staff       (20)     3884 2023-04-16 07:13:04.000000 cfn-stk-0.15.2/src/stk/aws_config.py
+-rw-r--r--   0 johnw      (501) staff       (20)     2876 2023-01-30 23:26:06.000000 cfn-stk-0.15.2/src/stk/basic_stack.py
+-rw-r--r--   0 johnw      (501) staff       (20)     1769 2022-06-09 21:19:18.000000 cfn-stk-0.15.2/src/stk/cfn_bucket.py
+-rw-r--r--   0 johnw      (501) staff       (20)     5710 2023-01-31 00:05:56.000000 cfn-stk-0.15.2/src/stk/change_set.py
+-rw-r--r--   0 johnw      (501) staff       (20)        0 2023-05-27 23:17:41.216697 cfn-stk-0.15.2/src/stk/chdir.py
+-rw-r--r--   0 johnw      (501) staff       (20)    11502 2023-01-31 00:05:56.000000 cfn-stk-0.15.2/src/stk/cli.py
+-rw-r--r--   0 johnw      (501) staff       (20)    11211 2023-04-16 07:13:04.000000 cfn-stk-0.15.2/src/stk/config.py
+drwxr-xr-x   0 johnw      (501) staff       (20)        0 2023-05-27 23:18:39.336027 cfn-stk-0.15.2/src/stk/config_cmd/
+-rw-r--r--   0 johnw      (501) staff       (20)        0 2022-11-14 21:14:00.000000 cfn-stk-0.15.2/src/stk/config_cmd/__init__.py
+-rw-r--r--   0 johnw      (501) staff       (20)     8947 2022-11-28 21:14:54.000000 cfn-stk-0.15.2/src/stk/config_cmd/add_template.py
+-rw-r--r--   0 johnw      (501) staff       (20)     2061 2022-11-15 08:25:57.000000 cfn-stk-0.15.2/src/stk/config_cmd/cli.py
+-rw-r--r--   0 johnw      (501) staff       (20)     9164 2022-12-13 09:20:13.000000 cfn-stk-0.15.2/src/stk/config_cmd/init.py
+-rw-r--r--   0 johnw      (501) staff       (20)     7659 2023-04-16 07:13:04.000000 cfn-stk-0.15.2/src/stk/config_file.py
+-rw-r--r--   0 johnw      (501) staff       (20)     2513 2022-05-16 08:31:28.000000 cfn-stk-0.15.2/src/stk/human_bytes.py
+-rw-r--r--   0 johnw      (501) staff       (20)     6069 2022-04-22 02:04:14.000000 cfn-stk-0.15.2/src/stk/ignore_file.py
+-rw-r--r--   0 johnw      (501) staff       (20)     1261 2022-12-13 05:38:00.000000 cfn-stk-0.15.2/src/stk/interpolated_dict.py
+-rw-r--r--   0 johnw      (501) staff       (20)     1523 2022-05-10 10:04:13.000000 cfn-stk-0.15.2/src/stk/multipart_encoder.py
+-rw-r--r--   0 johnw      (501) staff       (20)     8891 2023-01-31 00:05:56.000000 cfn-stk-0.15.2/src/stk/provider.py
+-rw-r--r--   0 johnw      (501) staff       (20)     4531 2023-04-16 07:13:04.000000 cfn-stk-0.15.2/src/stk/stack.py
+-rw-r--r--   0 johnw      (501) staff       (20)     2214 2023-01-30 23:30:53.000000 cfn-stk-0.15.2/src/stk/stack_delegated_command.py
+-rw-r--r--   0 johnw      (501) staff       (20)     1016 2022-12-13 05:38:00.000000 cfn-stk-0.15.2/src/stk/stack_reference.py
+-rw-r--r--   0 johnw      (501) staff       (20)     6733 2022-12-14 23:11:07.000000 cfn-stk-0.15.2/src/stk/stack_refs.py
+-rw-r--r--   0 johnw      (501) staff       (20)     5589 2022-10-26 19:07:43.000000 cfn-stk-0.15.2/src/stk/stack_waiter.py
+-rw-r--r--   0 johnw      (501) staff       (20)     7455 2023-01-09 20:17:20.000000 cfn-stk-0.15.2/src/stk/template.py
+-rw-r--r--   0 johnw      (501) staff       (20)     1878 2023-03-13 03:43:19.000000 cfn-stk-0.15.2/src/stk/template_command.py
+-rw-r--r--   0 johnw      (501) staff       (20)    12216 2023-03-13 22:07:59.000000 cfn-stk-0.15.2/src/stk/template_helpers.py
+-rw-r--r--   0 johnw      (501) staff       (20)      773 2022-05-27 00:53:36.000000 cfn-stk-0.15.2/src/stk/template_source.py
+drwxr-xr-x   0 johnw      (501) staff       (20)        0 2023-05-27 23:18:39.338091 cfn-stk-0.15.2/src/stk/tests/
+-rw-r--r--   0 johnw      (501) staff       (20)     1970 2023-04-16 07:13:04.000000 cfn-stk-0.15.2/src/stk/tests/__init__.py
+-rw-r--r--   0 johnw      (501) staff       (20)      342 2023-04-16 07:13:04.000000 cfn-stk-0.15.2/src/stk/tests/test_aws_config.py
+-rw-r--r--   0 johnw      (501) staff       (20)     2507 2023-04-16 07:13:04.000000 cfn-stk-0.15.2/src/stk/tests/test_cli.py
+-rw-r--r--   0 johnw      (501) staff       (20)     5237 2023-04-16 07:13:04.000000 cfn-stk-0.15.2/src/stk/tests/test_config.py
+-rw-r--r--   0 johnw      (501) staff       (20)      649 2023-04-16 07:13:04.000000 cfn-stk-0.15.2/src/stk/tests/test_config_file.py
+-rw-r--r--   0 johnw      (501) staff       (20)      872 2023-04-14 21:42:08.000000 cfn-stk-0.15.2/src/stk/tests/test_deploy_metadata.py
+-rw-r--r--   0 johnw      (501) staff       (20)      175 2023-04-16 07:13:04.000000 cfn-stk-0.15.2/src/stk/tests/test_provider.py
+-rw-r--r--   0 johnw      (501) staff       (20)     5597 2023-04-16 07:13:04.000000 cfn-stk-0.15.2/src/stk/tests/test_refs.py
+-rw-r--r--   0 johnw      (501) staff       (20)     1029 2023-04-16 07:13:04.000000 cfn-stk-0.15.2/src/stk/tests/test_stack.py
+-rw-r--r--   0 johnw      (501) staff       (20)     2593 2022-05-20 01:16:56.000000 cfn-stk-0.15.2/src/stk/tests/test_template.py
+-rw-r--r--   0 johnw      (501) staff       (20)     4323 2023-04-16 07:13:04.000000 cfn-stk-0.15.2/src/stk/tests/test_template_helpers.py
+-rw-r--r--   0 johnw      (501) staff       (20)     1854 2023-01-09 23:51:50.000000 cfn-stk-0.15.2/src/stk/util.py
```

### Comparing `cfn-stk-0.15.1/LICENSE.txt` & `cfn-stk-0.15.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/PKG-INFO` & `cfn-stk-0.15.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfn-stk
-Version: 0.15.1
+Version: 0.15.2
 Summary: Opinionated CloudFormation deployments
 Home-page: https://github.com/jwoffindin/stk
 Author: John Woffindin
 Author-email: j.woffindin@gmail.com
 Keywords: cloudformation,aws,cfn,cli
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cfn-stk Version: 0.15.1 Summary: Opinionated
+Metadata-Version: 2.1 Name: cfn-stk Version: 0.15.2 Summary: Opinionated
 CloudFormation deployments Home-page: https://github.com/jwoffindin/stk Author:
 John Woffindin Author-email: j.woffindin@gmail.com Keywords:
 cloudformation,aws,cfn,cli Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE.txt
  [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
```

### Comparing `cfn-stk-0.15.1/README.md` & `cfn-stk-0.15.2/README.md`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/setup.cfg` & `cfn-stk-0.15.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/cfn_stk.egg-info/PKG-INFO` & `cfn-stk-0.15.2/src/cfn_stk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfn-stk
-Version: 0.15.1
+Version: 0.15.2
 Summary: Opinionated CloudFormation deployments
 Home-page: https://github.com/jwoffindin/stk
 Author: John Woffindin
 Author-email: j.woffindin@gmail.com
 Keywords: cloudformation,aws,cfn,cli
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cfn-stk Version: 0.15.1 Summary: Opinionated
+Metadata-Version: 2.1 Name: cfn-stk Version: 0.15.2 Summary: Opinionated
 CloudFormation deployments Home-page: https://github.com/jwoffindin/stk Author:
 John Woffindin Author-email: j.woffindin@gmail.com Keywords:
 cloudformation,aws,cfn,cli Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE.txt
  [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
```

### Comparing `cfn-stk-0.15.1/src/cfn_stk.egg-info/SOURCES.txt` & `cfn-stk-0.15.2/src/cfn_stk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/__init__.py` & `cfn-stk-0.15.2/src/stk/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 """
 """
 import logging
 import logging.handlers
 import yaml
 
-from os import environ
+from os import environ, path
 from rich.console import Console
 
-VERSION = "0.15.1"
+VERSION = "0.15.2"
 
 # Create application logger (for when things go wrong)
 log = logging.getLogger('cfn')
 log.setLevel(environ.get('CFN_LOG_LEVEL', environ.get("LOG_LEVEL", "WARN")).upper())
 
 if environ.get('LOG_FILE'):
     logging.basicConfig(filename=environ['LOG_FILE'], filemode="a")
 else:
-    handler = logging.handlers.SysLogHandler(address = '/dev/log')
-    formatter = logging.Formatter('cfn: %(message)s')
-    log.addHandler(handler)
+    syslog_path = '/dev/log'
+    if path.exists(syslog_path):
+        try:
+            handler = logging.handlers.SysLogHandler(address=syslog_path)
+        except:
+            # silently ignore if no syslog active
+            pass
+        else:
+            formatter = logging.Formatter('cfn: %(message)s')
+            handler.setFormatter(formatter)
+            log.addHandler(handler)
 
 
 # Console logger is for displaying updates to user - normal
 # events.
 console = Console(emoji=False, log_path=False, stderr=True)
 clog = console.log
```

### Comparing `cfn-stk-0.15.1/src/stk/aws_config.py` & `cfn-stk-0.15.2/src/stk/aws_config.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/basic_stack.py` & `cfn-stk-0.15.2/src/stk/basic_stack.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/cfn_bucket.py` & `cfn-stk-0.15.2/src/stk/cfn_bucket.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/change_set.py` & `cfn-stk-0.15.2/src/stk/change_set.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/cli.py` & `cfn-stk-0.15.2/src/stk/cli.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/config.py` & `cfn-stk-0.15.2/src/stk/config.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/config_cmd/add_template.py` & `cfn-stk-0.15.2/src/stk/config_cmd/add_template.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/config_cmd/cli.py` & `cfn-stk-0.15.2/src/stk/config_cmd/cli.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/config_cmd/init.py` & `cfn-stk-0.15.2/src/stk/config_cmd/init.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/config_file.py` & `cfn-stk-0.15.2/src/stk/config_file.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/human_bytes.py` & `cfn-stk-0.15.2/src/stk/human_bytes.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/ignore_file.py` & `cfn-stk-0.15.2/src/stk/ignore_file.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/interpolated_dict.py` & `cfn-stk-0.15.2/src/stk/interpolated_dict.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/multipart_encoder.py` & `cfn-stk-0.15.2/src/stk/multipart_encoder.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/provider.py` & `cfn-stk-0.15.2/src/stk/provider.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/stack.py` & `cfn-stk-0.15.2/src/stk/stack.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/stack_delegated_command.py` & `cfn-stk-0.15.2/src/stk/stack_delegated_command.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/stack_reference.py` & `cfn-stk-0.15.2/src/stk/stack_reference.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/stack_refs.py` & `cfn-stk-0.15.2/src/stk/stack_refs.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/stack_waiter.py` & `cfn-stk-0.15.2/src/stk/stack_waiter.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/template.py` & `cfn-stk-0.15.2/src/stk/template.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/template_command.py` & `cfn-stk-0.15.2/src/stk/template_command.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/template_helpers.py` & `cfn-stk-0.15.2/src/stk/template_helpers.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/template_source.py` & `cfn-stk-0.15.2/src/stk/template_source.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/tests/__init__.py` & `cfn-stk-0.15.2/src/stk/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/tests/test_cli.py` & `cfn-stk-0.15.2/src/stk/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/tests/test_config.py` & `cfn-stk-0.15.2/src/stk/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/tests/test_config_file.py` & `cfn-stk-0.15.2/src/stk/tests/test_config_file.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/tests/test_deploy_metadata.py` & `cfn-stk-0.15.2/src/stk/tests/test_deploy_metadata.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/tests/test_refs.py` & `cfn-stk-0.15.2/src/stk/tests/test_refs.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/tests/test_stack.py` & `cfn-stk-0.15.2/src/stk/tests/test_stack.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/tests/test_template.py` & `cfn-stk-0.15.2/src/stk/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/tests/test_template_helpers.py` & `cfn-stk-0.15.2/src/stk/tests/test_template_helpers.py`

 * *Files identical despite different names*

### Comparing `cfn-stk-0.15.1/src/stk/util.py` & `cfn-stk-0.15.2/src/stk/util.py`

 * *Files identical despite different names*

