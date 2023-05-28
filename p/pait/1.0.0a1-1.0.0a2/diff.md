# Comparing `tmp/pait-1.0.0a1.tar.gz` & `tmp/pait-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pait-1.0.0a1.tar", max compression
+gzip compressed data, was "pait-1.0.0a2.tar", max compression
```

## Comparing `pait-1.0.0a1.tar` & `pait-1.0.0a2.tar`

### file list

```diff
@@ -1,184 +1,183 @@
--rw-r--r--   0        0        0    11357 2021-12-05 05:37:05.000000 pait-1.0.0a1/LICENSE
--rw-r--r--   0        0        0     4608 2023-03-21 10:06:14.408062 pait-1.0.0a1/README.md
--rw-r--r--   0        0        0       37 2023-04-12 08:54:18.124162 pait-1.0.0a1/pait/__init__.py
--rw-r--r--   0        0        0       31 2023-05-09 17:42:05.966242 pait-1.0.0a1/pait/__version__.py
--rw-r--r--   0        0        0      199 2023-04-15 07:27:03.886801 pait-1.0.0a1/pait/app/__init__.py
--rw-r--r--   0        0        0     5448 2023-04-15 07:29:45.835731 pait-1.0.0a1/pait/app/any/__init__.py
--rw-r--r--   0        0        0      535 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/any/plugin/__init__.py
--rw-r--r--   0        0        0      460 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/any/plugin/auto_complete_json_resp.py
--rw-r--r--   0        0        0      425 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/any/plugin/cache_response.py
--rw-r--r--   0        0        0      405 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/any/plugin/check_json_resp.py
--rw-r--r--   0        0        0      373 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/any/plugin/mock_response.py
--rw-r--r--   0        0        0      424 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/any/plugin/unified_response.py
--rw-r--r--   0        0        0        0 2023-01-17 11:47:59.744123 pait-1.0.0a1/pait/app/any/security/__init__.py
--rw-r--r--   0        0        0      342 2023-02-08 03:58:49.610123 pait-1.0.0a1/pait/app/any/security/api_key.py
--rw-r--r--   0        0        0      653 2023-02-10 15:24:31.281635 pait-1.0.0a1/pait/app/any/security/http.py
--rw-r--r--   0        0        0      660 2023-02-08 03:43:07.655826 pait-1.0.0a1/pait/app/any/security/oauth2.py
--rw-r--r--   0        0        0     1328 2023-01-18 19:31:20.014191 pait-1.0.0a1/pait/app/any/util.py
--rw-r--r--   0        0        0      562 2023-02-15 10:04:32.538762 pait-1.0.0a1/pait/app/auto_load_app.py
--rw-r--r--   0        0        0      121 2023-01-09 15:13:50.000000 pait-1.0.0a1/pait/app/base/__init__.py
--rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a1/pait/app/base/adapter/__init__.py
--rw-r--r--   0        0        0     2427 2023-04-08 08:28:39.674480 pait-1.0.0a1/pait/app/base/adapter/request.py
--rw-r--r--   0        0        0     1806 2023-05-09 17:31:47.728377 pait-1.0.0a1/pait/app/base/app_helper.py
--rw-r--r--   0        0        0     8578 2023-04-12 08:47:20.207805 pait-1.0.0a1/pait/app/base/doc_route.py
--rw-r--r--   0        0        0        0 2023-02-10 10:23:08.836059 pait-1.0.0a1/pait/app/base/security/__init__.py
--rw-r--r--   0        0        0     1762 2023-03-28 15:33:21.719126 pait-1.0.0a1/pait/app/base/security/api_key.py
--rw-r--r--   0        0        0      587 2023-02-10 03:32:05.848598 pait-1.0.0a1/pait/app/base/security/base.py
--rw-r--r--   0        0        0     7379 2023-03-31 07:37:07.804728 pait-1.0.0a1/pait/app/base/security/http.py
--rw-r--r--   0        0        0     4010 2023-04-12 08:47:20.183805 pait-1.0.0a1/pait/app/base/security/oauth2.py
--rw-r--r--   0        0        0      794 2023-02-10 15:22:20.692947 pait-1.0.0a1/pait/app/base/security/util.py
--rw-r--r--   0        0        0      649 2023-04-12 08:26:12.386264 pait-1.0.0a1/pait/app/base/simple_route.py
--rw-r--r--   0        0        0    13748 2023-04-18 03:25:53.893314 pait-1.0.0a1/pait/app/base/test_helper.py
--rw-r--r--   0        0        0      319 2023-04-15 07:12:04.318861 pait-1.0.0a1/pait/app/flask/__init__.py
--rw-r--r--   0        0        0      719 2023-03-21 10:06:14.408062 pait-1.0.0a1/pait/app/flask/_app_helper.py
--rw-r--r--   0        0        0      394 2023-03-21 10:06:14.408062 pait-1.0.0a1/pait/app/flask/_attribute.py
--rw-r--r--   0        0        0      792 2023-04-15 06:34:05.735149 pait-1.0.0a1/pait/app/flask/_exception.py
--rw-r--r--   0        0        0     3495 2023-04-12 08:26:12.398264 pait-1.0.0a1/pait/app/flask/_load_app.py
--rw-r--r--   0        0        0      269 2022-01-10 09:58:31.000000 pait-1.0.0a1/pait/app/flask/_pait.py
--rw-r--r--   0        0        0     1775 2023-04-15 07:12:11.062879 pait-1.0.0a1/pait/app/flask/_simple_route.py
--rw-r--r--   0        0        0     1900 2023-04-12 08:23:56.321748 pait-1.0.0a1/pait/app/flask/_test_helper.py
--rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a1/pait/app/flask/adapter/__init__.py
--rw-r--r--   0        0        0     1689 2023-04-08 08:28:39.674480 pait-1.0.0a1/pait/app/flask/adapter/request.py
--rw-r--r--   0        0        0     1070 2023-04-19 15:03:14.295510 pait-1.0.0a1/pait/app/flask/adapter/response.py
--rw-r--r--   0        0        0      784 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/flask/plugin/__init__.py
--rw-r--r--   0        0        0      117 2023-02-06 11:24:42.996357 pait-1.0.0a1/pait/app/flask/plugin/auto_complete_json_resp.py
--rw-r--r--   0        0        0       94 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/flask/plugin/cache_response.py
--rw-r--r--   0        0        0      556 2023-04-19 16:11:36.294732 pait-1.0.0a1/pait/app/flask/plugin/check_json_resp.py
--rw-r--r--   0        0        0     1180 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/flask/plugin/mock_response.py
--rw-r--r--   0        0        0      746 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/flask/plugin/unified_response.py
--rw-r--r--   0        0        0        0 2023-01-09 09:37:04.000000 pait-1.0.0a1/pait/app/flask/security/__init__.py
--rw-r--r--   0        0        0      137 2023-04-15 06:37:25.447043 pait-1.0.0a1/pait/app/flask/security/api_key.py
--rw-r--r--   0        0        0      392 2023-04-15 06:37:25.447043 pait-1.0.0a1/pait/app/flask/security/http.py
--rw-r--r--   0        0        0      566 2023-04-15 06:37:25.447043 pait-1.0.0a1/pait/app/flask/security/oauth2.py
--rw-r--r--   0        0        0      321 2023-04-15 06:40:17.664067 pait-1.0.0a1/pait/app/flask/security/util.py
--rw-r--r--   0        0        0      319 2023-04-15 07:12:04.418861 pait-1.0.0a1/pait/app/sanic/__init__.py
--rw-r--r--   0        0        0      938 2023-03-21 10:06:14.408062 pait-1.0.0a1/pait/app/sanic/_app_helper.py
--rw-r--r--   0        0        0      403 2023-03-21 10:06:14.412062 pait-1.0.0a1/pait/app/sanic/_attribute.py
--rw-r--r--   0        0        0      319 2023-04-15 06:34:05.735149 pait-1.0.0a1/pait/app/sanic/_exception.py
--rw-r--r--   0        0        0     3773 2023-04-12 08:23:56.217747 pait-1.0.0a1/pait/app/sanic/_load_app.py
--rw-r--r--   0        0        0      374 2023-05-09 02:55:20.341357 pait-1.0.0a1/pait/app/sanic/_pait.py
--rw-r--r--   0        0        0     1749 2023-04-15 07:12:11.082880 pait-1.0.0a1/pait/app/sanic/_simple_route.py
--rw-r--r--   0        0        0     2172 2023-04-12 08:26:12.346264 pait-1.0.0a1/pait/app/sanic/_test_helper.py
--rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a1/pait/app/sanic/adapter/__init__.py
--rw-r--r--   0        0        0     2067 2023-05-09 17:31:47.728377 pait-1.0.0a1/pait/app/sanic/adapter/request.py
--rw-r--r--   0        0        0     1102 2023-04-19 15:03:14.279509 pait-1.0.0a1/pait/app/sanic/adapter/response.py
--rw-r--r--   0        0        0      716 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/sanic/plugin/__init__.py
--rw-r--r--   0        0        0      711 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/sanic/plugin/auto_complete_json_resp.py
--rw-r--r--   0        0        0       94 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/sanic/plugin/cache_response.py
--rw-r--r--   0        0        0      934 2023-04-19 16:11:36.354731 pait-1.0.0a1/pait/app/sanic/plugin/check_json_resp.py
--rw-r--r--   0        0        0     1432 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/sanic/plugin/mock_response.py
--rw-r--r--   0        0        0      746 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/sanic/plugin/unified_response.py
--rw-r--r--   0        0        0        0 2023-01-09 09:37:04.000000 pait-1.0.0a1/pait/app/sanic/security/__init__.py
--rw-r--r--   0        0        0      137 2023-04-15 06:37:25.447043 pait-1.0.0a1/pait/app/sanic/security/api_key.py
--rw-r--r--   0        0        0      392 2023-04-15 06:37:25.447043 pait-1.0.0a1/pait/app/sanic/security/http.py
--rw-r--r--   0        0        0      566 2023-04-15 06:37:25.447043 pait-1.0.0a1/pait/app/sanic/security/oauth2.py
--rw-r--r--   0        0        0      321 2023-04-15 06:38:51.947005 pait-1.0.0a1/pait/app/sanic/security/util.py
--rw-r--r--   0        0        0      323 2023-04-15 07:12:04.374861 pait-1.0.0a1/pait/app/starlette/__init__.py
--rw-r--r--   0        0        0      651 2023-03-21 10:06:14.412062 pait-1.0.0a1/pait/app/starlette/_app_helper.py
--rw-r--r--   0        0        0      430 2023-03-21 10:06:14.412062 pait-1.0.0a1/pait/app/starlette/_attribute.py
--rw-r--r--   0        0        0      319 2023-04-15 06:34:05.735149 pait-1.0.0a1/pait/app/starlette/_exception.py
--rw-r--r--   0        0        0     3877 2023-04-12 08:26:12.314264 pait-1.0.0a1/pait/app/starlette/_load_app.py
--rw-r--r--   0        0        0      291 2022-01-10 09:58:31.000000 pait-1.0.0a1/pait/app/starlette/_pait.py
--rw-r--r--   0        0        0      996 2023-04-15 08:13:17.515420 pait-1.0.0a1/pait/app/starlette/_simple_route.py
--rw-r--r--   0        0        0     1930 2023-04-12 08:26:12.430264 pait-1.0.0a1/pait/app/starlette/_test_helper.py
--rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a1/pait/app/starlette/adapter/__init__.py
--rw-r--r--   0        0        0     2718 2023-04-08 08:28:39.674480 pait-1.0.0a1/pait/app/starlette/adapter/request.py
--rw-r--r--   0        0        0     1065 2023-04-19 15:03:14.267508 pait-1.0.0a1/pait/app/starlette/adapter/response.py
--rw-r--r--   0        0        0      800 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/starlette/plugin/__init__.py
--rw-r--r--   0        0        0      711 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/starlette/plugin/auto_complete_json_resp.py
--rw-r--r--   0        0        0       94 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/starlette/plugin/cache_response.py
--rw-r--r--   0        0        0      785 2023-04-19 16:11:35.998735 pait-1.0.0a1/pait/app/starlette/plugin/check_json_resp.py
--rw-r--r--   0        0        0     1626 2023-02-16 07:49:53.639890 pait-1.0.0a1/pait/app/starlette/plugin/mock_response.py
--rw-r--r--   0        0        0      702 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/starlette/plugin/unified_response.py
--rw-r--r--   0        0        0        0 2023-01-09 09:37:04.000000 pait-1.0.0a1/pait/app/starlette/security/__init__.py
--rw-r--r--   0        0        0      137 2023-04-15 06:37:25.447043 pait-1.0.0a1/pait/app/starlette/security/api_key.py
--rw-r--r--   0        0        0      392 2023-04-15 06:37:25.447043 pait-1.0.0a1/pait/app/starlette/security/http.py
--rw-r--r--   0        0        0      522 2023-04-15 06:37:25.447043 pait-1.0.0a1/pait/app/starlette/security/oauth2.py
--rw-r--r--   0        0        0      325 2023-04-15 06:40:17.664067 pait-1.0.0a1/pait/app/starlette/security/util.py
--rw-r--r--   0        0        0      321 2023-04-15 07:12:04.378861 pait-1.0.0a1/pait/app/tornado/__init__.py
--rw-r--r--   0        0        0     1002 2023-03-21 10:06:14.412062 pait-1.0.0a1/pait/app/tornado/_app_helper.py
--rw-r--r--   0        0        0      424 2023-03-21 10:06:14.412062 pait-1.0.0a1/pait/app/tornado/_attribute.py
--rw-r--r--   0        0        0      298 2023-04-15 06:34:05.735149 pait-1.0.0a1/pait/app/tornado/_exception.py
--rw-r--r--   0        0        0     2499 2023-04-12 08:23:56.301748 pait-1.0.0a1/pait/app/tornado/_load_app.py
--rw-r--r--   0        0        0      291 2022-01-10 09:58:31.000000 pait-1.0.0a1/pait/app/tornado/_pait.py
--rw-r--r--   0        0        0     2839 2023-04-15 07:36:59.865873 pait-1.0.0a1/pait/app/tornado/_simple_route.py
--rw-r--r--   0        0        0     4664 2023-04-12 08:26:12.382264 pait-1.0.0a1/pait/app/tornado/_test_helper.py
--rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a1/pait/app/tornado/adapter/__init__.py
--rw-r--r--   0        0        0     2244 2023-04-08 08:28:39.674480 pait-1.0.0a1/pait/app/tornado/adapter/request.py
--rw-r--r--   0        0        0     1130 2023-04-19 15:03:14.287509 pait-1.0.0a1/pait/app/tornado/adapter/response.py
--rw-r--r--   0        0        0      792 2023-02-07 03:41:51.360782 pait-1.0.0a1/pait/app/tornado/plugin/__init__.py
--rw-r--r--   0        0        0      574 2023-02-07 03:41:51.360782 pait-1.0.0a1/pait/app/tornado/plugin/auto_complete_json_resp.py
--rw-r--r--   0        0        0     1329 2023-02-07 03:41:51.360782 pait-1.0.0a1/pait/app/tornado/plugin/cache_response.py
--rw-r--r--   0        0        0     1211 2023-04-19 16:11:36.402730 pait-1.0.0a1/pait/app/tornado/plugin/check_json_resp.py
--rw-r--r--   0        0        0     1237 2023-02-07 03:41:51.360782 pait-1.0.0a1/pait/app/tornado/plugin/mock_response.py
--rw-r--r--   0        0        0     1247 2023-02-07 03:41:51.360782 pait-1.0.0a1/pait/app/tornado/plugin/unified_response.py
--rw-r--r--   0        0        0        0 2023-02-03 19:54:29.188502 pait-1.0.0a1/pait/app/tornado/security/__init__.py
--rw-r--r--   0        0        0      137 2023-04-15 06:37:25.447043 pait-1.0.0a1/pait/app/tornado/security/api_key.py
--rw-r--r--   0        0        0      392 2023-04-15 06:37:25.447043 pait-1.0.0a1/pait/app/tornado/security/http.py
--rw-r--r--   0        0        0      522 2023-04-15 06:37:25.447043 pait-1.0.0a1/pait/app/tornado/security/oauth2.py
--rw-r--r--   0        0        0      323 2023-04-15 06:39:33.671398 pait-1.0.0a1/pait/app/tornado/security/util.py
--rw-r--r--   0        0        0    18340 2023-05-09 17:31:47.728377 pait-1.0.0a1/pait/core.py
--rw-r--r--   0        0        0     1645 2023-04-12 08:23:56.325748 pait-1.0.0a1/pait/data.py
--rw-r--r--   0        0        0      688 2023-01-11 17:12:40.000000 pait-1.0.0a1/pait/exceptions.py
--rw-r--r--   0        0        0        0 2022-04-03 14:03:33.000000 pait-1.0.0a1/pait/extra/__init__.py
--rw-r--r--   0        0        0     7452 2023-04-12 08:47:20.055805 pait-1.0.0a1/pait/extra/config.py
--rw-r--r--   0        0        0      637 2023-04-12 08:47:20.219805 pait-1.0.0a1/pait/extra/util.py
--rw-r--r--   0        0        0    11023 2023-05-09 17:31:47.728377 pait-1.0.0a1/pait/field.py
--rw-r--r--   0        0        0     1261 2023-04-12 08:47:20.207805 pait-1.0.0a1/pait/g.py
--rw-r--r--   0        0        0      508 2023-04-12 08:47:20.799805 pait-1.0.0a1/pait/grpc/__init__.py
--rw-r--r--   0        0        0     4623 2023-05-09 17:31:34.510840 pait-1.0.0a1/pait/grpc/base_gateway.py
--rw-r--r--   0        0        0      511 2023-04-12 08:47:20.099805 pait-1.0.0a1/pait/grpc/desc_template.py
--rw-r--r--   0        0        0    13407 2023-04-12 08:47:20.103805 pait-1.0.0a1/pait/grpc/gateway.py
--rw-r--r--   0        0        0    10237 2023-05-09 17:31:34.510840 pait-1.0.0a1/pait/grpc/inspect.py
--rw-r--r--   0        0        0        0 2023-03-24 09:24:42.276250 pait-1.0.0a1/pait/grpc/plugin/__init__.py
--rw-r--r--   0        0        0       31 2023-03-24 09:24:42.276250 pait-1.0.0a1/pait/grpc/plugin/__main__.py
--rw-r--r--   0        0        0     1762 2023-03-31 09:09:09.660127 pait-1.0.0a1/pait/grpc/plugin/code_gen.py
--rw-r--r--   0        0        0     1322 2023-04-12 08:13:18.843706 pait-1.0.0a1/pait/grpc/plugin/config.py
--rw-r--r--   0        0        0    20548 2023-05-09 17:31:34.510840 pait-1.0.0a1/pait/grpc/plugin/field_desc_proto_to_route_code.py
--rw-r--r--   0        0        0     3248 2023-04-19 16:23:47.347674 pait-1.0.0a1/pait/grpc/plugin/gateway.py
--rwxr-xr-x   0        0        0      266 2023-03-24 09:24:42.276250 pait-1.0.0a1/pait/grpc/plugin/main.py
--rw-r--r--   0        0        0     1120 2023-04-19 16:29:34.584057 pait-1.0.0a1/pait/grpc/plugin/model.py
--rw-r--r--   0        0        0        0 2023-03-24 09:24:42.276250 pait-1.0.0a1/pait/grpc/proto/__init__.py
--rw-r--r--   0        0        0     4193 2023-04-10 06:13:16.195059 pait-1.0.0a1/pait/grpc/proto/api.proto
--rw-r--r--   0        0        0     5030 2023-04-11 03:13:43.474993 pait-1.0.0a1/pait/grpc/proto/api_pb2.py
--rw-r--r--   0        0        0    11716 2023-04-11 03:13:43.894994 pait-1.0.0a1/pait/grpc/proto/api_pb2.pyi
--rw-r--r--   0        0        0      146 2023-04-11 03:13:45.778998 pait-1.0.0a1/pait/grpc/proto/api_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-10 09:17:38.116710 pait-1.0.0a1/pait/grpc/proto/api_pb2_grpc.pyi
--rw-r--r--   0        0        0      436 2023-03-24 09:24:42.276250 pait-1.0.0a1/pait/grpc/types.py
--rw-r--r--   0        0        0     4915 2023-05-09 17:31:34.510840 pait-1.0.0a1/pait/grpc/util.py
--rw-r--r--   0        0        0      559 2023-04-12 08:23:56.233748 pait-1.0.0a1/pait/model/__init__.py
--rw-r--r--   0        0        0     3305 2023-04-13 18:01:44.819386 pait-1.0.0a1/pait/model/config.py
--rw-r--r--   0        0        0     1606 2023-04-12 08:47:20.947805 pait-1.0.0a1/pait/model/context.py
--rw-r--r--   0        0        0     9670 2023-05-09 17:31:47.728377 pait-1.0.0a1/pait/model/core.py
--rw-r--r--   0        0        0     6051 2023-04-12 16:05:40.728961 pait-1.0.0a1/pait/model/response.py
--rw-r--r--   0        0        0      700 2023-04-17 06:04:21.361298 pait-1.0.0a1/pait/model/status.py
--rw-r--r--   0        0        0     1400 2023-04-12 08:47:22.147805 pait-1.0.0a1/pait/model/tag.py
--rw-r--r--   0        0        0     1166 2022-09-26 15:06:36.000000 pait-1.0.0a1/pait/model/template.py
--rw-r--r--   0        0        0        0 2022-01-21 03:47:13.000000 pait-1.0.0a1/pait/openapi/__init__.py
--rw-r--r--   0        0        0    10110 2023-04-15 08:16:39.307851 pait-1.0.0a1/pait/openapi/doc_route.py
--rw-r--r--   0        0        0    12360 2023-04-08 08:28:39.674480 pait-1.0.0a1/pait/openapi/openapi.py
--rw-r--r--   0        0        0      105 2023-02-07 03:41:51.360782 pait-1.0.0a1/pait/param_handle/__init__.py
--rw-r--r--   0        0        0     6362 2023-05-09 17:31:47.728377 pait-1.0.0a1/pait/param_handle/_async.py
--rw-r--r--   0        0        0     5305 2023-05-09 17:31:47.728377 pait-1.0.0a1/pait/param_handle/_sync.py
--rw-r--r--   0        0        0    12308 2023-05-09 17:31:47.732377 pait-1.0.0a1/pait/param_handle/base.py
--rw-r--r--   0        0        0       87 2023-02-07 03:41:51.360782 pait-1.0.0a1/pait/plugin/__init__.py
--rw-r--r--   0        0        0     2298 2023-02-07 03:41:51.360782 pait-1.0.0a1/pait/plugin/at_most_one_of.py
--rw-r--r--   0        0        0     2599 2023-04-18 03:27:33.637660 pait-1.0.0a1/pait/plugin/auto_complete_json_resp.py
--rw-r--r--   0        0        0     3592 2023-04-19 15:26:48.912272 pait-1.0.0a1/pait/plugin/base.py
--rw-r--r--   0        0        0     8794 2023-03-31 07:37:07.804728 pait-1.0.0a1/pait/plugin/cache_response.py
--rw-r--r--   0        0        0     2228 2023-04-19 16:14:57.640339 pait-1.0.0a1/pait/plugin/check_json_resp.py
--rw-r--r--   0        0        0     5105 2023-04-18 03:25:53.869314 pait-1.0.0a1/pait/plugin/mock_response.py
--rw-r--r--   0        0        0     3312 2023-02-07 03:41:51.360782 pait-1.0.0a1/pait/plugin/required.py
--rw-r--r--   0        0        0     2109 2023-04-18 03:25:53.877313 pait-1.0.0a1/pait/plugin/unified_response.py
--rw-r--r--   0        0        0     1161 2023-02-08 11:47:07.069892 pait-1.0.0a1/pait/types.py
--rw-r--r--   0        0        0      524 2023-02-14 09:33:41.434168 pait-1.0.0a1/pait/util/__init__.py
--rw-r--r--   0        0        0     1979 2023-02-08 14:21:51.755841 pait-1.0.0a1/pait/util/_func_sig.py
--rw-r--r--   0        0        0     2607 2023-01-12 10:30:13.000000 pait-1.0.0a1/pait/util/_gen_tip.py
--rw-r--r--   0        0        0     1907 2022-04-10 08:10:06.000000 pait-1.0.0a1/pait/util/_lazy_property.py
--rw-r--r--   0        0        0      957 2023-04-10 07:15:56.924352 pait-1.0.0a1/pait/util/_pydantic_util.py
--rw-r--r--   0        0        0     4211 2023-04-15 06:41:46.425281 pait-1.0.0a1/pait/util/_types.py
--rw-r--r--   0        0        0    13475 2023-04-26 06:56:27.310437 pait-1.0.0a1/pait/util/_util.py
--rw-r--r--   0        0        0      869 2023-04-13 18:01:45.039386 pait-1.0.0a1/pait/util/encoder.py
--rw-r--r--   0        0        0     3561 2023-05-09 17:42:05.962242 pait-1.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     6749 1970-01-01 00:00:00.000000 pait-1.0.0a1/setup.py
--rw-r--r--   0        0        0     6165 1970-01-01 00:00:00.000000 pait-1.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2021-12-05 05:37:05.000000 pait-1.0.0a2/LICENSE
+-rw-r--r--   0        0        0     5244 2023-05-10 15:19:11.464788 pait-1.0.0a2/README.md
+-rw-r--r--   0        0        0       37 2023-05-24 03:47:38.134524 pait-1.0.0a2/pait/__init__.py
+-rw-r--r--   0        0        0       31 2023-05-28 10:07:40.409718 pait-1.0.0a2/pait/__version__.py
+-rw-r--r--   0        0        0      199 2023-05-10 15:19:11.476786 pait-1.0.0a2/pait/app/__init__.py
+-rw-r--r--   0        0        0     5528 2023-05-23 09:37:37.084528 pait-1.0.0a2/pait/app/any/__init__.py
+-rw-r--r--   0        0        0      535 2023-02-07 03:41:51.356781 pait-1.0.0a2/pait/app/any/plugin/__init__.py
+-rw-r--r--   0        0        0      460 2023-02-07 03:41:51.356781 pait-1.0.0a2/pait/app/any/plugin/auto_complete_json_resp.py
+-rw-r--r--   0        0        0      425 2023-02-07 03:41:51.356781 pait-1.0.0a2/pait/app/any/plugin/cache_response.py
+-rw-r--r--   0        0        0      405 2023-02-07 03:41:51.356781 pait-1.0.0a2/pait/app/any/plugin/check_json_resp.py
+-rw-r--r--   0        0        0      373 2023-02-07 03:41:51.356781 pait-1.0.0a2/pait/app/any/plugin/mock_response.py
+-rw-r--r--   0        0        0      424 2023-02-07 03:41:51.356781 pait-1.0.0a2/pait/app/any/plugin/unified_response.py
+-rw-r--r--   0        0        0        0 2023-01-17 11:47:59.744123 pait-1.0.0a2/pait/app/any/security/__init__.py
+-rw-r--r--   0        0        0      342 2023-02-08 03:58:49.610123 pait-1.0.0a2/pait/app/any/security/api_key.py
+-rw-r--r--   0        0        0      653 2023-02-10 15:24:31.281635 pait-1.0.0a2/pait/app/any/security/http.py
+-rw-r--r--   0        0        0      660 2023-02-08 03:43:07.655826 pait-1.0.0a2/pait/app/any/security/oauth2.py
+-rw-r--r--   0        0        0     1328 2023-01-18 19:31:20.014191 pait-1.0.0a2/pait/app/any/util.py
+-rw-r--r--   0        0        0      562 2023-02-15 10:04:32.538762 pait-1.0.0a2/pait/app/auto_load_app.py
+-rw-r--r--   0        0        0      121 2023-01-09 15:13:50.000000 pait-1.0.0a2/pait/app/base/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a2/pait/app/base/adapter/__init__.py
+-rw-r--r--   0        0        0     2427 2023-04-08 08:28:39.674480 pait-1.0.0a2/pait/app/base/adapter/request.py
+-rw-r--r--   0        0        0     1806 2023-05-10 15:19:11.476786 pait-1.0.0a2/pait/app/base/app_helper.py
+-rw-r--r--   0        0        0        0 2023-02-10 10:23:08.836059 pait-1.0.0a2/pait/app/base/security/__init__.py
+-rw-r--r--   0        0        0     1636 2023-05-24 16:45:31.309997 pait-1.0.0a2/pait/app/base/security/api_key.py
+-rw-r--r--   0        0        0      575 2023-05-24 16:53:27.735226 pait-1.0.0a2/pait/app/base/security/base.py
+-rw-r--r--   0        0        0     7130 2023-05-24 16:53:10.775208 pait-1.0.0a2/pait/app/base/security/http.py
+-rw-r--r--   0        0        0     4978 2023-05-24 16:53:10.759208 pait-1.0.0a2/pait/app/base/security/oauth2.py
+-rw-r--r--   0        0        0      794 2023-05-16 11:28:00.165083 pait-1.0.0a2/pait/app/base/security/util.py
+-rw-r--r--   0        0        0      649 2023-05-10 15:19:11.476786 pait-1.0.0a2/pait/app/base/simple_route.py
+-rw-r--r--   0        0        0    13846 2023-05-23 07:58:06.372833 pait-1.0.0a2/pait/app/base/test_helper.py
+-rw-r--r--   0        0        0      319 2023-05-10 15:19:11.476786 pait-1.0.0a2/pait/app/flask/__init__.py
+-rw-r--r--   0        0        0      719 2023-03-21 10:06:14.408062 pait-1.0.0a2/pait/app/flask/_app_helper.py
+-rw-r--r--   0        0        0      394 2023-03-21 10:06:14.408062 pait-1.0.0a2/pait/app/flask/_attribute.py
+-rw-r--r--   0        0        0      792 2023-05-10 15:19:11.476786 pait-1.0.0a2/pait/app/flask/_exception.py
+-rw-r--r--   0        0        0     3495 2023-05-10 15:19:11.476786 pait-1.0.0a2/pait/app/flask/_load_app.py
+-rw-r--r--   0        0        0      269 2022-01-10 09:58:31.000000 pait-1.0.0a2/pait/app/flask/_pait.py
+-rw-r--r--   0        0        0     1775 2023-05-10 15:19:11.476786 pait-1.0.0a2/pait/app/flask/_simple_route.py
+-rw-r--r--   0        0        0     1900 2023-05-10 15:19:11.476786 pait-1.0.0a2/pait/app/flask/_test_helper.py
+-rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a2/pait/app/flask/adapter/__init__.py
+-rw-r--r--   0        0        0     1689 2023-04-08 08:28:39.674480 pait-1.0.0a2/pait/app/flask/adapter/request.py
+-rw-r--r--   0        0        0     1070 2023-05-10 15:19:11.476786 pait-1.0.0a2/pait/app/flask/adapter/response.py
+-rw-r--r--   0        0        0      784 2023-02-07 03:41:51.356781 pait-1.0.0a2/pait/app/flask/plugin/__init__.py
+-rw-r--r--   0        0        0      117 2023-02-06 11:24:42.996357 pait-1.0.0a2/pait/app/flask/plugin/auto_complete_json_resp.py
+-rw-r--r--   0        0        0      138 2023-05-23 09:37:36.512526 pait-1.0.0a2/pait/app/flask/plugin/cache_response.py
+-rw-r--r--   0        0        0      556 2023-05-10 15:19:11.476786 pait-1.0.0a2/pait/app/flask/plugin/check_json_resp.py
+-rw-r--r--   0        0        0     1208 2023-05-23 03:11:41.942069 pait-1.0.0a2/pait/app/flask/plugin/mock_response.py
+-rw-r--r--   0        0        0      746 2023-02-07 03:41:51.356781 pait-1.0.0a2/pait/app/flask/plugin/unified_response.py
+-rw-r--r--   0        0        0        0 2023-01-09 09:37:04.000000 pait-1.0.0a2/pait/app/flask/security/__init__.py
+-rw-r--r--   0        0        0      137 2023-04-15 06:37:25.447043 pait-1.0.0a2/pait/app/flask/security/api_key.py
+-rw-r--r--   0        0        0      392 2023-04-15 06:37:25.447043 pait-1.0.0a2/pait/app/flask/security/http.py
+-rw-r--r--   0        0        0      566 2023-04-15 06:37:25.447043 pait-1.0.0a2/pait/app/flask/security/oauth2.py
+-rw-r--r--   0        0        0      321 2023-05-10 15:19:11.476786 pait-1.0.0a2/pait/app/flask/security/util.py
+-rw-r--r--   0        0        0      319 2023-05-10 15:19:11.476786 pait-1.0.0a2/pait/app/sanic/__init__.py
+-rw-r--r--   0        0        0      938 2023-03-21 10:06:14.408062 pait-1.0.0a2/pait/app/sanic/_app_helper.py
+-rw-r--r--   0        0        0      403 2023-03-21 10:06:14.412062 pait-1.0.0a2/pait/app/sanic/_attribute.py
+-rw-r--r--   0        0        0      319 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/app/sanic/_exception.py
+-rw-r--r--   0        0        0     3902 2023-05-19 10:54:00.027470 pait-1.0.0a2/pait/app/sanic/_load_app.py
+-rw-r--r--   0        0        0      374 2023-05-09 02:55:20.341357 pait-1.0.0a2/pait/app/sanic/_pait.py
+-rw-r--r--   0        0        0     1749 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/app/sanic/_simple_route.py
+-rw-r--r--   0        0        0     2172 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/app/sanic/_test_helper.py
+-rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a2/pait/app/sanic/adapter/__init__.py
+-rw-r--r--   0        0        0     2067 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/app/sanic/adapter/request.py
+-rw-r--r--   0        0        0     1102 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/app/sanic/adapter/response.py
+-rw-r--r--   0        0        0      716 2023-02-07 03:41:51.356781 pait-1.0.0a2/pait/app/sanic/plugin/__init__.py
+-rw-r--r--   0        0        0      711 2023-02-07 03:41:51.356781 pait-1.0.0a2/pait/app/sanic/plugin/auto_complete_json_resp.py
+-rw-r--r--   0        0        0      138 2023-05-23 09:37:36.508526 pait-1.0.0a2/pait/app/sanic/plugin/cache_response.py
+-rw-r--r--   0        0        0      934 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/app/sanic/plugin/check_json_resp.py
+-rw-r--r--   0        0        0     1432 2023-02-07 03:41:51.356781 pait-1.0.0a2/pait/app/sanic/plugin/mock_response.py
+-rw-r--r--   0        0        0      746 2023-02-07 03:41:51.356781 pait-1.0.0a2/pait/app/sanic/plugin/unified_response.py
+-rw-r--r--   0        0        0        0 2023-01-09 09:37:04.000000 pait-1.0.0a2/pait/app/sanic/security/__init__.py
+-rw-r--r--   0        0        0      137 2023-04-15 06:37:25.447043 pait-1.0.0a2/pait/app/sanic/security/api_key.py
+-rw-r--r--   0        0        0      392 2023-04-15 06:37:25.447043 pait-1.0.0a2/pait/app/sanic/security/http.py
+-rw-r--r--   0        0        0      566 2023-04-15 06:37:25.447043 pait-1.0.0a2/pait/app/sanic/security/oauth2.py
+-rw-r--r--   0        0        0      321 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/app/sanic/security/util.py
+-rw-r--r--   0        0        0      323 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/app/starlette/__init__.py
+-rw-r--r--   0        0        0      651 2023-03-21 10:06:14.412062 pait-1.0.0a2/pait/app/starlette/_app_helper.py
+-rw-r--r--   0        0        0      430 2023-03-21 10:06:14.412062 pait-1.0.0a2/pait/app/starlette/_attribute.py
+-rw-r--r--   0        0        0      319 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/app/starlette/_exception.py
+-rw-r--r--   0        0        0     3877 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/app/starlette/_load_app.py
+-rw-r--r--   0        0        0      291 2022-01-10 09:58:31.000000 pait-1.0.0a2/pait/app/starlette/_pait.py
+-rw-r--r--   0        0        0      996 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/app/starlette/_simple_route.py
+-rw-r--r--   0        0        0     1930 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/app/starlette/_test_helper.py
+-rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a2/pait/app/starlette/adapter/__init__.py
+-rw-r--r--   0        0        0     2718 2023-04-08 08:28:39.674480 pait-1.0.0a2/pait/app/starlette/adapter/request.py
+-rw-r--r--   0        0        0     1065 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/app/starlette/adapter/response.py
+-rw-r--r--   0        0        0      800 2023-02-07 03:41:51.356781 pait-1.0.0a2/pait/app/starlette/plugin/__init__.py
+-rw-r--r--   0        0        0      711 2023-02-07 03:41:51.356781 pait-1.0.0a2/pait/app/starlette/plugin/auto_complete_json_resp.py
+-rw-r--r--   0        0        0      138 2023-05-23 09:37:36.560526 pait-1.0.0a2/pait/app/starlette/plugin/cache_response.py
+-rw-r--r--   0        0        0      785 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/app/starlette/plugin/check_json_resp.py
+-rw-r--r--   0        0        0     1626 2023-02-16 07:49:53.639890 pait-1.0.0a2/pait/app/starlette/plugin/mock_response.py
+-rw-r--r--   0        0        0      702 2023-02-07 03:41:51.356781 pait-1.0.0a2/pait/app/starlette/plugin/unified_response.py
+-rw-r--r--   0        0        0        0 2023-01-09 09:37:04.000000 pait-1.0.0a2/pait/app/starlette/security/__init__.py
+-rw-r--r--   0        0        0      137 2023-04-15 06:37:25.447043 pait-1.0.0a2/pait/app/starlette/security/api_key.py
+-rw-r--r--   0        0        0      392 2023-04-15 06:37:25.447043 pait-1.0.0a2/pait/app/starlette/security/http.py
+-rw-r--r--   0        0        0      522 2023-04-15 06:37:25.447043 pait-1.0.0a2/pait/app/starlette/security/oauth2.py
+-rw-r--r--   0        0        0      325 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/app/starlette/security/util.py
+-rw-r--r--   0        0        0      321 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/app/tornado/__init__.py
+-rw-r--r--   0        0        0     1002 2023-03-21 10:06:14.412062 pait-1.0.0a2/pait/app/tornado/_app_helper.py
+-rw-r--r--   0        0        0      424 2023-03-21 10:06:14.412062 pait-1.0.0a2/pait/app/tornado/_attribute.py
+-rw-r--r--   0        0        0      298 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/app/tornado/_exception.py
+-rw-r--r--   0        0        0     2559 2023-05-19 10:54:00.027470 pait-1.0.0a2/pait/app/tornado/_load_app.py
+-rw-r--r--   0        0        0      291 2022-01-10 09:58:31.000000 pait-1.0.0a2/pait/app/tornado/_pait.py
+-rw-r--r--   0        0        0     2839 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/app/tornado/_simple_route.py
+-rw-r--r--   0        0        0     4664 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/app/tornado/_test_helper.py
+-rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a2/pait/app/tornado/adapter/__init__.py
+-rw-r--r--   0        0        0     2244 2023-04-08 08:28:39.674480 pait-1.0.0a2/pait/app/tornado/adapter/request.py
+-rw-r--r--   0        0        0     1130 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/app/tornado/adapter/response.py
+-rw-r--r--   0        0        0      792 2023-02-07 03:41:51.360782 pait-1.0.0a2/pait/app/tornado/plugin/__init__.py
+-rw-r--r--   0        0        0      574 2023-02-07 03:41:51.360782 pait-1.0.0a2/pait/app/tornado/plugin/auto_complete_json_resp.py
+-rw-r--r--   0        0        0     1411 2023-05-23 09:37:36.612527 pait-1.0.0a2/pait/app/tornado/plugin/cache_response.py
+-rw-r--r--   0        0        0     1211 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/app/tornado/plugin/check_json_resp.py
+-rw-r--r--   0        0        0     1237 2023-02-07 03:41:51.360782 pait-1.0.0a2/pait/app/tornado/plugin/mock_response.py
+-rw-r--r--   0        0        0     1247 2023-02-07 03:41:51.360782 pait-1.0.0a2/pait/app/tornado/plugin/unified_response.py
+-rw-r--r--   0        0        0        0 2023-02-03 19:54:29.188502 pait-1.0.0a2/pait/app/tornado/security/__init__.py
+-rw-r--r--   0        0        0      137 2023-04-15 06:37:25.447043 pait-1.0.0a2/pait/app/tornado/security/api_key.py
+-rw-r--r--   0        0        0      392 2023-04-15 06:37:25.447043 pait-1.0.0a2/pait/app/tornado/security/http.py
+-rw-r--r--   0        0        0      522 2023-04-15 06:37:25.447043 pait-1.0.0a2/pait/app/tornado/security/oauth2.py
+-rw-r--r--   0        0        0      323 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/app/tornado/security/util.py
+-rw-r--r--   0        0        0    18186 2023-05-23 08:13:27.664682 pait-1.0.0a2/pait/core.py
+-rw-r--r--   0        0        0     1645 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/data.py
+-rw-r--r--   0        0        0      688 2023-01-11 17:12:40.000000 pait-1.0.0a2/pait/exceptions.py
+-rw-r--r--   0        0        0        0 2022-04-03 14:03:33.000000 pait-1.0.0a2/pait/extra/__init__.py
+-rw-r--r--   0        0        0     7254 2023-05-19 10:54:00.027470 pait-1.0.0a2/pait/extra/config.py
+-rw-r--r--   0        0        0      729 2023-05-21 10:48:05.570392 pait-1.0.0a2/pait/extra/util.py
+-rw-r--r--   0        0        0    11023 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/field.py
+-rw-r--r--   0        0        0     1261 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/g.py
+-rw-r--r--   0        0        0      508 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/grpc/__init__.py
+-rw-r--r--   0        0        0     4623 2023-05-21 09:27:09.618683 pait-1.0.0a2/pait/grpc/base_gateway.py
+-rw-r--r--   0        0        0      511 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/grpc/desc_template.py
+-rw-r--r--   0        0        0    13491 2023-05-23 09:37:37.496529 pait-1.0.0a2/pait/grpc/gateway.py
+-rw-r--r--   0        0        0    10338 2023-05-23 08:36:43.286298 pait-1.0.0a2/pait/grpc/inspect.py
+-rw-r--r--   0        0        0        0 2023-03-24 09:24:42.276250 pait-1.0.0a2/pait/grpc/plugin/__init__.py
+-rw-r--r--   0        0        0       31 2023-03-24 09:24:42.276250 pait-1.0.0a2/pait/grpc/plugin/__main__.py
+-rw-r--r--   0        0        0     1762 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/grpc/plugin/code_gen.py
+-rw-r--r--   0        0        0     1322 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/grpc/plugin/config.py
+-rw-r--r--   0        0        0    20548 2023-05-10 15:19:11.480786 pait-1.0.0a2/pait/grpc/plugin/field_desc_proto_to_route_code.py
+-rw-r--r--   0        0        0     3248 2023-05-21 10:37:23.919357 pait-1.0.0a2/pait/grpc/plugin/gateway.py
+-rwxr-xr-x   0        0        0      266 2023-03-24 09:24:42.276250 pait-1.0.0a2/pait/grpc/plugin/main.py
+-rw-r--r--   0        0        0     1120 2023-05-10 15:19:11.484786 pait-1.0.0a2/pait/grpc/plugin/model.py
+-rw-r--r--   0        0        0        0 2023-03-24 09:24:42.276250 pait-1.0.0a2/pait/grpc/proto/__init__.py
+-rw-r--r--   0        0        0     4193 2023-05-10 15:19:11.484786 pait-1.0.0a2/pait/grpc/proto/api.proto
+-rw-r--r--   0        0        0     5030 2023-05-10 15:19:11.484786 pait-1.0.0a2/pait/grpc/proto/api_pb2.py
+-rw-r--r--   0        0        0    11716 2023-05-10 15:19:11.484786 pait-1.0.0a2/pait/grpc/proto/api_pb2.pyi
+-rw-r--r--   0        0        0      146 2023-04-11 03:13:45.778998 pait-1.0.0a2/pait/grpc/proto/api_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-04-10 09:17:38.116710 pait-1.0.0a2/pait/grpc/proto/api_pb2_grpc.pyi
+-rw-r--r--   0        0        0      436 2023-03-24 09:24:42.276250 pait-1.0.0a2/pait/grpc/types.py
+-rw-r--r--   0        0        0     5420 2023-05-23 09:37:37.100528 pait-1.0.0a2/pait/grpc/util.py
+-rw-r--r--   0        0        0      559 2023-05-10 15:19:11.484786 pait-1.0.0a2/pait/model/__init__.py
+-rw-r--r--   0        0        0     3305 2023-05-10 15:19:11.484786 pait-1.0.0a2/pait/model/config.py
+-rw-r--r--   0        0        0     1606 2023-05-10 15:19:11.484786 pait-1.0.0a2/pait/model/context.py
+-rw-r--r--   0        0        0     9443 2023-05-23 09:37:37.408529 pait-1.0.0a2/pait/model/core.py
+-rw-r--r--   0        0        0     6051 2023-05-10 15:19:11.484786 pait-1.0.0a2/pait/model/response.py
+-rw-r--r--   0        0        0      908 2023-05-28 10:00:37.748027 pait-1.0.0a2/pait/model/status.py
+-rw-r--r--   0        0        0     1400 2023-05-10 15:19:11.484786 pait-1.0.0a2/pait/model/tag.py
+-rw-r--r--   0        0        0     1166 2022-09-26 15:06:36.000000 pait-1.0.0a2/pait/model/template.py
+-rw-r--r--   0        0        0        0 2022-01-21 03:47:13.000000 pait-1.0.0a2/pait/openapi/__init__.py
+-rw-r--r--   0        0        0     9731 2023-05-19 10:54:00.027470 pait-1.0.0a2/pait/openapi/doc_route.py
+-rw-r--r--   0        0        0    12159 2023-05-28 10:02:29.009525 pait-1.0.0a2/pait/openapi/openapi.py
+-rw-r--r--   0        0        0      105 2023-02-07 03:41:51.360782 pait-1.0.0a2/pait/param_handle/__init__.py
+-rw-r--r--   0        0        0     6371 2023-05-24 16:52:04.735131 pait-1.0.0a2/pait/param_handle/_async.py
+-rw-r--r--   0        0        0     5314 2023-05-24 16:51:16.947064 pait-1.0.0a2/pait/param_handle/_sync.py
+-rw-r--r--   0        0        0    12403 2023-05-26 07:44:39.308601 pait-1.0.0a2/pait/param_handle/base.py
+-rw-r--r--   0        0        0       87 2023-02-07 03:41:51.360782 pait-1.0.0a2/pait/plugin/__init__.py
+-rw-r--r--   0        0        0     2298 2023-02-07 03:41:51.360782 pait-1.0.0a2/pait/plugin/at_most_one_of.py
+-rw-r--r--   0        0        0     2599 2023-05-10 15:19:11.484786 pait-1.0.0a2/pait/plugin/auto_complete_json_resp.py
+-rw-r--r--   0        0        0     3592 2023-05-10 15:19:11.484786 pait-1.0.0a2/pait/plugin/base.py
+-rw-r--r--   0        0        0     8867 2023-05-23 09:45:50.401974 pait-1.0.0a2/pait/plugin/cache_response.py
+-rw-r--r--   0        0        0     2228 2023-05-10 15:19:11.484786 pait-1.0.0a2/pait/plugin/check_json_resp.py
+-rw-r--r--   0        0        0     5145 2023-05-23 09:37:37.272529 pait-1.0.0a2/pait/plugin/mock_response.py
+-rw-r--r--   0        0        0     3312 2023-02-07 03:41:51.360782 pait-1.0.0a2/pait/plugin/required.py
+-rw-r--r--   0        0        0     2109 2023-05-10 15:19:11.484786 pait-1.0.0a2/pait/plugin/unified_response.py
+-rw-r--r--   0        0        0     1161 2023-02-08 11:47:07.069892 pait-1.0.0a2/pait/types.py
+-rw-r--r--   0        0        0      524 2023-02-14 09:33:41.434168 pait-1.0.0a2/pait/util/__init__.py
+-rw-r--r--   0        0        0     1970 2023-05-24 16:53:10.667208 pait-1.0.0a2/pait/util/_func_sig.py
+-rw-r--r--   0        0        0     2607 2023-01-12 10:30:13.000000 pait-1.0.0a2/pait/util/_gen_tip.py
+-rw-r--r--   0        0        0     1907 2022-04-10 08:10:06.000000 pait-1.0.0a2/pait/util/_lazy_property.py
+-rw-r--r--   0        0        0      957 2023-05-10 15:19:11.484786 pait-1.0.0a2/pait/util/_pydantic_util.py
+-rw-r--r--   0        0        0     4211 2023-05-10 15:19:11.484786 pait-1.0.0a2/pait/util/_types.py
+-rw-r--r--   0        0        0    13534 2023-05-24 06:31:18.686584 pait-1.0.0a2/pait/util/_util.py
+-rw-r--r--   0        0        0      869 2023-05-10 15:19:11.484786 pait-1.0.0a2/pait/util/encoder.py
+-rw-r--r--   0        0        0     3527 2023-05-28 10:07:40.409718 pait-1.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0     7405 1970-01-01 00:00:00.000000 pait-1.0.0a2/setup.py
+-rw-r--r--   0        0        0     6801 1970-01-01 00:00:00.000000 pait-1.0.0a2/PKG-INFO
```

### Comparing `pait-1.0.0a1/LICENSE` & `pait-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/README.md` & `pait-1.0.0a2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ![](https://cdn.jsdelivr.net/gh/so1n/so1n_blog_photo@master/blog_photo/1652600629491%E6%9C%AA%E5%91%BD%E5%90%8D.jpg)
 <p align="center">
-    <em>Python Modern API Tools, fast to code</em>
+    Pait(π tool) - <em>Python Modern API Tools, easier to use web frameworks/write API routing</em>
 </p>
 <p align="center">
     <a href="https://codecov.io/gh/so1n/pait" target="_blank">
         <img src="https://codecov.io/gh/so1n/pait/branch/master/graph/badge.svg?token=NEVM1VODHR" alt="Coverage">
     </a>
 </p>
 <p align="center">
@@ -36,59 +36,64 @@
 ---
 **Documentation**: [https://so1n.me/pait/](https://so1n.me/pait/)
 
 **中文文档**: [https://so1n.me/pait-zh-doc/](https://so1n.me/pait-zh-doc/)
 
 ---
 
+# Warning
+There are changes between the current version and the 0.8 version of the API, For more information, please refer to [1.0.0version change](https://github.com/so1n/pait/blob/master/CHANGELOG.md)
+
 # pait
 
-Pait is an api tool that can be used in any python web framework (currently only `flask`, `starlette`, `sanic`, `tornado` are supported, other frameworks will be supported once Pait is stable).
+Pait is an api tool that can be used in any python web framework, the features provided are as follows:
+ - [x] Parameter checksum automatic conversion (parameter check depends on `Pydantic`)
+ - [x] Parameter dependency verification
+ - [x] Automatically generate openapi files
+ - [x] Swagger, Redoc, Rapidoc, Elements, OpenAPI route
+ - [x] gRPC Gateway route
+ - [x] TestClient support, support response result verification
+ - [x] Support for plugin extensions, such as the Mock plugin, CheckResponse Plugin, Cache Response Plugin
+ - [ ] WebSocket support
+ - [ ] Auto API Test support
+
 
 > Note:
 >
-> mypy check 100%
->
-> test coverage 95%+ (exclude api_doc)
+> - mypy check 100%
 >
-> python version >= 3.7 (support postponed annotations)
->
-> The following code does not specify, all default to use the `starlette` framework.
+> - python version >= 3.7 (support postponed annotations)
 
-# Warning
-There are changes between the current version and the 0.8 version of the API, For more information, please refer to [0.9.0version change](https://github.com/so1n/pait/blob/master/CHANGELOG.md)
 
-# Feature
- - [x] Parameter checksum automatic conversion (parameter check depends on `Pydantic`)
- - [x] Parameter dependency verification
- - [x] Automatically generate openapi files
- - [x] Swagger, Redoc route
- - [x] gRPC Gateway route
- - [x] TestClient support, support response result verification
- - [x] Support for plugin extensions, such as the Mock plugin
 
 # Installation
 ```Bash
-pip install pait
+pip install pait --pre
+```
+If want to use the gRPC gateway feature, need to add a 'grpc' dependency:
+```bash
+pip install pait[grpc] --pre
 ```
 # Simple Example
 ```python
 from typing import Type
 import uvicorn  # type: ignore
 from starlette.applications import Starlette
 from starlette.responses import JSONResponse
 from starlette.routing import Route
 
-from pait.app.starlette import pait, add_doc_route
+from pait.app.starlette import pait
 from pait.field import Body
-from pait.model.response import PaitResponseModel
+from pait.openapi.doc_route import add_doc_route
+from pait.model.response import JsonResponseModel
 from pydantic import BaseModel, Field
 
 
-class DemoResponseModel(PaitResponseModel):
+class DemoResponseModel(JsonResponseModel):
+    """demo post api response model"""
     class ResponseModel(BaseModel):
         uid: int = Field()
         user_name: str = Field()
 
     description: str = "demo response"
     response_data: Type[BaseModel] = ResponseModel
 
@@ -101,21 +106,34 @@
     return JSONResponse({'uid': uid, 'user_name': user_name})
 
 
 app = Starlette(routes=[Route('/api', demo_post, methods=['POST'])])
 add_doc_route(app)
 uvicorn.run(app)
 ```
+See [documentation](https://so1n.me/pait/) for more features
+
+# Support Web framework
 
-# How to used in other web framework?
-If the web framework is not supported, which you are using.
+| Framework | Description            |
+|-----------|------------------------|
+| Flask     | All features supported |
+| Sanic     | All features supported |
+| Starlette | All features supported |
+| Tornado   | All features supported |
+| Django    | Coming soon            |
+
+
+If the web framework is not supported(which you are using).
 
 Can be modified sync web framework according to [pait.app.flask](https://github.com/so1n/pait/blob/master/pait/app/flask.py)
 
 Can be modified async web framework according to [pait.app.starlette](https://github.com/so1n/pait/blob/master/pait/app/starlette.py)
-# IDE Support
-While pydantic will work well with any IDE out of the box.
-- [PyCharm plugin](https://pydantic-docs.helpmanual.io/pycharm_plugin/)
-- [Mypy plugin](https://pydantic-docs.helpmanual.io/mypy_plugin/)
+
+# Performance
+For the parameter validation and transformation feature, Pait is mainly responsible for injecting the request data dependency into the `Pydantic` model, and then the `Pydanitc` verifies and transforms the data.
+
+The time consumed by this process <=0.0003 (s), for benchmarks data and subsequent optimization, see [#27](https://github.com/so1n/pait/issues/27)
+
 
 # Full example
 For more complete examples, please refer to [example](https://github.com/so1n/pait/tree/master/example)
```

### Comparing `pait-1.0.0a1/pait/app/any/__init__.py` & `pait-1.0.0a2/pait/app/any/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,24 +20,24 @@
 _NotFoundFrameworkException = RuntimeError(
     "The web framework to use cannot be found automatically, please specify it manually"
 )
 
 
 class Empty(object):
     def __int__(self) -> NoReturn:
-        raise _NotFoundFrameworkException
+        raise _NotFoundFrameworkException  # pragma: no cover
 
     def __setattr__(self, key: Any, value: Any) -> NoReturn:
-        raise _NotFoundFrameworkException
+        raise _NotFoundFrameworkException  # pragma: no cover
 
     def __getattr__(self, item: Any) -> NoReturn:
-        raise _NotFoundFrameworkException
+        raise _NotFoundFrameworkException  # pragma: no cover
 
     def __call__(self, *args: Any, **kwargs: Any) -> NoReturn:
-        raise _NotFoundFrameworkException
+        raise _NotFoundFrameworkException  # pragma: no cover
 
 
 try:
     load_class_app: Any = auto_load_app_class()
     pait_app_path: str = "pait.app." + load_class_app.__name__.lower()
     from typing import TYPE_CHECKING
```

### Comparing `pait-1.0.0a1/pait/app/any/plugin/__init__.py` & `pait-1.0.0a2/pait/app/any/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/any/security/http.py` & `pait-1.0.0a2/pait/app/any/security/http.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/any/security/oauth2.py` & `pait-1.0.0a2/pait/app/any/security/oauth2.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/any/util.py` & `pait-1.0.0a2/pait/app/any/util.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/auto_load_app.py` & `pait-1.0.0a2/pait/app/auto_load_app.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/base/adapter/request.py` & `pait-1.0.0a2/pait/app/base/adapter/request.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/base/app_helper.py` & `pait-1.0.0a2/pait/app/base/app_helper.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/base/security/api_key.py` & `pait-1.0.0a2/pait/app/base/security/api_key.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,19 +28,16 @@
 
         self.verify_api_key_callable: Optional[Callable[[str], bool]] = verify_api_key_callable
         self.model: security.ApiKeySecurityModel = security.ApiKeySecurityModel(
             name=name, in_stub=field_name  # type: ignore
         )
         self.security_name = security_name or self.__class__.__name__
 
-        def __call__(authorization: str = field) -> str:
+        def pait_handler(authorization: str = field) -> str:
             return self.authorization_handler(authorization)
 
-        self._override_call_sig(__call__)
-
-    def __call__(self, authorization: str = Header.i()) -> Optional[str]:
-        return self.authorization_handler(authorization)
+        self.set_pait_handler(pait_handler)
 
     def authorization_handler(self, authorization: str) -> str:
         if self.verify_api_key_callable and not self.verify_api_key_callable(authorization):
             raise self.not_authenticated_exc
         return authorization
```

### Comparing `pait-1.0.0a1/pait/app/base/security/base.py` & `pait-1.0.0a2/pait/app/base/security/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 from any_api.openapi import SecurityModelType
 
 
 class BaseSecurity:
     model: SecurityModelType
     security_name: str
 
-    def _override_call_sig(self, func: Callable) -> None:
-        # Compatible with the following syntax
-        # BaseSecurity()()
-        # BaseSecurity().__call__()
-        setattr(self, "_override_call_sig", True)
-        setattr(self, "__call__", func)
+    def set_pait_handler(self, func: Callable) -> None:
+        if hasattr(func, "pait_handler"):
+            raise ValueError("'func' already has pait_handler")  # pragma: no cover
+        setattr(self, "pait_handler", func)
 
     @classmethod
     def get_exception(cls, *, status_code: int, message: str, headers: Optional[Dict] = None) -> Exception:
-        return NotImplementedError()
+        return NotImplementedError()  # pragma: no cover
```

### Comparing `pait-1.0.0a1/pait/app/base/security/http.py` & `pait-1.0.0a2/pait/app/base/security/http.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,34 +35,31 @@
         :param realm: realm of http basic auth security model
         :param is_raise: is raise exception if there is invalid http basic auth data
 
         Note: If the validation fails and 'is raise' is true, only a 401 exception will be thrown,
             and if you want to throw a 403 exception, you need to handle it through inheritance or other methods
         """
         if security_model.scheme != "basic":
-            raise ValueError(f"{self.__class__.__name__} only support basic scheme")
+            raise ValueError(f"{self.__class__.__name__} only support basic scheme")  # pragma: no cover
         self.model = security_model
         self.is_raise: bool = is_raise
         self.security_name = security_name or self.__class__.__name__
         self.header_field: Header = header_field or Header.i(openapi_include=False)
         self.realm: Optional[str] = realm
         self.not_authorization_exc: Exception = self.get_exception(
             status_code=401,
             message="Not authentication",
             headers={"WWW-Authenticate": f'Basic realm="{realm}"'} if realm else {"WWW-Authenticate": "Basic"},
         )
         set_and_check_field(self.header_field, "Authorization", self.not_authorization_exc if is_raise else None)
 
-        def __call__(authorization: str = self.header_field) -> Optional[HTTPBasicCredentials]:
+        def pait_handler(authorization: str = self.header_field) -> Optional[HTTPBasicCredentials]:
             return self.authorization_handler(authorization)
 
-        self._override_call_sig(__call__)
-
-    def __call__(self, authorization: str = Header.i()) -> Optional[HTTPBasicCredentials]:
-        return self.authorization_handler(authorization)
+        self.set_pait_handler(pait_handler)
 
     def authorization_handler(self, authorization: str) -> Optional[HTTPBasicCredentials]:
         scheme, param = get_authorization_scheme_param(authorization)
         if not authorization or (scheme.lower() != "basic"):
             if self.is_raise:
                 raise self.not_authorization_exc
             else:
@@ -100,21 +97,18 @@
         self.header_field: Header = header_field or Header.i(openapi_include=False)
         self.is_raise: bool = is_raise
         self.verify_callable: Optional[Callable[[str], bool]] = verify_callable
 
         self.not_authenticated_exc: Exception = self.get_exception(status_code=403, message="Not authenticated")
         set_and_check_field(self.header_field, "Authorization", self.not_authenticated_exc if is_raise else None)
 
-        def __call__(authorization: str = self.header_field) -> Optional[str]:
+        def pait_handler(authorization: str = self.header_field) -> Optional[str]:
             return self.authorization_handler(authorization)
 
-        self._override_call_sig(__call__)
-
-    def __call__(self, authorization: str = Header.i()) -> Optional[str]:
-        return self.authorization_handler(authorization)
+        self.set_pait_handler(pait_handler)
 
     def authorization_handler(self, authorization: str) -> Optional[str]:
         scheme, credentials = get_authorization_scheme_param(authorization)
         if (not (authorization and scheme and credentials)) or (scheme.lower() != self.model.scheme):
             if self.is_raise:
                 raise self.not_authenticated_exc
             else:
```

### Comparing `pait-1.0.0a1/pait/app/base/security/oauth2.py` & `pait-1.0.0a2/pait/app/base/security/oauth2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, Callable, Dict, Generator, List, Optional, Type
 
 from any_api.openapi.model.openapi import Oauth2SecurityModel, OAuthFlowModel, OAuthFlowsModel
+from any_api.openapi.model.openapi.security import UserScopesOauth2SecurityModel
 from pydantic import BaseModel, Field
 
 from pait.field import Form, Header
 from pait.model import JsonResponseModel, PaitCoreModel, get_core_model
 
 from .base import BaseSecurity, SecurityModelType
 from .util import get_authorization_scheme_param, set_and_check_field
@@ -48,67 +49,93 @@
     class ResponseModel(BaseModel):
         access_token: str = Field(description="")
         token_type: str = Field(default="bearer")
 
     response_data: Type[BaseModel] = ResponseModel
 
 
+class BaseOAuth2PasswordBearerProxy(BaseSecurity):
+    def __init__(self, *, security: "BaseOAuth2PasswordBearer", use_scopes: Optional[List[str]] = None):
+        self.security = security
+        self.use_scopes = use_scopes
+        self.security_name = security.security_name
+
+        def pait_handler(authorization: str = security.header_field) -> str:
+            return self.authorization_handler(authorization)
+
+        self.set_pait_handler(pait_handler)
+
+    @property
+    def model(self) -> SecurityModelType:
+        if self.use_scopes:
+            return UserScopesOauth2SecurityModel(
+                use_scopes=self.use_scopes, model=self.security.model, flows=self.security.model.flows
+            )
+        return self.security.model
+
+    def is_allow(self, scopes: List[str]) -> bool:
+        return len(set(scopes) & set(self.model.get_security_scope())) > 0
+
+    def authorization_handler(self, authorization: str) -> str:
+        scheme, param = get_authorization_scheme_param(authorization)
+        if not authorization or scheme.lower() != "bearer":
+            raise self.security.not_authenticated_exc
+        return param
+
+
 class BaseOAuth2PasswordBearer(BaseSecurity):
+    _proxy = BaseOAuth2PasswordBearerProxy
+
     def __init__(
         self,
         *,
         route: Optional[Callable] = None,
         security_name: Optional[str] = None,
         scopes: Optional[Dict[str, str]] = None,
         header_field: Optional[Header] = None,
     ):
         self._model: Optional[SecurityModelType] = None
+        self._scopes: Dict[str, str] = scopes or {}
 
-        self.route: Optional[Callable] = route
+        self.route: Optional[Callable] = None
         self.security_name = security_name or self.__class__.__name__
-        self.scopes: Dict[str, str] = scopes or {}
         self.header_field: Header = header_field or Header.i(openapi_include=False)
 
         if route:
             self.with_route(route)
 
         # init field
         self.not_authenticated_exc: Exception = self.get_exception(
             status_code=401, message="Not authenticated", headers={"WWW-Authenticate": "Bearer"}
         )
         set_and_check_field(self.header_field, "Authorization", self.not_authenticated_exc)
 
-        def __call__(authorization: str = self.header_field) -> str:
-            return self.authorization_handler(authorization)
-
-        self._override_call_sig(__call__)
-
     def with_route(self, route: Callable) -> "BaseOAuth2PasswordBearer":
         if self.route is not None:
             raise ValueError("route has been set")
         self.route = route
         core_model: PaitCoreModel = get_core_model(route)
-        self._set_model(core_model.path, self.scopes)
+        self._set_model(core_model.path)
 
         def _set_model_by_core_model_change(*args: Any) -> None:
-            self._set_model(core_model.path, self.scopes)
+            self._set_model(core_model.path)
 
         core_model.add_change_notify(_set_model_by_core_model_change)
         return self
 
-    def _set_model(self, path: str, scopes: Dict[str, str]) -> None:
-        self._model = Oauth2SecurityModel(flows=OAuthFlowsModel(password=OAuthFlowModel(tokenUrl=path, scopes=scopes)))
+    def _set_model(self, path: str) -> None:
+        self._model = Oauth2SecurityModel(
+            flows=OAuthFlowsModel(password=OAuthFlowModel(tokenUrl=path, scopes=self._scopes))
+        )
 
     @property
     def model(self) -> SecurityModelType:
         if self._model is None:
             raise ValueError("The model is invalid, please use the `with_route` method to set the routing function")
         return self._model
 
-    def __call__(self, authorization: str = Header.i()) -> str:
-        return self.authorization_handler(authorization)
-
-    def authorization_handler(self, authorization: str) -> str:
-        scheme, param = get_authorization_scheme_param(authorization)
-        if not authorization or scheme.lower() != "bearer":
-            raise self.not_authenticated_exc
-        return param
+    def get_depend(self, use_scopes: Optional[List[str]] = None) -> "BaseOAuth2PasswordBearerProxy":
+        self.model  # It is only used to check whether a route is bound
+        return self._proxy(
+            security=self,
+            use_scopes=use_scopes,
+        )
```

### Comparing `pait-1.0.0a1/pait/app/base/security/util.py` & `pait-1.0.0a2/pait/app/base/security/util.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/base/simple_route.py` & `pait-1.0.0a2/pait/app/base/simple_route.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/base/test_helper.py` & `pait-1.0.0a2/pait/app/base/test_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         file_dict: Optional[dict] = None,
         form_dict: Optional[dict] = None,
         header_dict: Optional[dict] = None,
         path_dict: Optional[dict] = None,
         query_dict: Optional[dict] = None,
         strict_inspection_check_json_content: bool = True,
         find_response_model: bool = False,
+        enable_assert_response: bool = True,
         target_pait_response_class: Optional[Type["response.BaseResponseModel"]] = None,
     ):
         """
         :param client:  test client
         :param func:  route handle decorated by pait
         :param pait_dict:  pait core data
         :param body_dict:  request body param
@@ -81,14 +82,15 @@
         self.cookie_dict: Optional[dict] = cookie_dict
         self.file_dict: Optional[dict] = file_dict
         self.form_dict: Optional[dict] = form_dict
         self.header_dict: dict = header_dict or {}
         self.path_dict: Optional[dict] = path_dict
         self.query_dict: Optional[dict] = query_dict
         self.strict_inspection_check_json_content: bool = strict_inspection_check_json_content
+        self.enable_assert_response: bool = enable_assert_response
 
         # path handle
         self.path: str = self.pait_core_model.path
         if self.path_dict:
             path_list: List[str] = self.path.split("/")
             new_path_list: List[str] = []
             for sub_path in path_list:
@@ -275,17 +277,15 @@
                 message=(
                     " maybe error result: \n" f"    {error_str}\n\n" f" by response model:{real_response_model}\n"
                 ),
             )
 
         error_str = ""
         for k, v in model_check_msg_dict.items():
-            error_str += str(k)
-            error_str += ":\n"
-            error_str += "    \n".join(v)
+            error_str += str(k) + ":\n" + "    \n".join(v)
         raise CheckResponseException(
             status_code=self._get_status_code(resp),
             media_type=self._get_content_type(resp),
             headers=self._get_headers(resp),
             resp=resp,
             func=self.func,
             message=(
@@ -308,15 +308,15 @@
             if len(self.pait_core_model.method_list) == 1:
                 method = self.pait_core_model.method_list[0]
             else:
                 raise RuntimeError(
                     f"Pait Can not auto select method, please choice method in {self.pait_core_model.method_list}"
                 )
         resp: RESP_T = self._real_request(method)
-        if self.pait_core_model.response_model_list:
+        if self.pait_core_model.response_model_list and self.enable_assert_response:
             self._assert_response(resp)
         return resp
 
     def json(self, method: Optional[str] = None) -> dict:
         return self._get_json(self.request(method))
 
     def text(self, method: Optional[str] = None) -> str:
```

### Comparing `pait-1.0.0a1/pait/app/flask/_app_helper.py` & `pait-1.0.0a2/pait/app/flask/_app_helper.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/flask/_exception.py` & `pait-1.0.0a2/pait/app/flask/_exception.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/flask/_load_app.py` & `pait-1.0.0a2/pait/app/flask/_load_app.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/flask/_simple_route.py` & `pait-1.0.0a2/pait/app/flask/_simple_route.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/flask/_test_helper.py` & `pait-1.0.0a2/pait/app/flask/_test_helper.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/flask/adapter/request.py` & `pait-1.0.0a2/pait/app/flask/adapter/request.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/flask/adapter/response.py` & `pait-1.0.0a2/pait/app/flask/adapter/response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/flask/plugin/__init__.py` & `pait-1.0.0a2/pait/app/flask/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/flask/plugin/check_json_resp.py` & `pait-1.0.0a2/pait/app/flask/plugin/check_json_resp.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/flask/plugin/mock_response.py` & `pait-1.0.0a2/pait/app/flask/plugin/mock_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,11 +20,12 @@
         try:
             f.write(self.pait_response_model.get_example_value(example_column_name=self.example_column_name))
             f.seek(0)
             _, f_path, f_filename = temporary_file.name.split("/")
             return send_from_directory("/" + f_path, f_filename, mimetype=self.pait_response_model.media_type)
         finally:
             exc_type, exc_val, exc_tb = sys.exc_info()
-            temporary_file.__exit__(exc_type, exc_val, exc_tb)
+            if exc_type is None:
+                temporary_file.__exit__(None, None, None)
 
     def set_info_to_response(self, resp: Response) -> None:
         set_info_to_response(resp, self.pait_response_model)
```

### Comparing `pait-1.0.0a1/pait/app/flask/plugin/unified_response.py` & `pait-1.0.0a2/pait/app/flask/plugin/unified_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/flask/security/oauth2.py` & `pait-1.0.0a2/pait/app/flask/security/oauth2.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/sanic/_app_helper.py` & `pait-1.0.0a2/pait/app/sanic/_app_helper.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/sanic/_load_app.py` & `pait-1.0.0a2/pait/app/sanic/_load_app.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,21 +15,25 @@
 def load_app(app: Sanic, auto_load_route: bool = False) -> Dict[str, PaitCoreModel]:
     """Read data from the route that has been registered to `pait`"""
     _pait_data: Dict[str, PaitCoreModel] = {}
     for route in app.router.routes:
         route_name: str = route.name
         method_set: Set[str] = route.methods
         path: str = route.path
+        if not path.startswith("/"):
+            path = "/" + path
         openapi_path: str = path
         handler: Callable = route.handler
 
         # replace path <xxx> to {xxx}
         if "<" in openapi_path and ">" in openapi_path:
             new_path_list: list = []
             for sub_path in openapi_path.split("/"):
+                if not sub_path:
+                    continue
                 if sub_path[0] == "<" and sub_path[-1] == ">":
                     real_sub_path: str = sub_path[1:-1]
                     if ":" in real_sub_path:
                         real_sub_path = real_sub_path.split(":")[0]
                     real_sub_path = "{" + real_sub_path + "}"
                 else:
                     real_sub_path = sub_path
```

### Comparing `pait-1.0.0a1/pait/app/sanic/_simple_route.py` & `pait-1.0.0a2/pait/app/sanic/_simple_route.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/sanic/_test_helper.py` & `pait-1.0.0a2/pait/app/sanic/_test_helper.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/sanic/adapter/request.py` & `pait-1.0.0a2/pait/app/sanic/adapter/request.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/sanic/adapter/response.py` & `pait-1.0.0a2/pait/app/sanic/adapter/response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/sanic/plugin/__init__.py` & `pait-1.0.0a2/pait/app/sanic/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/sanic/plugin/auto_complete_json_resp.py` & `pait-1.0.0a2/pait/app/sanic/plugin/auto_complete_json_resp.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/sanic/plugin/check_json_resp.py` & `pait-1.0.0a2/pait/app/sanic/plugin/check_json_resp.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/sanic/plugin/mock_response.py` & `pait-1.0.0a2/pait/app/sanic/plugin/mock_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/sanic/plugin/unified_response.py` & `pait-1.0.0a2/pait/app/sanic/plugin/unified_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/sanic/security/oauth2.py` & `pait-1.0.0a2/pait/app/sanic/security/oauth2.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/starlette/_app_helper.py` & `pait-1.0.0a2/pait/app/starlette/_app_helper.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/starlette/_load_app.py` & `pait-1.0.0a2/pait/app/starlette/_load_app.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/starlette/_simple_route.py` & `pait-1.0.0a2/pait/app/starlette/_simple_route.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/starlette/_test_helper.py` & `pait-1.0.0a2/pait/app/starlette/_test_helper.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/starlette/adapter/request.py` & `pait-1.0.0a2/pait/app/starlette/adapter/request.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/starlette/adapter/response.py` & `pait-1.0.0a2/pait/app/starlette/adapter/response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/starlette/plugin/__init__.py` & `pait-1.0.0a2/pait/app/starlette/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/starlette/plugin/auto_complete_json_resp.py` & `pait-1.0.0a2/pait/app/starlette/plugin/auto_complete_json_resp.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/starlette/plugin/check_json_resp.py` & `pait-1.0.0a2/pait/app/starlette/plugin/check_json_resp.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/starlette/plugin/mock_response.py` & `pait-1.0.0a2/pait/app/starlette/plugin/mock_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/starlette/plugin/unified_response.py` & `pait-1.0.0a2/pait/app/starlette/plugin/unified_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/starlette/security/oauth2.py` & `pait-1.0.0a2/pait/app/starlette/security/oauth2.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/tornado/_app_helper.py` & `pait-1.0.0a2/pait/app/tornado/_app_helper.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/tornado/_load_app.py` & `pait-1.0.0a2/pait/app/tornado/_load_app.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 
 def load_app(app: Application, auto_load_route: bool = False) -> Dict[str, PaitCoreModel]:
     """Read data from the route that has been registered to `pait`"""
     _pait_data: Dict[str, PaitCoreModel] = {}
     for rule in app.wildcard_router.rules:
         path: str = rule.matcher.regex.pattern  # type: ignore
+        if path.endswith("$"):
+            path = path[:-1]
         openapi_path: str = path
         # replace path regex to {xxx}
         if "<" in openapi_path and ">" in openapi_path:
             new_path_list: list = []
             for sub_path in openapi_path.split("/"):
                 if not sub_path:
                     continue
```

### Comparing `pait-1.0.0a1/pait/app/tornado/_simple_route.py` & `pait-1.0.0a2/pait/app/tornado/_simple_route.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/tornado/_test_helper.py` & `pait-1.0.0a2/pait/app/tornado/_test_helper.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/tornado/adapter/request.py` & `pait-1.0.0a2/pait/app/tornado/adapter/request.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/tornado/adapter/response.py` & `pait-1.0.0a2/pait/app/tornado/adapter/response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/tornado/plugin/__init__.py` & `pait-1.0.0a2/pait/app/tornado/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/tornado/plugin/auto_complete_json_resp.py` & `pait-1.0.0a2/pait/app/tornado/plugin/auto_complete_json_resp.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/tornado/plugin/cache_response.py` & `pait-1.0.0a2/pait/app/tornado/plugin/cache_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Any, Dict, Tuple
 
 from tornado.web import RequestHandler
 
+from pait.plugin.cache_response import CacheRespExtraParam
 from pait.plugin.cache_response import CacheResponsePlugin as _CacheResponsePlugin
 
-__all__ = ["CacheResponsePlugin"]
+__all__ = ["CacheResponsePlugin", "CacheRespExtraParam"]
 
 
 class CacheResponsePlugin(_CacheResponsePlugin):
     def _gen_key(self, *args: Any, **kwargs: Any) -> Tuple[str, str]:
         return super()._gen_key(*args[1:], **kwargs)
 
     def _dumps(self, response: Any, *args: Any, **kwargs: Any) -> Any:
```

### Comparing `pait-1.0.0a1/pait/app/tornado/plugin/check_json_resp.py` & `pait-1.0.0a2/pait/app/tornado/plugin/check_json_resp.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/tornado/plugin/mock_response.py` & `pait-1.0.0a2/pait/app/tornado/plugin/mock_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/tornado/plugin/unified_response.py` & `pait-1.0.0a2/pait/app/tornado/plugin/unified_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/app/tornado/security/oauth2.py` & `pait-1.0.0a2/pait/app/tornado/security/oauth2.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/core.py` & `pait-1.0.0a2/pait/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     def _append_data(
         key: str,
         target_container: Optional[_AppendT],
         append_container: Optional[_AppendT],
         self_container: Optional[_AppendT],
     ) -> Optional[_AppendT]:
         if target_container and append_container:
-            raise KeyError(f"{key} and append_{key} cannot be used together")
+            raise KeyError(f"{key} and append_{key} cannot be used together")  # pragma: no cover
         if append_container:
             return (self_container or append_container.__class__()) + append_container
         elif target_container is None:
             return self_container
         else:
             return target_container
 
@@ -278,20 +278,14 @@
             the default is pait.param_handler.x
         :param feature_code: Specify the prefix of the pait id corresponding to the generated routing function.
             Usually, the pait_id is equal to md5(func), but during dynamic generation,
             there may be multiple different routing functions generated by the same func.
             In this case, different feature_code is needed to generate different pait_id(feature_code + md5(func))
         """
         app_name: str = self.app_helper_class.app_name
-        pydantic_model_config = pydantic_model_config or self._pydantic_model_config
-        pydantic_basemodel = pydantic_basemodel or self._pydantic_basemodel
-        desc = desc or self._desc
-        summary = summary or self._summary
-        name = name or self._name
-        group = group or self._group
 
         pre_depend_list = self._append_data(
             "pre_depend_list", pre_depend_list, append_pre_depend_list, self._pre_depend_list
         )
         author = self._append_data("author", author, append_author, self._author)
         tag = self._append_data("tag", tag, append_tag, self._tag)
         response_model_list = self._append_data(
@@ -314,24 +308,24 @@
                 else:
                     _param_handler_plugin = self.param_handler_plugin_class
             # gen pait core model and register to pait data
             pait_core_model: PaitCoreModel = PaitCoreModel(
                 func,
                 self.app_helper_class,
                 author=author,
-                desc=desc,
-                summary=summary,
-                func_name=name,
-                status=status,
-                group=group,
+                desc=desc or self._desc,
+                summary=summary or self._summary,
+                func_name=name or self._name,
+                status=status or self._status,
+                group=group or self._group,
                 tag=tag,
                 response_model_list=response_model_list,
                 pre_depend_list=pre_depend_list,
-                pydantic_model_config=pydantic_model_config,
-                pydantic_basemodel=pydantic_basemodel,
+                pydantic_model_config=pydantic_model_config or self._pydantic_model_config,
+                pydantic_basemodel=pydantic_basemodel or self._pydantic_basemodel,
                 plugin_list=plugin_list,
                 post_plugin_list=post_plugin_list,
                 param_handler_plugin=_param_handler_plugin,
                 feature_code=feature_code,
                 default_field_class=default_field_class or self._default_field_class,
                 **(kwargs or self.extra),
             )
```

### Comparing `pait-1.0.0a1/pait/data.py` & `pait-1.0.0a2/pait/data.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/exceptions.py` & `pait-1.0.0a2/pait/exceptions.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/extra/config.py` & `pait-1.0.0a2/pait/extra/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,17 +117,14 @@
 
 def apply_response_model(
     response_model_list: List[Type[BaseResponseModel]], match_rule: Optional["MatchRule"] = None
 ) -> "APPLY_FN":
     """
     Add a default response structure for routing handles
     """
-    for response_model in response_model_list:
-        if response_model.is_core:
-            raise ValueError(f"{response_model} is core response model can not set to default_response_model_list")
 
     def _apply(pait_core_model: "PaitCoreModel") -> None:
         if _is_match(pait_core_model, match_rule):
             pait_core_model.add_response_model_list(response_model_list)
 
     return _apply
```

### Comparing `pait-1.0.0a1/pait/field.py` & `pait-1.0.0a2/pait/field.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/g.py` & `pait-1.0.0a2/pait/g.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/grpc/base_gateway.py` & `pait-1.0.0a2/pait/grpc/base_gateway.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/grpc/gateway.py` & `pait-1.0.0a2/pait/grpc/gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 __all__ = ["DynamicGrpcGatewayRoute", "AsyncGrpcGatewayRoute", "GrpcGatewayRoute"]
 
 
 def _gen_response_model_handle(grpc_model: GrpcModel) -> Type[BaseResponseModel]:
     if grpc_model.response is Empty:
         response_model: Any = dict
-    elif grpc_model.grpc_service_option_model.response_message:
+    elif grpc_model.grpc_service_option_model.response_message.has_value():
         response_model = rebuild_message_type(
             msg_to_pydantic_model(grpc_model.response),
             grpc_model.invoke_name,
             exclude_column_name=grpc_model.grpc_service_option_model.response_message.exclude_column_name,
             nested=grpc_model.grpc_service_option_model.response_message.nested,
         )
     else:
@@ -107,25 +107,25 @@
         """
         http_method: str = grpc_model.grpc_service_option_model.http_method
         if http_method == "GET":
             default_field: Type[BaseField] = Query
         elif http_method == "POST":
             default_field = Body
         else:
-            raise RuntimeError(f"{http_method} is not supported")
+            raise RuntimeError(f"{http_method} is not supported")  # pragma: no cover
         request_model: Type[BaseModel] = msg_to_pydantic_model(
             grpc_model.request,
             default_field=default_field,
             comment_prefix="pait",
             desc_template=self.desc_template,
             parse_msg_desc_method=getattr(grpc_model.request, "_message_module")
             if self._parse_msg_desc == "by_mypy"
             else self._parse_msg_desc,
         )
-        if grpc_model.grpc_service_option_model.request_message:
+        if grpc_model.grpc_service_option_model.request_message.has_value():
             return rebuild_message_type(
                 request_model,
                 grpc_model.invoke_name,
                 exclude_column_name=grpc_model.grpc_service_option_model.request_message.exclude_column_name,
                 nested=grpc_model.grpc_service_option_model.request_message.nested,
             )
         else:
@@ -158,15 +158,15 @@
             response_model_list=response_model_list,
         )
 
     def get_grpc_func(self, grpc_model: GrpcModel) -> Callable:
         """Get grpc invoke func"""
         func: Optional[Callable] = self.grpc_method_url_func_dict.get(grpc_model.grpc_method_url, None)
         if not func:
-            raise RuntimeError(
+            raise RuntimeError(  # pragma: no cover
                 f"{grpc_model.grpc_method_url}'s func is not found, Please call init_channel to register the channel"
             )
         return func
 
     def gen_route(self, grpc_model: GrpcModel, request_pydantic_model_class: Type) -> Callable:
         """Generate the routing function corresponding to grpc invoke fun"""
         raise NotImplementedError()
@@ -254,15 +254,15 @@
             request_msg: Message = self.msg_from_dict_handle(
                 grpc_model.request,
                 request_pydantic_model.dict(),  # type: ignore
                 grpc_model.grpc_service_option_model.request_message.nested,
             )
             loop: asyncio.AbstractEventLoop = asyncio.get_event_loop()
             if loop != func._loop:  # type: ignore
-                raise RuntimeError(
+                raise RuntimeError(  # pragma: no cover
                     "Loop is not same, "
                     "the grpc channel must be initialized after the event loop of the api server is initialized"
                 )
             else:
                 grpc_msg: Message = await func(request_msg)
             return self.msg_to_dict_handle(
                 grpc_msg,
```

### Comparing `pait-1.0.0a1/pait/grpc/inspect.py` & `pait-1.0.0a2/pait/grpc/inspect.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 ]
 
 
 class BuildMessageModel(BaseModel):
     exclude_column_name: list = Field(default_factory=list)
     nested: list = Field(default_factory=list)
 
+    def has_value(self) -> bool:
+        return bool(self.exclude_column_name) or bool(self.nested)
+
     @validator("exclude_column_name", pre=True)
     def exclude_column_name_validator(cls, v: Union[str, list]) -> list:
         if isinstance(v, str):
             return [i for i in v.split(",") if i]
         return v
 
     @validator("nested", pre=True)
```

### Comparing `pait-1.0.0a1/pait/grpc/plugin/code_gen.py` & `pait-1.0.0a2/pait/grpc/plugin/code_gen.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/grpc/plugin/config.py` & `pait-1.0.0a2/pait/grpc/plugin/config.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/grpc/plugin/field_desc_proto_to_route_code.py` & `pait-1.0.0a2/pait/grpc/plugin/field_desc_proto_to_route_code.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/grpc/plugin/gateway.py` & `pait-1.0.0a2/pait/grpc/plugin/gateway.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/grpc/plugin/model.py` & `pait-1.0.0a2/pait/grpc/plugin/model.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/grpc/proto/api.proto` & `pait-1.0.0a2/pait/grpc/proto/api.proto`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/grpc/proto/api_pb2.py` & `pait-1.0.0a2/pait/grpc/proto/api_pb2.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/grpc/proto/api_pb2.pyi` & `pait-1.0.0a2/pait/grpc/proto/api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/grpc/util.py` & `pait-1.0.0a2/pait/grpc/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     exclude_column_name: Optional[list] = None,
     nested: Optional[list] = None,
 ) -> Type:
     if not exclude_column_name and not nested:
         return raw_type
     if exclude_column_name:
         if not issubclass(raw_type, BaseModel):
-            pass
+            raise TypeError("The value must be Base Model")
         raw_pydantic_model: Type[BaseModel] = raw_type
         annotation_dict: Dict[str, Tuple[Type, Any]] = {}
         pydantic_validators: Dict[str, classmethod] = {}
         for column_name, model_field in raw_pydantic_model.__fields__.items():
             if column_name in exclude_column_name:
                 continue
             annotation_dict[column_name] = (model_field.type_, model_field.field_info)
@@ -36,38 +36,46 @@
             pydantic_base=raw_pydantic_model.__base__,  # type: ignore
             pydantic_module=raw_pydantic_model.__module__,
         )
     elif nested:
         for index, column in enumerate(nested):
             if column == "$[]":
                 if not isinstance(raw_type, _GenericAlias) and not getattr(raw_type, "_name", "") == "List":
-                    raise ValueError(f"Parse `{column}({nested})` is error: {raw_type} is not a List. ")
+                    raise ValueError(  # pragma: no cover
+                        f"Parse `{column}({nested})` is error: {raw_type} is not a List. "
+                    )
                 raw_type = List[  # type: ignore[misc,index]
                     rebuild_message_type(raw_type.__args__[0], route_func_name, nested=nested[1 + index :])
                 ]
                 break
             elif column == "${}":
                 if not isinstance(raw_type, _GenericAlias) and not getattr(raw_type, "_name", "") == "Dict":
-                    raise ValueError(f"Parse `{column}({nested})` is error: {raw_type} is not a Dict. ")
+                    raise ValueError(  # pragma: no cover
+                        f"Parse `{column}({nested})` is error: {raw_type} is not a Dict. "
+                    )
                 raw_type = Dict[  # type: ignore[misc,index]
                     raw_type.__args__[0],  # type: ignore[name-defined]
                     rebuild_message_type(raw_type.__args__[1], route_func_name, nested=nested[1 + index :]),
                 ]
                 break
             elif column.startswith("$."):
                 if not issubclass(raw_type, BaseModel):
-                    raise ValueError(f"Parse `{column}({nested})` is error: {raw_type} is not a pydantic.BaseModel. ")
+                    raise ValueError(  # pragma: no cover
+                        f"Parse `{column}({nested})` is error: {raw_type} is not a pydantic.BaseModel. "
+                    )
                 key = column[2:]
                 raw_type.__fields__[key].outer_type_ = rebuild_message_type(
                     raw_type.__fields__[key].outer_type_, route_func_name, nested=nested[1 + index :]
                 )
                 break
             else:
                 if not issubclass(raw_type, BaseModel):
-                    raise ValueError(f"Parse `{column}({nested})` is error: {raw_type} is not a pydantic.BaseModel. ")
+                    raise ValueError(  # pragma: no cover
+                        f"Parse `{column}({nested})` is error: {raw_type} is not a pydantic.BaseModel. "
+                    )
                 raw_type = raw_type.__fields__[column].outer_type_
             if not (inspect.isclass(raw_type) and issubclass(raw_type, BaseModel)):
                 continue
     return raw_type
 
 
 def rebuild_dict(
@@ -79,24 +87,30 @@
         return raw_dict
     if exclude_column_name:
         raw_dict = {k: v for k, v in raw_dict.items() if k not in exclude_column_name}
     elif nested:
         for index, column in enumerate(nested):
             if column == "$[]":
                 if not isinstance(raw_dict, list):
-                    raise ValueError(f"Parse `{column}({nested})` is error: {raw_dict} is not a list. ")
+                    raise ValueError(  # pragma: no cover
+                        f"Parse `{column}({nested})` is error: {raw_dict} is not a list. "
+                    )
                 raw_dict = [rebuild_dict(item, nested=nested[index + 1 :]) for item in raw_dict]
                 break
             elif column == "${}":
                 if not isinstance(raw_dict, dict):
-                    raise ValueError(f"Parse `{column}({nested})` is error: {raw_dict} is not a dict. ")
+                    raise ValueError(  # pragma: no cover
+                        f"Parse `{column}({nested})` is error: {raw_dict} is not a dict. "
+                    )
                 raw_dict = {k: rebuild_dict(v, nested=nested[index + 1 :]) for k, v in raw_dict.items()}
                 break
             elif column.startswith("$."):
                 if not isinstance(raw_dict, dict):
-                    raise ValueError(f"Parse `{column}({nested})` is error: {raw_dict} is not a dict. ")
+                    raise ValueError(  # pragma: no cover
+                        f"Parse `{column}({nested})` is error: {raw_dict} is not a dict. "
+                    )
                 key = column[2:]
                 raw_dict[key] = rebuild_dict(raw_dict[key], nested=nested[index + 1 :])
                 break
             else:
                 raw_dict = raw_dict[column]
     return raw_dict
```

### Comparing `pait-1.0.0a1/pait/model/__init__.py` & `pait-1.0.0a2/pait/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/model/config.py` & `pait-1.0.0a2/pait/model/config.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/model/context.py` & `pait-1.0.0a2/pait/model/context.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/model/core.py` & `pait-1.0.0a2/pait/model/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,25 +57,26 @@
         feature_code: str = "",
         **kwargs: Any,
     ):
         # pait
         self.app_helper_class: "Type[BaseAppHelper]" = app_helper_class
         self.default_field_class: Optional[Type["BaseField"]] = default_field_class
         self.func: Callable = func  # route func
-        # self.qualname: str = func.__qualname__.split(".<locals>", 1)[0].rsplit(".", 1)[0]
-        self.pait_id: str = f"{func.__qualname__}_{self.func_md5}"
+        self.pait_id: str = f"{func.__module__}_{func.__qualname__}"
         # Some functions have the same md5 as the name and need to be distinguished by the feature code
         if feature_code:
             self.pait_id = f"{feature_code}_{self.pait_id}"
         setattr(func, "_pait_id", self.pait_id)
         setattr(func, "pait_core_model", self)
         self.pre_depend_list: List[Callable] = pre_depend_list or []
         self.func_path: str = ""
         self.block_http_method_set: Set[str] = set()
+        # TODO
         self.pydantic_model_config: Optional[Type[BaseConfig]] = pydantic_model_config
+        # TODO
         self.pydantic_basemodel: Optional[Type[BaseModel]] = pydantic_basemodel
         self.extra: dict = kwargs
 
         # api doc
         self.path: str = path or ""  # request url path
         self.openapi_path: str = openapi_path or ""
         self._method_list: List[str] = sorted(list(method_set or set()))  # request method set
@@ -130,22 +131,14 @@
                 self._param_handler_plugin.pre_check_hook(self)
             self._param_handler_plugin.pre_load_hook(self)
         except Exception as e:
             raise gen_tip_exc(self.func, RuntimeError(f"set param plugin error: {e}")) from e
         self.add_plugin([], [])
 
     @property
-    def func_md5(self) -> str:
-        from hashlib import md5
-
-        h = md5()
-        h.update(self.func.__code__.co_code)  # type: ignore
-        return h.hexdigest()
-
-    @property
     def method_list(self) -> List[str]:
         _temp_set: Set[str] = set(self._method_list.copy())
         _temp_set.difference_update(self.block_http_method_set)
         return sorted(list(_temp_set))
 
     @method_list.setter
     def method_list(self, method_list: List[str]) -> None:
@@ -160,15 +153,15 @@
         return self._response_model_list
 
     def add_response_model_list(self, response_model_list: List[Type[BaseResponseModel]]) -> None:
         for response_model in response_model_list:
             if response_model in self._response_model_list:
                 continue
             if issubclass(response_model, PaitResponseModel):
-                logging.warning(
+                logging.warning(  # pragma: no cover
                     f"Please replace {self.operation_id}'s response model {response_model}" f" with {BaseResponseModel}"
                 )
             self._response_model_list.append(response_model)
 
     @property
     def extra_openapi_model_list(self) -> List[Type[BaseModel]]:
         return self._extra_openapi_model_list
```

### Comparing `pait-1.0.0a1/pait/model/response.py` & `pait-1.0.0a2/pait/model/response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/model/tag.py` & `pait-1.0.0a2/pait/model/tag.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/model/template.py` & `pait-1.0.0a2/pait/model/template.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/openapi/doc_route.py` & `pait-1.0.0a2/pait/openapi/doc_route.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pydantic import BaseModel, Field
 
 from pait.app.any.util import import_func_from_app
 from pait.app.base.simple_route import SimpleRoute
 from pait.core import Pait
 from pait.field import Depends, Path, Query
 from pait.g import config, pait_context
-from pait.model import HtmlResponseModel, JsonResponseModel, PaitCoreModel, PaitStatus, Tag, TemplateContext
+from pait.model import HtmlResponseModel, JsonResponseModel, PaitStatus, Tag, TemplateContext
 from pait.openapi.openapi import InfoModel, OpenAPI, ServerModel
 
 logger: logging.Logger = logging.getLogger(__name__)
 __all__ = [
     "DocHtmlRespModel",
     "OpenAPIRespModel",
     "AddDocRoute",
@@ -51,30 +51,28 @@
 class DocEnum(str, Enum):
     pass
 
 
 class AddDocRoute(object):
     not_found_exc: Exception
     pait: Pait
-    load_app: staticmethod
     add_multi_simple_route: staticmethod
 
     def __init__(
         self,
         app: Any,
         scheme: Optional[str] = None,
         openapi_json_url_only_path: bool = False,
         prefix: str = "",
         pin_code: str = "",
         title: str = "",
         doc_fn_dict: Optional[Dict[str, Callable]] = None,
         openapi: Optional[Type[OpenAPI]] = None,
         pait: Optional[Pait] = None,
         add_multi_simple_route: Optional[Callable] = None,
-        load_app: Optional[Callable] = None,
         not_found_exc: Optional[Exception] = None,
     ):
         """
         :param app: The app instance to which the doc route is bound
         :param scheme: The scheme of the specified url, if the value is empty,
             it will be automatically selected according to the request
 
@@ -91,15 +89,14 @@
                 pin_code: 6666, url `http://127.0.0.1:8080/api/path?pin-code=6666`
         :param title: Doc route group name,
             the title of multiple doc routes registered for the same app instance must be different
         :param openapi: OpenAPI class
         :param doc_fn_dict: doc ui dict, default `pait.app.base.doc_route.default_doc_fn_dict`
         :param pait: instance of pait
         :param add_multi_simple_route: add_multi_simple_route
-        :param load_app: load_app
         :param not_found_exc:  not_found_exc
         """
         if pin_code:
             logging.info(f"doc route start pin code:{pin_code}")
         self.scheme: Optional[str] = scheme
         self.openapi_json_url_only_path: bool = openapi_json_url_only_path
         self.prefix: str = prefix or "/"
@@ -117,15 +114,14 @@
             group="pait_doc",
         )
         self._add_multi_simple_route = (
             add_multi_simple_route
             or getattr(self, "add_multi_simple_route", None)
             or import_func_from_app("add_multi_simple_route", app=app)
         )
-        self._load_app = load_app or getattr(self, "load_app", None) or import_func_from_app("load_app", app=app)
         self._not_found_exc = (
             not_found_exc
             or getattr(self, "not_found_exc", None)
             or import_func_from_app("http_exception", app=app)(status_code=404, message="Not Found")
         )
         self._gen_route(app)
 
@@ -213,18 +209,17 @@
             feature_code=self.title,
         )
         def _openapi_route(
             url_dict: Dict[str, Any] = Depends.i(self._get_request_template_map(extra_key=True)),
         ) -> dict:
             re = pait_context.get().app_helper.request.request_extend()
             _scheme: str = self.scheme or re.scheme
-            pait_dict: Dict[str, PaitCoreModel] = self._load_app(app)
             with TemplateContext(url_dict):
                 pait_openapi: OpenAPI = OpenAPI(
-                    pait_dict,
+                    app,
                     openapi_info_model=InfoModel(title=self.title),
                     server_model_list=[ServerModel(url=f"{_scheme}://{re.hostname}")],
                 )
                 return json.loads(pait_openapi.content())
 
         return _openapi_route
 
@@ -236,24 +231,22 @@
     prefix: str = "",
     pin_code: str = "",
     title: str = "",
     doc_fn_dict: Optional[Dict[str, Callable]] = None,
     openapi: Optional[Type[OpenAPI]] = None,
     pait: Optional[Pait] = None,
     add_multi_simple_route: Optional[Callable] = None,
-    load_app: Optional[Callable] = None,
     not_found_exc: Optional[Exception] = None,
 ) -> None:
     AddDocRoute(
         scheme=scheme,
         openapi_json_url_only_path=openapi_json_url_only_path,
         prefix=prefix,
         pin_code=pin_code,
         title=title,
         app=app,
         openapi=openapi,
         doc_fn_dict=doc_fn_dict,
         pait=pait,
         add_multi_simple_route=add_multi_simple_route,
-        load_app=load_app,
         not_found_exc=not_found_exc,
     )
```

### Comparing `pait-1.0.0a1/pait/openapi/openapi.py` & `pait-1.0.0a2/pait/openapi/openapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 from any_api.openapi import SecurityModelType, ServerModel, TagModel, openapi_model
 from any_api.openapi.model.links import LinksModel
 from any_api.openapi.model.openapi import OpenAPIModel
 from any_api.openapi.model.requests import RequestModel
 from pydantic import BaseModel, Field
 from pydantic.fields import FieldInfo, Undefined
 
+from pait.app import load_app
 from pait.field import BaseField, Depends
 from pait.g import config
 from pait.model.core import PaitCoreModel
-from pait.model.status import PaitStatus
 from pait.types import CallType
 from pait.util import FuncSig, create_pydantic_model, get_func_sig, get_parameter_list_from_class
 
 HttpParamTypeDictType = Dict[HttpParamTypeLiteral, List[RequestModel]]
 
 
 __all__ = ["LinksModel", "ApiModel", "ParsePaitModel", "OpenAPI"]
@@ -34,33 +34,33 @@
 
     def add_to_operation_model(self, _openapi_model: openapi_model.OperationModel) -> None:
         # Not an openapi standard parameter
         _openapi_model.pait_info = {
             "group": self.pait_core_model.group,
             "status": self.pait_core_model.status.value,
             "author": self.pait_core_model.author,
-            "md5": self.pait_core_model.func_md5,
+            "pait_id": self.pait_core_model.pait_id,
         }
 
 
 class ParsePaitModel(object):
     def __init__(self, pait_model: PaitCoreModel) -> None:
         self.pait_model: PaitCoreModel = pait_model
         self.http_param_type_dict: HttpParamTypeDictType = {}
         self.security_dict: Dict[str, openapi_model.security.SecurityModelType] = {}
         self.http_param_type_alias_dict: Dict[str, HttpParamTypeLiteral] = {"multiquery": "query"}
 
         self.param_field_dict: Dict[str, BaseField] = {}
         self.http_param_type_annotation_dict: Dict[HttpParamTypeLiteral, Dict[str, Tuple[Type, FieldInfo]]] = {}
 
-        self._parse_call_type(pait_model.func)
-        for pre_depend in pait_model.pre_depend_list:
-            self._parse_call_type(pre_depend)
         for extra_openapi_model in self.pait_model.extra_openapi_model_list:
             self._parse_base_model(extra_openapi_model)
+        for pre_depend in pait_model.pre_depend_list:
+            self._parse_call_type(pre_depend)
+        self._parse_call_type(pait_model.func)
 
         for http_param_type, annotation_dict in self.http_param_type_annotation_dict.items():
             http_param_type = self.http_param_type_alias_dict.get(http_param_type, http_param_type)
             if http_param_type not in self.http_param_type_dict:
                 self.http_param_type_dict[http_param_type] = []
             self.http_param_type_dict[http_param_type].append(
                 RequestModel(
@@ -195,15 +195,15 @@
             )
             self._parse_base_model(_pydantic_model)
 
 
 class OpenAPI(object):
     def __init__(
         self,
-        pait_dict: Dict[str, PaitCoreModel],
+        app: Any,
         undefined: Any = Undefined,
         openapi_info_model: Optional[InfoModel] = None,
         server_model_list: Optional[List[ServerModel]] = None,
         tag_model_list: Optional[List[TagModel]] = None,
         external_docs: Optional[ExternalDocumentationModel] = None,
         security_dict: Optional[Dict[str, SecurityModelType]] = None,
     ):
@@ -211,35 +211,30 @@
         self._openapi: _OpenAPI = _OpenAPI(
             openapi_info_model=openapi_info_model,
             server_model_list=server_model_list,
             tag_model_list=tag_model_list,
             external_docs=external_docs,
             security_dict=security_dict,
         )
+        self._pait_dict: Dict[str, PaitCoreModel] = load_app(app)
         api_model_list: List[ApiModel] = []
-        for pait_id, pait_model in pait_dict.items():
+        for pait_id, pait_model in self._pait_dict.items():
             try:
                 parse_pait_model: ParsePaitModel = ParsePaitModel(pait_model)
                 api_model_list.append(
                     ApiModel(
                         path=pait_model.openapi_path,
                         http_method_list=pait_model.openapi_method_list,
                         tags=[i.to_tag_model() for i in pait_model.tag],
                         operation_id=pait_model.operation_id,
                         summary=pait_model.summary,
                         request_dict=parse_pait_model.http_param_type_dict,
                         response_list=pait_model.response_model_list,
                         description=pait_model.desc,
-                        deprecated=pait_model.status
-                        in (
-                            PaitStatus.abnormal,
-                            PaitStatus.maintenance,
-                            PaitStatus.archive,
-                            PaitStatus.abandoned,
-                        ),
+                        deprecated=pait_model.status.is_deprecated(),
                         pait_core_model=pait_model,
                         security=parse_pait_model.security_dict,
                     )
                 )
             except Exception as e:
                 logging.error(f"parse pait model error by func: {pait_model.func_path}/{pait_model.func_name}")
                 raise e
```

### Comparing `pait-1.0.0a1/pait/param_handle/_async.py` & `pait-1.0.0a2/pait/param_handle/_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         class_: Optional[type] = getattr(func, "__class__", None)
         if class_ and not inspect.isfunction(func):
             _, kwargs = await self.param_handle(context, func.__class__, get_parameter_list_from_class(func.__class__))
             func.__dict__.update(kwargs)
 
         func_sig: FuncSig = get_func_sig(func)
         _func_args, _func_kwargs = await self.param_handle(context, func_sig, func_sig.param_list)
-        func_result: Any = func(*_func_args, **_func_kwargs)
+        func_result: Any = func_sig.func(*_func_args, **_func_kwargs)
         if asyncio.iscoroutine(func_result):
             func_result = await func_result
         if isinstance(func_result, AbstractAsyncContextManager):
             context.contextmanager_list.append(func_result)
             return await func_result.__aenter__()
         elif isinstance(func_result, AbstractContextManager):
             context.contextmanager_list.append(func_result)
```

### Comparing `pait-1.0.0a1/pait/param_handle/_sync.py` & `pait-1.0.0a2/pait/param_handle/_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         class_: Optional[type] = getattr(func, "__class__", None)
         if class_ and not inspect.isfunction(func):
             _, kwargs = self.param_handle(context, func.__class__, get_parameter_list_from_class(func.__class__))
             func.__dict__.update(kwargs)
 
         func_sig: FuncSig = get_func_sig(func)
         _func_args, _func_kwargs = self.param_handle(context, func_sig, func_sig.param_list)
-        func_result: Any = func(*_func_args, **_func_kwargs)
+        func_result: Any = func_sig.func(*_func_args, **_func_kwargs)
         if isinstance(func_result, AbstractContextManager):
             context.contextmanager_list.append(func_result)
             return func_result.__enter__()
         else:
             return func_result
 
     def _gen_param(self, context: "ParamHandleContext") -> None:
```

### Comparing `pait-1.0.0a1/pait/param_handle/base.py` & `pait-1.0.0a2/pait/param_handle/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,16 @@
         func_sig: FuncSig = get_func_sig(func)  # get and cache func sig
         cls.check_param_field_handle(pait_core_model, func_sig, func_sig.param_list)
 
     @staticmethod
     def check_field_type(value: Any, target_type: Any, error_msg: str) -> None:
         if isinstance(value, UndefinedType):
             return
+        if inspect.isclass(target_type) and isinstance(value, target_type):
+            return
         if getattr(value, "__call__", None):
             value = value()
         try:
             create_pydantic_model({"faker_param_name": (target_type, ...)})(faker_param_name=value)
         except Exception:
             raise ParseTypeError(error_msg)
```

### Comparing `pait-1.0.0a1/pait/plugin/at_most_one_of.py` & `pait-1.0.0a2/pait/plugin/at_most_one_of.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/plugin/auto_complete_json_resp.py` & `pait-1.0.0a2/pait/plugin/auto_complete_json_resp.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/plugin/base.py` & `pait-1.0.0a2/pait/plugin/base.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/plugin/cache_response.py` & `pait-1.0.0a2/pait/plugin/cache_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     cache_time: Optional[int]
     timeout: Optional[float]
     sleep: Optional[float]
     blocking_timeout: Optional[float]
 
     def __post_init__(self, **kwargs: Any) -> None:
         self.lock_name: str = self.name + ":" + "lock"
+        self._cache_name_param_set = kwargs.pop("_cache_name_param_set")
 
     @classmethod
     def check_redis(cls, redis: Union[Redis, AsyncioRedis]) -> None:
         if redis.connection_pool.connection_kwargs["decode_responses"] is False:
             raise ValueError("Please set redis`s param:decode_responses to True")
 
     @classmethod
```

### Comparing `pait-1.0.0a1/pait/plugin/check_json_resp.py` & `pait-1.0.0a2/pait/plugin/check_json_resp.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/plugin/mock_response.py` & `pait-1.0.0a2/pait/plugin/mock_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,18 +55,18 @@
         kwargs["pait_response_model"] = pait_response
         return kwargs
 
     def get_response(self) -> RESP_T:
         raise NotImplementedError()
 
     def get_file_response(self, temporary_file: IO[bytes], f: Any) -> RESP_T:
-        raise RuntimeError("Not IMplemented")
+        raise RuntimeError("Not Implemented")  # pragma: no cover
 
     async def async_get_file_response(self, temporary_file: Any, f: Any) -> RESP_T:
-        raise RuntimeError("Not IMplemented")
+        raise RuntimeError("Not Implemented")  # pragma: no cover
 
     def set_info_to_response(self, resp: RESP_T) -> None:
         raise NotImplementedError()
 
     def mock_response(self) -> RESP_T:
         if issubclass(self.pait_response_model, response.FileResponseModel):
             named_temporary_file: IO[bytes] = NamedTemporaryFile()
```

### Comparing `pait-1.0.0a1/pait/plugin/required.py` & `pait-1.0.0a2/pait/plugin/required.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/plugin/unified_response.py` & `pait-1.0.0a2/pait/plugin/unified_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/types.py` & `pait-1.0.0a2/pait/types.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/util/__init__.py` & `pait-1.0.0a2/pait/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/util/_func_sig.py` & `pait-1.0.0a2/pait/util/_func_sig.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,35 +24,37 @@
 
 
 def get_func_sig(func: Callable) -> FuncSig:
     """get func inspect.Signature model"""
     if func in _func_sig_dict:
         return _func_sig_dict[func]
 
-    # __call__ method that supports func override
-    if getattr(func, "_override_call_sig", False):
-        func = getattr(func, "__call__", func)
+    # support pait handler
+    pait_handler = getattr(func, "pait_handler", func)
 
-    sig: inspect.Signature = inspect.signature(func)
+    sig: inspect.Signature = inspect.signature(pait_handler)
     param_list: List[inspect.Parameter] = []
     for key in sig.parameters:
         # NOTE:
         #   The cbv func decorated in Pait is unbound, so it can get to self；
         #   Depend func must be bound func when it is used, so it cannot get self；
         if not (sig.parameters[key].annotation != sig.empty or sig.parameters[key].name == "self"):
             if sig.parameters[key].annotation != Self:
                 # If the name of the self variable is not self and the annotation is not Self,
                 # it will be ignored directly
                 continue
         parameter: inspect.Parameter = sig.parameters[key]
-        setattr(parameter, "_annotation", get_real_annotation(parameter.annotation, func))
+        setattr(parameter, "_annotation", get_real_annotation(parameter.annotation, pait_handler))
         param_list.append(parameter)
 
     func_sig: FuncSig = FuncSig(
-        func=func, sig=sig, param_list=param_list, return_param=get_real_annotation(sig.return_annotation, func)
+        func=pait_handler,
+        sig=sig,
+        param_list=param_list,
+        return_param=get_real_annotation(sig.return_annotation, pait_handler),
     )
     _func_sig_dict[func] = func_sig
     return func_sig
 
 
 def is_bounded_func(func: Callable) -> bool:
     return inspect.signature(func).parameters.get("self", None) is None
```

### Comparing `pait-1.0.0a1/pait/util/_gen_tip.py` & `pait-1.0.0a2/pait/util/_gen_tip.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/util/_lazy_property.py` & `pait-1.0.0a2/pait/util/_lazy_property.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/util/_pydantic_util.py` & `pait-1.0.0a2/pait/util/_pydantic_util.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/util/_types.py` & `pait-1.0.0a2/pait/util/_types.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pait/util/_util.py` & `pait-1.0.0a2/pait/util/_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import inspect
 import json
 import os
 import sys
-from dataclasses import MISSING
-from datetime import datetime
+from datetime import date, datetime
 from decimal import Decimal
 from enum import Enum
 from functools import wraps
 from json import JSONEncoder
 from typing import (  # type: ignore
     TYPE_CHECKING,
     Any,
@@ -39,14 +38,16 @@
     from pait.model.response import BaseResponseModel
 
 __all__ = [
     "gen_example_dict_from_pydantic_base_model",
     "gen_example_dict_from_schema",
     "gen_example_json_from_schema",
     "get_parameter_list_from_pydantic_basemodel",
+    "gen_example_value_from_type",
+    "get_pydantic_annotation",
     "get_parameter_list_from_class",
     "http_method_tuple",
     "json_type_default_value_dict",
     "python_type_default_value_dict",
     "get_pait_response_model",
     "example_value_handle",
     "ignore_pre_check",
@@ -77,14 +78,15 @@
     float: 0.0,
     int: 0,
     str: "",
     list: [],
     tuple: (),
     dict: {},
     datetime: datetime.fromtimestamp(0),
+    date: date.today(),
     Decimal: Decimal("0.0"),
     Any: {},
 }
 
 
 P = ParamSpec("P")
 R_T = TypeVar("R_T")
@@ -142,37 +144,32 @@
     if inspect.isclass(target_obj) and annotation in target_obj.__dict__:
         new_annotation: Type = target_obj.__dict__[annotation]
     else:
         # get real type
         value: ForwardRef = ForwardRef(annotation, is_argument=False)
 
         if sys.version_info >= (3, 9):
-            new_annotation = value._evaluate(global_dict, None, frozenset())  # type: ignore
+            new_annotation = value._evaluate(global_dict, None, frozenset())  # type: ignore    # pragma: no cover
         else:
             new_annotation = value._evaluate(global_dict, None)  # type: ignore
         if not new_annotation:
             raise RuntimeError(f"get real annotation from {target_obj} fail")  # pragma: no cover
     return _eval_type(new_annotation, global_dict, None)
 
 
 def get_pydantic_annotation(key: str, pydantic_base_model: Type[BaseModel]) -> Type:
     """Get the annotation from BaseModel's properties"""
-    annotation: Any = MISSING
-    for base in reversed(pydantic_base_model.__mro__):
-        ann: Union[str, Type] = base.__dict__.get("__annotations__", {}).get(key, MISSING)
-        if ann is not MISSING:
-            annotation = ann
-            break
-    if annotation is MISSING:
-        raise RuntimeError(f"get {key}'s annotation from {pydantic_base_model} fail")  # pragma: no cover
+    annotation = pydantic_base_model.__fields__[key].annotation
     annotation = get_real_annotation(annotation, pydantic_base_model)
-
     if getattr(annotation, "real", None) and annotation != bool:
         # support like pydantic.ConstrainedIntValue
-        annotation = annotation.real.__objclass__  # type: ignore
+        return annotation.real.__objclass__  # type: ignore
+    __base__ = getattr(annotation, "__base__", None)
+    if __base__ and getattr(__base__, "__module__", "") == "pydantic.types":
+        return annotation.__mro__[2]
     return annotation
 
 
 def get_pait_response_model(
     response_model_list: List[Type["BaseResponseModel"]],
     target_pait_response_class: Optional[Type["BaseResponseModel"]] = None,
 ) -> Type["BaseResponseModel"]:
@@ -204,23 +201,23 @@
             real_type: Type = parse_typing_result[0]
             annotation_arg_list: list = getattr(value_type, "__args__", [])
             if annotation_arg_list:
                 sub_type_set: Set[Type] = set(annotation_arg_list)
                 if len(sub_type_set) == 1:
                     sub_type = sub_type_set.pop()
         except ParseTypeError:
-            real_type = value_type
+            real_type = value_type  # pragma: no cover
         if real_type is list and sub_type:
             return [gen_example_value_from_type(sub_type, example_column_name=example_column_name)]
         else:
             # if real_type is Option[xxx], sub_type is None
             # so must parse real_type
             return gen_example_value_from_type(real_type, example_column_name=example_column_name)
     elif not inspect.isclass(value_type):
-        return python_type_default_value_dict[value_type]
+        return python_type_default_value_dict[value_type]  # pragma: no cover
     elif issubclass(value_type, Enum):
         return [i for i in value_type.__members__.values()][0].value
     elif issubclass(value_type, BaseModel):
         return gen_example_dict_from_pydantic_base_model(value_type, example_column_name=example_column_name)
     else:
         return python_type_default_value_dict[value_type]
 
@@ -232,36 +229,38 @@
     Gets the default value for pydantic.BaseModel
     :param pydantic_base_model: pydantic.BaseModel
     :param example_column_name: Gets sample values from the properties specified by pydantic.FieldInfo
     """
     gen_dict: Dict[str, Any] = {}
     for key, model_field in pydantic_base_model.__fields__.items():
         if model_field.alias:
-            key = model_field.alias
+            real_key = model_field.alias
         if example_column_name:
             example_value: Any = model_field.field_info.extra.get(example_column_name, Undefined)
             if not isinstance(example_value, UndefinedType):
-                gen_dict[key] = example_value_handle(example_value)
+                gen_dict[real_key] = example_value_handle(example_value)
                 continue
 
         if not isinstance(model_field.field_info.default, UndefinedType):
-            gen_dict[key] = model_field.field_info.default
+            gen_dict[real_key] = model_field.field_info.default
         elif model_field.field_info.default_factory and not isinstance(
             model_field.field_info.default_factory, UndefinedType
         ):
-            gen_dict[key] = model_field.field_info.default_factory()
+            gen_dict[real_key] = model_field.field_info.default_factory()
         else:
             annotation: Type = get_pydantic_annotation(key, pydantic_base_model)
-            gen_dict[key] = gen_example_value_from_type(annotation, example_column_name=example_column_name)
+            gen_dict[real_key] = gen_example_value_from_type(annotation, example_column_name=example_column_name)
     return gen_dict
 
 
 def gen_example_dict_from_schema(schema_dict: Dict[str, Any], definition_dict: Optional[dict] = None) -> Dict[str, Any]:
     gen_dict: Dict[str, Any] = {}
-    if "properties" not in schema_dict:
+    if "enum" in schema_dict:
+        return schema_dict["enum"][0]
+    elif "properties" not in schema_dict:
         return gen_dict
     property_dict: Dict[str, Any] = schema_dict["properties"]
     if not definition_dict:
         _definition_dict: dict = schema_dict.get("definitions", {})
     else:
         _definition_dict = definition_dict
     for key, value in property_dict.items():
@@ -282,16 +281,16 @@
             else:
                 if "type" in value:
                     if value["type"] not in json_type_default_value_dict:
                         raise KeyError(f"Can not found type: {key} in json type")
                     gen_dict[key] = json_type_default_value_dict[value["type"]]
                 else:
                     gen_dict[key] = "object"
-            if isinstance(gen_dict[key], Enum):
-                gen_dict[key] = gen_dict[key].value
+            # if isinstance(gen_dict[key], Enum):
+            #     gen_dict[key] = gen_dict[key].value
     return gen_dict
 
 
 def gen_example_json_from_schema(schema_dict: Dict[str, Any], cls: Optional[Type[JSONEncoder]] = None) -> str:
     return json.dumps(gen_example_dict_from_schema(schema_dict), cls=cls)
```

### Comparing `pait-1.0.0a1/pait/util/encoder.py` & `pait-1.0.0a2/pait/util/encoder.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a1/pyproject.toml` & `pait-1.0.0a2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "pait"
-version = "v1.0.0-alpha.1"
+version = "v1.0.0-alpha.2"
 description = "Pait is a Python api tool. Pait enables your Python web framework to have type checking, parameter type conversion, interface document generation and can display your documents through Redoc or Swagger (power by inspect, pydantic)"
 authors = ["So1n <so1n897046026@gmail.com>"]
 license = "Apache Software License"
 readme = "./README.md"
 repository = "https://github.com/so1n/pait"
 homepage = "https://github.com/so1n/pait"
 
 [tool.poetry.scripts]
 protoc-gen-pait-route = "pait.grpc.plugin.main:main"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-
-any-api = "^0.1.0.3"
 pydantic = "^1.7.3"
 typing-extensions = "^4.1.1"
-# protobuf-to-pydantic = { version="^0.1.7.3", optional = true}
+
+any-api = "^0.1.0.4"
+protobuf-to-pydantic = "^0.1.7.3"
+
 redis = { version = "^4.2.2", optional = true }
 jinja2 = {version = ">=2.0.0", optional = true}
-protobuf-to-pydantic = "^0.1.7.3"
 
 [tool.poetry.urls]
 "Source" = "https://github.com/so1n/pait"
 "Tracker" = "https://github.com/so1n/pait/issues"
 "Changelog" = "https://github.com/so1n/pait/blob/master/CHANGELOG.md"
 "Documentation" = "https://so1n.me/pait/"
 
@@ -104,15 +104,16 @@
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 
 [tool.coverage.run]
 branch = true
 source = ["pait"]
 omit = [
-    "pait/api_doc/*",
+    "pait/grpc/plugin/*",
+    "pait/grpc/proto/*",
 ]
 
 [tool.coverage.report]
 exclude_lines = [
     # Have to re-enable the standard pragma
     "pragma: no cover",
```

### Comparing `pait-1.0.0a1/setup.py` & `pait-1.0.0a2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,32 +36,32 @@
  'pait.plugin',
  'pait.util']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['any-api>=0.1.0.3,<0.2.0.0',
+['any-api>=0.1.0.4,<0.2.0.0',
  'pydantic>=1.7.3,<2.0.0',
  'typing-extensions>=4.1.1,<5.0.0']
 
 extras_require = \
 {':extra == "grpc" or extra == "all"': ['protobuf-to-pydantic>=0.1.7.3,<0.2.0.0'],
  'all': ['redis>=4.2.2,<5.0.0', 'jinja2>=2.0.0'],
  'grpc': ['jinja2>=2.0.0'],
  'redis': ['redis>=4.2.2,<5.0.0']}
 
 entry_points = \
 {'console_scripts': ['protoc-gen-pait-route = pait.grpc.plugin.main:main']}
 
 setup_kwargs = {
     'name': 'pait',
-    'version': '1.0.0a1',
+    'version': '1.0.0a2',
     'description': 'Pait is a Python api tool. Pait enables your Python web framework to have type checking, parameter type conversion, interface document generation and can display your documents through Redoc or Swagger (power by inspect, pydantic)',
-    'long_description': '![](https://cdn.jsdelivr.net/gh/so1n/so1n_blog_photo@master/blog_photo/1652600629491%E6%9C%AA%E5%91%BD%E5%90%8D.jpg)\n<p align="center">\n    <em>Python Modern API Tools, fast to code</em>\n</p>\n<p align="center">\n    <a href="https://codecov.io/gh/so1n/pait" target="_blank">\n        <img src="https://codecov.io/gh/so1n/pait/branch/master/graph/badge.svg?token=NEVM1VODHR" alt="Coverage">\n    </a>\n</p>\n<p align="center">\n    <a href="https://pypi.org/project/pait/" target="_blank">\n        <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/pait">\n    </a>\n    <a href="https://pypi.org/project/pait/" target="_blank">\n        <img alt="PyPI" src="https://img.shields.io/pypi/v/pait">\n    </a>\n</p>\n<p align="center">\n    <a href="https://github.com/so1n/pait/actions?query=event%3Apush+branch%3Amaster" target="_blank">\n        <img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/so1n/pait/python-package.yml">\n    </a>\n    <a href="https://github.com/so1n/pait/releases" target="_blank">\n        <img alt="GitHub release (release name instead of tag name)" src="https://img.shields.io/github/v/release/so1n/pait?include_prereleases">\n    </a>\n    <a href="https://github.com/so1n/pait/actions?query=event%3Apush+branch%3Amaster" target="_blank">\n        <img src="https://github.com/so1n/pait/actions/workflows/python-package.yml/badge.svg?event=push&branch=master" alt="Test">\n    </a>\n</p>\n<p align="center">\n    <a href="https://github.com/so1n/pait/tree/master/example" target="_blank">\n        <img src="https://img.shields.io/badge/Support%20framework-Flask%2CSanic%2CStarlette%2CTornado-brightgreen" alt="Support framework">\n    </a>\n</p>\n\n\n---\n**Documentation**: [https://so1n.me/pait/](https://so1n.me/pait/)\n\n**中文文档**: [https://so1n.me/pait-zh-doc/](https://so1n.me/pait-zh-doc/)\n\n---\n\n# pait\n\nPait is an api tool that can be used in any python web framework (currently only `flask`, `starlette`, `sanic`, `tornado` are supported, other frameworks will be supported once Pait is stable).\n\n> Note:\n>\n> mypy check 100%\n>\n> test coverage 95%+ (exclude api_doc)\n>\n> python version >= 3.7 (support postponed annotations)\n>\n> The following code does not specify, all default to use the `starlette` framework.\n\n# Warning\nThere are changes between the current version and the 0.8 version of the API, For more information, please refer to [0.9.0version change](https://github.com/so1n/pait/blob/master/CHANGELOG.md)\n\n# Feature\n - [x] Parameter checksum automatic conversion (parameter check depends on `Pydantic`)\n - [x] Parameter dependency verification\n - [x] Automatically generate openapi files\n - [x] Swagger, Redoc route\n - [x] gRPC Gateway route\n - [x] TestClient support, support response result verification\n - [x] Support for plugin extensions, such as the Mock plugin\n\n# Installation\n```Bash\npip install pait\n```\n# Simple Example\n```python\nfrom typing import Type\nimport uvicorn  # type: ignore\nfrom starlette.applications import Starlette\nfrom starlette.responses import JSONResponse\nfrom starlette.routing import Route\n\nfrom pait.app.starlette import pait, add_doc_route\nfrom pait.field import Body\nfrom pait.model.response import PaitResponseModel\nfrom pydantic import BaseModel, Field\n\n\nclass DemoResponseModel(PaitResponseModel):\n    class ResponseModel(BaseModel):\n        uid: int = Field()\n        user_name: str = Field()\n\n    description: str = "demo response"\n    response_data: Type[BaseModel] = ResponseModel\n\n\n@pait(response_model_list=[DemoResponseModel])\nasync def demo_post(\n    uid: int = Body.i(description="user id", gt=10, lt=1000),\n    user_name: str = Body.i(description="user name", min_length=2, max_length=4)\n) -> JSONResponse:\n    return JSONResponse({\'uid\': uid, \'user_name\': user_name})\n\n\napp = Starlette(routes=[Route(\'/api\', demo_post, methods=[\'POST\'])])\nadd_doc_route(app)\nuvicorn.run(app)\n```\n\n# How to used in other web framework?\nIf the web framework is not supported, which you are using.\n\nCan be modified sync web framework according to [pait.app.flask](https://github.com/so1n/pait/blob/master/pait/app/flask.py)\n\nCan be modified async web framework according to [pait.app.starlette](https://github.com/so1n/pait/blob/master/pait/app/starlette.py)\n# IDE Support\nWhile pydantic will work well with any IDE out of the box.\n- [PyCharm plugin](https://pydantic-docs.helpmanual.io/pycharm_plugin/)\n- [Mypy plugin](https://pydantic-docs.helpmanual.io/mypy_plugin/)\n\n# Full example\nFor more complete examples, please refer to [example](https://github.com/so1n/pait/tree/master/example)\n',
+    'long_description': '![](https://cdn.jsdelivr.net/gh/so1n/so1n_blog_photo@master/blog_photo/1652600629491%E6%9C%AA%E5%91%BD%E5%90%8D.jpg)\n<p align="center">\n    Pait(π tool) - <em>Python Modern API Tools, easier to use web frameworks/write API routing</em>\n</p>\n<p align="center">\n    <a href="https://codecov.io/gh/so1n/pait" target="_blank">\n        <img src="https://codecov.io/gh/so1n/pait/branch/master/graph/badge.svg?token=NEVM1VODHR" alt="Coverage">\n    </a>\n</p>\n<p align="center">\n    <a href="https://pypi.org/project/pait/" target="_blank">\n        <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/pait">\n    </a>\n    <a href="https://pypi.org/project/pait/" target="_blank">\n        <img alt="PyPI" src="https://img.shields.io/pypi/v/pait">\n    </a>\n</p>\n<p align="center">\n    <a href="https://github.com/so1n/pait/actions?query=event%3Apush+branch%3Amaster" target="_blank">\n        <img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/so1n/pait/python-package.yml">\n    </a>\n    <a href="https://github.com/so1n/pait/releases" target="_blank">\n        <img alt="GitHub release (release name instead of tag name)" src="https://img.shields.io/github/v/release/so1n/pait?include_prereleases">\n    </a>\n    <a href="https://github.com/so1n/pait/actions?query=event%3Apush+branch%3Amaster" target="_blank">\n        <img src="https://github.com/so1n/pait/actions/workflows/python-package.yml/badge.svg?event=push&branch=master" alt="Test">\n    </a>\n</p>\n<p align="center">\n    <a href="https://github.com/so1n/pait/tree/master/example" target="_blank">\n        <img src="https://img.shields.io/badge/Support%20framework-Flask%2CSanic%2CStarlette%2CTornado-brightgreen" alt="Support framework">\n    </a>\n</p>\n\n\n---\n**Documentation**: [https://so1n.me/pait/](https://so1n.me/pait/)\n\n**中文文档**: [https://so1n.me/pait-zh-doc/](https://so1n.me/pait-zh-doc/)\n\n---\n\n# Warning\nThere are changes between the current version and the 0.8 version of the API, For more information, please refer to [1.0.0version change](https://github.com/so1n/pait/blob/master/CHANGELOG.md)\n\n# pait\n\nPait is an api tool that can be used in any python web framework, the features provided are as follows:\n - [x] Parameter checksum automatic conversion (parameter check depends on `Pydantic`)\n - [x] Parameter dependency verification\n - [x] Automatically generate openapi files\n - [x] Swagger, Redoc, Rapidoc, Elements, OpenAPI route\n - [x] gRPC Gateway route\n - [x] TestClient support, support response result verification\n - [x] Support for plugin extensions, such as the Mock plugin, CheckResponse Plugin, Cache Response Plugin\n - [ ] WebSocket support\n - [ ] Auto API Test support\n\n\n> Note:\n>\n> - mypy check 100%\n>\n> - python version >= 3.7 (support postponed annotations)\n\n\n\n# Installation\n```Bash\npip install pait --pre\n```\nIf want to use the gRPC gateway feature, need to add a \'grpc\' dependency:\n```bash\npip install pait[grpc] --pre\n```\n# Simple Example\n```python\nfrom typing import Type\nimport uvicorn  # type: ignore\nfrom starlette.applications import Starlette\nfrom starlette.responses import JSONResponse\nfrom starlette.routing import Route\n\nfrom pait.app.starlette import pait\nfrom pait.field import Body\nfrom pait.openapi.doc_route import add_doc_route\nfrom pait.model.response import JsonResponseModel\nfrom pydantic import BaseModel, Field\n\n\nclass DemoResponseModel(JsonResponseModel):\n    """demo post api response model"""\n    class ResponseModel(BaseModel):\n        uid: int = Field()\n        user_name: str = Field()\n\n    description: str = "demo response"\n    response_data: Type[BaseModel] = ResponseModel\n\n\n@pait(response_model_list=[DemoResponseModel])\nasync def demo_post(\n    uid: int = Body.i(description="user id", gt=10, lt=1000),\n    user_name: str = Body.i(description="user name", min_length=2, max_length=4)\n) -> JSONResponse:\n    return JSONResponse({\'uid\': uid, \'user_name\': user_name})\n\n\napp = Starlette(routes=[Route(\'/api\', demo_post, methods=[\'POST\'])])\nadd_doc_route(app)\nuvicorn.run(app)\n```\nSee [documentation](https://so1n.me/pait/) for more features\n\n# Support Web framework\n\n| Framework | Description            |\n|-----------|------------------------|\n| Flask     | All features supported |\n| Sanic     | All features supported |\n| Starlette | All features supported |\n| Tornado   | All features supported |\n| Django    | Coming soon            |\n\n\nIf the web framework is not supported(which you are using).\n\nCan be modified sync web framework according to [pait.app.flask](https://github.com/so1n/pait/blob/master/pait/app/flask.py)\n\nCan be modified async web framework according to [pait.app.starlette](https://github.com/so1n/pait/blob/master/pait/app/starlette.py)\n\n# Performance\nFor the parameter validation and transformation feature, Pait is mainly responsible for injecting the request data dependency into the `Pydantic` model, and then the `Pydanitc` verifies and transforms the data.\n\nThe time consumed by this process <=0.0003 (s), for benchmarks data and subsequent optimization, see [#27](https://github.com/so1n/pait/issues/27)\n\n\n# Full example\nFor more complete examples, please refer to [example](https://github.com/so1n/pait/tree/master/example)\n',
     'author': 'So1n',
     'author_email': 'so1n897046026@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/so1n/pait',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -5,74 +5,84 @@
 'pait.app.flask.security', 'pait.app.sanic', 'pait.app.sanic.adapter',
 'pait.app.sanic.plugin', 'pait.app.sanic.security', 'pait.app.starlette',
 'pait.app.starlette.adapter', 'pait.app.starlette.plugin',
 'pait.app.starlette.security', 'pait.app.tornado', 'pait.app.tornado.adapter',
 'pait.app.tornado.plugin', 'pait.app.tornado.security', 'pait.extra',
 'pait.grpc', 'pait.grpc.plugin', 'pait.grpc.proto', 'pait.model',
 'pait.openapi', 'pait.param_handle', 'pait.plugin', 'pait.util'] package_data =
-\ {'': ['*']} install_requires = \ ['any-api>=0.1.0.3,<0.2.0.0',
+\ {'': ['*']} install_requires = \ ['any-api>=0.1.0.4,<0.2.0.0',
 'pydantic>=1.7.3,<2.0.0', 'typing-extensions>=4.1.1,<5.0.0'] extras_require = \
 {':extra == "grpc" or extra == "all"': ['protobuf-to-
 pydantic>=0.1.7.3,<0.2.0.0'], 'all': ['redis>=4.2.2,<5.0.0', 'jinja2>=2.0.0'],
 'grpc': ['jinja2>=2.0.0'], 'redis': ['redis>=4.2.2,<5.0.0']} entry_points = \
 {'console_scripts': ['protoc-gen-pait-route = pait.grpc.plugin.main:main']}
-setup_kwargs = { 'name': 'pait', 'version': '1.0.0a1', 'description': 'Pait is
+setup_kwargs = { 'name': 'pait', 'version': '1.0.0a2', 'description': 'Pait is
 a Python api tool. Pait enables your Python web framework to have type
 checking, parameter type conversion, interface document generation and can
 display your documents through Redoc or Swagger (power by inspect, pydantic)',
 'long_description': '![](https://cdn.jsdelivr.net/gh/so1n/
 so1n_blog_photo@master/blog_photo/
 1652600629491%E6%9C%AA%E5%91%BD%E5%90%8D.jpg)\n
-                  \n Python Modern API Tools, fast to code\n
+\n Pait(Ï tool) - Python Modern API Tools, easier to use web frameworks/write
+                                 API routing\n
 \n
                              \n \n_[Coverage]\n\n
 \n
                 \n \n_[PyPI_-_Python_Version]\n\n \n_[PyPI]\n\n
 \n
 \n \n_[GitHub_Workflow_Status]\n\n \n_[GitHub_release_(release_name_instead_of
                          tag_name)]\n\n \n_[Test]\n\n
 \n
                          \n \n_[Support_framework]\n\n
 \n\n\n---\n**Documentation**: [https://so1n.me/pait/](https://so1n.me/pait/
 )\n\n**ä¸­æææ¡£**: [https://so1n.me/pait-zh-doc/](https://so1n.me/pait-zh-
-doc/)\n\n---\n\n# pait\n\nPait is an api tool that can be used in any python
-web framework (currently only `flask`, `starlette`, `sanic`, `tornado` are
-supported, other frameworks will be supported once Pait is stable).\n\n> Note:
-\n>\n> mypy check 100%\n>\n> test coverage 95%+ (exclude api_doc)\n>\n> python
-version >= 3.7 (support postponed annotations)\n>\n> The following code does
-not specify, all default to use the `starlette` framework.\n\n# Warning\nThere
-are changes between the current version and the 0.8 version of the API, For
-more information, please refer to [0.9.0version change](https://github.com/
-so1n/pait/blob/master/CHANGELOG.md)\n\n# Feature\n - [x] Parameter checksum
-automatic conversion (parameter check depends on `Pydantic`)\n - [x] Parameter
-dependency verification\n - [x] Automatically generate openapi files\n - [x]
-Swagger, Redoc route\n - [x] gRPC Gateway route\n - [x] TestClient support,
-support response result verification\n - [x] Support for plugin extensions,
-such as the Mock plugin\n\n# Installation\n```Bash\npip install pait\n```\n#
-Simple Example\n```python\nfrom typing import Type\nimport uvicorn # type:
-ignore\nfrom starlette.applications import Starlette\nfrom starlette.responses
-import JSONResponse\nfrom starlette.routing import Route\n\nfrom
-pait.app.starlette import pait, add_doc_route\nfrom pait.field import
-Body\nfrom pait.model.response import PaitResponseModel\nfrom pydantic import
-BaseModel, Field\n\n\nclass DemoResponseModel(PaitResponseModel):\n class
-ResponseModel(BaseModel):\n uid: int = Field()\n user_name: str = Field()\n\n
-description: str = "demo response"\n response_data: Type[BaseModel] =
-ResponseModel\n\n\n@pait(response_model_list=[DemoResponseModel])\nasync def
-demo_post(\n uid: int = Body.i(description="user id", gt=10, lt=1000),\n
-user_name: str = Body.i(description="user name", min_length=2, max_length=4)\n)
--> JSONResponse:\n return JSONResponse({\'uid\': uid, \'user_name\':
-user_name})\n\n\napp = Starlette(routes=[Route(\'/api\', demo_post, methods=
-[\'POST\'])])\nadd_doc_route(app)\nuvicorn.run(app)\n```\n\n# How to used in
-other web framework?\nIf the web framework is not supported, which you are
-using.\n\nCan be modified sync web framework according to [pait.app.flask]
-(https://github.com/so1n/pait/blob/master/pait/app/flask.py)\n\nCan be modified
-async web framework according to [pait.app.starlette](https://github.com/so1n/
-pait/blob/master/pait/app/starlette.py)\n# IDE Support\nWhile pydantic will
-work well with any IDE out of the box.\n- [PyCharm plugin](https://pydantic-
-docs.helpmanual.io/pycharm_plugin/)\n- [Mypy plugin](https://pydantic-
-docs.helpmanual.io/mypy_plugin/)\n\n# Full example\nFor more complete examples,
-please refer to [example](https://github.com/so1n/pait/tree/master/example)\n',
-'author': 'So1n', 'author_email': 'so1n897046026@gmail.com', 'maintainer':
-'None', 'maintainer_email': 'None', 'url': 'https://github.com/so1n/pait',
-'packages': packages, 'package_data': package_data, 'install_requires':
-install_requires, 'extras_require': extras_require, 'entry_points':
-entry_points, 'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
+doc/)\n\n---\n\n# Warning\nThere are changes between the current version and
+the 0.8 version of the API, For more information, please refer to [1.0.0version
+change](https://github.com/so1n/pait/blob/master/CHANGELOG.md)\n\n#
+pait\n\nPait is an api tool that can be used in any python web framework, the
+features provided are as follows:\n - [x] Parameter checksum automatic
+conversion (parameter check depends on `Pydantic`)\n - [x] Parameter dependency
+verification\n - [x] Automatically generate openapi files\n - [x] Swagger,
+Redoc, Rapidoc, Elements, OpenAPI route\n - [x] gRPC Gateway route\n - [x]
+TestClient support, support response result verification\n - [x] Support for
+plugin extensions, such as the Mock plugin, CheckResponse Plugin, Cache
+Response Plugin\n - [ ] WebSocket support\n - [ ] Auto API Test support\n\n\n>
+Note:\n>\n> - mypy check 100%\n>\n> - python version >= 3.7 (support postponed
+annotations)\n\n\n\n# Installation\n```Bash\npip install pait --pre\n```\nIf
+want to use the gRPC gateway feature, need to add a \'grpc\' dependency:
+\n```bash\npip install pait[grpc] --pre\n```\n# Simple Example\n```python\nfrom
+typing import Type\nimport uvicorn # type: ignore\nfrom starlette.applications
+import Starlette\nfrom starlette.responses import JSONResponse\nfrom
+starlette.routing import Route\n\nfrom pait.app.starlette import pait\nfrom
+pait.field import Body\nfrom pait.openapi.doc_route import add_doc_route\nfrom
+pait.model.response import JsonResponseModel\nfrom pydantic import BaseModel,
+Field\n\n\nclass DemoResponseModel(JsonResponseModel):\n """demo post api
+response model"""\n class ResponseModel(BaseModel):\n uid: int = Field()\n
+user_name: str = Field()\n\n description: str = "demo response"\n
+response_data: Type[BaseModel] = ResponseModel\n\n\n@pait(response_model_list=
+[DemoResponseModel])\nasync def demo_post(\n uid: int = Body.i
+(description="user id", gt=10, lt=1000),\n user_name: str = Body.i
+(description="user name", min_length=2, max_length=4)\n) -> JSONResponse:\n
+return JSONResponse({\'uid\': uid, \'user_name\': user_name})\n\n\napp =
+Starlette(routes=[Route(\'/api\', demo_post, methods=
+[\'POST\'])])\nadd_doc_route(app)\nuvicorn.run(app)\n```\nSee [documentation]
+(https://so1n.me/pait/) for more features\n\n# Support Web framework\n\n|
+Framework | Description |\n|-----------|------------------------|\n| Flask |
+All features supported |\n| Sanic | All features supported |\n| Starlette | All
+features supported |\n| Tornado | All features supported |\n| Django | Coming
+soon |\n\n\nIf the web framework is not supported(which you are using).\n\nCan
+be modified sync web framework according to [pait.app.flask](https://
+github.com/so1n/pait/blob/master/pait/app/flask.py)\n\nCan be modified async
+web framework according to [pait.app.starlette](https://github.com/so1n/pait/
+blob/master/pait/app/starlette.py)\n\n# Performance\nFor the parameter
+validation and transformation feature, Pait is mainly responsible for injecting
+the request data dependency into the `Pydantic` model, and then the `Pydanitc`
+verifies and transforms the data.\n\nThe time consumed by this process <=0.0003
+(s), for benchmarks data and subsequent optimization, see [#27](https://
+github.com/so1n/pait/issues/27)\n\n\n# Full example\nFor more complete
+examples, please refer to [example](https://github.com/so1n/pait/tree/master/
+example)\n', 'author': 'So1n', 'author_email': 'so1n897046026@gmail.com',
+'maintainer': 'None', 'maintainer_email': 'None', 'url': 'https://github.com/
+so1n/pait', 'packages': packages, 'package_data': package_data,
+'install_requires': install_requires, 'extras_require': extras_require,
+'entry_points': entry_points, 'python_requires': '>=3.7,<4.0', } setup
+(**setup_kwargs)
```

### Comparing `pait-1.0.0a1/PKG-INFO` & `pait-1.0.0a2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pait
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Pait is a Python api tool. Pait enables your Python web framework to have type checking, parameter type conversion, interface document generation and can display your documents through Redoc or Swagger (power by inspect, pydantic)
 Home-page: https://github.com/so1n/pait
 License: Apache Software License
 Author: So1n
 Author-email: so1n897046026@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
@@ -13,30 +13,30 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: grpc
 Provides-Extra: redis
-Requires-Dist: any-api (>=0.1.0.3,<0.2.0.0)
+Requires-Dist: any-api (>=0.1.0.4,<0.2.0.0)
 Requires-Dist: jinja2 (>=2.0.0) ; extra == "grpc" or extra == "all"
 Requires-Dist: protobuf-to-pydantic (>=0.1.7.3,<0.2.0.0) ; extra == "grpc" or extra == "all"
 Requires-Dist: pydantic (>=1.7.3,<2.0.0)
 Requires-Dist: redis (>=4.2.2,<5.0.0) ; extra == "redis" or extra == "all"
 Requires-Dist: typing-extensions (>=4.1.1,<5.0.0)
 Project-URL: Changelog, https://github.com/so1n/pait/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://so1n.me/pait/
 Project-URL: Repository, https://github.com/so1n/pait
 Project-URL: Source, https://github.com/so1n/pait
 Project-URL: Tracker, https://github.com/so1n/pait/issues
 Description-Content-Type: text/markdown
 
 ![](https://cdn.jsdelivr.net/gh/so1n/so1n_blog_photo@master/blog_photo/1652600629491%E6%9C%AA%E5%91%BD%E5%90%8D.jpg)
 <p align="center">
-    <em>Python Modern API Tools, fast to code</em>
+    Pait(π tool) - <em>Python Modern API Tools, easier to use web frameworks/write API routing</em>
 </p>
 <p align="center">
     <a href="https://codecov.io/gh/so1n/pait" target="_blank">
         <img src="https://codecov.io/gh/so1n/pait/branch/master/graph/badge.svg?token=NEVM1VODHR" alt="Coverage">
     </a>
 </p>
 <p align="center">
@@ -68,59 +68,64 @@
 ---
 **Documentation**: [https://so1n.me/pait/](https://so1n.me/pait/)
 
 **中文文档**: [https://so1n.me/pait-zh-doc/](https://so1n.me/pait-zh-doc/)
 
 ---
 
+# Warning
+There are changes between the current version and the 0.8 version of the API, For more information, please refer to [1.0.0version change](https://github.com/so1n/pait/blob/master/CHANGELOG.md)
+
 # pait
 
-Pait is an api tool that can be used in any python web framework (currently only `flask`, `starlette`, `sanic`, `tornado` are supported, other frameworks will be supported once Pait is stable).
+Pait is an api tool that can be used in any python web framework, the features provided are as follows:
+ - [x] Parameter checksum automatic conversion (parameter check depends on `Pydantic`)
+ - [x] Parameter dependency verification
+ - [x] Automatically generate openapi files
+ - [x] Swagger, Redoc, Rapidoc, Elements, OpenAPI route
+ - [x] gRPC Gateway route
+ - [x] TestClient support, support response result verification
+ - [x] Support for plugin extensions, such as the Mock plugin, CheckResponse Plugin, Cache Response Plugin
+ - [ ] WebSocket support
+ - [ ] Auto API Test support
+
 
 > Note:
 >
-> mypy check 100%
->
-> test coverage 95%+ (exclude api_doc)
+> - mypy check 100%
 >
-> python version >= 3.7 (support postponed annotations)
->
-> The following code does not specify, all default to use the `starlette` framework.
+> - python version >= 3.7 (support postponed annotations)
 
-# Warning
-There are changes between the current version and the 0.8 version of the API, For more information, please refer to [0.9.0version change](https://github.com/so1n/pait/blob/master/CHANGELOG.md)
 
-# Feature
- - [x] Parameter checksum automatic conversion (parameter check depends on `Pydantic`)
- - [x] Parameter dependency verification
- - [x] Automatically generate openapi files
- - [x] Swagger, Redoc route
- - [x] gRPC Gateway route
- - [x] TestClient support, support response result verification
- - [x] Support for plugin extensions, such as the Mock plugin
 
 # Installation
 ```Bash
-pip install pait
+pip install pait --pre
+```
+If want to use the gRPC gateway feature, need to add a 'grpc' dependency:
+```bash
+pip install pait[grpc] --pre
 ```
 # Simple Example
 ```python
 from typing import Type
 import uvicorn  # type: ignore
 from starlette.applications import Starlette
 from starlette.responses import JSONResponse
 from starlette.routing import Route
 
-from pait.app.starlette import pait, add_doc_route
+from pait.app.starlette import pait
 from pait.field import Body
-from pait.model.response import PaitResponseModel
+from pait.openapi.doc_route import add_doc_route
+from pait.model.response import JsonResponseModel
 from pydantic import BaseModel, Field
 
 
-class DemoResponseModel(PaitResponseModel):
+class DemoResponseModel(JsonResponseModel):
+    """demo post api response model"""
     class ResponseModel(BaseModel):
         uid: int = Field()
         user_name: str = Field()
 
     description: str = "demo response"
     response_data: Type[BaseModel] = ResponseModel
 
@@ -133,22 +138,35 @@
     return JSONResponse({'uid': uid, 'user_name': user_name})
 
 
 app = Starlette(routes=[Route('/api', demo_post, methods=['POST'])])
 add_doc_route(app)
 uvicorn.run(app)
 ```
+See [documentation](https://so1n.me/pait/) for more features
+
+# Support Web framework
 
-# How to used in other web framework?
-If the web framework is not supported, which you are using.
+| Framework | Description            |
+|-----------|------------------------|
+| Flask     | All features supported |
+| Sanic     | All features supported |
+| Starlette | All features supported |
+| Tornado   | All features supported |
+| Django    | Coming soon            |
+
+
+If the web framework is not supported(which you are using).
 
 Can be modified sync web framework according to [pait.app.flask](https://github.com/so1n/pait/blob/master/pait/app/flask.py)
 
 Can be modified async web framework according to [pait.app.starlette](https://github.com/so1n/pait/blob/master/pait/app/starlette.py)
-# IDE Support
-While pydantic will work well with any IDE out of the box.
-- [PyCharm plugin](https://pydantic-docs.helpmanual.io/pycharm_plugin/)
-- [Mypy plugin](https://pydantic-docs.helpmanual.io/mypy_plugin/)
+
+# Performance
+For the parameter validation and transformation feature, Pait is mainly responsible for injecting the request data dependency into the `Pydantic` model, and then the `Pydanitc` verifies and transforms the data.
+
+The time consumed by this process <=0.0003 (s), for benchmarks data and subsequent optimization, see [#27](https://github.com/so1n/pait/issues/27)
+
 
 # Full example
 For more complete examples, please refer to [example](https://github.com/so1n/pait/tree/master/example)
```

