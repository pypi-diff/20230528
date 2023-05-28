# Comparing `tmp/qwak_core-0.0.79.tar.gz` & `tmp/qwak_core-0.0.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.79.tar", max compression
+gzip compressed data, was "qwak_core-0.0.80.tar", max compression
```

## Comparing `qwak_core-0.0.79.tar` & `qwak_core-0.0.80.tar`

### file list

```diff
@@ -1,582 +1,582 @@
--rw-r--r--   0        0        0      264 2023-05-28 07:36:02.598409 qwak_core-0.0.79/README.md
--rw-r--r--   0        0        0        0 2023-05-28 07:37:49.526860 qwak_core-0.0.79/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-05-28 07:37:49.550860 qwak_core-0.0.79/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-05-28 07:37:27.934770 qwak_core-0.0.79/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.554860 qwak_core-0.0.79/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-05-28 07:37:49.546860 qwak_core-0.0.79/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-05-28 07:37:27.554769 qwak_core-0.0.79/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.550860 qwak_core-0.0.79/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-05-28 07:37:49.550860 qwak_core-0.0.79/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-05-28 07:37:27.746770 qwak_core-0.0.79/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.550860 qwak_core-0.0.79/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-05-28 07:37:49.542860 qwak_core-0.0.79/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-05-28 07:37:26.998766 qwak_core-0.0.79/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-05-28 07:37:49.542860 qwak_core-0.0.79/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-28 07:37:49.542860 qwak_core-0.0.79/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-05-28 07:37:27.182767 qwak_core-0.0.79/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.546860 qwak_core-0.0.79/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4864 2023-05-28 07:37:49.546860 qwak_core-0.0.79/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5792 2023-05-28 07:37:27.370768 qwak_core-0.0.79/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.546860 qwak_core-0.0.79/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-05-28 07:37:49.530860 qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-05-28 07:37:26.810766 qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-05-28 07:37:49.530860 qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5670 2023-05-28 07:37:49.530860 qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8035 2023-05-28 07:37:28.126771 qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.530860 qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-05-28 07:37:49.534860 qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-05-28 07:37:28.510773 qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.534860 qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-05-28 07:37:49.538860 qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-05-28 07:37:28.702773 qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-05-28 07:37:49.538860 qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-05-28 07:37:49.534860 qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-05-28 07:37:28.318772 qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.534860 qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-05-28 07:37:49.538860 qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-05-28 07:37:28.890774 qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.542860 qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-05-28 07:37:49.582860 qwak_core-0.0.79/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-05-28 07:37:31.634786 qwak_core-0.0.79/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.582860 qwak_core-0.0.79/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-05-28 07:37:49.586860 qwak_core-0.0.79/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-05-28 07:37:31.830787 qwak_core-0.0.79/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-05-28 07:37:49.586860 qwak_core-0.0.79/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-05-28 07:37:49.650860 qwak_core-0.0.79/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-05-28 07:37:37.254809 qwak_core-0.0.79/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.654861 qwak_core-0.0.79/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-05-28 07:37:49.654861 qwak_core-0.0.79/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-05-28 07:37:37.442810 qwak_core-0.0.79/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-05-28 07:37:49.654861 qwak_core-0.0.79/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-05-28 07:37:49.658861 qwak_core-0.0.79/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-05-28 07:37:38.414814 qwak_core-0.0.79/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-05-28 07:37:49.658861 qwak_core-0.0.79/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-05-28 07:37:49.654861 qwak_core-0.0.79/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-05-28 07:37:38.226813 qwak_core-0.0.79/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.658861 qwak_core-0.0.79/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5777 2023-05-28 07:37:49.662860 qwak_core-0.0.79/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8264 2023-05-28 07:37:38.606815 qwak_core-0.0.79/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.662860 qwak_core-0.0.79/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-05-28 07:37:49.662860 qwak_core-0.0.79/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-05-28 07:37:38.794815 qwak_core-0.0.79/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-05-28 07:37:49.662860 qwak_core-0.0.79/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    12352 2023-05-28 07:37:49.754861 qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    18970 2023-05-28 07:37:47.142850 qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.754861 qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5775 2023-05-28 07:37:49.750861 qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8308 2023-05-28 07:37:46.750848 qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.750861 qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-05-28 07:37:49.754861 qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-05-28 07:37:46.942849 qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.754861 qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-05-28 07:37:49.746861 qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-05-28 07:37:46.358847 qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-05-28 07:37:49.746861 qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-05-28 07:37:49.746861 qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-05-28 07:37:46.558848 qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.750861 qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-05-28 07:37:49.762861 qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-05-28 07:37:47.722853 qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.762861 qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-05-28 07:37:49.758861 qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-05-28 07:37:47.530852 qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.758861 qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2023-05-28 07:37:49.758861 qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2023-05-28 07:37:47.334851 qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.758861 qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-05-28 07:37:49.742861 qwak_core-0.0.79/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-05-28 07:37:46.154846 qwak_core-0.0.79/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.746861 qwak_core-0.0.79/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-05-28 07:37:49.738861 qwak_core-0.0.79/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-05-28 07:37:45.742844 qwak_core-0.0.79/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.738861 qwak_core-0.0.79/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    42145 2023-05-28 07:37:49.742861 qwak_core-0.0.79/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    55993 2023-05-28 07:37:45.958845 qwak_core-0.0.79/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-05-28 07:37:49.742861 qwak_core-0.0.79/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    20255 2023-05-28 07:37:49.690861 qwak_core-0.0.79/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    17495 2023-05-28 07:37:40.762824 qwak_core-0.0.79/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    20359 2023-05-28 07:37:49.690861 qwak_core-0.0.79/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-05-28 07:37:49.686861 qwak_core-0.0.79/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-05-28 07:37:40.566823 qwak_core-0.0.79/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.686861 qwak_core-0.0.79/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11034 2023-05-28 07:37:49.678861 qwak_core-0.0.79/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18276 2023-05-28 07:37:40.182821 qwak_core-0.0.79/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.678861 qwak_core-0.0.79/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-05-28 07:37:49.682861 qwak_core-0.0.79/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-05-28 07:37:40.374822 qwak_core-0.0.79/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.682861 qwak_core-0.0.79/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-05-28 07:37:49.682861 qwak_core-0.0.79/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-05-28 07:37:40.954825 qwak_core-0.0.79/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-05-28 07:37:49.682861 qwak_core-0.0.79/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38245 2023-05-28 07:37:49.686861 qwak_core-0.0.79/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52572 2023-05-28 07:37:41.366826 qwak_core-0.0.79/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-05-28 07:37:49.686861 qwak_core-0.0.79/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-05-28 07:37:49.694861 qwak_core-0.0.79/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-05-28 07:37:41.770828 qwak_core-0.0.79/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.698861 qwak_core-0.0.79/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-05-28 07:37:49.698861 qwak_core-0.0.79/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-28 07:37:41.966829 qwak_core-0.0.79/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-28 07:37:49.698861 qwak_core-0.0.79/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-05-28 07:37:49.670861 qwak_core-0.0.79/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-05-28 07:37:39.598819 qwak_core-0.0.79/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.674861 qwak_core-0.0.79/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-05-28 07:37:49.674861 qwak_core-0.0.79/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-05-28 07:37:39.794820 qwak_core-0.0.79/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-05-28 07:37:49.674861 qwak_core-0.0.79/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-05-28 07:37:49.666860 qwak_core-0.0.79/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-05-28 07:37:39.198817 qwak_core-0.0.79/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.666860 qwak_core-0.0.79/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    43712 2023-05-28 07:37:49.666860 qwak_core-0.0.79/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    63341 2023-05-28 07:37:39.002816 qwak_core-0.0.79/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.666860 qwak_core-0.0.79/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-05-28 07:37:49.670861 qwak_core-0.0.79/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-05-28 07:37:39.402818 qwak_core-0.0.79/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-05-28 07:37:49.670861 qwak_core-0.0.79/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-05-28 07:37:49.570860 qwak_core-0.0.79/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-05-28 07:37:30.626781 qwak_core-0.0.79/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.574860 qwak_core-0.0.79/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-28 07:37:49.574860 qwak_core-0.0.79/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-05-28 07:37:30.818782 qwak_core-0.0.79/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.574860 qwak_core-0.0.79/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-05-28 07:37:49.578860 qwak_core-0.0.79/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-05-28 07:37:31.018783 qwak_core-0.0.79/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-05-28 07:37:49.578860 qwak_core-0.0.79/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-05-28 07:37:49.634860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-05-28 07:37:36.134804 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.634860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-05-28 07:37:49.630860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-05-28 07:37:35.946804 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-05-28 07:37:49.630860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0    11432 2023-05-28 07:37:49.610860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    12882 2023-05-28 07:37:34.214796 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.610860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5303 2023-05-28 07:37:49.610860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8604 2023-05-28 07:37:34.026796 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.610860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-05-28 07:37:49.602860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-05-28 07:37:33.426793 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.602860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    28920 2023-05-28 07:37:49.606860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20665 2023-05-28 07:37:33.830795 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    35307 2023-05-28 07:37:49.606860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-05-28 07:37:49.614860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-05-28 07:37:34.402797 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.614860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-05-28 07:37:49.614860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-05-28 07:37:34.594798 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-05-28 07:37:49.614860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    25222 2023-05-28 07:37:49.602860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    37429 2023-05-28 07:37:33.630794 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.606860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-05-28 07:37:49.618860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-05-28 07:37:34.782799 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.618860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0    11224 2023-05-28 07:37:49.618860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
--rw-r--r--   0        0        0    14819 2023-05-28 07:37:34.970800 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.622860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-05-28 07:37:49.634860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-05-28 07:37:49.058858 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.634860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-05-28 07:37:49.638860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-05-28 07:37:49.254859 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-05-28 07:37:49.638860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-05-28 07:37:49.638860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-05-28 07:37:36.698807 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.638860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-28 07:37:49.642861 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-05-28 07:37:36.882808 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-05-28 07:37:49.642861 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-05-28 07:37:49.642861 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-05-28 07:37:37.066808 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.642861 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-05-28 07:37:49.646860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-05-28 07:37:37.842811 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.650860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-05-28 07:37:49.646860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-05-28 07:37:37.642811 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-05-28 07:37:49.646860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-05-28 07:37:49.650860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-05-28 07:37:38.030812 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.650860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    14046 2023-05-28 07:37:49.622860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23615 2023-05-28 07:37:35.170800 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.622860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-05-28 07:37:49.622860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-05-28 07:37:35.362801 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.626860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-05-28 07:37:49.626860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-05-28 07:37:35.562802 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-05-28 07:37:49.626860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-05-28 07:37:49.626860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-05-28 07:37:35.754803 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.630860 qwak_core-0.0.79/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-05-28 07:37:49.762861 qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-05-28 07:37:47.910853 qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.762861 qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-05-28 07:37:49.766861 qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-05-28 07:37:48.098854 qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-28 07:37:49.766861 qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-05-28 07:37:49.770861 qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-05-28 07:37:48.286855 qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.770861 qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-05-28 07:37:49.770861 qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-05-28 07:37:48.482856 qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-28 07:37:49.770861 qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-05-28 07:37:49.774861 qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-05-28 07:37:48.682856 qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-05-28 07:37:49.774861 qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-05-28 07:37:49.774861 qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-05-28 07:37:48.870857 qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.774861 qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-05-28 07:37:49.702861 qwak_core-0.0.79/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-05-28 07:37:42.154830 qwak_core-0.0.79/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.702861 qwak_core-0.0.79/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-05-28 07:37:49.702861 qwak_core-0.0.79/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-28 07:37:42.350830 qwak_core-0.0.79/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-28 07:37:49.702861 qwak_core-0.0.79/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-05-28 07:37:49.590860 qwak_core-0.0.79/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-05-28 07:37:32.618790 qwak_core-0.0.79/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.590860 qwak_core-0.0.79/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-28 07:37:49.590860 qwak_core-0.0.79/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-05-28 07:37:32.814791 qwak_core-0.0.79/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.594860 qwak_core-0.0.79/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-05-28 07:37:49.594860 qwak_core-0.0.79/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-05-28 07:37:33.014791 qwak_core-0.0.79/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-05-28 07:37:49.598860 qwak_core-0.0.79/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-05-28 07:37:49.598860 qwak_core-0.0.79/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-05-28 07:37:33.214792 qwak_core-0.0.79/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.602860 qwak_core-0.0.79/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-05-28 07:37:49.674861 qwak_core-0.0.79/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-05-28 07:37:39.986821 qwak_core-0.0.79/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-05-28 07:37:49.678861 qwak_core-0.0.79/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     3757 2023-05-28 07:37:49.706861 qwak_core-0.0.79/_qwak_proto/qwak/instance_template/instance_template_pb2.py
--rw-r--r--   0        0        0     4235 2023-05-28 07:37:42.550831 qwak_core-0.0.79/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.706861 qwak_core-0.0.79/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
--rw-r--r--   0        0        0     4722 2023-05-28 07:37:49.706861 qwak_core-0.0.79/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
--rw-r--r--   0        0        0     3245 2023-05-28 07:37:42.754832 qwak_core-0.0.79/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
--rw-r--r--   0        0        0     5240 2023-05-28 07:37:49.706861 qwak_core-0.0.79/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-05-28 07:37:49.718861 qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-05-28 07:37:43.922837 qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.722861 qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-05-28 07:37:49.722861 qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-05-28 07:37:44.114838 qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.722861 qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-05-28 07:37:49.722861 qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-05-28 07:37:44.314839 qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.726861 qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-05-28 07:37:49.726861 qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-05-28 07:37:44.510839 qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.726861 qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-28 07:37:49.726861 qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-05-28 07:37:44.714840 qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.730861 qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-05-28 07:37:49.730861 qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-05-28 07:37:44.930841 qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-05-28 07:37:49.730861 qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-05-28 07:37:49.734861 qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-05-28 07:37:45.142842 qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.734861 qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-05-28 07:37:49.710861 qwak_core-0.0.79/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-05-28 07:37:43.146834 qwak_core-0.0.79/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.710861 qwak_core-0.0.79/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-05-28 07:37:49.718861 qwak_core-0.0.79/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-05-28 07:37:43.730836 qwak_core-0.0.79/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.718861 qwak_core-0.0.79/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-05-28 07:37:49.714861 qwak_core-0.0.79/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-05-28 07:37:43.346835 qwak_core-0.0.79/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-05-28 07:37:49.714861 qwak_core-0.0.79/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0    10138 2023-05-28 07:37:49.714861 qwak_core-0.0.79/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    14337 2023-05-28 07:37:43.538835 qwak_core-0.0.79/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.718861 qwak_core-0.0.79/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-05-28 07:37:49.694861 qwak_core-0.0.79/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-05-28 07:37:41.582827 qwak_core-0.0.79/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-05-28 07:37:49.694861 qwak_core-0.0.79/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-05-28 07:37:49.566860 qwak_core-0.0.79/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-05-28 07:37:32.218788 qwak_core-0.0.79/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-05-28 07:37:49.570860 qwak_core-0.0.79/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-05-28 07:37:49.566860 qwak_core-0.0.79/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-05-28 07:37:32.022787 qwak_core-0.0.79/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.566860 qwak_core-0.0.79/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-05-28 07:37:49.570860 qwak_core-0.0.79/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-05-28 07:37:32.418789 qwak_core-0.0.79/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-05-28 07:37:49.570860 qwak_core-0.0.79/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-05-28 07:37:49.690861 qwak_core-0.0.79/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-05-28 07:37:41.154825 qwak_core-0.0.79/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-05-28 07:37:49.694861 qwak_core-0.0.79/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-05-28 07:37:49.710861 qwak_core-0.0.79/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-05-28 07:37:42.954833 qwak_core-0.0.79/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-05-28 07:37:49.710861 qwak_core-0.0.79/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-05-28 07:37:49.562860 qwak_core-0.0.79/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-05-28 07:37:29.858778 qwak_core-0.0.79/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.566860 qwak_core-0.0.79/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-05-28 07:37:49.562860 qwak_core-0.0.79/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-05-28 07:37:29.666777 qwak_core-0.0.79/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-05-28 07:37:49.562860 qwak_core-0.0.79/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-05-28 07:37:49.554860 qwak_core-0.0.79/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-05-28 07:37:29.082775 qwak_core-0.0.79/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.554860 qwak_core-0.0.79/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-05-28 07:37:49.558860 qwak_core-0.0.79/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-05-28 07:37:29.278776 qwak_core-0.0.79/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.558860 qwak_core-0.0.79/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-05-28 07:37:49.558860 qwak_core-0.0.79/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-05-28 07:37:29.470777 qwak_core-0.0.79/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-05-28 07:37:49.558860 qwak_core-0.0.79/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-05-28 07:37:49.738861 qwak_core-0.0.79/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-05-28 07:37:45.538843 qwak_core-0.0.79/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-05-28 07:37:49.738861 qwak_core-0.0.79/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-05-28 07:37:49.734861 qwak_core-0.0.79/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-05-28 07:37:45.334843 qwak_core-0.0.79/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.734861 qwak_core-0.0.79/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0    10851 2023-05-28 07:37:49.578860 qwak_core-0.0.79/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0    13974 2023-05-28 07:37:31.254784 qwak_core-0.0.79/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.578860 qwak_core-0.0.79/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     2993 2023-05-28 07:37:49.582860 qwak_core-0.0.79/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2568 2023-05-28 07:37:31.446785 qwak_core-0.0.79/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 07:37:49.582860 qwak_core-0.0.79/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     2661 2023-05-28 07:37:51.330867 qwak_core-0.0.79/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-28 07:37:51.334867 qwak_core-0.0.79/qwak/__init__.py
--rw-r--r--   0        0        0     1501 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    12899 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/automations/automations.py
--rw-r--r--   0        0        0     9638 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/automations/batch_execution_action.py
--rw-r--r--   0        0        0    19120 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/automations/build_and_deploy_action.py
--rw-r--r--   0        0        0     1697 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/automations/common.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5362 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0      211 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    18388 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    14847 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/instance_template/__init__.py
--rw-r--r--   0        0        0     2495 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/instance_template/client.py
--rw-r--r--   0        0        0       41 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3316 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     4707 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     1263 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     1941 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2987 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1717 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-05-28 07:36:02.602409 qwak_core-0.0.79/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0       89 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0      738 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28013 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     9261 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/inner/const.py
--rw-r--r--   0        0        0     1435 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6083 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      873 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/schema.py
--rw-r--r--   0        0        0     2970 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      338 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     1963 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0      848 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2511 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      650 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0      975 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/testing/fixtures.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/tools/__init__.py
--rw-r--r--   0        0        0      107 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/tools/logger/__init__.py
--rw-r--r--   0        0        0     9598 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak/tools/logger/logging.yml
--rw-r--r--   0        0        0       46 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12316 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-05-28 07:36:02.606409 qwak_core-0.0.79/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-05-28 07:36:02.610409 qwak_core-0.0.79/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-05-28 07:36:02.610409 qwak_core-0.0.79/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-05-28 07:36:02.610409 qwak_core-0.0.79/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-05-28 07:36:02.610409 qwak_core-0.0.79/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-05-28 07:36:02.610409 qwak_core-0.0.79/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5806 2023-05-28 07:36:02.610409 qwak_core-0.0.79/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-05-28 07:36:02.610409 qwak_core-0.0.79/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-05-28 07:36:02.610409 qwak_core-0.0.79/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-05-28 07:36:02.610409 qwak_core-0.0.79/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-05-28 07:36:02.610409 qwak_core-0.0.79/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     3905 2023-05-28 07:36:02.610409 qwak_core-0.0.79/qwak_services_mock/mocks/instance_template_management_service.py
--rw-r--r--   0        0        0     2696 2023-05-28 07:36:02.610409 qwak_core-0.0.79/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-05-28 07:36:02.610409 qwak_core-0.0.79/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-05-28 07:36:02.610409 qwak_core-0.0.79/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-05-28 07:36:02.610409 qwak_core-0.0.79/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-05-28 07:36:02.610409 qwak_core-0.0.79/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     4186 2023-05-28 07:36:02.610409 qwak_core-0.0.79/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-05-28 07:36:02.610409 qwak_core-0.0.79/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-05-28 07:36:02.610409 qwak_core-0.0.79/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-05-28 07:36:02.610409 qwak_core-0.0.79/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.610409 qwak_core-0.0.79/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-05-28 07:36:02.610409 qwak_core-0.0.79/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13583 2023-05-28 07:36:02.610409 qwak_core-0.0.79/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-05-28 07:36:02.610409 qwak_core-0.0.79/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-05-28 07:36:02.610409 qwak_core-0.0.79/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.79/setup.py
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.79/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-05-28 08:32:06.172842 qwak_core-0.0.80/README.md
+-rw-r--r--   0        0        0        0 2023-05-28 08:33:53.945213 qwak_core-0.0.80/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-05-28 08:33:53.969213 qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-05-28 08:33:31.965134 qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:53.973213 qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-05-28 08:33:53.965213 qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-05-28 08:33:31.545132 qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:53.969213 qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-05-28 08:33:53.969213 qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-05-28 08:33:31.757133 qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:53.969213 qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-05-28 08:33:53.961213 qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-05-28 08:33:30.977130 qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-05-28 08:33:53.961213 qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-28 08:33:53.961213 qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-05-28 08:33:31.165131 qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:53.965213 qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4864 2023-05-28 08:33:53.965213 qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5792 2023-05-28 08:33:31.357132 qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:53.965213 qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-05-28 08:33:53.945213 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-05-28 08:33:30.789130 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-05-28 08:33:53.949213 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5670 2023-05-28 08:33:53.949213 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8035 2023-05-28 08:33:32.161134 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:53.949213 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-05-28 08:33:53.953213 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-05-28 08:33:32.565136 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:53.953213 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-05-28 08:33:53.957213 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-05-28 08:33:32.761137 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-05-28 08:33:53.957213 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-05-28 08:33:53.953213 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-05-28 08:33:32.353135 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:53.953213 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-05-28 08:33:53.957213 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-05-28 08:33:32.985137 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:53.957213 qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-05-28 08:33:54.001213 qwak_core-0.0.80/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-05-28 08:33:35.749148 qwak_core-0.0.80/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.001213 qwak_core-0.0.80/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-05-28 08:33:54.005213 qwak_core-0.0.80/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-05-28 08:33:35.949148 qwak_core-0.0.80/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-05-28 08:33:54.005213 qwak_core-0.0.80/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-05-28 08:33:54.069213 qwak_core-0.0.80/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-05-28 08:33:41.429168 qwak_core-0.0.80/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.073213 qwak_core-0.0.80/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-05-28 08:33:54.073213 qwak_core-0.0.80/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-05-28 08:33:41.621169 qwak_core-0.0.80/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-05-28 08:33:54.073213 qwak_core-0.0.80/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-05-28 08:33:54.077213 qwak_core-0.0.80/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-05-28 08:33:42.585172 qwak_core-0.0.80/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-05-28 08:33:54.077213 qwak_core-0.0.80/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-05-28 08:33:54.077213 qwak_core-0.0.80/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-05-28 08:33:42.397171 qwak_core-0.0.80/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.077213 qwak_core-0.0.80/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5777 2023-05-28 08:33:54.081213 qwak_core-0.0.80/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8264 2023-05-28 08:33:42.785173 qwak_core-0.0.80/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.081213 qwak_core-0.0.80/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-05-28 08:33:54.081213 qwak_core-0.0.80/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-05-28 08:33:42.973173 qwak_core-0.0.80/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-05-28 08:33:54.085214 qwak_core-0.0.80/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12352 2023-05-28 08:33:54.177214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    18970 2023-05-28 08:33:51.473204 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.177214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5775 2023-05-28 08:33:54.173214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8308 2023-05-28 08:33:51.069203 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.173214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-05-28 08:33:54.177214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-05-28 08:33:51.273203 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.177214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-05-28 08:33:54.169214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-05-28 08:33:50.661201 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-05-28 08:33:54.169214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-05-28 08:33:54.173214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-05-28 08:33:50.865202 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.173214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-05-28 08:33:54.185214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-05-28 08:33:52.073206 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.185214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-05-28 08:33:54.181214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-05-28 08:33:51.873206 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.185214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-05-28 08:33:54.181214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-05-28 08:33:51.665205 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.181214 qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-05-28 08:33:54.165214 qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-05-28 08:33:50.441201 qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.169214 qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-05-28 08:33:54.161214 qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-05-28 08:33:50.037199 qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.165214 qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    42145 2023-05-28 08:33:54.165214 qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    55993 2023-05-28 08:33:50.245200 qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-05-28 08:33:54.165214 qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    20255 2023-05-28 08:33:54.109213 qwak_core-0.0.80/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    17495 2023-05-28 08:33:44.981181 qwak_core-0.0.80/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    20359 2023-05-28 08:33:54.113214 qwak_core-0.0.80/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-05-28 08:33:54.109213 qwak_core-0.0.80/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-05-28 08:33:44.781180 qwak_core-0.0.80/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.109213 qwak_core-0.0.80/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11034 2023-05-28 08:33:54.097213 qwak_core-0.0.80/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18276 2023-05-28 08:33:44.381179 qwak_core-0.0.80/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.101214 qwak_core-0.0.80/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-05-28 08:33:54.101214 qwak_core-0.0.80/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-05-28 08:33:44.577179 qwak_core-0.0.80/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.101214 qwak_core-0.0.80/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-05-28 08:33:54.105213 qwak_core-0.0.80/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-05-28 08:33:45.185181 qwak_core-0.0.80/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-05-28 08:33:54.105213 qwak_core-0.0.80/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38245 2023-05-28 08:33:54.105213 qwak_core-0.0.80/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52572 2023-05-28 08:33:45.605183 qwak_core-0.0.80/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-05-28 08:33:54.105213 qwak_core-0.0.80/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-05-28 08:33:54.117214 qwak_core-0.0.80/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-05-28 08:33:46.021185 qwak_core-0.0.80/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.117214 qwak_core-0.0.80/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-05-28 08:33:54.121214 qwak_core-0.0.80/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-28 08:33:46.221185 qwak_core-0.0.80/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-28 08:33:54.121214 qwak_core-0.0.80/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-05-28 08:33:54.093213 qwak_core-0.0.80/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-05-28 08:33:43.789177 qwak_core-0.0.80/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.093213 qwak_core-0.0.80/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-05-28 08:33:54.093213 qwak_core-0.0.80/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-05-28 08:33:43.989177 qwak_core-0.0.80/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-05-28 08:33:54.093213 qwak_core-0.0.80/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-05-28 08:33:54.085214 qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-05-28 08:33:43.393175 qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.089213 qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    43712 2023-05-28 08:33:54.085214 qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    63341 2023-05-28 08:33:43.197174 qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.085214 qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-05-28 08:33:54.089213 qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-05-28 08:33:43.601176 qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-05-28 08:33:54.089213 qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-05-28 08:33:53.989213 qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-05-28 08:33:34.749144 qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:53.993213 qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-28 08:33:53.993213 qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-05-28 08:33:34.953144 qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:53.993213 qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-05-28 08:33:53.993213 qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-05-28 08:33:35.153145 qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-05-28 08:33:53.997213 qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-05-28 08:33:54.053213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-05-28 08:33:40.277164 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.053213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-05-28 08:33:54.049213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-05-28 08:33:40.089163 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-05-28 08:33:54.049213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11432 2023-05-28 08:33:54.029213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    12882 2023-05-28 08:33:38.345157 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.033213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5303 2023-05-28 08:33:54.029213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8604 2023-05-28 08:33:38.153156 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.029213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-05-28 08:33:54.021213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-05-28 08:33:37.553154 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.021213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    28920 2023-05-28 08:33:54.025213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20665 2023-05-28 08:33:37.957155 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    35307 2023-05-28 08:33:54.025213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-05-28 08:33:54.033213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-05-28 08:33:38.553158 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.033213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-05-28 08:33:54.033213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-05-28 08:33:38.749158 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-05-28 08:33:54.037213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    25222 2023-05-28 08:33:54.025213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    37429 2023-05-28 08:33:37.753155 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.025213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-05-28 08:33:54.037213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-05-28 08:33:38.937159 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.037213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0    11277 2023-05-28 08:33:54.037213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
+-rw-r--r--   0        0        0    15070 2023-05-28 08:33:39.129160 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.041213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-05-28 08:33:54.053213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-05-28 08:33:53.477211 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.053213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-05-28 08:33:54.057213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-05-28 08:33:53.673212 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-05-28 08:33:54.057213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-05-28 08:33:54.057213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-05-28 08:33:40.861166 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.061213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-28 08:33:54.061213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-05-28 08:33:41.049167 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-05-28 08:33:54.061213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-05-28 08:33:54.061213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-05-28 08:33:41.237167 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.065213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-05-28 08:33:54.065213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-05-28 08:33:42.009170 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.069213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-05-28 08:33:54.065213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-05-28 08:33:41.813169 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-05-28 08:33:54.065213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-05-28 08:33:54.069213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-05-28 08:33:42.193171 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.069213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    14046 2023-05-28 08:33:54.041213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23615 2023-05-28 08:33:39.329160 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.041213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-05-28 08:33:54.041213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-05-28 08:33:39.517161 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.045213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-05-28 08:33:54.045213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-05-28 08:33:39.709162 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-05-28 08:33:54.045213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-05-28 08:33:54.049213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-05-28 08:33:39.901162 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.049213 qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-05-28 08:33:54.185214 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-05-28 08:33:52.265207 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.189214 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-05-28 08:33:54.189214 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-05-28 08:33:52.461208 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-28 08:33:54.189214 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-05-28 08:33:54.189214 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-05-28 08:33:52.657208 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.193214 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-05-28 08:33:54.193214 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-05-28 08:33:52.897209 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-28 08:33:54.193214 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-05-28 08:33:54.193214 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-05-28 08:33:53.097210 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-05-28 08:33:54.197214 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-05-28 08:33:54.197214 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-05-28 08:33:53.289211 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.197214 qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-05-28 08:33:54.121214 qwak_core-0.0.80/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-05-28 08:33:46.421186 qwak_core-0.0.80/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.125213 qwak_core-0.0.80/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-05-28 08:33:54.125213 qwak_core-0.0.80/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-28 08:33:46.625187 qwak_core-0.0.80/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-28 08:33:54.125213 qwak_core-0.0.80/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-05-28 08:33:54.005213 qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-05-28 08:33:36.753151 qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.009213 qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-28 08:33:54.009213 qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-05-28 08:33:36.945152 qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.013213 qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-05-28 08:33:54.013213 qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-05-28 08:33:37.145152 qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-05-28 08:33:54.017213 qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-05-28 08:33:54.017213 qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-05-28 08:33:37.345153 qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.021213 qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-05-28 08:33:54.097213 qwak_core-0.0.80/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-05-28 08:33:44.181178 qwak_core-0.0.80/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-05-28 08:33:54.097213 qwak_core-0.0.80/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     3757 2023-05-28 08:33:54.125213 qwak_core-0.0.80/_qwak_proto/qwak/instance_template/instance_template_pb2.py
+-rw-r--r--   0        0        0     4235 2023-05-28 08:33:46.841188 qwak_core-0.0.80/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.129214 qwak_core-0.0.80/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
+-rw-r--r--   0        0        0     4722 2023-05-28 08:33:54.129214 qwak_core-0.0.80/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
+-rw-r--r--   0        0        0     3245 2023-05-28 08:33:47.049188 qwak_core-0.0.80/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
+-rw-r--r--   0        0        0     5240 2023-05-28 08:33:54.129214 qwak_core-0.0.80/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-05-28 08:33:54.141214 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-05-28 08:33:48.237192 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.145214 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-05-28 08:33:54.145214 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-05-28 08:33:48.429193 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.145214 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-05-28 08:33:54.145214 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-05-28 08:33:48.629194 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.149214 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-05-28 08:33:54.149214 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-05-28 08:33:48.833195 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.149214 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-28 08:33:54.149214 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-05-28 08:33:49.041195 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.153214 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-05-28 08:33:54.153214 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-05-28 08:33:49.249196 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-05-28 08:33:54.153214 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-05-28 08:33:54.157214 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-05-28 08:33:49.437197 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.157214 qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-05-28 08:33:54.133214 qwak_core-0.0.80/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-05-28 08:33:47.449190 qwak_core-0.0.80/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.133214 qwak_core-0.0.80/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-05-28 08:33:54.141214 qwak_core-0.0.80/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-05-28 08:33:48.049192 qwak_core-0.0.80/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.141214 qwak_core-0.0.80/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-05-28 08:33:54.137214 qwak_core-0.0.80/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-05-28 08:33:47.653190 qwak_core-0.0.80/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-05-28 08:33:54.137214 qwak_core-0.0.80/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10138 2023-05-28 08:33:54.137214 qwak_core-0.0.80/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    14337 2023-05-28 08:33:47.857191 qwak_core-0.0.80/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.137214 qwak_core-0.0.80/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-05-28 08:33:54.117214 qwak_core-0.0.80/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-05-28 08:33:45.829184 qwak_core-0.0.80/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-05-28 08:33:54.117214 qwak_core-0.0.80/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-05-28 08:33:53.985213 qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-05-28 08:33:36.345150 qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-05-28 08:33:53.989213 qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-05-28 08:33:53.985213 qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-05-28 08:33:36.145149 qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:53.985213 qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-05-28 08:33:53.989213 qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-05-28 08:33:36.549150 qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-05-28 08:33:53.989213 qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-05-28 08:33:54.113214 qwak_core-0.0.80/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-05-28 08:33:45.389182 qwak_core-0.0.80/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-05-28 08:33:54.113214 qwak_core-0.0.80/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-05-28 08:33:54.133214 qwak_core-0.0.80/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-05-28 08:33:47.241189 qwak_core-0.0.80/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-05-28 08:33:54.133214 qwak_core-0.0.80/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-05-28 08:33:53.981213 qwak_core-0.0.80/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-05-28 08:33:33.965141 qwak_core-0.0.80/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:53.981213 qwak_core-0.0.80/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-05-28 08:33:53.981213 qwak_core-0.0.80/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-05-28 08:33:33.773140 qwak_core-0.0.80/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-05-28 08:33:53.981213 qwak_core-0.0.80/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-05-28 08:33:53.973213 qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-05-28 08:33:33.185138 qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:53.973213 qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-05-28 08:33:53.973213 qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-05-28 08:33:33.373139 qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:53.977213 qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-05-28 08:33:53.977213 qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-05-28 08:33:33.569140 qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-05-28 08:33:53.977213 qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-05-28 08:33:54.161214 qwak_core-0.0.80/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-05-28 08:33:49.845198 qwak_core-0.0.80/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-05-28 08:33:54.161214 qwak_core-0.0.80/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-05-28 08:33:54.157214 qwak_core-0.0.80/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-05-28 08:33:49.645198 qwak_core-0.0.80/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.157214 qwak_core-0.0.80/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0    10851 2023-05-28 08:33:53.997213 qwak_core-0.0.80/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0    13974 2023-05-28 08:33:35.349146 qwak_core-0.0.80/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:53.997213 qwak_core-0.0.80/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     2993 2023-05-28 08:33:54.001213 qwak_core-0.0.80/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2568 2023-05-28 08:33:35.545147 qwak_core-0.0.80/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 08:33:54.001213 qwak_core-0.0.80/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2661 2023-05-28 08:33:55.445218 qwak_core-0.0.80/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-28 08:33:55.445218 qwak_core-0.0.80/qwak/__init__.py
+-rw-r--r--   0        0        0     1501 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    12899 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/automations/automations.py
+-rw-r--r--   0        0        0     9638 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/automations/batch_execution_action.py
+-rw-r--r--   0        0        0    19120 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/automations/build_and_deploy_action.py
+-rw-r--r--   0        0        0     1697 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/automations/common.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-05-28 08:32:06.172842 qwak_core-0.0.80/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0      211 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    18388 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    14847 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/instance_template/__init__.py
+-rw-r--r--   0        0        0     2495 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/instance_template/client.py
+-rw-r--r--   0        0        0       41 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3316 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     4707 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     1263 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     1941 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2987 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1717 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0       89 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0      738 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28013 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     9261 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/const.py
+-rw-r--r--   0        0        0     1435 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6083 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-05-28 08:32:06.176842 qwak_core-0.0.80/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      873 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/schema.py
+-rw-r--r--   0        0        0     2970 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      338 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     1963 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0      848 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2511 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      650 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0      975 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/tools/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/tools/logger/__init__.py
+-rw-r--r--   0        0        0     9598 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak/tools/logger/logging.yml
+-rw-r--r--   0        0        0       46 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12316 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5806 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     3905 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/instance_template_management_service.py
+-rw-r--r--   0        0        0     2696 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     4186 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13583 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-28 08:32:06.180842 qwak_core-0.0.80/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.80/setup.py
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.80/PKG-INFO
```

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from _qwak_proto.qwak.feature_store.features import execution_pb2 as qwak_dot_feature__store_dot_features_dot_execution__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n=qwak/feature_store/features/real_time_feature_extractor.proto\x12\x1bqwak.feature.store.features\x1a\x1fgoogle/protobuf/timestamp.proto\x1a+qwak/feature_store/features/execution.proto\"\xdc\x01\n\x18RealTimeFeatureExtractor\x12o\n&real_time_feature_extractor_definition\x18\x01 \x01(\x0b\x32?.qwak.feature.store.features.RealTimeFeatureExtractorDefinition\x12O\n\x08metadata\x18\x02 \x01(\x0b\x32=.qwak.feature.store.features.RealTimeFeatureExtractorMetadata\"\xa5\x02\n\"RealTimeFeatureExtractorDefinition\x12&\n\x1ereal_time_feature_extractor_id\x18\x01 \x01(\t\x12\x63\n real_time_feature_extractor_spec\x18\x02 \x01(\x0b\x32\x39.qwak.feature.store.features.RealTimeFeatureExtractorSpec\x12\x18\n\x10\x64\x65ployment_state\x18\x05 \x01(\t\x12X\n\x13registration_status\x18\x06 \x01(\x0e\x32;.qwak.feature.store.features.RealTimeFeatureExtractorStatus\"\xc8\x01\n RealTimeFeatureExtractorMetadata\x12\x35\n\x11\x63reated_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ncreated_by\x18\x02 \x01(\t\x12?\n\x1blast_modification_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10last_modified_by\x18\x04 \x01(\t\"\x9b\x02\n\x1cRealTimeFeatureExtractorSpec\x12K\n\x12real_time_artifact\x18\x01 \x01(\x0b\x32/.qwak.feature.store.features.ExtractionArtifact\x12P\n\x12\x64\x65pendency_manager\x18\x02 \x01(\x0b\x32\x34.qwak.feature.store.features.PythonDependencyManager\x12\\\n\x1c\x63lient_pod_compute_resources\x18\x03 \x01(\x0b\x32\x36.qwak.feature.store.features.ExtractorComputeResources\"U\n\x12\x45xtractionArtifact\x12\x34\n\x06\x61ws_s3\x18\x01 \x01(\x0b\x32\".qwak.feature.store.features.AwsS3H\x00\x42\t\n\x07\x66s_type\"\x1e\n\x05\x41wsS3\x12\x15\n\rartifact_path\x18\x01 \x01(\t\"\x98\x02\n\x17PythonDependencyManager\x12\x42\n\x0epython_version\x18\x01 \x01(\x0e\x32*.qwak.feature.store.features.PythonVersion\x12\x45\n\nvirtualenv\x18\x02 \x01(\x0b\x32/.qwak.feature.store.features.VirtualEnvironmentH\x00\x12\x33\n\x05\x63onda\x18\x03 \x01(\x0b\x32\".qwak.feature.store.features.CondaH\x00\x12\x35\n\x06poetry\x18\x04 \x01(\x0b\x32#.qwak.feature.store.features.PoetryH\x00\x42\x06\n\x04type\"*\n\x05\x43onda\x12!\n\x19\x62\x61se64_encoded_conda_file\x18\x01 \x01(\t\"*\n\x06Poetry\x12 \n\x18\x62\x61se64_encoded_lock_file\x18\x01 \x01(\t\"=\n\x12VirtualEnvironment\x12\'\n\x1f\x62\x61se64_encoded_requirements_txt\x18\x01 \x01(\t\"\x9a\x01\n\x19\x45xtractorComputeResources\x12[\n\x19\x63ompute_resource_template\x18\x01 \x01(\x0e\x32\x36.qwak.feature.store.features.execution.ClusterTemplateH\x00\x12\x13\n\x0bparallelism\x18\x02 \x01(\x05\x42\x0b\n\tresources*s\n\rPythonVersion\x12\x1a\n\x16PYTHON_VERSION_INVALID\x10\x00\x12\x16\n\x12PYTHON_VERSION_3_7\x10\x01\x12\x16\n\x12PYTHON_VERSION_3_8\x10\x02\x12\x16\n\x12PYTHON_VERSION_3_9\x10\x03*\xf1\x01\n\x1eRealTimeFeatureExtractorStatus\x12\x15\n\x11\x45XTRACTOR_INVALID\x10\x00\x12\x13\n\x0f\x45XTRACTOR_VALID\x10\x01\x12\x15\n\x11\x45XTRACTOR_DELETED\x10\x02\x12!\n\x1d\x45XTRACTOR_REGISTRATION_FAILED\x10\x03\x12&\n\"EXTRACTOR_REGISTRATION_IN_PROGRESS\x10\x04\x12\"\n\x1e\x45XTRACTOR_DELETION_IN_PROGRESS\x10\x05\x12\x1d\n\x19\x45XTRACTOR_DELETION_FAILED\x10\x06\x42[\n&com.qwak.ai.feature.store.features.apiP\x01Z/qwak/featurestore/features;featurestorefeaturesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n=qwak/feature_store/features/real_time_feature_extractor.proto\x12\x1bqwak.feature.store.features\x1a\x1fgoogle/protobuf/timestamp.proto\x1a+qwak/feature_store/features/execution.proto\"\xdc\x01\n\x18RealTimeFeatureExtractor\x12o\n&real_time_feature_extractor_definition\x18\x01 \x01(\x0b\x32?.qwak.feature.store.features.RealTimeFeatureExtractorDefinition\x12O\n\x08metadata\x18\x02 \x01(\x0b\x32=.qwak.feature.store.features.RealTimeFeatureExtractorMetadata\"\xa5\x02\n\"RealTimeFeatureExtractorDefinition\x12&\n\x1ereal_time_feature_extractor_id\x18\x01 \x01(\t\x12\x63\n real_time_feature_extractor_spec\x18\x02 \x01(\x0b\x32\x39.qwak.feature.store.features.RealTimeFeatureExtractorSpec\x12\x18\n\x10\x64\x65ployment_state\x18\x05 \x01(\t\x12X\n\x13registration_status\x18\x06 \x01(\x0e\x32;.qwak.feature.store.features.RealTimeFeatureExtractorStatus\"\xc8\x01\n RealTimeFeatureExtractorMetadata\x12\x35\n\x11\x63reated_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ncreated_by\x18\x02 \x01(\t\x12?\n\x1blast_modification_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10last_modified_by\x18\x04 \x01(\t\"\xba\x02\n\x1cRealTimeFeatureExtractorSpec\x12K\n\x12real_time_artifact\x18\x01 \x01(\x0b\x32/.qwak.feature.store.features.ExtractionArtifact\x12P\n\x12\x64\x65pendency_manager\x18\x02 \x01(\x0b\x32\x34.qwak.feature.store.features.PythonDependencyManager\x12\\\n\x1c\x63lient_pod_compute_resources\x18\x03 \x01(\x0b\x32\x36.qwak.feature.store.features.ExtractorComputeResources\x12\x1d\n\x15max_staleness_seconds\x18\x04 \x01(\x03\"U\n\x12\x45xtractionArtifact\x12\x34\n\x06\x61ws_s3\x18\x01 \x01(\x0b\x32\".qwak.feature.store.features.AwsS3H\x00\x42\t\n\x07\x66s_type\"\x1e\n\x05\x41wsS3\x12\x15\n\rartifact_path\x18\x01 \x01(\t\"\x98\x02\n\x17PythonDependencyManager\x12\x42\n\x0epython_version\x18\x01 \x01(\x0e\x32*.qwak.feature.store.features.PythonVersion\x12\x45\n\nvirtualenv\x18\x02 \x01(\x0b\x32/.qwak.feature.store.features.VirtualEnvironmentH\x00\x12\x33\n\x05\x63onda\x18\x03 \x01(\x0b\x32\".qwak.feature.store.features.CondaH\x00\x12\x35\n\x06poetry\x18\x04 \x01(\x0b\x32#.qwak.feature.store.features.PoetryH\x00\x42\x06\n\x04type\"*\n\x05\x43onda\x12!\n\x19\x62\x61se64_encoded_conda_file\x18\x01 \x01(\t\"*\n\x06Poetry\x12 \n\x18\x62\x61se64_encoded_lock_file\x18\x01 \x01(\t\"=\n\x12VirtualEnvironment\x12\'\n\x1f\x62\x61se64_encoded_requirements_txt\x18\x01 \x01(\t\"\x9a\x01\n\x19\x45xtractorComputeResources\x12[\n\x19\x63ompute_resource_template\x18\x01 \x01(\x0e\x32\x36.qwak.feature.store.features.execution.ClusterTemplateH\x00\x12\x13\n\x0bparallelism\x18\x02 \x01(\x05\x42\x0b\n\tresources*s\n\rPythonVersion\x12\x1a\n\x16PYTHON_VERSION_INVALID\x10\x00\x12\x16\n\x12PYTHON_VERSION_3_7\x10\x01\x12\x16\n\x12PYTHON_VERSION_3_8\x10\x02\x12\x16\n\x12PYTHON_VERSION_3_9\x10\x03*\xf1\x01\n\x1eRealTimeFeatureExtractorStatus\x12\x15\n\x11\x45XTRACTOR_INVALID\x10\x00\x12\x13\n\x0f\x45XTRACTOR_VALID\x10\x01\x12\x15\n\x11\x45XTRACTOR_DELETED\x10\x02\x12!\n\x1d\x45XTRACTOR_REGISTRATION_FAILED\x10\x03\x12&\n\"EXTRACTOR_REGISTRATION_IN_PROGRESS\x10\x04\x12\"\n\x1e\x45XTRACTOR_DELETION_IN_PROGRESS\x10\x05\x12\x1d\n\x19\x45XTRACTOR_DELETION_FAILED\x10\x06\x42[\n&com.qwak.ai.feature.store.features.apiP\x01Z/qwak/featurestore/features;featurestorefeaturesb\x06proto3')
 
 _PYTHONVERSION = DESCRIPTOR.enum_types_by_name['PythonVersion']
 PythonVersion = enum_type_wrapper.EnumTypeWrapper(_PYTHONVERSION)
 _REALTIMEFEATUREEXTRACTORSTATUS = DESCRIPTOR.enum_types_by_name['RealTimeFeatureExtractorStatus']
 RealTimeFeatureExtractorStatus = enum_type_wrapper.EnumTypeWrapper(_REALTIMEFEATUREEXTRACTORSTATUS)
 PYTHON_VERSION_INVALID = 0
 PYTHON_VERSION_3_7 = 1
@@ -124,34 +124,34 @@
   })
 _sym_db.RegisterMessage(ExtractorComputeResources)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n&com.qwak.ai.feature.store.features.apiP\001Z/qwak/featurestore/features;featurestorefeatures'
-  _PYTHONVERSION._serialized_start=1890
-  _PYTHONVERSION._serialized_end=2005
-  _REALTIMEFEATUREEXTRACTORSTATUS._serialized_start=2008
-  _REALTIMEFEATUREEXTRACTORSTATUS._serialized_end=2249
+  _PYTHONVERSION._serialized_start=1921
+  _PYTHONVERSION._serialized_end=2036
+  _REALTIMEFEATUREEXTRACTORSTATUS._serialized_start=2039
+  _REALTIMEFEATUREEXTRACTORSTATUS._serialized_end=2280
   _REALTIMEFEATUREEXTRACTOR._serialized_start=173
   _REALTIMEFEATUREEXTRACTOR._serialized_end=393
   _REALTIMEFEATUREEXTRACTORDEFINITION._serialized_start=396
   _REALTIMEFEATUREEXTRACTORDEFINITION._serialized_end=689
   _REALTIMEFEATUREEXTRACTORMETADATA._serialized_start=692
   _REALTIMEFEATUREEXTRACTORMETADATA._serialized_end=892
   _REALTIMEFEATUREEXTRACTORSPEC._serialized_start=895
-  _REALTIMEFEATUREEXTRACTORSPEC._serialized_end=1178
-  _EXTRACTIONARTIFACT._serialized_start=1180
-  _EXTRACTIONARTIFACT._serialized_end=1265
-  _AWSS3._serialized_start=1267
-  _AWSS3._serialized_end=1297
-  _PYTHONDEPENDENCYMANAGER._serialized_start=1300
-  _PYTHONDEPENDENCYMANAGER._serialized_end=1580
-  _CONDA._serialized_start=1582
-  _CONDA._serialized_end=1624
-  _POETRY._serialized_start=1626
-  _POETRY._serialized_end=1668
-  _VIRTUALENVIRONMENT._serialized_start=1670
-  _VIRTUALENVIRONMENT._serialized_end=1731
-  _EXTRACTORCOMPUTERESOURCES._serialized_start=1734
-  _EXTRACTORCOMPUTERESOURCES._serialized_end=1888
+  _REALTIMEFEATUREEXTRACTORSPEC._serialized_end=1209
+  _EXTRACTIONARTIFACT._serialized_start=1211
+  _EXTRACTIONARTIFACT._serialized_end=1296
+  _AWSS3._serialized_start=1298
+  _AWSS3._serialized_end=1328
+  _PYTHONDEPENDENCYMANAGER._serialized_start=1331
+  _PYTHONDEPENDENCYMANAGER._serialized_end=1611
+  _CONDA._serialized_start=1613
+  _CONDA._serialized_end=1655
+  _POETRY._serialized_start=1657
+  _POETRY._serialized_end=1699
+  _VIRTUALENVIRONMENT._serialized_start=1701
+  _VIRTUALENVIRONMENT._serialized_end=1762
+  _EXTRACTORCOMPUTERESOURCES._serialized_start=1765
+  _EXTRACTORCOMPUTERESOURCES._serialized_end=1919
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -145,32 +145,36 @@
 
 class RealTimeFeatureExtractorSpec(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     REAL_TIME_ARTIFACT_FIELD_NUMBER: builtins.int
     DEPENDENCY_MANAGER_FIELD_NUMBER: builtins.int
     CLIENT_POD_COMPUTE_RESOURCES_FIELD_NUMBER: builtins.int
+    MAX_STALENESS_SECONDS_FIELD_NUMBER: builtins.int
     @property
     def real_time_artifact(self) -> global___ExtractionArtifact:
         """Extraction artifact field containing all relevant information related to the code's artifact"""
     @property
     def dependency_manager(self) -> global___PythonDependencyManager:
         """Python dependency manager"""
     @property
     def client_pod_compute_resources(self) -> global___ExtractorComputeResources:
         """Resources dedicated to the real time extractor"""
+    max_staleness_seconds: builtins.int
+    """Max staleness time interval passed in seconds"""
     def __init__(
         self,
         *,
         real_time_artifact: global___ExtractionArtifact | None = ...,
         dependency_manager: global___PythonDependencyManager | None = ...,
         client_pod_compute_resources: global___ExtractorComputeResources | None = ...,
+        max_staleness_seconds: builtins.int = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["client_pod_compute_resources", b"client_pod_compute_resources", "dependency_manager", b"dependency_manager", "real_time_artifact", b"real_time_artifact"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["client_pod_compute_resources", b"client_pod_compute_resources", "dependency_manager", b"dependency_manager", "real_time_artifact", b"real_time_artifact"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["client_pod_compute_resources", b"client_pod_compute_resources", "dependency_manager", b"dependency_manager", "max_staleness_seconds", b"max_staleness_seconds", "real_time_artifact", b"real_time_artifact"]) -> None: ...
 
 global___RealTimeFeatureExtractorSpec = RealTimeFeatureExtractorSpec
 
 class ExtractionArtifact(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     AWS_S3_FIELD_NUMBER: builtins.int
```

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/instance_template/instance_template_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/instance_template/instance_template_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.80/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.80/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.80/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/pyproject.toml` & `qwak_core-0.0.80/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.79"
+version = "0.0.80"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.0.79/qwak/automations/__init__.py` & `qwak_core-0.0.80/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/automations/automation_executions.py` & `qwak_core-0.0.80/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/automations/automations.py` & `qwak_core-0.0.80/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/automations/batch_execution_action.py` & `qwak_core-0.0.80/qwak/automations/batch_execution_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/automations/build_and_deploy_action.py` & `qwak_core-0.0.80/qwak/automations/build_and_deploy_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/automations/common.py` & `qwak_core-0.0.80/qwak/automations/common.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.80/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.80/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.80/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.80/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.80/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/clients/alert_management/client.py` & `qwak_core-0.0.80/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/clients/analytics/client.py` & `qwak_core-0.0.80/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/clients/audience/client.py` & `qwak_core-0.0.80/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/clients/automation_management/client.py` & `qwak_core-0.0.80/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.80/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.80/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.80/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.80/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/clients/build_management/client.py` & `qwak_core-0.0.80/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.80/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.80/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/clients/deployment/client.py` & `qwak_core-0.0.80/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.80/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.80/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.80/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.80/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/clients/instance_template/client.py` & `qwak_core-0.0.80/qwak/clients/instance_template/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.80/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/clients/logging_client/client.py` & `qwak_core-0.0.80/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/clients/model_management/client.py` & `qwak_core-0.0.80/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/clients/project/client.py` & `qwak_core-0.0.80/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/clients/secret_service/client.py` & `qwak_core-0.0.80/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.80/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.80/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.80/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.0.80/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/feature_store/_common/functions.py` & `qwak_core-0.0.80/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.80/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.80/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.80/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.80/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.80/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.80/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.80/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.80/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.80/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.0.80/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.0.80/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/feature_store/offline/client.py` & `qwak_core-0.0.80/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/feature_store/online/client.py` & `qwak_core-0.0.80/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/inner/const.py` & `qwak_core-0.0.80/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.80/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.80/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.80/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.80/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/inner/singleton_meta.py` & `qwak_core-0.0.80/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/inner/tool/auth.py` & `qwak_core-0.0.80/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.80/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.80/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.80/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.80/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/model/adapters/__init__.py` & `qwak_core-0.0.80/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.80/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.80/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.80/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.80/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.80/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/model/base.py` & `qwak_core-0.0.80/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/model/decorators/api.py` & `qwak_core-0.0.80/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.80/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/model/experiment_tracking.py` & `qwak_core-0.0.80/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/model/schema.py` & `qwak_core-0.0.80/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/model/schema_entities.py` & `qwak_core-0.0.80/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.0.80/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/model/tools/adapters/input.py` & `qwak_core-0.0.80/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.0.80/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.0.80/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.0.80/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.0.80/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.0.80/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/model/tools/adapters/output.py` & `qwak_core-0.0.80/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.0.80/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.0.80/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.0.80/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.0.80/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/model/tools/run_model_locally.py` & `qwak_core-0.0.80/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.80/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.80/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.80/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.80/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.80/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.80/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/qwak_client/client.py` & `qwak_core-0.0.80/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.80/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/qwak_client/models/model.py` & `qwak_core-0.0.80/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.80/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.80/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/tools/logger/logger.py` & `qwak_core-0.0.80/qwak/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak/tools/logger/logging.yml` & `qwak_core-0.0.80/qwak/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/instance_template_management_service.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/instance_template_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.80/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/qwak_services_mock/services_mock.py` & `qwak_core-0.0.80/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.79/setup.py` & `qwak_core-0.0.80/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
  'typeguard>=2,<3']
 
 extras_require = \
 {'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.79',
+    'version': '0.0.80',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.79/PKG-INFO` & `qwak_core-0.0.80/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.79
+Version: 0.0.80
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

