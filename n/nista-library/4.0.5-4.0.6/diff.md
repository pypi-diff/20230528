# Comparing `tmp/nista_library-4.0.5.tar.gz` & `tmp/nista_library-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nista_library-4.0.5.tar", max compression
+gzip compressed data, was "nista_library-4.0.6.tar", max compression
```

## Comparing `nista_library-4.0.5.tar` & `nista_library-4.0.6.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0     1117 2023-05-25 12:03:49.719800 nista_library-4.0.5/LICENSE.md
--rw-r--r--   0        0        0     6428 2023-05-25 12:03:49.719800 nista_library-4.0.5/README.md
--rw-r--r--   0        0        0      153 2023-05-25 12:03:49.720800 nista_library-4.0.5/data_point_client/__init__.py
--rw-r--r--   0        0        0       47 2023-05-25 12:03:49.720800 nista_library-4.0.5/data_point_client/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 12:03:49.720800 nista_library-4.0.5/data_point_client/api/data_export/__init__.py
--rw-r--r--   0        0        0     5330 2023-05-25 12:03:49.720800 nista_library-4.0.5/data_point_client/api/data_export/data_export_create_csv_export.py
--rw-r--r--   0        0        0        0 2023-05-25 12:03:49.720800 nista_library-4.0.5/data_point_client/api/data_point/__init__.py
--rw-r--r--   0        0        0     5482 2023-05-25 12:03:49.720800 nista_library-4.0.5/data_point_client/api/data_point/data_point_append_execution_result_data.py
--rw-r--r--   0        0        0     5376 2023-05-25 12:03:49.720800 nista_library-4.0.5/data_point_client/api/data_point/data_point_append_time_series_data.py
--rw-r--r--   0        0        0     5768 2023-05-25 12:03:49.720800 nista_library-4.0.5/data_point_client/api/data_point/data_point_create_area.py
--rw-r--r--   0        0        0     6225 2023-05-25 12:03:49.720800 nista_library-4.0.5/data_point_client/api/data_point/data_point_create_area_message.py
--rw-r--r--   0        0        0     5323 2023-05-25 12:03:49.720800 nista_library-4.0.5/data_point_client/api/data_point/data_point_create_chiller_samples.py
--rw-r--r--   0        0        0     5441 2023-05-25 12:03:49.720800 nista_library-4.0.5/data_point_client/api/data_point/data_point_create_data_point.py
--rw-r--r--   0        0        0     4789 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_delete_area.py
--rw-r--r--   0        0        0     4473 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_delete_data_point.py
--rw-r--r--   0        0        0     4478 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py
--rw-r--r--   0        0        0     5168 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_delete_message.py
--rw-r--r--   0        0        0     5472 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_get_data.py
--rw-r--r--   0        0        0     5005 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_get_data_point.py
--rw-r--r--   0        0        0     5326 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_get_data_point_by_version.py
--rw-r--r--   0        0        0     8928 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_get_data_points.py
--rw-r--r--   0        0        0     7699 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_get_tags.py
--rw-r--r--   0        0        0     4805 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_get_tags_2.py
--rw-r--r--   0        0        0     5296 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_list_areas.py
--rw-r--r--   0        0        0     5769 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_update_area.py
--rw-r--r--   0        0        0     5397 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_update_constant_data.py
--rw-r--r--   0        0        0     5442 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_update_data_point.py
--rw-r--r--   0        0        0     5518 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py
--rw-r--r--   0        0        0     5262 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_update_data_point_unit.py
--rw-r--r--   0        0        0     5369 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_update_day_period_data.py
--rw-r--r--   0        0        0     6226 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_update_message.py
--rw-r--r--   0        0        0     5381 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_update_time_series_data.py
--rw-r--r--   0        0        0     5381 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_update_week_period_data.py
--rw-r--r--   0        0        0     2817 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/client.py
--rw-r--r--   0        0        0      470 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/errors.py
--rw-r--r--   0        0        0     4795 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/models/__init__.py
--rw-r--r--   0        0        0     1965 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/models/append_execution_result_data_request.py
--rw-r--r--   0        0        0     1906 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/models/append_time_series_request.py
--rw-r--r--   0        0        0     4359 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/models/area_of_interest_response.py
--rw-r--r--   0        0        0     1858 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/models/calculation_origin.py
--rw-r--r--   0        0        0     7547 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/models/constant_data_bucket.py
--rw-r--r--   0        0        0     2965 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/models/constant_data_point_data.py
--rw-r--r--   0        0        0     2597 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/models/continuous_location_rest.py
--rw-r--r--   0        0        0      923 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/create_area_message_request.py
--rw-r--r--   0        0        0     2319 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/create_area_request.py
--rw-r--r--   0        0        0     5874 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/data_bucket_base.py
--rw-r--r--   0        0        0     2054 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/data_export_request.py
--rw-r--r--   0        0        0     2702 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/data_point_comment_message_response.py
--rw-r--r--   0        0        0     2016 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/data_point_data_base.py
--rw-r--r--   0        0        0     2418 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/data_point_data_response.py
--rw-r--r--   0        0        0      779 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/data_point_origin.py
--rw-r--r--   0        0        0     3212 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/data_point_request.py
--rw-r--r--   0        0        0     7362 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/data_point_response_base.py
--rw-r--r--   0        0        0     7281 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/day_data_by_hour_transfer.py
--rw-r--r--   0        0        0     7564 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/day_period_data_bucket.py
--rw-r--r--   0        0        0     4321 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/day_period_data_point_data.py
--rw-r--r--   0        0        0      191 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/en_area_type_rest.py
--rw-r--r--   0        0        0      192 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/en_data_bucket_state.py
--rw-r--r--   0        0        0      208 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/en_data_point_existence_dto.py
--rw-r--r--   0        0        0      214 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/en_data_point_state_dto.py
--rw-r--r--   0        0        0      192 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/en_data_point_status.py
--rw-r--r--   0        0        0      250 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/en_data_point_type.py
--rw-r--r--   0        0        0      181 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/en_operator.py
--rw-r--r--   0        0        0     2375 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/file_origin.py
--rw-r--r--   0        0        0     2579 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/get_constant_response.py
--rw-r--r--   0        0        0     3472 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/get_data_request.py
--rw-r--r--   0        0        0      779 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/get_data_response.py
--rw-r--r--   0        0        0     3900 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/get_day_period_response.py
--rw-r--r--   0        0        0     2529 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/get_series_response.py
--rw-r--r--   0        0        0     3227 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/get_week_period_response.py
--rw-r--r--   0        0        0     1176 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/gnista_unit_response.py
--rw-r--r--   0        0        0     1810 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/live_data_origin.py
--rw-r--r--   0        0        0      765 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/location_rest.py
--rw-r--r--   0        0        0     2045 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/point_location_rest.py
--rw-r--r--   0        0        0     3377 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/problem_details.py
--rw-r--r--   0        0        0     1215 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/problem_details_extensions.py
--rw-r--r--   0        0        0     1449 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/remote_origin.py
--rw-r--r--   0        0        0     1247 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/rule.py
--rw-r--r--   0        0        0     9273 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/series_data_bucket.py
--rw-r--r--   0        0        0     3058 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/series_data_point_data.py
--rw-r--r--   0        0        0     1446 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/sub_series_request.py
--rw-r--r--   0        0        0     1214 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/sub_series_request_values.py
--rw-r--r--   0        0        0     1631 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/time_series_period.py
--rw-r--r--   0        0        0     2675 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/time_series_response.py
--rw-r--r--   0        0        0     1219 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/time_series_response_curve.py
--rw-r--r--   0        0        0      923 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/update_area_message_request.py
--rw-r--r--   0        0        0     2674 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/update_area_request.py
--rw-r--r--   0        0        0     1401 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/update_constant_data_request.py
--rw-r--r--   0        0        0     2725 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/update_day_period_request.py
--rw-r--r--   0        0        0     3346 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/update_time_series_request.py
--rw-r--r--   0        0        0     2052 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/update_week_period_request.py
--rw-r--r--   0        0        0     7478 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/week_data_transfere.py
--rw-r--r--   0        0        0     7576 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/week_period_data_bucket.py
--rw-r--r--   0        0        0     3648 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/week_period_data_point_data.py
--rw-r--r--   0        0        0       25 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/py.typed
--rw-r--r--   0        0        0      993 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/types.py
--rw-r--r--   0        0        0     1007 2023-05-25 12:03:49.724800 nista_library-4.0.5/nista_library/__init__.py
--rw-r--r--   0        0        0    11406 2023-05-25 12:03:49.724800 nista_library-4.0.5/nista_library/nista_connetion.py
--rw-r--r--   0        0        0     1049 2023-05-25 12:03:49.724800 nista_library-4.0.5/nista_library/nista_credential_manager.py
--rw-r--r--   0        0        0    18118 2023-05-25 12:03:49.724800 nista_library-4.0.5/nista_library/nista_data_point.py
--rw-r--r--   0        0        0     1970 2023-05-25 12:03:49.724800 nista_library-4.0.5/nista_library/nista_data_points.py
--rw-r--r--   0        0        0     1383 2023-05-25 12:03:49.725800 nista_library-4.0.5/pyproject.toml
--rw-r--r--   0        0        0     7471 1970-01-01 00:00:00.000000 nista_library-4.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1117 2023-05-28 14:31:25.791221 nista_library-4.0.6/LICENSE.md
+-rw-r--r--   0        0        0     6428 2023-05-28 14:31:25.791221 nista_library-4.0.6/README.md
+-rw-r--r--   0        0        0      153 2023-05-28 14:31:25.793221 nista_library-4.0.6/data_point_client/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-28 14:31:25.793221 nista_library-4.0.6/data_point_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 14:31:25.823221 nista_library-4.0.6/data_point_client/api/data_export/__init__.py
+-rw-r--r--   0        0        0     5330 2023-05-28 14:31:25.793221 nista_library-4.0.6/data_point_client/api/data_export/data_export_create_csv_export.py
+-rw-r--r--   0        0        0        0 2023-05-28 14:31:25.823221 nista_library-4.0.6/data_point_client/api/data_point/__init__.py
+-rw-r--r--   0        0        0     5482 2023-05-28 14:31:25.793221 nista_library-4.0.6/data_point_client/api/data_point/data_point_append_execution_result_data.py
+-rw-r--r--   0        0        0     5376 2023-05-28 14:31:25.793221 nista_library-4.0.6/data_point_client/api/data_point/data_point_append_time_series_data.py
+-rw-r--r--   0        0        0     5768 2023-05-28 14:31:25.794221 nista_library-4.0.6/data_point_client/api/data_point/data_point_create_area.py
+-rw-r--r--   0        0        0     6225 2023-05-28 14:31:25.794221 nista_library-4.0.6/data_point_client/api/data_point/data_point_create_area_message.py
+-rw-r--r--   0        0        0     5323 2023-05-28 14:31:25.794221 nista_library-4.0.6/data_point_client/api/data_point/data_point_create_chiller_samples.py
+-rw-r--r--   0        0        0     5441 2023-05-28 14:31:25.794221 nista_library-4.0.6/data_point_client/api/data_point/data_point_create_data_point.py
+-rw-r--r--   0        0        0     4789 2023-05-28 14:31:25.794221 nista_library-4.0.6/data_point_client/api/data_point/data_point_delete_area.py
+-rw-r--r--   0        0        0     4473 2023-05-28 14:31:25.794221 nista_library-4.0.6/data_point_client/api/data_point/data_point_delete_data_point.py
+-rw-r--r--   0        0        0     4478 2023-05-28 14:31:25.794221 nista_library-4.0.6/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py
+-rw-r--r--   0        0        0     5168 2023-05-28 14:31:25.794221 nista_library-4.0.6/data_point_client/api/data_point/data_point_delete_message.py
+-rw-r--r--   0        0        0     5472 2023-05-28 14:31:25.794221 nista_library-4.0.6/data_point_client/api/data_point/data_point_get_data.py
+-rw-r--r--   0        0        0     5005 2023-05-28 14:31:25.794221 nista_library-4.0.6/data_point_client/api/data_point/data_point_get_data_point.py
+-rw-r--r--   0        0        0     5326 2023-05-28 14:31:25.794221 nista_library-4.0.6/data_point_client/api/data_point/data_point_get_data_point_by_version.py
+-rw-r--r--   0        0        0     8928 2023-05-28 14:31:25.794221 nista_library-4.0.6/data_point_client/api/data_point/data_point_get_data_points.py
+-rw-r--r--   0        0        0     7699 2023-05-28 14:31:25.794221 nista_library-4.0.6/data_point_client/api/data_point/data_point_get_tags.py
+-rw-r--r--   0        0        0     4805 2023-05-28 14:31:25.794221 nista_library-4.0.6/data_point_client/api/data_point/data_point_get_tags_2.py
+-rw-r--r--   0        0        0     5296 2023-05-28 14:31:25.794221 nista_library-4.0.6/data_point_client/api/data_point/data_point_list_areas.py
+-rw-r--r--   0        0        0     5769 2023-05-28 14:31:25.794221 nista_library-4.0.6/data_point_client/api/data_point/data_point_update_area.py
+-rw-r--r--   0        0        0     5397 2023-05-28 14:31:25.794221 nista_library-4.0.6/data_point_client/api/data_point/data_point_update_constant_data.py
+-rw-r--r--   0        0        0     5442 2023-05-28 14:31:25.794221 nista_library-4.0.6/data_point_client/api/data_point/data_point_update_data_point.py
+-rw-r--r--   0        0        0     5518 2023-05-28 14:31:25.794221 nista_library-4.0.6/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py
+-rw-r--r--   0        0        0     5262 2023-05-28 14:31:25.794221 nista_library-4.0.6/data_point_client/api/data_point/data_point_update_data_point_unit.py
+-rw-r--r--   0        0        0     5369 2023-05-28 14:31:25.795220 nista_library-4.0.6/data_point_client/api/data_point/data_point_update_day_period_data.py
+-rw-r--r--   0        0        0     6226 2023-05-28 14:31:25.795220 nista_library-4.0.6/data_point_client/api/data_point/data_point_update_message.py
+-rw-r--r--   0        0        0     5381 2023-05-28 14:31:25.795220 nista_library-4.0.6/data_point_client/api/data_point/data_point_update_time_series_data.py
+-rw-r--r--   0        0        0     5381 2023-05-28 14:31:25.795220 nista_library-4.0.6/data_point_client/api/data_point/data_point_update_week_period_data.py
+-rw-r--r--   0        0        0     2817 2023-05-28 14:31:25.795220 nista_library-4.0.6/data_point_client/client.py
+-rw-r--r--   0        0        0      470 2023-05-28 14:31:25.795220 nista_library-4.0.6/data_point_client/errors.py
+-rw-r--r--   0        0        0     4795 2023-05-28 14:31:25.795220 nista_library-4.0.6/data_point_client/models/__init__.py
+-rw-r--r--   0        0        0     2253 2023-05-28 14:31:25.795220 nista_library-4.0.6/data_point_client/models/append_execution_result_data_request.py
+-rw-r--r--   0        0        0     1906 2023-05-28 14:31:25.795220 nista_library-4.0.6/data_point_client/models/append_time_series_request.py
+-rw-r--r--   0        0        0     4359 2023-05-28 14:31:25.795220 nista_library-4.0.6/data_point_client/models/area_of_interest_response.py
+-rw-r--r--   0        0        0     1858 2023-05-28 14:31:25.795220 nista_library-4.0.6/data_point_client/models/calculation_origin.py
+-rw-r--r--   0        0        0     7547 2023-05-28 14:31:25.795220 nista_library-4.0.6/data_point_client/models/constant_data_bucket.py
+-rw-r--r--   0        0        0     2965 2023-05-28 14:31:25.795220 nista_library-4.0.6/data_point_client/models/constant_data_point_data.py
+-rw-r--r--   0        0        0     2597 2023-05-28 14:31:25.795220 nista_library-4.0.6/data_point_client/models/continuous_location_rest.py
+-rw-r--r--   0        0        0      923 2023-05-28 14:31:25.795220 nista_library-4.0.6/data_point_client/models/create_area_message_request.py
+-rw-r--r--   0        0        0     2319 2023-05-28 14:31:25.795220 nista_library-4.0.6/data_point_client/models/create_area_request.py
+-rw-r--r--   0        0        0     5874 2023-05-28 14:31:25.795220 nista_library-4.0.6/data_point_client/models/data_bucket_base.py
+-rw-r--r--   0        0        0     2054 2023-05-28 14:31:25.795220 nista_library-4.0.6/data_point_client/models/data_export_request.py
+-rw-r--r--   0        0        0     2702 2023-05-28 14:31:25.795220 nista_library-4.0.6/data_point_client/models/data_point_comment_message_response.py
+-rw-r--r--   0        0        0     2016 2023-05-28 14:31:25.795220 nista_library-4.0.6/data_point_client/models/data_point_data_base.py
+-rw-r--r--   0        0        0     2418 2023-05-28 14:31:25.796221 nista_library-4.0.6/data_point_client/models/data_point_data_response.py
+-rw-r--r--   0        0        0      779 2023-05-28 14:31:25.796221 nista_library-4.0.6/data_point_client/models/data_point_origin.py
+-rw-r--r--   0        0        0     3212 2023-05-28 14:31:25.796221 nista_library-4.0.6/data_point_client/models/data_point_request.py
+-rw-r--r--   0        0        0     7362 2023-05-28 14:31:25.796221 nista_library-4.0.6/data_point_client/models/data_point_response_base.py
+-rw-r--r--   0        0        0     7281 2023-05-28 14:31:25.796221 nista_library-4.0.6/data_point_client/models/day_data_by_hour_transfer.py
+-rw-r--r--   0        0        0     7564 2023-05-28 14:31:25.796221 nista_library-4.0.6/data_point_client/models/day_period_data_bucket.py
+-rw-r--r--   0        0        0     4321 2023-05-28 14:31:25.796221 nista_library-4.0.6/data_point_client/models/day_period_data_point_data.py
+-rw-r--r--   0        0        0      191 2023-05-28 14:31:25.796221 nista_library-4.0.6/data_point_client/models/en_area_type_rest.py
+-rw-r--r--   0        0        0      192 2023-05-28 14:31:25.796221 nista_library-4.0.6/data_point_client/models/en_data_bucket_state.py
+-rw-r--r--   0        0        0      208 2023-05-28 14:31:25.796221 nista_library-4.0.6/data_point_client/models/en_data_point_existence_dto.py
+-rw-r--r--   0        0        0      214 2023-05-28 14:31:25.796221 nista_library-4.0.6/data_point_client/models/en_data_point_state_dto.py
+-rw-r--r--   0        0        0      192 2023-05-28 14:31:25.796221 nista_library-4.0.6/data_point_client/models/en_data_point_status.py
+-rw-r--r--   0        0        0      250 2023-05-28 14:31:25.796221 nista_library-4.0.6/data_point_client/models/en_data_point_type.py
+-rw-r--r--   0        0        0      181 2023-05-28 14:31:25.796221 nista_library-4.0.6/data_point_client/models/en_operator.py
+-rw-r--r--   0        0        0     2375 2023-05-28 14:31:25.796221 nista_library-4.0.6/data_point_client/models/file_origin.py
+-rw-r--r--   0        0        0     2579 2023-05-28 14:31:25.796221 nista_library-4.0.6/data_point_client/models/get_constant_response.py
+-rw-r--r--   0        0        0     3472 2023-05-28 14:31:25.796221 nista_library-4.0.6/data_point_client/models/get_data_request.py
+-rw-r--r--   0        0        0      779 2023-05-28 14:31:25.796221 nista_library-4.0.6/data_point_client/models/get_data_response.py
+-rw-r--r--   0        0        0     3900 2023-05-28 14:31:25.796221 nista_library-4.0.6/data_point_client/models/get_day_period_response.py
+-rw-r--r--   0        0        0     2529 2023-05-28 14:31:25.796221 nista_library-4.0.6/data_point_client/models/get_series_response.py
+-rw-r--r--   0        0        0     3227 2023-05-28 14:31:25.796221 nista_library-4.0.6/data_point_client/models/get_week_period_response.py
+-rw-r--r--   0        0        0     1176 2023-05-28 14:31:25.796221 nista_library-4.0.6/data_point_client/models/gnista_unit_response.py
+-rw-r--r--   0        0        0     1810 2023-05-28 14:31:25.796221 nista_library-4.0.6/data_point_client/models/live_data_origin.py
+-rw-r--r--   0        0        0      765 2023-05-28 14:31:25.796221 nista_library-4.0.6/data_point_client/models/location_rest.py
+-rw-r--r--   0        0        0     2045 2023-05-28 14:31:25.796221 nista_library-4.0.6/data_point_client/models/point_location_rest.py
+-rw-r--r--   0        0        0     3377 2023-05-28 14:31:25.796221 nista_library-4.0.6/data_point_client/models/problem_details.py
+-rw-r--r--   0        0        0     1215 2023-05-28 14:31:25.796221 nista_library-4.0.6/data_point_client/models/problem_details_extensions.py
+-rw-r--r--   0        0        0     1449 2023-05-28 14:31:25.797221 nista_library-4.0.6/data_point_client/models/remote_origin.py
+-rw-r--r--   0        0        0     1247 2023-05-28 14:31:25.797221 nista_library-4.0.6/data_point_client/models/rule.py
+-rw-r--r--   0        0        0     9273 2023-05-28 14:31:25.797221 nista_library-4.0.6/data_point_client/models/series_data_bucket.py
+-rw-r--r--   0        0        0     3058 2023-05-28 14:31:25.797221 nista_library-4.0.6/data_point_client/models/series_data_point_data.py
+-rw-r--r--   0        0        0     1446 2023-05-28 14:31:25.797221 nista_library-4.0.6/data_point_client/models/sub_series_request.py
+-rw-r--r--   0        0        0     1214 2023-05-28 14:31:25.797221 nista_library-4.0.6/data_point_client/models/sub_series_request_values.py
+-rw-r--r--   0        0        0     1631 2023-05-28 14:31:25.797221 nista_library-4.0.6/data_point_client/models/time_series_period.py
+-rw-r--r--   0        0        0     2675 2023-05-28 14:31:25.797221 nista_library-4.0.6/data_point_client/models/time_series_response.py
+-rw-r--r--   0        0        0     1219 2023-05-28 14:31:25.797221 nista_library-4.0.6/data_point_client/models/time_series_response_curve.py
+-rw-r--r--   0        0        0      923 2023-05-28 14:31:25.797221 nista_library-4.0.6/data_point_client/models/update_area_message_request.py
+-rw-r--r--   0        0        0     2674 2023-05-28 14:31:25.797221 nista_library-4.0.6/data_point_client/models/update_area_request.py
+-rw-r--r--   0        0        0     1401 2023-05-28 14:31:25.797221 nista_library-4.0.6/data_point_client/models/update_constant_data_request.py
+-rw-r--r--   0        0        0     2725 2023-05-28 14:31:25.797221 nista_library-4.0.6/data_point_client/models/update_day_period_request.py
+-rw-r--r--   0        0        0     3346 2023-05-28 14:31:25.797221 nista_library-4.0.6/data_point_client/models/update_time_series_request.py
+-rw-r--r--   0        0        0     2052 2023-05-28 14:31:25.797221 nista_library-4.0.6/data_point_client/models/update_week_period_request.py
+-rw-r--r--   0        0        0     7478 2023-05-28 14:31:25.797221 nista_library-4.0.6/data_point_client/models/week_data_transfere.py
+-rw-r--r--   0        0        0     7576 2023-05-28 14:31:25.797221 nista_library-4.0.6/data_point_client/models/week_period_data_bucket.py
+-rw-r--r--   0        0        0     3648 2023-05-28 14:31:25.797221 nista_library-4.0.6/data_point_client/models/week_period_data_point_data.py
+-rw-r--r--   0        0        0       25 2023-05-28 14:31:25.797221 nista_library-4.0.6/data_point_client/py.typed
+-rw-r--r--   0        0        0      993 2023-05-28 14:31:25.797221 nista_library-4.0.6/data_point_client/types.py
+-rw-r--r--   0        0        0     1007 2023-05-28 14:31:25.798220 nista_library-4.0.6/nista_library/__init__.py
+-rw-r--r--   0        0        0    11406 2023-05-28 14:31:25.798220 nista_library-4.0.6/nista_library/nista_connetion.py
+-rw-r--r--   0        0        0     1049 2023-05-28 14:31:25.798220 nista_library-4.0.6/nista_library/nista_credential_manager.py
+-rw-r--r--   0        0        0    18270 2023-05-28 14:31:25.798220 nista_library-4.0.6/nista_library/nista_data_point.py
+-rw-r--r--   0        0        0     1970 2023-05-28 14:31:25.799221 nista_library-4.0.6/nista_library/nista_data_points.py
+-rw-r--r--   0        0        0     1383 2023-05-28 14:31:25.800221 nista_library-4.0.6/pyproject.toml
+-rw-r--r--   0        0        0     7471 1970-01-01 00:00:00.000000 nista_library-4.0.6/PKG-INFO
```

### Comparing `nista_library-4.0.5/LICENSE.md` & `nista_library-4.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/README.md` & `nista_library-4.0.6/README.md`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/api/data_export/data_export_create_csv_export.py` & `nista_library-4.0.6/data_point_client/api/data_export/data_export_create_csv_export.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/api/data_point/data_point_append_execution_result_data.py` & `nista_library-4.0.6/data_point_client/api/data_point/data_point_append_execution_result_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/api/data_point/data_point_append_time_series_data.py` & `nista_library-4.0.6/data_point_client/api/data_point/data_point_append_time_series_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/api/data_point/data_point_create_area.py` & `nista_library-4.0.6/data_point_client/api/data_point/data_point_create_area.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/api/data_point/data_point_create_area_message.py` & `nista_library-4.0.6/data_point_client/api/data_point/data_point_create_area_message.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/api/data_point/data_point_create_chiller_samples.py` & `nista_library-4.0.6/data_point_client/api/data_point/data_point_create_chiller_samples.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/api/data_point/data_point_create_data_point.py` & `nista_library-4.0.6/data_point_client/api/data_point/data_point_create_data_point.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/api/data_point/data_point_delete_area.py` & `nista_library-4.0.6/data_point_client/api/data_point/data_point_delete_area.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/api/data_point/data_point_delete_data_point.py` & `nista_library-4.0.6/data_point_client/api/data_point/data_point_delete_data_point.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py` & `nista_library-4.0.6/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/api/data_point/data_point_delete_message.py` & `nista_library-4.0.6/data_point_client/api/data_point/data_point_delete_message.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/api/data_point/data_point_get_data.py` & `nista_library-4.0.6/data_point_client/api/data_point/data_point_get_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/api/data_point/data_point_get_data_point.py` & `nista_library-4.0.6/data_point_client/api/data_point/data_point_get_data_point.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/api/data_point/data_point_get_data_point_by_version.py` & `nista_library-4.0.6/data_point_client/api/data_point/data_point_get_data_point_by_version.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/api/data_point/data_point_get_data_points.py` & `nista_library-4.0.6/data_point_client/api/data_point/data_point_get_data_points.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/api/data_point/data_point_get_tags.py` & `nista_library-4.0.6/data_point_client/api/data_point/data_point_get_tags.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/api/data_point/data_point_get_tags_2.py` & `nista_library-4.0.6/data_point_client/api/data_point/data_point_get_tags_2.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/api/data_point/data_point_list_areas.py` & `nista_library-4.0.6/data_point_client/api/data_point/data_point_list_areas.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/api/data_point/data_point_update_area.py` & `nista_library-4.0.6/data_point_client/api/data_point/data_point_update_area.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/api/data_point/data_point_update_constant_data.py` & `nista_library-4.0.6/data_point_client/api/data_point/data_point_update_constant_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/api/data_point/data_point_update_data_point.py` & `nista_library-4.0.6/data_point_client/api/data_point/data_point_update_data_point.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py` & `nista_library-4.0.6/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/api/data_point/data_point_update_data_point_unit.py` & `nista_library-4.0.6/data_point_client/api/data_point/data_point_update_data_point_unit.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/api/data_point/data_point_update_day_period_data.py` & `nista_library-4.0.6/data_point_client/api/data_point/data_point_update_day_period_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/api/data_point/data_point_update_message.py` & `nista_library-4.0.6/data_point_client/api/data_point/data_point_update_message.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/api/data_point/data_point_update_time_series_data.py` & `nista_library-4.0.6/data_point_client/api/data_point/data_point_update_time_series_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/api/data_point/data_point_update_week_period_data.py` & `nista_library-4.0.6/data_point_client/api/data_point/data_point_update_week_period_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/client.py` & `nista_library-4.0.6/data_point_client/client.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/__init__.py` & `nista_library-4.0.6/data_point_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/append_execution_result_data_request.py` & `nista_library-4.0.6/data_point_client/models/append_execution_result_data_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,40 +14,45 @@
 @attr.s(auto_attribs=True)
 class AppendExecutionResultDataRequest:
     """
     Attributes:
         sub_series (List['SubSeriesRequest']):
         unit (Union[Unset, None, str]):
         execution_id (Union[Unset, str]):
+        time_zone (Union[Unset, None, str]):
     """
 
     sub_series: List["SubSeriesRequest"]
     unit: Union[Unset, None, str] = UNSET
     execution_id: Union[Unset, str] = UNSET
+    time_zone: Union[Unset, None, str] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         sub_series = []
         for sub_series_item_data in self.sub_series:
             sub_series_item = sub_series_item_data.to_dict()
 
             sub_series.append(sub_series_item)
 
         unit = self.unit
         execution_id = self.execution_id
+        time_zone = self.time_zone
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(
             {
                 "subSeries": sub_series,
             }
         )
         if unit is not UNSET:
             field_dict["unit"] = unit
         if execution_id is not UNSET:
             field_dict["executionId"] = execution_id
+        if time_zone is not UNSET:
+            field_dict["timeZone"] = time_zone
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.sub_series_request import SubSeriesRequest
 
@@ -59,14 +64,17 @@
 
             sub_series.append(sub_series_item)
 
         unit = d.pop("unit", UNSET)
 
         execution_id = d.pop("executionId", UNSET)
 
+        time_zone = d.pop("timeZone", UNSET)
+
         append_execution_result_data_request = cls(
             sub_series=sub_series,
             unit=unit,
             execution_id=execution_id,
+            time_zone=time_zone,
         )
 
         return append_execution_result_data_request
```

### Comparing `nista_library-4.0.5/data_point_client/models/append_time_series_request.py` & `nista_library-4.0.6/data_point_client/models/append_time_series_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/area_of_interest_response.py` & `nista_library-4.0.6/data_point_client/models/area_of_interest_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/calculation_origin.py` & `nista_library-4.0.6/data_point_client/models/calculation_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/constant_data_bucket.py` & `nista_library-4.0.6/data_point_client/models/constant_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/constant_data_point_data.py` & `nista_library-4.0.6/data_point_client/models/constant_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/continuous_location_rest.py` & `nista_library-4.0.6/data_point_client/models/continuous_location_rest.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/create_area_message_request.py` & `nista_library-4.0.6/data_point_client/models/create_area_message_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/create_area_request.py` & `nista_library-4.0.6/data_point_client/models/create_area_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/data_bucket_base.py` & `nista_library-4.0.6/data_point_client/models/data_bucket_base.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/data_export_request.py` & `nista_library-4.0.6/data_point_client/models/data_export_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/data_point_comment_message_response.py` & `nista_library-4.0.6/data_point_client/models/data_point_comment_message_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/data_point_data_base.py` & `nista_library-4.0.6/data_point_client/models/data_point_data_base.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/data_point_data_response.py` & `nista_library-4.0.6/data_point_client/models/data_point_data_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/data_point_origin.py` & `nista_library-4.0.6/data_point_client/models/data_point_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/data_point_request.py` & `nista_library-4.0.6/data_point_client/models/data_point_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/data_point_response_base.py` & `nista_library-4.0.6/data_point_client/models/data_point_response_base.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/day_data_by_hour_transfer.py` & `nista_library-4.0.6/data_point_client/models/day_data_by_hour_transfer.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/day_period_data_bucket.py` & `nista_library-4.0.6/data_point_client/models/day_period_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/day_period_data_point_data.py` & `nista_library-4.0.6/data_point_client/models/day_period_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/file_origin.py` & `nista_library-4.0.6/data_point_client/models/file_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/get_constant_response.py` & `nista_library-4.0.6/data_point_client/models/get_constant_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/get_data_request.py` & `nista_library-4.0.6/data_point_client/models/get_data_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/get_data_response.py` & `nista_library-4.0.6/data_point_client/models/get_data_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/get_day_period_response.py` & `nista_library-4.0.6/data_point_client/models/get_day_period_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/get_series_response.py` & `nista_library-4.0.6/data_point_client/models/get_series_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/get_week_period_response.py` & `nista_library-4.0.6/data_point_client/models/get_week_period_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/gnista_unit_response.py` & `nista_library-4.0.6/data_point_client/models/gnista_unit_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/live_data_origin.py` & `nista_library-4.0.6/data_point_client/models/live_data_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/location_rest.py` & `nista_library-4.0.6/data_point_client/models/location_rest.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/point_location_rest.py` & `nista_library-4.0.6/data_point_client/models/point_location_rest.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/problem_details.py` & `nista_library-4.0.6/data_point_client/models/problem_details.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/problem_details_extensions.py` & `nista_library-4.0.6/data_point_client/models/problem_details_extensions.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/remote_origin.py` & `nista_library-4.0.6/data_point_client/models/remote_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/rule.py` & `nista_library-4.0.6/data_point_client/models/rule.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/series_data_bucket.py` & `nista_library-4.0.6/data_point_client/models/series_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/series_data_point_data.py` & `nista_library-4.0.6/data_point_client/models/series_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/sub_series_request.py` & `nista_library-4.0.6/data_point_client/models/sub_series_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/sub_series_request_values.py` & `nista_library-4.0.6/data_point_client/models/sub_series_request_values.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/time_series_period.py` & `nista_library-4.0.6/data_point_client/models/time_series_period.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/time_series_response.py` & `nista_library-4.0.6/data_point_client/models/time_series_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/time_series_response_curve.py` & `nista_library-4.0.6/data_point_client/models/time_series_response_curve.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/update_area_message_request.py` & `nista_library-4.0.6/data_point_client/models/update_area_message_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/update_area_request.py` & `nista_library-4.0.6/data_point_client/models/update_area_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/update_constant_data_request.py` & `nista_library-4.0.6/data_point_client/models/update_constant_data_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/update_day_period_request.py` & `nista_library-4.0.6/data_point_client/models/update_day_period_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/update_time_series_request.py` & `nista_library-4.0.6/data_point_client/models/update_time_series_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/update_week_period_request.py` & `nista_library-4.0.6/data_point_client/models/update_week_period_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/week_data_transfere.py` & `nista_library-4.0.6/data_point_client/models/week_data_transfere.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/week_period_data_bucket.py` & `nista_library-4.0.6/data_point_client/models/week_period_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/models/week_period_data_point_data.py` & `nista_library-4.0.6/data_point_client/models/week_period_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/data_point_client/types.py` & `nista_library-4.0.6/data_point_client/types.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/nista_library/__init__.py` & `nista_library-4.0.6/nista_library/__init__.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/nista_library/nista_connetion.py` & `nista_library-4.0.6/nista_library/nista_connetion.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/nista_library/nista_credential_manager.py` & `nista_library-4.0.6/nista_library/nista_credential_manager.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/nista_library/nista_data_point.py` & `nista_library-4.0.6/nista_library/nista_data_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -320,20 +320,22 @@
 
     def append_data_point_result_parts(
         self,
         data: Union[List[DataFrame], float],
         unit: Optional[str],
         execution_id: uuid.UUID,
         timeout: float = 5.0,
+        time_zone: ZoneInfo = ZoneInfo("UTC"),
     ) -> Optional[Response[Union[Any, ProblemDetails]]]:
         """Append data as an execution Result. This method is used for nista.io Internal Execution handling
         :param data: To be added to a DataPoint
         :param unit: The Unit to set on the DataPoint Store
         :param execution_id: the execution ID that this data is assignable to
         :param timeout: How long to wait for response
+        :param time_zone: The Time Zone of the newly added Data, default is UTC
         """
         token = self.connection.get_access_token()
         client = AuthenticatedClient(
             base_url=self.connection.datapoint_base_url,
             token=token,
             verify_ssl=self.connection.verify_ssl,
             timeout=timeout,
@@ -344,15 +346,15 @@
             for data_frame in data:
                 data_dict = self._to_dict(data_frame)
                 value = SubSeriesRequestValues.from_dict(src_dict=data_dict)
                 request = SubSeriesRequest(values=value)
                 sub_series.append(request)
 
             append_request = AppendExecutionResultDataRequest(
-                sub_series=sub_series, unit=unit, execution_id=str(execution_id)
+                sub_series=sub_series, unit=unit, execution_id=str(execution_id), time_zone=time_zone.key
             )
 
             return data_point_append_execution_result_data.sync_detailed(
                 workspace_id=self.connection.workspace_id,
                 client=client,
                 data_point_id=str(self.data_point_id),
                 json_body=append_request,
```

### Comparing `nista_library-4.0.5/nista_library/nista_data_points.py` & `nista_library-4.0.6/nista_library/nista_data_points.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.5/pyproject.toml` & `nista_library-4.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nista-library"
-version = "4.0.5"
+version = "4.0.6"
 description = "A client library for accessing nista.io"
 license = "MIT"
 
 authors = ["Markus Hoffmann <markus.hoffmann@nista.io>"]
 
 readme = "README.md"
 homepage = "https://nista.io"
```

### Comparing `nista_library-4.0.5/PKG-INFO` & `nista_library-4.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nista-library
-Version: 4.0.5
+Version: 4.0.6
 Summary: A client library for accessing nista.io
 Home-page: https://nista.io
 License: MIT
 Author: Markus Hoffmann
 Author-email: markus.hoffmann@nista.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

