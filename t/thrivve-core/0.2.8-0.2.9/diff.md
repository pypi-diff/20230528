# Comparing `tmp/thrivve_core-0.2.8.tar.gz` & `tmp/thrivve_core-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/thrivve_core/dist/.tmp-b538v70u/thrivve_core-0.2.8.tar", last modified: Wed May 24 14:01:53 2023, max compression
+gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/thrivve_core/dist/.tmp-wb9tij0w/thrivve_core-0.2.9.tar", last modified: Sun May 28 12:33:12 2023, max compression
```

## Comparing `thrivve_core-0.2.8.tar` & `thrivve_core-0.2.9.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:01:53.000000 thrivve_core-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-05-24 14:01:53.000000 thrivve_core-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-24 14:01:53.000000 thrivve_core-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:01:53.000000 thrivve_core-0.2.8/thrivve_core/
--rw-r--r--   0 runner    (1001) docker     (122)      881 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:01:53.000000 thrivve_core-0.2.8/thrivve_core/app_decorators/
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/app_decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      979 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/app_decorators/app_entry.py
--rw-r--r--   0 runner    (1001) docker     (122)     2464 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/app_decorators/handle_auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     2327 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/app_decorators/handle_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      786 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/app_decorators/handle_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     4611 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/app_decorators/serializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:01:53.000000 thrivve_core-0.2.8/thrivve_core/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      855 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/acl_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:01:53.000000 thrivve_core-0.2.8/thrivve_core/helpers/amazon/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/amazon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      579 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py
--rw-r--r--   0 runner    (1001) docker     (122)     1353 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/amazon/get_file_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      318 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/amazon/get_plain_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/amazon/get_s3_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      564 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/amazon/upload_file.py
--rw-r--r--   0 runner    (1001) docker     (122)      833 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/atomic_transactions.py
--rw-r--r--   0 runner    (1001) docker     (122)      921 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/atomic_transactions_v2.py
--rw-r--r--   0 runner    (1001) docker     (122)     1938 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:01:53.000000 thrivve_core-0.2.8/thrivve_core/helpers/database/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      677 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/database/base_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3983 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/database/log_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2244 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3692 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/fetch_relational_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4723 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/format_exception.py
--rw-r--r--   0 runner    (1001) docker     (122)      385 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/get_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)      223 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/get_country_code.py
--rw-r--r--   0 runner    (1001) docker     (122)      622 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/get_embedded_function.py
--rw-r--r--   0 runner    (1001) docker     (122)      424 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/get_obj_value.py
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/get_prefix.py
--rw-r--r--   0 runner    (1001) docker     (122)     2723 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/kafka_listener.py
--rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/kafka_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:01:53.000000 thrivve_core-0.2.8/thrivve_core/helpers/kafka_producers/
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/kafka_producers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/kafka_producers/log_model_changes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2061 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/kafka_producers/notification_center.py
--rw-r--r--   0 runner    (1001) docker     (122)      276 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/kafka_producers/send_sms.py
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/kafka_producers/send_topic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/log_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    12352 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/micro_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/numbers.py
--rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/search_function.py
--rw-r--r--   0 runner    (1001) docker     (122)      644 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/service_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      825 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/sql.py
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/system_roles.py
--rw-r--r--   0 runner    (1001) docker     (122)     6823 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/time.py
--rw-r--r--   0 runner    (1001) docker     (122)      393 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/topics.py
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/validate_mobile_number.py
--rw-r--r--   0 runner    (1001) docker     (122)      995 2023-05-24 14:01:42.000000 thrivve_core-0.2.8/thrivve_core/helpers/validate_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:01:53.000000 thrivve_core-0.2.8/thrivve_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-05-24 14:01:53.000000 thrivve_core-0.2.8/thrivve_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2246 2023-05-24 14:01:53.000000 thrivve_core-0.2.8/thrivve_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 14:01:53.000000 thrivve_core-0.2.8/thrivve_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-05-24 14:01:53.000000 thrivve_core-0.2.8/thrivve_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-24 14:01:53.000000 thrivve_core-0.2.8/thrivve_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-28 12:33:12.000000 thrivve_core-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-05-28 12:33:12.000000 thrivve_core-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-28 12:33:12.000000 thrivve_core-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-28 12:33:12.000000 thrivve_core-0.2.9/thrivve_core/
+-rw-r--r--   0 runner    (1001) docker     (122)      881 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-28 12:33:12.000000 thrivve_core-0.2.9/thrivve_core/app_decorators/
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/app_decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      979 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/app_decorators/app_entry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2464 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/app_decorators/handle_auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2327 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/app_decorators/handle_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/app_decorators/handle_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4611 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/app_decorators/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-28 12:33:12.000000 thrivve_core-0.2.9/thrivve_core/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/acl_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-28 12:33:12.000000 thrivve_core-0.2.9/thrivve_core/helpers/amazon/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/amazon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      579 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1353 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/amazon/get_file_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/amazon/get_plain_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/amazon/get_s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      564 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/amazon/upload_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)      833 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/atomic_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      921 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/atomic_transactions_v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1797 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-28 12:33:12.000000 thrivve_core-0.2.9/thrivve_core/helpers/database/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      677 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/database/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3983 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/database/log_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2244 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3692 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/fetch_relational_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4723 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/format_exception.py
+-rw-r--r--   0 runner    (1001) docker     (122)      385 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/get_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/get_country_code.py
+-rw-r--r--   0 runner    (1001) docker     (122)      622 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/get_embedded_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/get_obj_value.py
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/get_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2723 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/kafka_listener.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/kafka_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-28 12:33:12.000000 thrivve_core-0.2.9/thrivve_core/helpers/kafka_producers/
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/kafka_producers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/kafka_producers/log_model_changes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2061 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/kafka_producers/notification_center.py
+-rw-r--r--   0 runner    (1001) docker     (122)      276 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/kafka_producers/send_sms.py
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/kafka_producers/send_topic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12352 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/micro_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/search_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)      644 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/service_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      825 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/sql.py
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/system_roles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6823 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)      393 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/topics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1198 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/validate_mobile_number.py
+-rw-r--r--   0 runner    (1001) docker     (122)      995 2023-05-28 12:33:03.000000 thrivve_core-0.2.9/thrivve_core/helpers/validate_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-28 12:33:12.000000 thrivve_core-0.2.9/thrivve_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-05-28 12:33:12.000000 thrivve_core-0.2.9/thrivve_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2246 2023-05-28 12:33:12.000000 thrivve_core-0.2.9/thrivve_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-28 12:33:12.000000 thrivve_core-0.2.9/thrivve_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-05-28 12:33:12.000000 thrivve_core-0.2.9/thrivve_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-28 12:33:12.000000 thrivve_core-0.2.9/thrivve_core.egg-info/top_level.txt
```

### Comparing `thrivve_core-0.2.8/PKG-INFO` & `thrivve_core-0.2.9/thrivve_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: thrivve_core
-Version: 0.2.8
+Name: thrivve-core
+Version: 0.2.9
 Summary: thrivveCore package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `thrivve_core-0.2.8/setup.py` & `thrivve_core-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "Programming Language :: Python :: 3.4",
     "Programming Language :: Python :: 3.5",
     "Programming Language :: Python :: 3.6",
 ]
 
 setup(
     name="thrivve_core",
-    version="0.2.8",
+    version="0.2.9",
     description="thrivveCore package",
     long_description="""# Markdown supported!\n\n* thrivve\n* List of features\n""",
     long_description_content_type="text/markdown",
     url="https://www.wedeliverapp.com/",
     author="Eyad Farra",
     author_email="info@wedeliverapp.com",
     license="MIT",
```

### Comparing `thrivve_core-0.2.8/thrivve_core/__init__.py` & `thrivve_core-0.2.9/thrivve_core/__init__.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/app_decorators/app_entry.py` & `thrivve_core-0.2.9/thrivve_core/app_decorators/app_entry.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/app_decorators/handle_auth.py` & `thrivve_core-0.2.9/thrivve_core/app_decorators/handle_auth.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/app_decorators/handle_exceptions.py` & `thrivve_core-0.2.9/thrivve_core/app_decorators/handle_exceptions.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/app_decorators/handle_response.py` & `thrivve_core-0.2.9/thrivve_core/app_decorators/handle_response.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/app_decorators/serializer.py` & `thrivve_core-0.2.9/thrivve_core/app_decorators/serializer.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/base.py` & `thrivve_core-0.2.9/thrivve_core/base.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/helpers/acl_enum.py` & `thrivve_core-0.2.9/thrivve_core/helpers/acl_enum.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py` & `thrivve_core-0.2.9/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/helpers/amazon/get_file_url.py` & `thrivve_core-0.2.9/thrivve_core/helpers/amazon/get_file_url.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/helpers/amazon/get_s3_client.py` & `thrivve_core-0.2.9/thrivve_core/helpers/amazon/get_s3_client.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/helpers/amazon/upload_file.py` & `thrivve_core-0.2.9/thrivve_core/helpers/amazon/upload_file.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/helpers/atomic_transactions.py` & `thrivve_core-0.2.9/thrivve_core/helpers/atomic_transactions.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/helpers/atomic_transactions_v2.py` & `thrivve_core-0.2.9/thrivve_core/helpers/atomic_transactions_v2.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/helpers/config.py` & `thrivve_core-0.2.9/thrivve_core/helpers/config.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/helpers/database/base_model.py` & `thrivve_core-0.2.9/thrivve_core/helpers/database/base_model.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/helpers/database/log_model.py` & `thrivve_core-0.2.9/thrivve_core/helpers/database/log_model.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/helpers/enums.py` & `thrivve_core-0.2.9/thrivve_core/helpers/enums.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/helpers/exceptions.py` & `thrivve_core-0.2.9/thrivve_core/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/helpers/fetch_relational_data.py` & `thrivve_core-0.2.9/thrivve_core/helpers/fetch_relational_data.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/helpers/filters.py` & `thrivve_core-0.2.9/thrivve_core/helpers/filters.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/helpers/format_exception.py` & `thrivve_core-0.2.9/thrivve_core/helpers/format_exception.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/helpers/get_embedded_function.py` & `thrivve_core-0.2.9/thrivve_core/helpers/get_embedded_function.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/helpers/kafka_listener.py` & `thrivve_core-0.2.9/thrivve_core/helpers/kafka_listener.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/helpers/kafka_producer.py` & `thrivve_core-0.2.9/thrivve_core/helpers/kafka_producer.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/helpers/kafka_producers/notification_center.py` & `thrivve_core-0.2.9/thrivve_core/helpers/kafka_producers/notification_center.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/helpers/log_config.py` & `thrivve_core-0.2.9/thrivve_core/helpers/log_config.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/helpers/micro_fetcher.py` & `thrivve_core-0.2.9/thrivve_core/helpers/micro_fetcher.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/helpers/search_function.py` & `thrivve_core-0.2.9/thrivve_core/helpers/search_function.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/helpers/service_config.py` & `thrivve_core-0.2.9/thrivve_core/helpers/service_config.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/helpers/sql.py` & `thrivve_core-0.2.9/thrivve_core/helpers/sql.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/helpers/time.py` & `thrivve_core-0.2.9/thrivve_core/helpers/time.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core/helpers/validate_mobile_number.py` & `thrivve_core-0.2.9/thrivve_core/helpers/validate_mobile_number.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,43 @@
 import re
 from thrivve_core.helpers.get_country_code import get_country_code
 
 
-def validate_mobile_number(mobile):
+def validate_mobile_number(mobile, force_only=None):
     mobile = mobile.replace("+", "").replace(" ", "").lstrip("0")
     if len(mobile) < 12:
         country_code = get_country_code()
         if country_code == "sa":
             dial = "966"
         elif country_code == "ps":
             dial = "970"
         elif country_code == "eg":
             dial = "20"
         else:
             return False
+
         mobile = "{0}{1}".format(dial, int(mobile))
-    if (
-        re.match(
-            r"^(009665|9665|\+9665|05|5)(5|0|3|6|4|9|1|8|7)([0-9]{7})$", str(mobile)
-        )
-        or re.match(r"^(009705|9705|\+9705|05|5)([0-9]{8})$", str(mobile))
-        or re.match(r"^(201|01|\+201|00201)[0-9]{9}$", str(mobile))
-    ):
-        return mobile
+
+    saudi_regex     = re.match(r"^(009665|9665|\+9665|05|5)([0-9]{8})$", str(mobile))
+    palestine_regex = re.match(r"^(009705|9705|\+9705|05|5)([0-9]{8})$", str(mobile))
+
+    if force_only:
+        if force_only == "sa":
+            if saudi_regex:
+                return mobile
+            else:
+                return False
+        elif force_only == "ps":
+            if palestine_regex:
+                return mobile
+            else:
+                return False
+        else:
+            return False
     else:
-        return False
+        if (
+            saudi_regex
+            or palestine_regex
+        ):
+            return mobile
+        else:
+            return False
```

### Comparing `thrivve_core-0.2.8/thrivve_core/helpers/validate_parameters.py` & `thrivve_core-0.2.9/thrivve_core/helpers/validate_parameters.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.8/thrivve_core.egg-info/PKG-INFO` & `thrivve_core-0.2.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: thrivve-core
-Version: 0.2.8
+Name: thrivve_core
+Version: 0.2.9
 Summary: thrivveCore package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `thrivve_core-0.2.8/thrivve_core.egg-info/SOURCES.txt` & `thrivve_core-0.2.9/thrivve_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

