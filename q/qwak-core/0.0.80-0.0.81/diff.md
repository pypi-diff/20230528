# Comparing `tmp/qwak_core-0.0.80.tar.gz` & `tmp/qwak_core-0.0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.80.tar", max compression
+gzip compressed data, was "qwak_core-0.0.81.tar", max compression
```

## Comparing `qwak_core-0.0.80.tar` & `qwak_core-0.0.81.tar`

### file list

```diff
@@ -1,582 +1,582 @@
--rw-r--r--   0        0        0      264 2023-05-28 08:32:06.172842 qwak_core-0.0.80/README.md
--rw-r--r--   0        0        0        0 2023-05-28 08:33:53.945213 qwak_core-0.0.80/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-05-28 08:33:53.969213 qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-05-28 08:33:31.965134 qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:53.973213 qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-05-28 08:33:53.965213 qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-05-28 08:33:31.545132 qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:53.969213 qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-05-28 08:33:53.969213 qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-05-28 08:33:31.757133 qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:53.969213 qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-05-28 08:33:53.961213 qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-05-28 08:33:30.977130 qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-05-28 08:33:53.961213 qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-28 08:33:53.961213 qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-05-28 08:33:31.165131 qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:53.965213 qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4864 2023-05-28 08:33:53.965213 qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5792 2023-05-28 08:33:31.357132 qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:53.965213 qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-05-28 08:33:53.945213 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-05-28 08:33:30.789130 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-05-28 08:33:53.949213 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5670 2023-05-28 08:33:53.949213 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8035 2023-05-28 08:33:32.161134 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:53.949213 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-05-28 08:33:53.953213 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-05-28 08:33:32.565136 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:53.953213 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-05-28 08:33:53.957213 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-05-28 08:33:32.761137 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-05-28 08:33:53.957213 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-05-28 08:33:53.953213 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-05-28 08:33:32.353135 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:53.953213 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-05-28 08:33:53.957213 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-05-28 08:33:32.985137 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:53.957213 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-05-28 08:33:54.001213 qwak_core-0.0.80/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-05-28 08:33:35.749148 qwak_core-0.0.80/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.001213 qwak_core-0.0.80/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-05-28 08:33:54.005213 qwak_core-0.0.80/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-05-28 08:33:35.949148 qwak_core-0.0.80/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-05-28 08:33:54.005213 qwak_core-0.0.80/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-05-28 08:33:54.069213 qwak_core-0.0.80/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-05-28 08:33:41.429168 qwak_core-0.0.80/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.073213 qwak_core-0.0.80/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-05-28 08:33:54.073213 qwak_core-0.0.80/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-05-28 08:33:41.621169 qwak_core-0.0.80/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-05-28 08:33:54.073213 qwak_core-0.0.80/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-05-28 08:33:54.077213 qwak_core-0.0.80/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-05-28 08:33:42.585172 qwak_core-0.0.80/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-05-28 08:33:54.077213 qwak_core-0.0.80/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-05-28 08:33:54.077213 qwak_core-0.0.80/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-05-28 08:33:42.397171 qwak_core-0.0.80/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.077213 qwak_core-0.0.80/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5777 2023-05-28 08:33:54.081213 qwak_core-0.0.80/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8264 2023-05-28 08:33:42.785173 qwak_core-0.0.80/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.081213 qwak_core-0.0.80/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-05-28 08:33:54.081213 qwak_core-0.0.80/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-05-28 08:33:42.973173 qwak_core-0.0.80/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-05-28 08:33:54.085214 qwak_core-0.0.80/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    12352 2023-05-28 08:33:54.177214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    18970 2023-05-28 08:33:51.473204 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.177214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5775 2023-05-28 08:33:54.173214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8308 2023-05-28 08:33:51.069203 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.173214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-05-28 08:33:54.177214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-05-28 08:33:51.273203 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.177214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-05-28 08:33:54.169214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-05-28 08:33:50.661201 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-05-28 08:33:54.169214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-05-28 08:33:54.173214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-05-28 08:33:50.865202 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.173214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-05-28 08:33:54.185214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-05-28 08:33:52.073206 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.185214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-05-28 08:33:54.181214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-05-28 08:33:51.873206 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.185214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2023-05-28 08:33:54.181214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2023-05-28 08:33:51.665205 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.181214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-05-28 08:33:54.165214 qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-05-28 08:33:50.441201 qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.169214 qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-05-28 08:33:54.161214 qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-05-28 08:33:50.037199 qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.165214 qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    42145 2023-05-28 08:33:54.165214 qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    55993 2023-05-28 08:33:50.245200 qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-05-28 08:33:54.165214 qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    20255 2023-05-28 08:33:54.109213 qwak_core-0.0.80/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    17495 2023-05-28 08:33:44.981181 qwak_core-0.0.80/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    20359 2023-05-28 08:33:54.113214 qwak_core-0.0.80/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-05-28 08:33:54.109213 qwak_core-0.0.80/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-05-28 08:33:44.781180 qwak_core-0.0.80/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.109213 qwak_core-0.0.80/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11034 2023-05-28 08:33:54.097213 qwak_core-0.0.80/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18276 2023-05-28 08:33:44.381179 qwak_core-0.0.80/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.101214 qwak_core-0.0.80/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-05-28 08:33:54.101214 qwak_core-0.0.80/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-05-28 08:33:44.577179 qwak_core-0.0.80/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.101214 qwak_core-0.0.80/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-05-28 08:33:54.105213 qwak_core-0.0.80/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-05-28 08:33:45.185181 qwak_core-0.0.80/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-05-28 08:33:54.105213 qwak_core-0.0.80/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38245 2023-05-28 08:33:54.105213 qwak_core-0.0.80/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52572 2023-05-28 08:33:45.605183 qwak_core-0.0.80/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-05-28 08:33:54.105213 qwak_core-0.0.80/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-05-28 08:33:54.117214 qwak_core-0.0.80/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-05-28 08:33:46.021185 qwak_core-0.0.80/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.117214 qwak_core-0.0.80/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-05-28 08:33:54.121214 qwak_core-0.0.80/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-28 08:33:46.221185 qwak_core-0.0.80/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-28 08:33:54.121214 qwak_core-0.0.80/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-05-28 08:33:54.093213 qwak_core-0.0.80/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-05-28 08:33:43.789177 qwak_core-0.0.80/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.093213 qwak_core-0.0.80/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-05-28 08:33:54.093213 qwak_core-0.0.80/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-05-28 08:33:43.989177 qwak_core-0.0.80/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-05-28 08:33:54.093213 qwak_core-0.0.80/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-05-28 08:33:54.085214 qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-05-28 08:33:43.393175 qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.089213 qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    43712 2023-05-28 08:33:54.085214 qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    63341 2023-05-28 08:33:43.197174 qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.085214 qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-05-28 08:33:54.089213 qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-05-28 08:33:43.601176 qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-05-28 08:33:54.089213 qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-05-28 08:33:53.989213 qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-05-28 08:33:34.749144 qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:53.993213 qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-28 08:33:53.993213 qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-05-28 08:33:34.953144 qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:53.993213 qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-05-28 08:33:53.993213 qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-05-28 08:33:35.153145 qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-05-28 08:33:53.997213 qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-05-28 08:33:54.053213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-05-28 08:33:40.277164 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.053213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-05-28 08:33:54.049213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-05-28 08:33:40.089163 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-05-28 08:33:54.049213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0    11432 2023-05-28 08:33:54.029213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    12882 2023-05-28 08:33:38.345157 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.033213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5303 2023-05-28 08:33:54.029213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8604 2023-05-28 08:33:38.153156 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.029213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-05-28 08:33:54.021213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-05-28 08:33:37.553154 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.021213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    28920 2023-05-28 08:33:54.025213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20665 2023-05-28 08:33:37.957155 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    35307 2023-05-28 08:33:54.025213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-05-28 08:33:54.033213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-05-28 08:33:38.553158 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.033213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-05-28 08:33:54.033213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-05-28 08:33:38.749158 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-05-28 08:33:54.037213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    25222 2023-05-28 08:33:54.025213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    37429 2023-05-28 08:33:37.753155 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.025213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-05-28 08:33:54.037213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-05-28 08:33:38.937159 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.037213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0    11277 2023-05-28 08:33:54.037213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
--rw-r--r--   0        0        0    15070 2023-05-28 08:33:39.129160 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.041213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-05-28 08:33:54.053213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-05-28 08:33:53.477211 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.053213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-05-28 08:33:54.057213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-05-28 08:33:53.673212 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-05-28 08:33:54.057213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-05-28 08:33:54.057213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-05-28 08:33:40.861166 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.061213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-28 08:33:54.061213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-05-28 08:33:41.049167 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-05-28 08:33:54.061213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-05-28 08:33:54.061213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-05-28 08:33:41.237167 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.065213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-05-28 08:33:54.065213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-05-28 08:33:42.009170 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.069213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-05-28 08:33:54.065213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-05-28 08:33:41.813169 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-05-28 08:33:54.065213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-05-28 08:33:54.069213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-05-28 08:33:42.193171 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.069213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    14046 2023-05-28 08:33:54.041213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23615 2023-05-28 08:33:39.329160 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.041213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-05-28 08:33:54.041213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-05-28 08:33:39.517161 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.045213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-05-28 08:33:54.045213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-05-28 08:33:39.709162 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-05-28 08:33:54.045213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-05-28 08:33:54.049213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-05-28 08:33:39.901162 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.049213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-05-28 08:33:54.185214 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-05-28 08:33:52.265207 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.189214 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-05-28 08:33:54.189214 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-05-28 08:33:52.461208 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-28 08:33:54.189214 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-05-28 08:33:54.189214 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-05-28 08:33:52.657208 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.193214 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-05-28 08:33:54.193214 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-05-28 08:33:52.897209 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-28 08:33:54.193214 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-05-28 08:33:54.193214 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-05-28 08:33:53.097210 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-05-28 08:33:54.197214 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-05-28 08:33:54.197214 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-05-28 08:33:53.289211 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.197214 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-05-28 08:33:54.121214 qwak_core-0.0.80/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-05-28 08:33:46.421186 qwak_core-0.0.80/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.125213 qwak_core-0.0.80/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-05-28 08:33:54.125213 qwak_core-0.0.80/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-28 08:33:46.625187 qwak_core-0.0.80/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-28 08:33:54.125213 qwak_core-0.0.80/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-05-28 08:33:54.005213 qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-05-28 08:33:36.753151 qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.009213 qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-28 08:33:54.009213 qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-05-28 08:33:36.945152 qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.013213 qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-05-28 08:33:54.013213 qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-05-28 08:33:37.145152 qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-05-28 08:33:54.017213 qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-05-28 08:33:54.017213 qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-05-28 08:33:37.345153 qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.021213 qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-05-28 08:33:54.097213 qwak_core-0.0.80/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-05-28 08:33:44.181178 qwak_core-0.0.80/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-05-28 08:33:54.097213 qwak_core-0.0.80/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     3757 2023-05-28 08:33:54.125213 qwak_core-0.0.80/_qwak_proto/qwak/instance_template/instance_template_pb2.py
--rw-r--r--   0        0        0     4235 2023-05-28 08:33:46.841188 qwak_core-0.0.80/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.129214 qwak_core-0.0.80/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
--rw-r--r--   0        0        0     4722 2023-05-28 08:33:54.129214 qwak_core-0.0.80/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
--rw-r--r--   0        0        0     3245 2023-05-28 08:33:47.049188 qwak_core-0.0.80/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
--rw-r--r--   0        0        0     5240 2023-05-28 08:33:54.129214 qwak_core-0.0.80/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-05-28 08:33:54.141214 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-05-28 08:33:48.237192 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.145214 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-05-28 08:33:54.145214 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-05-28 08:33:48.429193 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.145214 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-05-28 08:33:54.145214 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-05-28 08:33:48.629194 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.149214 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-05-28 08:33:54.149214 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-05-28 08:33:48.833195 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.149214 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-28 08:33:54.149214 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-05-28 08:33:49.041195 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.153214 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-05-28 08:33:54.153214 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-05-28 08:33:49.249196 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-05-28 08:33:54.153214 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-05-28 08:33:54.157214 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-05-28 08:33:49.437197 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.157214 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-05-28 08:33:54.133214 qwak_core-0.0.80/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-05-28 08:33:47.449190 qwak_core-0.0.80/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.133214 qwak_core-0.0.80/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-05-28 08:33:54.141214 qwak_core-0.0.80/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-05-28 08:33:48.049192 qwak_core-0.0.80/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.141214 qwak_core-0.0.80/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-05-28 08:33:54.137214 qwak_core-0.0.80/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-05-28 08:33:47.653190 qwak_core-0.0.80/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-05-28 08:33:54.137214 qwak_core-0.0.80/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0    10138 2023-05-28 08:33:54.137214 qwak_core-0.0.80/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    14337 2023-05-28 08:33:47.857191 qwak_core-0.0.80/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.137214 qwak_core-0.0.80/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-05-28 08:33:54.117214 qwak_core-0.0.80/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-05-28 08:33:45.829184 qwak_core-0.0.80/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-05-28 08:33:54.117214 qwak_core-0.0.80/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-05-28 08:33:53.985213 qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-05-28 08:33:36.345150 qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-05-28 08:33:53.989213 qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-05-28 08:33:53.985213 qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-05-28 08:33:36.145149 qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:53.985213 qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-05-28 08:33:53.989213 qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-05-28 08:33:36.549150 qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-05-28 08:33:53.989213 qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-05-28 08:33:54.113214 qwak_core-0.0.80/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-05-28 08:33:45.389182 qwak_core-0.0.80/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-05-28 08:33:54.113214 qwak_core-0.0.80/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-05-28 08:33:54.133214 qwak_core-0.0.80/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-05-28 08:33:47.241189 qwak_core-0.0.80/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-05-28 08:33:54.133214 qwak_core-0.0.80/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-05-28 08:33:53.981213 qwak_core-0.0.80/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-05-28 08:33:33.965141 qwak_core-0.0.80/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:53.981213 qwak_core-0.0.80/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-05-28 08:33:53.981213 qwak_core-0.0.80/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-05-28 08:33:33.773140 qwak_core-0.0.80/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-05-28 08:33:53.981213 qwak_core-0.0.80/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-05-28 08:33:53.973213 qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-05-28 08:33:33.185138 qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:53.973213 qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-05-28 08:33:53.973213 qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-05-28 08:33:33.373139 qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:53.977213 qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-05-28 08:33:53.977213 qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-05-28 08:33:33.569140 qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-05-28 08:33:53.977213 qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-05-28 08:33:54.161214 qwak_core-0.0.80/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-05-28 08:33:49.845198 qwak_core-0.0.80/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-05-28 08:33:54.161214 qwak_core-0.0.80/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-05-28 08:33:54.157214 qwak_core-0.0.80/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-05-28 08:33:49.645198 qwak_core-0.0.80/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.157214 qwak_core-0.0.80/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0    10851 2023-05-28 08:33:53.997213 qwak_core-0.0.80/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0    13974 2023-05-28 08:33:35.349146 qwak_core-0.0.80/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:53.997213 qwak_core-0.0.80/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     2993 2023-05-28 08:33:54.001213 qwak_core-0.0.80/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2568 2023-05-28 08:33:35.545147 qwak_core-0.0.80/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 08:33:54.001213 qwak_core-0.0.80/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     2661 2023-05-28 08:33:55.445218 qwak_core-0.0.80/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-28 08:33:55.445218 qwak_core-0.0.80/qwak/__init__.py
--rw-r--r--   0        0        0     1501 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    12899 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/automations/automations.py
--rw-r--r--   0        0        0     9638 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/automations/batch_execution_action.py
--rw-r--r--   0        0        0    19120 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/automations/build_and_deploy_action.py
--rw-r--r--   0        0        0     1697 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/automations/common.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5362 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0      211 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    18388 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    14847 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/instance_template/__init__.py
--rw-r--r--   0        0        0     2495 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/instance_template/client.py
--rw-r--r--   0        0        0       41 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3316 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     4707 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     1263 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     1941 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2987 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1717 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0       89 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0      738 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28013 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     9261 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/const.py
--rw-r--r--   0        0        0     1435 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6083 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      873 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/schema.py
--rw-r--r--   0        0        0     2970 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      338 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     1963 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0      848 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2511 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      650 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0      975 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/testing/fixtures.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/tools/__init__.py
--rw-r--r--   0        0        0      107 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/tools/logger/__init__.py
--rw-r--r--   0        0        0     9598 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/tools/logger/logging.yml
--rw-r--r--   0        0        0       46 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12316 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5806 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     3905 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/instance_template_management_service.py
--rw-r--r--   0        0        0     2696 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     4186 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13583 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.80/setup.py
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.80/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-05-28 11:32:53.200344 qwak_core-0.0.81/README.md
+-rw-r--r--   0        0        0        0 2023-05-28 11:34:28.292432 qwak_core-0.0.81/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-05-28 11:34:28.316432 qwak_core-0.0.81/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-05-28 11:34:09.708412 qwak_core-0.0.81/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.316432 qwak_core-0.0.81/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-05-28 11:34:28.312432 qwak_core-0.0.81/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-05-28 11:34:09.384412 qwak_core-0.0.81/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.312432 qwak_core-0.0.81/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-05-28 11:34:28.312432 qwak_core-0.0.81/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-05-28 11:34:09.548412 qwak_core-0.0.81/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.312432 qwak_core-0.0.81/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-05-28 11:34:28.304432 qwak_core-0.0.81/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-05-28 11:34:08.888411 qwak_core-0.0.81/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-05-28 11:34:28.308432 qwak_core-0.0.81/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-28 11:34:28.308432 qwak_core-0.0.81/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-05-28 11:34:09.056411 qwak_core-0.0.81/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.308432 qwak_core-0.0.81/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4864 2023-05-28 11:34:28.308432 qwak_core-0.0.81/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5792 2023-05-28 11:34:09.224412 qwak_core-0.0.81/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.312432 qwak_core-0.0.81/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-05-28 11:34:28.296432 qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-05-28 11:34:08.720411 qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-05-28 11:34:28.296432 qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5670 2023-05-28 11:34:28.296432 qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8035 2023-05-28 11:34:09.872412 qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.296432 qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-05-28 11:34:28.300432 qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-05-28 11:34:10.200413 qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.300432 qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-05-28 11:34:28.304432 qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-05-28 11:34:10.364413 qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-05-28 11:34:28.304432 qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-05-28 11:34:28.300432 qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-05-28 11:34:10.036412 qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.300432 qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-05-28 11:34:28.304432 qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-05-28 11:34:10.528413 qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.304432 qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-05-28 11:34:28.340432 qwak_core-0.0.81/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-05-28 11:34:12.868415 qwak_core-0.0.81/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.344432 qwak_core-0.0.81/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-05-28 11:34:28.344432 qwak_core-0.0.81/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-05-28 11:34:13.032415 qwak_core-0.0.81/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-05-28 11:34:28.344432 qwak_core-0.0.81/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-05-28 11:34:28.404432 qwak_core-0.0.81/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-05-28 11:34:17.696420 qwak_core-0.0.81/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.404432 qwak_core-0.0.81/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-05-28 11:34:28.404432 qwak_core-0.0.81/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-05-28 11:34:17.856420 qwak_core-0.0.81/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-05-28 11:34:28.404432 qwak_core-0.0.81/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-05-28 11:34:28.408432 qwak_core-0.0.81/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-05-28 11:34:18.696421 qwak_core-0.0.81/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-05-28 11:34:28.408432 qwak_core-0.0.81/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-05-28 11:34:28.408432 qwak_core-0.0.81/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-05-28 11:34:18.532421 qwak_core-0.0.81/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.408432 qwak_core-0.0.81/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5777 2023-05-28 11:34:28.412432 qwak_core-0.0.81/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8264 2023-05-28 11:34:18.860422 qwak_core-0.0.81/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.412432 qwak_core-0.0.81/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-05-28 11:34:28.412432 qwak_core-0.0.81/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-05-28 11:34:19.024422 qwak_core-0.0.81/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-05-28 11:34:28.412432 qwak_core-0.0.81/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12352 2023-05-28 11:34:28.492432 qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    18970 2023-05-28 11:34:26.084430 qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.492432 qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5775 2023-05-28 11:34:28.488433 qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8308 2023-05-28 11:34:25.752429 qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.488433 qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-05-28 11:34:28.492432 qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-05-28 11:34:25.912429 qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.492432 qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-05-28 11:34:28.484433 qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-05-28 11:34:25.412429 qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-05-28 11:34:28.484433 qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-05-28 11:34:28.488433 qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-05-28 11:34:25.588429 qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.488433 qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-05-28 11:34:28.496432 qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-05-28 11:34:26.572430 qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.500433 qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-05-28 11:34:28.496432 qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-05-28 11:34:26.412430 qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.496432 qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-05-28 11:34:28.496432 qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-05-28 11:34:26.248430 qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.496432 qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-05-28 11:34:28.484433 qwak_core-0.0.81/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-05-28 11:34:25.240429 qwak_core-0.0.81/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.484433 qwak_core-0.0.81/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-05-28 11:34:28.480432 qwak_core-0.0.81/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-05-28 11:34:24.896428 qwak_core-0.0.81/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.480432 qwak_core-0.0.81/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    42145 2023-05-28 11:34:28.480432 qwak_core-0.0.81/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    55993 2023-05-28 11:34:25.072428 qwak_core-0.0.81/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-05-28 11:34:28.480432 qwak_core-0.0.81/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    20255 2023-05-28 11:34:28.436432 qwak_core-0.0.81/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    17495 2023-05-28 11:34:20.712423 qwak_core-0.0.81/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    20359 2023-05-28 11:34:28.436432 qwak_core-0.0.81/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-05-28 11:34:28.432433 qwak_core-0.0.81/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-05-28 11:34:20.544423 qwak_core-0.0.81/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.436432 qwak_core-0.0.81/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11034 2023-05-28 11:34:28.424432 qwak_core-0.0.81/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18276 2023-05-28 11:34:20.212423 qwak_core-0.0.81/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.428432 qwak_core-0.0.81/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-05-28 11:34:28.428432 qwak_core-0.0.81/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-05-28 11:34:20.376423 qwak_core-0.0.81/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.428432 qwak_core-0.0.81/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-05-28 11:34:28.428432 qwak_core-0.0.81/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-05-28 11:34:20.876423 qwak_core-0.0.81/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-05-28 11:34:28.432433 qwak_core-0.0.81/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38245 2023-05-28 11:34:28.432433 qwak_core-0.0.81/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52572 2023-05-28 11:34:21.232424 qwak_core-0.0.81/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-05-28 11:34:28.432433 qwak_core-0.0.81/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-05-28 11:34:28.440432 qwak_core-0.0.81/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-05-28 11:34:21.572424 qwak_core-0.0.81/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.444432 qwak_core-0.0.81/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-05-28 11:34:28.444432 qwak_core-0.0.81/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-28 11:34:21.736425 qwak_core-0.0.81/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-28 11:34:28.444432 qwak_core-0.0.81/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-05-28 11:34:28.420432 qwak_core-0.0.81/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-05-28 11:34:19.716422 qwak_core-0.0.81/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.420432 qwak_core-0.0.81/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-05-28 11:34:28.420432 qwak_core-0.0.81/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-05-28 11:34:19.884423 qwak_core-0.0.81/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-05-28 11:34:28.424432 qwak_core-0.0.81/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-05-28 11:34:28.416432 qwak_core-0.0.81/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-05-28 11:34:19.372422 qwak_core-0.0.81/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.416432 qwak_core-0.0.81/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    43712 2023-05-28 11:34:28.416432 qwak_core-0.0.81/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    63341 2023-05-28 11:34:19.200422 qwak_core-0.0.81/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.416432 qwak_core-0.0.81/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-05-28 11:34:28.416432 qwak_core-0.0.81/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-05-28 11:34:19.548422 qwak_core-0.0.81/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-05-28 11:34:28.420432 qwak_core-0.0.81/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-05-28 11:34:28.332432 qwak_core-0.0.81/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-05-28 11:34:12.024414 qwak_core-0.0.81/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.332432 qwak_core-0.0.81/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-28 11:34:28.332432 qwak_core-0.0.81/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-05-28 11:34:12.196415 qwak_core-0.0.81/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.336432 qwak_core-0.0.81/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-05-28 11:34:28.336432 qwak_core-0.0.81/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-05-28 11:34:12.368415 qwak_core-0.0.81/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-05-28 11:34:28.336432 qwak_core-0.0.81/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-05-28 11:34:28.384432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-05-28 11:34:16.708419 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.388432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-05-28 11:34:28.384432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-05-28 11:34:16.548419 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-05-28 11:34:28.384432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11432 2023-05-28 11:34:28.368432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    12882 2023-05-28 11:34:15.056418 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.368432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5303 2023-05-28 11:34:28.364432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8604 2023-05-28 11:34:14.892417 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.364432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-05-28 11:34:28.360432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-05-28 11:34:14.380417 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.360432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    28920 2023-05-28 11:34:28.364432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20665 2023-05-28 11:34:14.728417 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    35307 2023-05-28 11:34:28.364432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-05-28 11:34:28.368432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-05-28 11:34:15.220418 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.368432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-05-28 11:34:28.372432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-05-28 11:34:15.384418 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-05-28 11:34:28.372432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    25269 2023-05-28 11:34:28.360432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    37664 2023-05-28 11:34:14.552417 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.360432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-05-28 11:34:28.372432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-05-28 11:34:15.548418 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.372432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0    11277 2023-05-28 11:34:28.376432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
+-rw-r--r--   0        0        0    15070 2023-05-28 11:34:15.712418 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.376432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-05-28 11:34:28.388432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-05-28 11:34:27.768432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.388432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-05-28 11:34:28.388432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-05-28 11:34:27.968432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-05-28 11:34:28.392432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-05-28 11:34:28.392432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-05-28 11:34:17.200420 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.392432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-28 11:34:28.392432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-05-28 11:34:17.368420 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-05-28 11:34:28.396432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-05-28 11:34:28.396432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-05-28 11:34:17.528420 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.396432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-05-28 11:34:28.400432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-05-28 11:34:18.200421 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.400432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-05-28 11:34:28.396432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-05-28 11:34:18.028421 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-05-28 11:34:28.400432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-05-28 11:34:28.400432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-05-28 11:34:18.368421 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.400432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    14046 2023-05-28 11:34:28.376432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23615 2023-05-28 11:34:15.876418 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.376432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-05-28 11:34:28.380432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-05-28 11:34:16.044419 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.380432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-05-28 11:34:28.380432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-05-28 11:34:16.212419 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-05-28 11:34:28.380432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-05-28 11:34:28.380432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-05-28 11:34:16.380419 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.384432 qwak_core-0.0.81/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-05-28 11:34:28.500433 qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-05-28 11:34:26.736430 qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.500433 qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-05-28 11:34:28.500433 qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-05-28 11:34:26.900431 qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-28 11:34:28.504433 qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-05-28 11:34:28.504433 qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-05-28 11:34:27.064431 qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.504433 qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-05-28 11:34:28.504433 qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-05-28 11:34:27.244431 qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-28 11:34:28.508432 qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-05-28 11:34:28.508432 qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-05-28 11:34:27.416431 qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-05-28 11:34:28.508432 qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-05-28 11:34:28.508432 qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-05-28 11:34:27.580431 qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.512432 qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-05-28 11:34:28.444432 qwak_core-0.0.81/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-05-28 11:34:21.896425 qwak_core-0.0.81/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.444432 qwak_core-0.0.81/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-05-28 11:34:28.448433 qwak_core-0.0.81/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-28 11:34:22.060425 qwak_core-0.0.81/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-28 11:34:28.448433 qwak_core-0.0.81/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-05-28 11:34:28.348432 qwak_core-0.0.81/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-05-28 11:34:13.708416 qwak_core-0.0.81/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.348432 qwak_core-0.0.81/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-28 11:34:28.348432 qwak_core-0.0.81/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-05-28 11:34:13.876416 qwak_core-0.0.81/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.352432 qwak_core-0.0.81/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-05-28 11:34:28.352432 qwak_core-0.0.81/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-05-28 11:34:14.040417 qwak_core-0.0.81/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-05-28 11:34:28.356432 qwak_core-0.0.81/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-05-28 11:34:28.356432 qwak_core-0.0.81/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-05-28 11:34:14.208417 qwak_core-0.0.81/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.360432 qwak_core-0.0.81/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-05-28 11:34:28.424432 qwak_core-0.0.81/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-05-28 11:34:20.048423 qwak_core-0.0.81/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-05-28 11:34:28.424432 qwak_core-0.0.81/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     3757 2023-05-28 11:34:28.448433 qwak_core-0.0.81/_qwak_proto/qwak/instance_template/instance_template_pb2.py
+-rw-r--r--   0        0        0     4235 2023-05-28 11:34:22.224425 qwak_core-0.0.81/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.448433 qwak_core-0.0.81/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
+-rw-r--r--   0        0        0     4722 2023-05-28 11:34:28.452432 qwak_core-0.0.81/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
+-rw-r--r--   0        0        0     3245 2023-05-28 11:34:22.388425 qwak_core-0.0.81/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
+-rw-r--r--   0        0        0     5240 2023-05-28 11:34:28.452432 qwak_core-0.0.81/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-05-28 11:34:28.460432 qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-05-28 11:34:23.388426 qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.464433 qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-05-28 11:34:28.464433 qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-05-28 11:34:23.552427 qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.464433 qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-05-28 11:34:28.464433 qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-05-28 11:34:23.724427 qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.468433 qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-05-28 11:34:28.468433 qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-05-28 11:34:23.892427 qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.468433 qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-28 11:34:28.468433 qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-05-28 11:34:24.064427 qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.472432 qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-05-28 11:34:28.472432 qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-05-28 11:34:24.244427 qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-05-28 11:34:28.472432 qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-05-28 11:34:28.472432 qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-05-28 11:34:24.408428 qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.476432 qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-05-28 11:34:28.456432 qwak_core-0.0.81/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-05-28 11:34:22.720425 qwak_core-0.0.81/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.456432 qwak_core-0.0.81/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-05-28 11:34:28.460432 qwak_core-0.0.81/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-05-28 11:34:23.224426 qwak_core-0.0.81/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.460432 qwak_core-0.0.81/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-05-28 11:34:28.456432 qwak_core-0.0.81/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-05-28 11:34:22.888426 qwak_core-0.0.81/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-05-28 11:34:28.456432 qwak_core-0.0.81/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10138 2023-05-28 11:34:28.456432 qwak_core-0.0.81/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    14337 2023-05-28 11:34:23.056426 qwak_core-0.0.81/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.460432 qwak_core-0.0.81/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-05-28 11:34:28.440432 qwak_core-0.0.81/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-05-28 11:34:21.408424 qwak_core-0.0.81/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-05-28 11:34:28.440432 qwak_core-0.0.81/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-05-28 11:34:28.328432 qwak_core-0.0.81/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-05-28 11:34:13.368416 qwak_core-0.0.81/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-05-28 11:34:28.328432 qwak_core-0.0.81/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-05-28 11:34:28.328432 qwak_core-0.0.81/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-05-28 11:34:13.200416 qwak_core-0.0.81/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.328432 qwak_core-0.0.81/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-05-28 11:34:28.328432 qwak_core-0.0.81/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-05-28 11:34:13.532416 qwak_core-0.0.81/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-05-28 11:34:28.332432 qwak_core-0.0.81/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-05-28 11:34:28.436432 qwak_core-0.0.81/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-05-28 11:34:21.048424 qwak_core-0.0.81/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-05-28 11:34:28.440432 qwak_core-0.0.81/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-05-28 11:34:28.452432 qwak_core-0.0.81/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-05-28 11:34:22.556425 qwak_core-0.0.81/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-05-28 11:34:28.452432 qwak_core-0.0.81/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-05-28 11:34:28.324432 qwak_core-0.0.81/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-05-28 11:34:11.360414 qwak_core-0.0.81/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.324432 qwak_core-0.0.81/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-05-28 11:34:28.324432 qwak_core-0.0.81/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-05-28 11:34:11.196414 qwak_core-0.0.81/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-05-28 11:34:28.324432 qwak_core-0.0.81/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-05-28 11:34:28.316432 qwak_core-0.0.81/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-05-28 11:34:10.688413 qwak_core-0.0.81/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.316432 qwak_core-0.0.81/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-05-28 11:34:28.320432 qwak_core-0.0.81/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-05-28 11:34:10.852413 qwak_core-0.0.81/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.320432 qwak_core-0.0.81/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-05-28 11:34:28.320432 qwak_core-0.0.81/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-05-28 11:34:11.020413 qwak_core-0.0.81/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-05-28 11:34:28.320432 qwak_core-0.0.81/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-05-28 11:34:28.476432 qwak_core-0.0.81/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-05-28 11:34:24.736428 qwak_core-0.0.81/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-05-28 11:34:28.476432 qwak_core-0.0.81/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-05-28 11:34:28.476432 qwak_core-0.0.81/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-05-28 11:34:24.572428 qwak_core-0.0.81/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.476432 qwak_core-0.0.81/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0    10851 2023-05-28 11:34:28.336432 qwak_core-0.0.81/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0    13974 2023-05-28 11:34:12.536415 qwak_core-0.0.81/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.340432 qwak_core-0.0.81/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     2993 2023-05-28 11:34:28.340432 qwak_core-0.0.81/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2568 2023-05-28 11:34:12.700415 qwak_core-0.0.81/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 11:34:28.340432 qwak_core-0.0.81/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2661 2023-05-28 11:34:29.520434 qwak_core-0.0.81/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-28 11:34:29.520434 qwak_core-0.0.81/qwak/__init__.py
+-rw-r--r--   0        0        0     1501 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    12899 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/automations/automations.py
+-rw-r--r--   0        0        0     9638 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/automations/batch_execution_action.py
+-rw-r--r--   0        0        0    19120 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/automations/build_and_deploy_action.py
+-rw-r--r--   0        0        0     1697 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/automations/common.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0      211 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    18388 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    14847 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/instance_template/__init__.py
+-rw-r--r--   0        0        0     2495 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/instance_template/client.py
+-rw-r--r--   0        0        0       41 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-05-28 11:32:53.200344 qwak_core-0.0.81/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3316 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     4707 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     1263 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     1941 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2987 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1717 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0       89 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0      738 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28013 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     9261 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/inner/const.py
+-rw-r--r--   0        0        0     1435 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6083 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      873 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/schema.py
+-rw-r--r--   0        0        0     2970 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      338 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     1963 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0      848 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2511 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      650 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0      975 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-05-28 11:32:53.204344 qwak_core-0.0.81/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak/tools/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak/tools/logger/__init__.py
+-rw-r--r--   0        0        0     9598 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak/tools/logger/logging.yml
+-rw-r--r--   0        0        0       46 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12316 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5806 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     3905 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/instance_template_management_service.py
+-rw-r--r--   0        0        0     2696 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     4186 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13583 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-28 11:32:53.208344 qwak_core-0.0.81/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.81/setup.py
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.81/PKG-INFO
```

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from _qwak_proto.qwak.feature_store.sources import streaming_pb2 as qwak_dot_feature__store_dot_sources_dot_streaming__pb2
 from _qwak_proto.qwak.feature_store.features import execution_pb2 as qwak_dot_feature__store_dot_features_dot_execution__pb2
 from _qwak_proto.qwak.feature_store.features import aggregation_pb2 as qwak_dot_feature__store_dot_features_dot_aggregation__pb2
 from _qwak_proto.qwak.feature_store.features import monitoring_pb2 as qwak_dot_feature__store_dot_features_dot_monitoring__pb2
 from _qwak_proto.qwak.feature_store.features import real_time_feature_extractor_pb2 as qwak_dot_feature__store_dot_features_dot_real__time__feature__extractor__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3qwak/feature_store/features/feature_set_types.proto\x12\x1bqwak.feature.store.features\x1a\x1fgoogle/protobuf/timestamp.proto\x1a&qwak/feature_store/sources/batch.proto\x1a*qwak/feature_store/sources/streaming.proto\x1a+qwak/feature_store/features/execution.proto\x1a-qwak/feature_store/features/aggregation.proto\x1a,qwak/feature_store/features/monitoring.proto\x1a=qwak/feature_store/features/real_time_feature_extractor.proto\"\x9f\x04\n\x0e\x46\x65\x61tureSetType\x12I\n\x11\x62\x61tch_feature_set\x18\x05 \x01(\x0b\x32,.qwak.feature.store.features.BatchFeatureSetH\x00\x12Q\n\x16on_the_fly_feature_set\x18\x06 \x01(\x0b\x32/.qwak.feature.store.features.OnTheFlyFeatureSetH\x00\x12Q\n\x15streaming_feature_set\x18\x07 \x01(\x0b\x32\x30.qwak.feature.store.features.StreamingFeatureSetH\x00\x12V\n\x18streaming_feature_set_v1\x18\x08 \x01(\x0b\x32\x32.qwak.feature.store.features.StreamingFeatureSetV1H\x00\x12N\n\x14\x62\x61tch_feature_set_v1\x18\t \x01(\x0b\x32..qwak.feature.store.features.BatchFeatureSetV1H\x00\x12h\n!streaming_aggregation_feature_set\x18\n \x01(\x0b\x32;.qwak.feature.store.features.StreamingAggregationFeatureSetH\x00\x42\n\n\x08set_type\"\x9d\x03\n\x0f\x42\x61tchFeatureSet\x12\x19\n\x11scheduling_policy\x18\x01 \x01(\t\x12\x41\n\x0c\x64\x61ta_sources\x18\x02 \x03(\x0b\x32\'.qwak.feature.store.sources.BatchSourceB\x02\x18\x01\x12\x37\n\x08\x62\x61\x63kfill\x18\x03 \x01(\x0b\x32%.qwak.feature.store.features.Backfill\x12\x37\n\x08\x66unction\x18\x04 \x01(\x0b\x32%.qwak.feature.store.features.Function\x12U\n\x19\x66\x65\x61ture_set_batch_sources\x18\x05 \x03(\x0b\x32\x32.qwak.feature.store.features.FeatureSetBatchSource\x12\x63\n\x19monitoring_configurations\x18\x06 \x01(\x0b\x32@.qwak.feature.store.features.monitoring.MonitoringConfigurations\"\xc0\x05\n\x11\x42\x61tchFeatureSetV1\x12\x19\n\x11scheduling_policy\x18\x01 \x01(\t\x12\x37\n\x08\x62\x61\x63kfill\x18\x02 \x01(\x0b\x32%.qwak.feature.store.features.Backfill\x12;\n\x08\x66unction\x18\x03 \x01(\x0b\x32%.qwak.feature.store.features.FunctionB\x02\x18\x01\x12U\n\x19\x66\x65\x61ture_set_batch_sources\x18\x04 \x03(\x0b\x32\x32.qwak.feature.store.features.FeatureSetBatchSource\x12L\n\x0e\x65xecution_spec\x18\x05 \x01(\x0b\x32\x34.qwak.feature.store.features.execution.ExecutionSpec\x12\x14\n\x0coffline_sink\x18\x06 \x01(\x08\x12\x13\n\x0bonline_sink\x18\x07 \x01(\x08\x12\x63\n\x19monitoring_configurations\x18\x08 \x01(\x0b\x32@.qwak.feature.store.features.monitoring.MonitoringConfigurations\x12\x1d\n\x15timestamp_column_name\x18\t \x01(\t\x12\x43\n\x0etransformation\x18\n \x01(\x0b\x32+.qwak.feature.store.features.Transformation\x12&\n\x1eqwak_internal_protocol_version\x18\x0b \x01(\x05\x12Y\n\x1areal_time_feature_extrator\x18\x0c \x01(\x0b\x32\x35.qwak.feature.store.features.RealTimeFeatureExtractor\"\x9d\x01\n\x15\x46\x65\x61tureSetBatchSource\x12<\n\x0b\x64\x61ta_source\x18\x01 \x01(\x0b\x32\'.qwak.feature.store.sources.BatchSource\x12\x46\n\x0bread_policy\x18\x02 \x01(\x0b\x32\x31.qwak.feature.store.features.DataSourceReadPolicy\"X\n\x13StreamingFeatureSet\x12\x41\n\x0c\x64\x61ta_sources\x18\x01 \x03(\x0b\x32+.qwak.feature.store.sources.StreamingSource\"\x81\x03\n\x15StreamingFeatureSetV1\x12\x41\n\x0c\x64\x61ta_sources\x18\x01 \x03(\x0b\x32+.qwak.feature.store.sources.StreamingSource\x12\x43\n\x0etransformation\x18\x02 \x01(\x0b\x32+.qwak.feature.store.features.Transformation\x12U\n\x0e\x65xecution_spec\x18\x03 \x01(\x0b\x32=.qwak.feature.store.features.execution.StreamingExecutionSpec\x12\x1d\n\x15timestamp_column_name\x18\x04 \x01(\t\x12\x1f\n\x17online_trigger_interval\x18\x05 \x01(\x05\x12!\n\x19offline_scheduling_policy\x18\x06 \x01(\t\x12&\n\x1eqwak_internal_protocol_version\x18\x07 \x01(\x05\"\x97\x04\n\x1eStreamingAggregationFeatureSet\x12\x41\n\x0c\x64\x61ta_sources\x18\x01 \x03(\x0b\x32+.qwak.feature.store.sources.StreamingSource\x12\x43\n\x0etransformation\x18\x02 \x01(\x0b\x32+.qwak.feature.store.features.Transformation\x12U\n\x0e\x65xecution_spec\x18\x03 \x01(\x0b\x32=.qwak.feature.store.features.execution.StreamingExecutionSpec\x12\x1d\n\x15timestamp_column_name\x18\x04 \x01(\t\x12\x1f\n\x17online_trigger_interval\x18\x05 \x01(\x05\x12$\n\x1c\x63ompaction_scheduling_policy\x18\x06 \x01(\t\x12\x46\n\x10\x61ggregation_spec\x18\x07 \x01(\x0b\x32,.qwak.feature.store.features.AggregationSpec\x12@\n\rbackfill_spec\x18\x08 \x01(\x0b\x32).qwak.feature.store.features.BackfillSpec\x12&\n\x1eqwak_internal_protocol_version\x18\t \x01(\x05\"\xc3\x01\n\x1b\x42\x61\x63kfillBatchDataSourceSpec\x12<\n\x0b\x64\x61ta_source\x18\x01 \x01(\x0b\x32\'.qwak.feature.store.sources.BatchSource\x12\x33\n\x0fstart_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"|\n\x16\x42\x61\x63kfillDataSourceSpec\x12Z\n\x16\x62\x61tch_data_source_spec\x18\x01 \x01(\x0b\x32\x38.qwak.feature.store.features.BackfillBatchDataSourceSpecH\x00\x42\x06\n\x04type\"\xe1\x02\n\x0c\x42\x61\x63kfillSpec\x12T\n\x0e\x65xecution_spec\x18\x01 \x01(\x0b\x32<.qwak.feature.store.features.execution.BackfillExecutionSpec\x12\x33\n\x0fstart_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x43\n\x0etransformation\x18\x04 \x01(\x0b\x32+.qwak.feature.store.features.Transformation\x12N\n\x11\x64\x61ta_source_specs\x18\x05 \x03(\x0b\x32\x33.qwak.feature.store.features.BackfillDataSourceSpec\"\x9f\x01\n\x0f\x41ggregationSpec\x12O\n\x0c\x61ggregations\x18\x01 \x03(\x0b\x32\x39.qwak.feature.store.features.aggregation.AggregationField\x12\x15\n\rslide_seconds\x18\x02 \x01(\x05\x12$\n\x1c\x61llowed_late_arrival_seconds\x18\x03 \x01(\x05\"\x9f\x02\n\x0eTransformation\x12L\n\x12udf_transformation\x18\x01 \x01(\x0b\x32..qwak.feature.store.features.UdfTransformationH\x00\x12L\n\x12sql_transformation\x18\x02 \x01(\x0b\x32..qwak.feature.store.features.SqlTransformationH\x00\x12R\n\x15koalas_transformation\x18\x03 \x01(\x0b\x32\x31.qwak.feature.store.features.KoalasTransformationH\x00\x12\x15\n\rartifact_path\x18\x04 \x01(\tB\x06\n\x04type\"*\n\x11UdfTransformation\x12\x15\n\rfunction_name\x18\x01 \x01(\t\"8\n\x11SqlTransformation\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\x16\n\x0e\x66unction_names\x18\x02 \x03(\t\"-\n\x14KoalasTransformation\x12\x15\n\rfunction_name\x18\x01 \x01(\t\"f\n\x12OnTheFlyFeatureSet\x12:\n\x08\x66unction\x18\x01 \x01(\x0b\x32(.qwak.feature.store.features.UdfFunction\x12\x14\n\x0crequirements\x18\x02 \x01(\x0c\"\x96\x01\n\x08\x46unction\x12@\n\x0csql_function\x18\x01 \x01(\x0b\x32(.qwak.feature.store.features.SqlFunctionH\x00\x12@\n\x0cudf_function\x18\x02 \x01(\x0b\x32(.qwak.feature.store.features.UdfFunctionH\x00\x42\x06\n\x04type\"\xb5\x01\n\x08\x42\x61\x63kfill\x12.\n\nstart_date\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\rfillup_method\x18\x02 \x01(\x0e\x32\x32.qwak.feature.store.features.Backfill.FillUpMethod\".\n\x0c\x46illUpMethod\x12\x10\n\x0c\x41S_SCHEDULED\x10\x00\x12\x0c\n\x08SNAPSHOT\x10\x01\"\x1a\n\x0bSqlFunction\x12\x0b\n\x03sql\x18\x01 \x01(\t\"\x1b\n\x0bUdfFunction\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x0c\"\t\n\x07NewOnly\"\xa0\x01\n\tTimeFrame\x12\x0f\n\x07minutes\x18\x01 \x01(\x05\x12\x37\n\x07vanilla\x18\x02 \x01(\x0b\x32$.qwak.feature.store.features.VanillaH\x00\x12?\n\x0b\x61ggregation\x18\x03 \x01(\x0b\x32(.qwak.feature.store.features.AggregationH\x00\x42\x08\n\x06\x66lavor\"k\n\x0b\x41ggregation\x12T\n\x16\x61ggregation_population\x18\x01 \x01(\x0b\x32\x32.qwak.feature.store.features.AggregationPopulationH\x00\x42\x06\n\x04type\"\x17\n\x15\x41ggregationPopulation\"\x1c\n\x1aPopulationTimeframeNewOnly\"j\n\x13PopulationTimeframe\x12K\n\x08new_only\x18\x01 \x01(\x0b\x32\x37.qwak.feature.store.features.PopulationTimeframeNewOnlyH\x00\x42\x06\n\x04type\"\t\n\x07Vanilla\"\x9f\x01\n\x08\x46ullRead\x12\x37\n\x07\x64\x65\x66\x61ult\x18\x01 \x01(\x0b\x32$.qwak.feature.store.features.VanillaH\x00\x12P\n\x14population_timeframe\x18\x02 \x01(\x0b\x32\x30.qwak.feature.store.features.PopulationTimeframeH\x00\x42\x08\n\x06\x66lavor\"\xd2\x01\n\x14\x44\x61taSourceReadPolicy\x12\x38\n\x08new_only\x18\x01 \x01(\x0b\x32$.qwak.feature.store.features.NewOnlyH\x00\x12<\n\ntime_frame\x18\x02 \x01(\x0b\x32&.qwak.feature.store.features.TimeFrameH\x00\x12:\n\tfull_read\x18\x03 \x01(\x0b\x32%.qwak.feature.store.features.FullReadH\x00\x42\x06\n\x04typeB[\n&com.qwak.ai.feature.store.features.apiP\x01Z/qwak/featurestore/features;featurestorefeaturesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3qwak/feature_store/features/feature_set_types.proto\x12\x1bqwak.feature.store.features\x1a\x1fgoogle/protobuf/timestamp.proto\x1a&qwak/feature_store/sources/batch.proto\x1a*qwak/feature_store/sources/streaming.proto\x1a+qwak/feature_store/features/execution.proto\x1a-qwak/feature_store/features/aggregation.proto\x1a,qwak/feature_store/features/monitoring.proto\x1a=qwak/feature_store/features/real_time_feature_extractor.proto\"\x9f\x04\n\x0e\x46\x65\x61tureSetType\x12I\n\x11\x62\x61tch_feature_set\x18\x05 \x01(\x0b\x32,.qwak.feature.store.features.BatchFeatureSetH\x00\x12Q\n\x16on_the_fly_feature_set\x18\x06 \x01(\x0b\x32/.qwak.feature.store.features.OnTheFlyFeatureSetH\x00\x12Q\n\x15streaming_feature_set\x18\x07 \x01(\x0b\x32\x30.qwak.feature.store.features.StreamingFeatureSetH\x00\x12V\n\x18streaming_feature_set_v1\x18\x08 \x01(\x0b\x32\x32.qwak.feature.store.features.StreamingFeatureSetV1H\x00\x12N\n\x14\x62\x61tch_feature_set_v1\x18\t \x01(\x0b\x32..qwak.feature.store.features.BatchFeatureSetV1H\x00\x12h\n!streaming_aggregation_feature_set\x18\n \x01(\x0b\x32;.qwak.feature.store.features.StreamingAggregationFeatureSetH\x00\x42\n\n\x08set_type\"\x9d\x03\n\x0f\x42\x61tchFeatureSet\x12\x19\n\x11scheduling_policy\x18\x01 \x01(\t\x12\x41\n\x0c\x64\x61ta_sources\x18\x02 \x03(\x0b\x32\'.qwak.feature.store.sources.BatchSourceB\x02\x18\x01\x12\x37\n\x08\x62\x61\x63kfill\x18\x03 \x01(\x0b\x32%.qwak.feature.store.features.Backfill\x12\x37\n\x08\x66unction\x18\x04 \x01(\x0b\x32%.qwak.feature.store.features.Function\x12U\n\x19\x66\x65\x61ture_set_batch_sources\x18\x05 \x03(\x0b\x32\x32.qwak.feature.store.features.FeatureSetBatchSource\x12\x63\n\x19monitoring_configurations\x18\x06 \x01(\x0b\x32@.qwak.feature.store.features.monitoring.MonitoringConfigurations\"\xd8\x05\n\x11\x42\x61tchFeatureSetV1\x12\x19\n\x11scheduling_policy\x18\x01 \x01(\t\x12\x37\n\x08\x62\x61\x63kfill\x18\x02 \x01(\x0b\x32%.qwak.feature.store.features.Backfill\x12;\n\x08\x66unction\x18\x03 \x01(\x0b\x32%.qwak.feature.store.features.FunctionB\x02\x18\x01\x12U\n\x19\x66\x65\x61ture_set_batch_sources\x18\x04 \x03(\x0b\x32\x32.qwak.feature.store.features.FeatureSetBatchSource\x12L\n\x0e\x65xecution_spec\x18\x05 \x01(\x0b\x32\x34.qwak.feature.store.features.execution.ExecutionSpec\x12\x14\n\x0coffline_sink\x18\x06 \x01(\x08\x12\x13\n\x0bonline_sink\x18\x07 \x01(\x08\x12\x63\n\x19monitoring_configurations\x18\x08 \x01(\x0b\x32@.qwak.feature.store.features.monitoring.MonitoringConfigurations\x12\x1d\n\x15timestamp_column_name\x18\t \x01(\t\x12\x43\n\x0etransformation\x18\n \x01(\x0b\x32+.qwak.feature.store.features.Transformation\x12&\n\x1eqwak_internal_protocol_version\x18\x0b \x01(\x05\x12\\\n\x1breal_time_feature_extractor\x18\x0c \x01(\x0b\x32\x35.qwak.feature.store.features.RealTimeFeatureExtractorH\x00\x42\x13\n\x11\x66\x65\x61ture_extractor\"\x9d\x01\n\x15\x46\x65\x61tureSetBatchSource\x12<\n\x0b\x64\x61ta_source\x18\x01 \x01(\x0b\x32\'.qwak.feature.store.sources.BatchSource\x12\x46\n\x0bread_policy\x18\x02 \x01(\x0b\x32\x31.qwak.feature.store.features.DataSourceReadPolicy\"X\n\x13StreamingFeatureSet\x12\x41\n\x0c\x64\x61ta_sources\x18\x01 \x03(\x0b\x32+.qwak.feature.store.sources.StreamingSource\"\x81\x03\n\x15StreamingFeatureSetV1\x12\x41\n\x0c\x64\x61ta_sources\x18\x01 \x03(\x0b\x32+.qwak.feature.store.sources.StreamingSource\x12\x43\n\x0etransformation\x18\x02 \x01(\x0b\x32+.qwak.feature.store.features.Transformation\x12U\n\x0e\x65xecution_spec\x18\x03 \x01(\x0b\x32=.qwak.feature.store.features.execution.StreamingExecutionSpec\x12\x1d\n\x15timestamp_column_name\x18\x04 \x01(\t\x12\x1f\n\x17online_trigger_interval\x18\x05 \x01(\x05\x12!\n\x19offline_scheduling_policy\x18\x06 \x01(\t\x12&\n\x1eqwak_internal_protocol_version\x18\x07 \x01(\x05\"\x97\x04\n\x1eStreamingAggregationFeatureSet\x12\x41\n\x0c\x64\x61ta_sources\x18\x01 \x03(\x0b\x32+.qwak.feature.store.sources.StreamingSource\x12\x43\n\x0etransformation\x18\x02 \x01(\x0b\x32+.qwak.feature.store.features.Transformation\x12U\n\x0e\x65xecution_spec\x18\x03 \x01(\x0b\x32=.qwak.feature.store.features.execution.StreamingExecutionSpec\x12\x1d\n\x15timestamp_column_name\x18\x04 \x01(\t\x12\x1f\n\x17online_trigger_interval\x18\x05 \x01(\x05\x12$\n\x1c\x63ompaction_scheduling_policy\x18\x06 \x01(\t\x12\x46\n\x10\x61ggregation_spec\x18\x07 \x01(\x0b\x32,.qwak.feature.store.features.AggregationSpec\x12@\n\rbackfill_spec\x18\x08 \x01(\x0b\x32).qwak.feature.store.features.BackfillSpec\x12&\n\x1eqwak_internal_protocol_version\x18\t \x01(\x05\"\xc3\x01\n\x1b\x42\x61\x63kfillBatchDataSourceSpec\x12<\n\x0b\x64\x61ta_source\x18\x01 \x01(\x0b\x32\'.qwak.feature.store.sources.BatchSource\x12\x33\n\x0fstart_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"|\n\x16\x42\x61\x63kfillDataSourceSpec\x12Z\n\x16\x62\x61tch_data_source_spec\x18\x01 \x01(\x0b\x32\x38.qwak.feature.store.features.BackfillBatchDataSourceSpecH\x00\x42\x06\n\x04type\"\xe1\x02\n\x0c\x42\x61\x63kfillSpec\x12T\n\x0e\x65xecution_spec\x18\x01 \x01(\x0b\x32<.qwak.feature.store.features.execution.BackfillExecutionSpec\x12\x33\n\x0fstart_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x43\n\x0etransformation\x18\x04 \x01(\x0b\x32+.qwak.feature.store.features.Transformation\x12N\n\x11\x64\x61ta_source_specs\x18\x05 \x03(\x0b\x32\x33.qwak.feature.store.features.BackfillDataSourceSpec\"\x9f\x01\n\x0f\x41ggregationSpec\x12O\n\x0c\x61ggregations\x18\x01 \x03(\x0b\x32\x39.qwak.feature.store.features.aggregation.AggregationField\x12\x15\n\rslide_seconds\x18\x02 \x01(\x05\x12$\n\x1c\x61llowed_late_arrival_seconds\x18\x03 \x01(\x05\"\x9f\x02\n\x0eTransformation\x12L\n\x12udf_transformation\x18\x01 \x01(\x0b\x32..qwak.feature.store.features.UdfTransformationH\x00\x12L\n\x12sql_transformation\x18\x02 \x01(\x0b\x32..qwak.feature.store.features.SqlTransformationH\x00\x12R\n\x15koalas_transformation\x18\x03 \x01(\x0b\x32\x31.qwak.feature.store.features.KoalasTransformationH\x00\x12\x15\n\rartifact_path\x18\x04 \x01(\tB\x06\n\x04type\"*\n\x11UdfTransformation\x12\x15\n\rfunction_name\x18\x01 \x01(\t\"8\n\x11SqlTransformation\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\x16\n\x0e\x66unction_names\x18\x02 \x03(\t\"-\n\x14KoalasTransformation\x12\x15\n\rfunction_name\x18\x01 \x01(\t\"f\n\x12OnTheFlyFeatureSet\x12:\n\x08\x66unction\x18\x01 \x01(\x0b\x32(.qwak.feature.store.features.UdfFunction\x12\x14\n\x0crequirements\x18\x02 \x01(\x0c\"\x96\x01\n\x08\x46unction\x12@\n\x0csql_function\x18\x01 \x01(\x0b\x32(.qwak.feature.store.features.SqlFunctionH\x00\x12@\n\x0cudf_function\x18\x02 \x01(\x0b\x32(.qwak.feature.store.features.UdfFunctionH\x00\x42\x06\n\x04type\"\xb5\x01\n\x08\x42\x61\x63kfill\x12.\n\nstart_date\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\rfillup_method\x18\x02 \x01(\x0e\x32\x32.qwak.feature.store.features.Backfill.FillUpMethod\".\n\x0c\x46illUpMethod\x12\x10\n\x0c\x41S_SCHEDULED\x10\x00\x12\x0c\n\x08SNAPSHOT\x10\x01\"\x1a\n\x0bSqlFunction\x12\x0b\n\x03sql\x18\x01 \x01(\t\"\x1b\n\x0bUdfFunction\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x0c\"\t\n\x07NewOnly\"\xa0\x01\n\tTimeFrame\x12\x0f\n\x07minutes\x18\x01 \x01(\x05\x12\x37\n\x07vanilla\x18\x02 \x01(\x0b\x32$.qwak.feature.store.features.VanillaH\x00\x12?\n\x0b\x61ggregation\x18\x03 \x01(\x0b\x32(.qwak.feature.store.features.AggregationH\x00\x42\x08\n\x06\x66lavor\"k\n\x0b\x41ggregation\x12T\n\x16\x61ggregation_population\x18\x01 \x01(\x0b\x32\x32.qwak.feature.store.features.AggregationPopulationH\x00\x42\x06\n\x04type\"\x17\n\x15\x41ggregationPopulation\"\x1c\n\x1aPopulationTimeframeNewOnly\"j\n\x13PopulationTimeframe\x12K\n\x08new_only\x18\x01 \x01(\x0b\x32\x37.qwak.feature.store.features.PopulationTimeframeNewOnlyH\x00\x42\x06\n\x04type\"\t\n\x07Vanilla\"\x9f\x01\n\x08\x46ullRead\x12\x37\n\x07\x64\x65\x66\x61ult\x18\x01 \x01(\x0b\x32$.qwak.feature.store.features.VanillaH\x00\x12P\n\x14population_timeframe\x18\x02 \x01(\x0b\x32\x30.qwak.feature.store.features.PopulationTimeframeH\x00\x42\x08\n\x06\x66lavor\"\xd2\x01\n\x14\x44\x61taSourceReadPolicy\x12\x38\n\x08new_only\x18\x01 \x01(\x0b\x32$.qwak.feature.store.features.NewOnlyH\x00\x12<\n\ntime_frame\x18\x02 \x01(\x0b\x32&.qwak.feature.store.features.TimeFrameH\x00\x12:\n\tfull_read\x18\x03 \x01(\x0b\x32%.qwak.feature.store.features.FullReadH\x00\x42\x06\n\x04typeB[\n&com.qwak.ai.feature.store.features.apiP\x01Z/qwak/featurestore/features;featurestorefeaturesb\x06proto3')
 
 
 
 _FEATURESETTYPE = DESCRIPTOR.message_types_by_name['FeatureSetType']
 _BATCHFEATURESET = DESCRIPTOR.message_types_by_name['BatchFeatureSet']
 _BATCHFEATURESETV1 = DESCRIPTOR.message_types_by_name['BatchFeatureSetV1']
 _FEATURESETBATCHSOURCE = DESCRIPTOR.message_types_by_name['FeatureSetBatchSource']
@@ -267,63 +267,63 @@
   _BATCHFEATURESETV1.fields_by_name['function']._options = None
   _BATCHFEATURESETV1.fields_by_name['function']._serialized_options = b'\030\001'
   _FEATURESETTYPE._serialized_start=403
   _FEATURESETTYPE._serialized_end=946
   _BATCHFEATURESET._serialized_start=949
   _BATCHFEATURESET._serialized_end=1362
   _BATCHFEATURESETV1._serialized_start=1365
-  _BATCHFEATURESETV1._serialized_end=2069
-  _FEATURESETBATCHSOURCE._serialized_start=2072
-  _FEATURESETBATCHSOURCE._serialized_end=2229
-  _STREAMINGFEATURESET._serialized_start=2231
-  _STREAMINGFEATURESET._serialized_end=2319
-  _STREAMINGFEATURESETV1._serialized_start=2322
-  _STREAMINGFEATURESETV1._serialized_end=2707
-  _STREAMINGAGGREGATIONFEATURESET._serialized_start=2710
-  _STREAMINGAGGREGATIONFEATURESET._serialized_end=3245
-  _BACKFILLBATCHDATASOURCESPEC._serialized_start=3248
-  _BACKFILLBATCHDATASOURCESPEC._serialized_end=3443
-  _BACKFILLDATASOURCESPEC._serialized_start=3445
-  _BACKFILLDATASOURCESPEC._serialized_end=3569
-  _BACKFILLSPEC._serialized_start=3572
-  _BACKFILLSPEC._serialized_end=3925
-  _AGGREGATIONSPEC._serialized_start=3928
-  _AGGREGATIONSPEC._serialized_end=4087
-  _TRANSFORMATION._serialized_start=4090
-  _TRANSFORMATION._serialized_end=4377
-  _UDFTRANSFORMATION._serialized_start=4379
-  _UDFTRANSFORMATION._serialized_end=4421
-  _SQLTRANSFORMATION._serialized_start=4423
-  _SQLTRANSFORMATION._serialized_end=4479
-  _KOALASTRANSFORMATION._serialized_start=4481
-  _KOALASTRANSFORMATION._serialized_end=4526
-  _ONTHEFLYFEATURESET._serialized_start=4528
-  _ONTHEFLYFEATURESET._serialized_end=4630
-  _FUNCTION._serialized_start=4633
-  _FUNCTION._serialized_end=4783
-  _BACKFILL._serialized_start=4786
-  _BACKFILL._serialized_end=4967
-  _BACKFILL_FILLUPMETHOD._serialized_start=4921
-  _BACKFILL_FILLUPMETHOD._serialized_end=4967
-  _SQLFUNCTION._serialized_start=4969
-  _SQLFUNCTION._serialized_end=4995
-  _UDFFUNCTION._serialized_start=4997
-  _UDFFUNCTION._serialized_end=5024
-  _NEWONLY._serialized_start=5026
-  _NEWONLY._serialized_end=5035
-  _TIMEFRAME._serialized_start=5038
-  _TIMEFRAME._serialized_end=5198
-  _AGGREGATION._serialized_start=5200
-  _AGGREGATION._serialized_end=5307
-  _AGGREGATIONPOPULATION._serialized_start=5309
-  _AGGREGATIONPOPULATION._serialized_end=5332
-  _POPULATIONTIMEFRAMENEWONLY._serialized_start=5334
-  _POPULATIONTIMEFRAMENEWONLY._serialized_end=5362
-  _POPULATIONTIMEFRAME._serialized_start=5364
-  _POPULATIONTIMEFRAME._serialized_end=5470
-  _VANILLA._serialized_start=5472
-  _VANILLA._serialized_end=5481
-  _FULLREAD._serialized_start=5484
-  _FULLREAD._serialized_end=5643
-  _DATASOURCEREADPOLICY._serialized_start=5646
-  _DATASOURCEREADPOLICY._serialized_end=5856
+  _BATCHFEATURESETV1._serialized_end=2093
+  _FEATURESETBATCHSOURCE._serialized_start=2096
+  _FEATURESETBATCHSOURCE._serialized_end=2253
+  _STREAMINGFEATURESET._serialized_start=2255
+  _STREAMINGFEATURESET._serialized_end=2343
+  _STREAMINGFEATURESETV1._serialized_start=2346
+  _STREAMINGFEATURESETV1._serialized_end=2731
+  _STREAMINGAGGREGATIONFEATURESET._serialized_start=2734
+  _STREAMINGAGGREGATIONFEATURESET._serialized_end=3269
+  _BACKFILLBATCHDATASOURCESPEC._serialized_start=3272
+  _BACKFILLBATCHDATASOURCESPEC._serialized_end=3467
+  _BACKFILLDATASOURCESPEC._serialized_start=3469
+  _BACKFILLDATASOURCESPEC._serialized_end=3593
+  _BACKFILLSPEC._serialized_start=3596
+  _BACKFILLSPEC._serialized_end=3949
+  _AGGREGATIONSPEC._serialized_start=3952
+  _AGGREGATIONSPEC._serialized_end=4111
+  _TRANSFORMATION._serialized_start=4114
+  _TRANSFORMATION._serialized_end=4401
+  _UDFTRANSFORMATION._serialized_start=4403
+  _UDFTRANSFORMATION._serialized_end=4445
+  _SQLTRANSFORMATION._serialized_start=4447
+  _SQLTRANSFORMATION._serialized_end=4503
+  _KOALASTRANSFORMATION._serialized_start=4505
+  _KOALASTRANSFORMATION._serialized_end=4550
+  _ONTHEFLYFEATURESET._serialized_start=4552
+  _ONTHEFLYFEATURESET._serialized_end=4654
+  _FUNCTION._serialized_start=4657
+  _FUNCTION._serialized_end=4807
+  _BACKFILL._serialized_start=4810
+  _BACKFILL._serialized_end=4991
+  _BACKFILL_FILLUPMETHOD._serialized_start=4945
+  _BACKFILL_FILLUPMETHOD._serialized_end=4991
+  _SQLFUNCTION._serialized_start=4993
+  _SQLFUNCTION._serialized_end=5019
+  _UDFFUNCTION._serialized_start=5021
+  _UDFFUNCTION._serialized_end=5048
+  _NEWONLY._serialized_start=5050
+  _NEWONLY._serialized_end=5059
+  _TIMEFRAME._serialized_start=5062
+  _TIMEFRAME._serialized_end=5222
+  _AGGREGATION._serialized_start=5224
+  _AGGREGATION._serialized_end=5331
+  _AGGREGATIONPOPULATION._serialized_start=5333
+  _AGGREGATIONPOPULATION._serialized_end=5356
+  _POPULATIONTIMEFRAMENEWONLY._serialized_start=5358
+  _POPULATIONTIMEFRAMENEWONLY._serialized_end=5386
+  _POPULATIONTIMEFRAME._serialized_start=5388
+  _POPULATIONTIMEFRAME._serialized_end=5494
+  _VANILLA._serialized_start=5496
+  _VANILLA._serialized_end=5505
+  _FULLREAD._serialized_start=5508
+  _FULLREAD._serialized_end=5667
+  _DATASOURCEREADPOLICY._serialized_start=5670
+  _DATASOURCEREADPOLICY._serialized_end=5880
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     EXECUTION_SPEC_FIELD_NUMBER: builtins.int
     OFFLINE_SINK_FIELD_NUMBER: builtins.int
     ONLINE_SINK_FIELD_NUMBER: builtins.int
     MONITORING_CONFIGURATIONS_FIELD_NUMBER: builtins.int
     TIMESTAMP_COLUMN_NAME_FIELD_NUMBER: builtins.int
     TRANSFORMATION_FIELD_NUMBER: builtins.int
     QWAK_INTERNAL_PROTOCOL_VERSION_FIELD_NUMBER: builtins.int
-    REAL_TIME_FEATURE_EXTRATOR_FIELD_NUMBER: builtins.int
+    REAL_TIME_FEATURE_EXTRACTOR_FIELD_NUMBER: builtins.int
     scheduling_policy: builtins.str
     """Scheduling policy of batch feature set. Can be a cron string format or @annotation: @daily, @monthly, @yearly"""
     @property
     def backfill(self) -> global___Backfill:
         """Backfill strategy"""
     @property
     def function(self) -> global___Function:
@@ -145,34 +145,34 @@
     """Name of the timestamp column (must exist in the result), i.e: event time column"""
     @property
     def transformation(self) -> global___Transformation:
         """Transformation"""
     qwak_internal_protocol_version: builtins.int
     """Qwak featureset version"""
     @property
-    def real_time_feature_extrator(self) -> qwak.feature_store.features.real_time_feature_extractor_pb2.RealTimeFeatureExtractor:
-        """Real time feature extractor"""
+    def real_time_feature_extractor(self) -> qwak.feature_store.features.real_time_feature_extractor_pb2.RealTimeFeatureExtractor: ...
     def __init__(
         self,
         *,
         scheduling_policy: builtins.str = ...,
         backfill: global___Backfill | None = ...,
         function: global___Function | None = ...,
         feature_set_batch_sources: collections.abc.Iterable[global___FeatureSetBatchSource] | None = ...,
         execution_spec: qwak.feature_store.features.execution_pb2.ExecutionSpec | None = ...,
         offline_sink: builtins.bool = ...,
         online_sink: builtins.bool = ...,
         monitoring_configurations: qwak.feature_store.features.monitoring_pb2.MonitoringConfigurations | None = ...,
         timestamp_column_name: builtins.str = ...,
         transformation: global___Transformation | None = ...,
         qwak_internal_protocol_version: builtins.int = ...,
-        real_time_feature_extrator: qwak.feature_store.features.real_time_feature_extractor_pb2.RealTimeFeatureExtractor | None = ...,
+        real_time_feature_extractor: qwak.feature_store.features.real_time_feature_extractor_pb2.RealTimeFeatureExtractor | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["backfill", b"backfill", "execution_spec", b"execution_spec", "function", b"function", "monitoring_configurations", b"monitoring_configurations", "real_time_feature_extrator", b"real_time_feature_extrator", "transformation", b"transformation"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["backfill", b"backfill", "execution_spec", b"execution_spec", "feature_set_batch_sources", b"feature_set_batch_sources", "function", b"function", "monitoring_configurations", b"monitoring_configurations", "offline_sink", b"offline_sink", "online_sink", b"online_sink", "qwak_internal_protocol_version", b"qwak_internal_protocol_version", "real_time_feature_extrator", b"real_time_feature_extrator", "scheduling_policy", b"scheduling_policy", "timestamp_column_name", b"timestamp_column_name", "transformation", b"transformation"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["backfill", b"backfill", "execution_spec", b"execution_spec", "feature_extractor", b"feature_extractor", "function", b"function", "monitoring_configurations", b"monitoring_configurations", "real_time_feature_extractor", b"real_time_feature_extractor", "transformation", b"transformation"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["backfill", b"backfill", "execution_spec", b"execution_spec", "feature_extractor", b"feature_extractor", "feature_set_batch_sources", b"feature_set_batch_sources", "function", b"function", "monitoring_configurations", b"monitoring_configurations", "offline_sink", b"offline_sink", "online_sink", b"online_sink", "qwak_internal_protocol_version", b"qwak_internal_protocol_version", "real_time_feature_extractor", b"real_time_feature_extractor", "scheduling_policy", b"scheduling_policy", "timestamp_column_name", b"timestamp_column_name", "transformation", b"transformation"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["feature_extractor", b"feature_extractor"]) -> typing_extensions.Literal["real_time_feature_extractor"] | None: ...
 
 global___BatchFeatureSetV1 = BatchFeatureSetV1
 
 class FeatureSetBatchSource(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DATA_SOURCE_FIELD_NUMBER: builtins.int
```

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/instance_template/instance_template_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/instance_template/instance_template_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.81/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.81/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.81/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/pyproject.toml` & `qwak_core-0.0.81/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.80"
+version = "0.0.81"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.0.80/qwak/automations/__init__.py` & `qwak_core-0.0.81/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/automations/automation_executions.py` & `qwak_core-0.0.81/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/automations/automations.py` & `qwak_core-0.0.81/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/automations/batch_execution_action.py` & `qwak_core-0.0.81/qwak/automations/batch_execution_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/automations/build_and_deploy_action.py` & `qwak_core-0.0.81/qwak/automations/build_and_deploy_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/automations/common.py` & `qwak_core-0.0.81/qwak/automations/common.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.81/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.81/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.81/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.81/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.81/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/clients/alert_management/client.py` & `qwak_core-0.0.81/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/clients/analytics/client.py` & `qwak_core-0.0.81/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/clients/audience/client.py` & `qwak_core-0.0.81/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/clients/automation_management/client.py` & `qwak_core-0.0.81/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.81/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.81/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.81/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.81/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/clients/build_management/client.py` & `qwak_core-0.0.81/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.81/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.81/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/clients/deployment/client.py` & `qwak_core-0.0.81/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.81/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.81/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.81/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.81/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/clients/instance_template/client.py` & `qwak_core-0.0.81/qwak/clients/instance_template/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.81/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/clients/logging_client/client.py` & `qwak_core-0.0.81/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/clients/model_management/client.py` & `qwak_core-0.0.81/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/clients/project/client.py` & `qwak_core-0.0.81/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/clients/secret_service/client.py` & `qwak_core-0.0.81/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.81/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.81/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.81/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.0.81/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/feature_store/_common/functions.py` & `qwak_core-0.0.81/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.81/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.81/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.81/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.81/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.81/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.81/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.81/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.81/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.81/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.81/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.81/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.81/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.81/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.81/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.81/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.81/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.81/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.81/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.81/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.81/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.81/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.0.81/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.0.81/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/feature_store/offline/client.py` & `qwak_core-0.0.81/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/feature_store/online/client.py` & `qwak_core-0.0.81/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/inner/const.py` & `qwak_core-0.0.81/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.81/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.81/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.81/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.81/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/inner/singleton_meta.py` & `qwak_core-0.0.81/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/inner/tool/auth.py` & `qwak_core-0.0.81/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.81/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.81/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.81/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.81/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/model/adapters/__init__.py` & `qwak_core-0.0.81/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.81/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.81/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.81/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.81/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.81/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/model/base.py` & `qwak_core-0.0.81/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/model/decorators/api.py` & `qwak_core-0.0.81/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.81/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/model/experiment_tracking.py` & `qwak_core-0.0.81/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/model/schema.py` & `qwak_core-0.0.81/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/model/schema_entities.py` & `qwak_core-0.0.81/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.0.81/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/model/tools/adapters/input.py` & `qwak_core-0.0.81/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.0.81/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.0.81/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.0.81/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.0.81/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.0.81/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/model/tools/adapters/output.py` & `qwak_core-0.0.81/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.0.81/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.0.81/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.0.81/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.0.81/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/model/tools/run_model_locally.py` & `qwak_core-0.0.81/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.81/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.81/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.81/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.81/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.81/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.81/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/qwak_client/client.py` & `qwak_core-0.0.81/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.81/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/qwak_client/models/model.py` & `qwak_core-0.0.81/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.81/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.81/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/tools/logger/logger.py` & `qwak_core-0.0.81/qwak/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak/tools/logger/logging.yml` & `qwak_core-0.0.81/qwak/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/instance_template_management_service.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/instance_template_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.81/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/qwak_services_mock/services_mock.py` & `qwak_core-0.0.81/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.80/setup.py` & `qwak_core-0.0.81/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
  'typeguard>=2,<3']
 
 extras_require = \
 {'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.80',
+    'version': '0.0.81',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.80/PKG-INFO` & `qwak_core-0.0.81/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.80
+Version: 0.0.81
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

