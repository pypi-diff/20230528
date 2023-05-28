# Comparing `tmp/wiliot-deployment-tools-4.0.3.tar.gz` & `tmp/wiliot-deployment-tools-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-deployment-tools-4.0.3.tar", last modified: Mon May 22 14:49:11 2023, max compression
+gzip compressed data, was "wiliot-deployment-tools-4.0.4.tar", last modified: Sun May 28 07:05:40 2023, max compression
```

## Comparing `wiliot-deployment-tools-4.0.3.tar` & `wiliot-deployment-tools-4.0.4.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 14:49:11.305935 wiliot-deployment-tools-4.0.3/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 14:49:11.293935 wiliot-deployment-tools-4.0.3/.devcontainer/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 14:49:11.297935 wiliot-deployment-tools-4.0.3/.devcontainer/private/
--rw-rw-rw-   0 root         (0) root         (0)     1043 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/.devcontainer/private/devcontainer.json
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 14:49:11.297935 wiliot-deployment-tools-4.0.3/.devcontainer/public/
--rw-rw-rw-   0 root         (0) root         (0)     1057 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/.devcontainer/public/devcontainer.json
--rw-rw-rw-   0 root         (0) root         (0)      321 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5159 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     7238 2023-05-22 14:49:11.305935 wiliot-deployment-tools-4.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6747 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)     8812 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)     2625 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/ci.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/dep-tools-public.dockerfile
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/dep-tools.dockerfile
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-22 14:49:11.305935 wiliot-deployment-tools-4.0.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3412 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 14:49:11.297935 wiliot-deployment-tools-4.0.3/unittests/
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/unittests/test_debug_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2250 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/unittests/test_extended_api_edge.py
--rw-rw-rw-   0 root         (0) root         (0)     1196 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/unittests/test_extended_api_platform.py
--rw-rw-rw-   0 root         (0) root         (0)     2045 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/unittests/test_power_mgmt.py
--rw-rw-rw-   0 root         (0) root         (0)     2710 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/unittests/test_slack_alerts.py
--rw-rw-rw-   0 root         (0) root         (0)     1607 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/unittests/test_test_tool.py
--rw-rw-rw-   0 root         (0) root         (0)     2129 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/unittests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 14:49:11.301935 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 14:49:11.301935 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    41546 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/api/extended_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1187 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/api/gw_ssid.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 14:49:11.301935 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/automatic_configuration_tool/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/automatic_configuration_tool/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15155 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py
--rw-rw-rw-   0 root         (0) root         (0)     3186 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 14:49:11.305935 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/common/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    68575 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/common/analysis_data_bricks.py
--rw-rw-rw-   0 root         (0) root         (0)     2310 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/common/debug.py
--rw-rw-rw-   0 root         (0) root         (0)     6004 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/common/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3112 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/common/utils_defines.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 14:49:11.305935 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/firmware_update/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/firmware_update/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23066 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/firmware_update/firmware_update.py
--rw-rw-rw-   0 root         (0) root         (0)     4342 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/firmware_update/firmware_update_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 14:49:11.305935 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/log_viewer/
--rw-rw-rw-   0 root         (0) root         (0)     1919 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/log_viewer/log_viewer_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 14:49:11.305935 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/power_mgmt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/power_mgmt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4653 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py
--rw-rw-rw-   0 root         (0) root         (0)    26163 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/power_mgmt/power_mgmt.py
--rw-rw-rw-   0 root         (0) root         (0)     4154 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 14:49:11.305935 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6057 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-22 14:49:11.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 14:49:11.301935 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     7238 2023-05-22 14:49:11.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2014 2023-05-22 14:49:11.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-22 14:49:11.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      345 2023-05-22 14:49:11.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-22 14:49:11.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-05-22 14:49:11.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-22 14:49:11.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 07:05:40.224493 wiliot-deployment-tools-4.0.4/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 07:05:40.208492 wiliot-deployment-tools-4.0.4/.devcontainer/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 07:05:40.212493 wiliot-deployment-tools-4.0.4/.devcontainer/private/
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/.devcontainer/private/devcontainer.json
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 07:05:40.212493 wiliot-deployment-tools-4.0.4/.devcontainer/public/
+-rw-rw-rw-   0 root         (0) root         (0)     1057 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/.devcontainer/public/devcontainer.json
+-rw-rw-rw-   0 root         (0) root         (0)      321 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     7307 2023-05-28 07:05:40.224493 wiliot-deployment-tools-4.0.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6816 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     8812 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2625 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/ci.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/dep-tools-public.dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)      577 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/dep-tools.dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-28 07:05:40.224493 wiliot-deployment-tools-4.0.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3457 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 07:05:40.216493 wiliot-deployment-tools-4.0.4/unittests/
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/unittests/test_debug_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2250 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/unittests/test_extended_api_edge.py
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/unittests/test_extended_api_platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     2045 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/unittests/test_power_mgmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     2710 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/unittests/test_slack_alerts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/unittests/test_test_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     2129 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/unittests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 07:05:40.216493 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 07:05:40.216493 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    41989 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/api/extended_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1187 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/api/gw_ssid.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 07:05:40.220493 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/automatic_configuration_tool/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/automatic_configuration_tool/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15257 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     3178 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 07:05:40.220493 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/common/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    68575 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/common/analysis_data_bricks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2310 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/common/debug.py
+-rw-rw-rw-   0 root         (0) root         (0)     6004 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/common/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3112 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/common/utils_defines.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 07:05:40.220493 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/firmware_update/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/firmware_update/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23066 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/firmware_update/firmware_update.py
+-rw-rw-rw-   0 root         (0) root         (0)     4348 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/firmware_update/firmware_update_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 07:05:40.220493 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/log_viewer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/log_viewer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1956 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/log_viewer/log_viewer_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 07:05:40.224493 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/power_mgmt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/power_mgmt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4653 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py
+-rw-rw-rw-   0 root         (0) root         (0)    26335 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/power_mgmt/power_mgmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     4143 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 07:05:40.224493 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6057 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-28 07:05:40.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 07:05:40.216493 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     7307 2023-05-28 07:05:40.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2061 2023-05-28 07:05:40.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-28 07:05:40.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      345 2023-05-28 07:05:40.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-28 07:05:40.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      362 2023-05-28 07:05:40.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-28 07:05:40.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools.egg-info/top_level.txt
```

### Comparing `wiliot-deployment-tools-4.0.3/.devcontainer/private/devcontainer.json` & `wiliot-deployment-tools-4.0.4/.devcontainer/private/devcontainer.json`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.3/.devcontainer/public/devcontainer.json` & `wiliot-deployment-tools-4.0.4/.devcontainer/public/devcontainer.json`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.3/LICENSE` & `wiliot-deployment-tools-4.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.3/PKG-INFO` & `wiliot-deployment-tools-4.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-deployment-tools
-Version: 4.0.3
+Version: 4.0.4
 Summary: A library for interacting with Wiliot's Deployment Tools
 Home-page: 
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Classifier: Programming Language :: Python :: 3
@@ -31,22 +31,22 @@
 
 ## Using wiliot-deployment-tools
 This package includes the following CLI Utilities:
 ### Automatic Configuration Tool
 Automatically connects to all Gateways / Bridges in the location specified, and configure them to optimal parameters.
 
 ```
-usage: wlt-config -owner OWNER -location LOCATION [-ota_upgrade] [-no_gp_zone] [-pacing_interval PACING_INTERVAL] [-ignore_bridges [IGNORE_BRIDGES [IGNORE_BRIDGES ...]]] [--expected_num_brgs EXPECTED_NUM_BRGS]
+usage: wlt-config -owner OWNER -location LOCATION [-ota] [-no_gp_zone] [-pacing_interval PACING_INTERVAL] [-ignore_bridges [IGNORE_BRIDGES [IGNORE_BRIDGES ...]]] [--expected_num_brgs EXPECTED_NUM_BRGS]
 
 required arguments:
   -owner OWNER         Platform owner id
   -location LOCATION   Location name in Wiliot platform. If location has ' ' in name, input location wrapped with double quotes: --location "LOCATION NAME"
 
 additional (optional) arguments:
-  -ota_upgrade         Updating FW version to latest for all devices
+  -ota         Updating FW version to latest for all devices
   -no_gp_zone          don't use Global pacing group by zone (all bridges will be GPG=0)
   -pacing_interval PACING_INTERVAL
                         Pacing interval for all devices
   -ignore_bridges [IGNORE_BRIDGES [IGNORE_BRIDGES ...]]
                         bridges to ignore in the tool - their configuration won't be changed
   -expected_num_brgs EXPECTED_NUM_BRGS
                         Number of expected bridges in location. The tool will try to connect to all bridges (excluding those specified in ignore bridges) until reaching expected number.
@@ -141,14 +141,17 @@
 ------------------
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.0.4:
+* Bugfixes, add relevant printouts to CLI to help understand errors.
+
 Version 4.0.3:
 * Initial release of CLI tools suite - Automatic Configuration Tool, Firmware Update, Power Management, Log Viewer.
 
 Version 4.0.0:
 * First version
```

### Comparing `wiliot-deployment-tools-4.0.3/README.md` & `wiliot-deployment-tools-4.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 
 ## Using wiliot-deployment-tools
 This package includes the following CLI Utilities:
 ### Automatic Configuration Tool
 Automatically connects to all Gateways / Bridges in the location specified, and configure them to optimal parameters.
 
 ```
-usage: wlt-config -owner OWNER -location LOCATION [-ota_upgrade] [-no_gp_zone] [-pacing_interval PACING_INTERVAL] [-ignore_bridges [IGNORE_BRIDGES [IGNORE_BRIDGES ...]]] [--expected_num_brgs EXPECTED_NUM_BRGS]
+usage: wlt-config -owner OWNER -location LOCATION [-ota] [-no_gp_zone] [-pacing_interval PACING_INTERVAL] [-ignore_bridges [IGNORE_BRIDGES [IGNORE_BRIDGES ...]]] [--expected_num_brgs EXPECTED_NUM_BRGS]
 
 required arguments:
   -owner OWNER         Platform owner id
   -location LOCATION   Location name in Wiliot platform. If location has ' ' in name, input location wrapped with double quotes: --location "LOCATION NAME"
 
 additional (optional) arguments:
-  -ota_upgrade         Updating FW version to latest for all devices
+  -ota         Updating FW version to latest for all devices
   -no_gp_zone          don't use Global pacing group by zone (all bridges will be GPG=0)
   -pacing_interval PACING_INTERVAL
                         Pacing interval for all devices
   -ignore_bridges [IGNORE_BRIDGES [IGNORE_BRIDGES ...]]
                         bridges to ignore in the tool - their configuration won't be changed
   -expected_num_brgs EXPECTED_NUM_BRGS
                         Number of expected bridges in location. The tool will try to connect to all bridges (excluding those specified in ignore bridges) until reaching expected number.
@@ -125,14 +125,17 @@
 ------------------
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.0.4:
+* Bugfixes, add relevant printouts to CLI to help understand errors.
+
 Version 4.0.3:
 * Initial release of CLI tools suite - Automatic Configuration Tool, Firmware Update, Power Management, Log Viewer.
 
 Version 4.0.0:
 * First version
```

### Comparing `wiliot-deployment-tools-4.0.3/bitbucket-pipelines.yml` & `wiliot-deployment-tools-4.0.4/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.3/ci.py` & `wiliot-deployment-tools-4.0.4/ci.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.3/setup.py` & `wiliot-deployment-tools-4.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,29 +36,29 @@
                      "Operating System :: OS Independent",
                  ],
                  packages=packages,
                 #  add all support files to the installation
                 #  package_data={"": ["*.*"]},
                  install_requires=[
                      'setuptools_scm==7.1.0',
-                     'wiliot-core',
-                     'wiliot-api',
+                     'wiliot-core==4.0.9',
+                     'wiliot-api==4.1.2',
                      'bitstruct==8.17.0',
                      'bokeh==2.4.1',
                      'boto3==1.26.77',
                      'colorama==0.4.6',
                      'jsonpickle==3.0.1',
                      'numpy==1.24.2',
                      'pandas==1.5.3',
                      'plotly==5.13.0',
                      'pytz==2022.7.1',
-                     'requests',
-                     'setuptools',
-                     'setuptools_scm',
-                     'tabulate',
+                     'requests==2.28.1',
+                     'setuptools==65.6.3',
+                     'setuptools_scm==7.1.0',
+                     'tabulate==0.8.10',
                      'backports.zoneinfo==0.2.1',
                      'tinytuya==1.10.2',
                      'pyserial==3.5',
                      'GitPython==3.1.31',
                      'tzdata==2023.3'
                  ],
                  zip_safe=False,
```

### Comparing `wiliot-deployment-tools-4.0.3/unittests/test_extended_api_edge.py` & `wiliot-deployment-tools-4.0.4/unittests/test_extended_api_edge.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.3/unittests/test_extended_api_platform.py` & `wiliot-deployment-tools-4.0.4/unittests/test_extended_api_platform.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.3/unittests/test_power_mgmt.py` & `wiliot-deployment-tools-4.0.4/unittests/test_power_mgmt.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.3/unittests/test_slack_alerts.py` & `wiliot-deployment-tools-4.0.4/unittests/test_slack_alerts.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.3/unittests/test_test_tool.py` & `wiliot-deployment-tools-4.0.4/unittests/test_test_tool.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.3/unittests/test_utils.py` & `wiliot-deployment-tools-4.0.4/unittests/test_utils.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/api/extended_api.py` & `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/api/extended_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # External Imports
 import pandas as pd
 import math
+import pytz
 from requests import JSONDecodeError
 from enum import Enum
 from time import sleep
 import datetime
 import random
 import urllib.parse
 
@@ -265,15 +266,15 @@
             res = self._post(path, payload)
             return res['data'].lower().find("ok") != -1
         except WiliotCloudError as e:
             print("Failed to send action to gateway")
             raise WiliotCloudError(
                 "Failed to send action to gateway. Received the following error: {}".format(e.args[0]))
 
-    def send_bridge_action_through_gw(self, gateway_id, action_type, payload, bridge_id=None, broadcast=False, reps=8):
+    def send_bridge_action_through_gw(self, gateway_id, action_type, payload='0', bridge_id=None, broadcast=False, reps=8):
         """
         Send an action to a bridge through a gateway
         :param broadcast:
         :param gateway_id: String - the ID of the gateway to send the action Through
         :param bridge_id: String - the ID of the bridge to send the action to
         :param action_type: BridgeThroughGatewayAction - Required
         :param payload: 28 bytes (hex string)
@@ -362,17 +363,20 @@
         prints gateway logs nicely
         :type gateway_id: str
         :param gateway_id: Gateway ID
         """
         logs = self.get_gateway_logs(gateway_id)
         logs = logs.reindex(index=logs.index[::-1])
         logs = logs.reset_index()
+        datetime_format = "%Y-%m-%dT%H:%M:%SZ"
 
         for row in logs.itertuples():
-            print(f'---Log No. {row.Index} | {row.level} | {row.timestamp}---')
+            timestamp = datetime.datetime.strptime(row.timestamp, datetime_format).replace(tzinfo=pytz.UTC).timestamp()
+            local_datetime = datetime.datetime.fromtimestamp(timestamp)
+            print(f'---Log No. {row.Index} | {row.level} | {local_datetime}---')
             print(f'*{row.message}')
             print(f'')
     
     def get_gateway_info(self, gateway_id):
         """
         get gateway info from gateway
         :param gateway_id: Gateway ID
@@ -978,7 +982,14 @@
         :return: list of brgs in location
         :rtype: list
         """
         location_id = self.get_location_id(location_name)
         loc_associations = self.get_location_associations(location_id)
         brgs_list = [assoc['associationValue'] for assoc in loc_associations if (assoc['associationType'] == 'bridge')]
         return brgs_list
+
+    def get_locations_names(self):
+        locations = super().get_locations()
+        names = []
+        for loc in locations:
+            names.append(loc['name'])
+        return names
```

### Comparing `wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/api/gw_ssid.py` & `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/api/gw_ssid.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py` & `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,17 @@
         self.use_gp_zone = use_gp_zone
         self.region = region
         if region in list(ATC_REGION_DICT.keys()):
             debug_print(f'Initialized region {region}')
 
         self.location_id = self.plat.get_location_id(self.location)
         if self.location_id is None:
-            raise ConfigurationToolError(f'No location named {self.location} Found!')
+            locations = self.plat.get_locations_names()
+            raise ConfigurationToolError(f'No location named {self.location} Found! Available locations: {locations}')
+            
         
         # Get bridges from location
         debug_print(f'Getting bridges from location {self.location}...')
         self.expected_bridges_dicts = self.plat.get_locations_bridges([self.location])
         self.expected_bridges_ids = [brg['bridgeId'] for brg in self.expected_bridges_dicts]
         self.expected_bridges_ids = list(set(self.expected_bridges_ids) - set(self.ignore_bridges))
         if not len(self.expected_bridges_ids) > 0:
```

### Comparing `wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py` & `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from argparse import ArgumentParser
 from wiliot_core import check_user_config_is_ok
 
 
 def main():
     parser = ArgumentParser(prog='wlt-config', 
                             description='Automatic Configuration Tool - CLI Tool to automatically configure Wiliot deployments',
-                            epilog='example usage: wlt-config -owner wiliot -location "My Deployment" -ota_upgrade -pacing_interval 10 -ignore_bridges 1234ABCD0123')
+                            epilog='example usage: wlt-config -owner wiliot -location "My Deployment" -ota -pacing_interval 10 -ignore_bridges 1234ABCD0123')
     
     # Required Arguments
     required = parser.add_argument_group('required arguments')
     required.add_argument("-owner", type=str, help="Platform owner id", required=True)
     required.add_argument("-location", type=str, help="Location name in Wiliot platform. If location has ' ' in name, input location wrapped with double quotes: -location \"LOCATION NAME\" ", required=True)
     
     # Optional Arguments
```

### Comparing `wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/common/analysis_data_bricks.py` & `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/common/analysis_data_bricks.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/common/debug.py` & `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/common/debug.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/common/utils.py` & `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/common/utils.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/common/utils_defines.py` & `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/common/utils_defines.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/firmware_update/firmware_update.py` & `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/firmware_update/firmware_update.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/firmware_update/firmware_update_cli.py` & `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/firmware_update/firmware_update_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,16 @@
                                required=False)
     parser_update.add_argument('-gw', nargs='+', help="Gateways to update (multiple allowed)", required=False)
     parser_update.add_argument('-brg', nargs='+', help="Bridges to update (multiple allowed)", required=False)
     parser_update.add_argument('-all_brgs', action='store_true', help="Update all bridges connected to Gateways", required=False)
     parser_update.add_argument('-ignore_bridges', nargs='+', required=False, help='Bridges to ignore')
     parser_update.add_argument('-action', action='store_true', help="Update using action API",
                                required=False)
-    parser_update.add_argument('-force', action='store_true',
-                               help='update bridge even if its already in desired version (applicable only with -action)')
+    # parser_update.add_argument('-force', action='store_true',
+    #                            help='update bridge even if its already in desired version (applicable only with -action)')
 
     if len(sys.argv) == 1:
         parser.print_help(sys.stderr)
         sys.exit(1)
         
     args = parser.parse_args()
     if args.test:
@@ -67,16 +67,16 @@
     args.fw.firmware_update(gws_list=args.gw,
                              brgs_to_update=args.brg,
                              update_all_connected_bridges=args.all_brgs,
                              desired_version=args.version,
                              update_to_latest=args.latest,
                              include_beta=args.beta,
                              ignore_bridges=args.ignore_bridges,
-                             action=args.action,
-                             force_update=args.force)
+                             action=args.action)
+                            #  force_update=args.force)
 
 def print_versions(args):
     args.fw.print_available_versions(args.beta)
 
 def main_cli():
     main()
```

### Comparing `wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/log_viewer/log_viewer_cli.py` & `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/log_viewer/log_viewer_cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,41 +9,41 @@
                             description='Log Viewer - CLI Tool to view Wiliot Gateway logs')
     required = parser.add_argument_group('required arguments')
     required.add_argument('-owner', type=str, help="Owner ID", required=True)
     required.add_argument('-gw', type=str, help="Gateway ID", required=True)
     parser.add_argument('-test', action='store_true',
                     help='If flag used, use test environment (prod is used by default)')
 
-    args = parser.parse_args()
-    if args.t:
+    args = parser.parse_args(
+        ['-owner', '832742983939', '-gw', 'GW98F4AB14DB4C'])
+    if args.test:
         env = 'test'
     else:
         env = 'prod'
 
-    owner_id = args.o
+    owner_id = args.owner
     conf_env = env if env == 'prod' else 'non-prod'
     user_config_file_path, api_key, is_success = check_user_config_is_ok(owner_id, conf_env, 'edge')
     if is_success:
         print('credentials saved/upload from {}'.format(user_config_file_path))
     else:
         raise Exception('invalid credentials - please try again to login')
 
     colorama.init()
     print(colorama.Fore.LIGHTBLACK_EX, end=None)
     print(colorama.Fore.GREEN +
           f'---Printing info for {args.gw}---' + colorama.Style.RESET_ALL)
     print(colorama.Style.RESET_ALL)
-    e = ExtendedEdgeClient(api_key, args.o, env)
+    e = ExtendedEdgeClient(api_key, args.owner, env)
     try:
         print_gw(e, args.gw)
     except AttributeError:
         parser.print_help()
 
 def print_gw(e, gw):
-    logs = e.get_gateway_logs(gw)
     info = e.get_gateway_info(gw)
 
     print(colorama.Fore.GREEN +
         f'---Gateway Info---' + colorama.Style.RESET_ALL)
     pprint.pprint(info)
     print()
     print(colorama.Fore.GREEN +
```

### Comparing `wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py` & `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/power_mgmt/power_mgmt.py` & `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/power_mgmt/power_mgmt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime
+from doctest import debug
 import sys
 import time
 import bitstruct
 from wiliot_deployment_tools.api.extended_api import BridgeThroughGatewayAction, ExtendedEdgeClient, GatewayType
 from wiliot_deployment_tools.common.debug import debug_print
 from wiliot_deployment_tools.common.utils_defines import KEEP_ALIVE_PERIOD, KEEP_ALIVE_SCAN_DURATION, SEC_TO_SEND, BROADCAST_DST_MAC, EXIT_POWER_MGMT_GW_DICT
 
@@ -162,21 +163,25 @@
         checks if gateway is compatible to send and receive power management configurations
         :type gateway_id: str
         :param gateway_id: gateway ID
         :rtype: bool
         """
         gateway_type = self.get_gateway_type(gateway_id)
         if gateway_type != GatewayType.WIFI:
+            debug_print(gateway_type)
             return False
         gw_dict = self.get_gateway(gateway_id)        
         ble_ver = gw_dict["reportedConf"]["bleChipSwVersion"]
         if gw_dict['online'] and \
            self.check_ble_power_mgmt_support(ble_ver):
             if gw_dict['reportedConf']['additional']['gwMgmtMode'] == 'transparent':
-                return self.check_gw_ble_transparent_power_mgmt_support(ble_ver)
+                support = self.check_gw_ble_transparent_power_mgmt_support(ble_ver)
+                if not support:
+                    debug_print(f'Please update GW {gateway_id} or change to active mode for power management support!')
+                return support
             return True
         return False
 
 
     def get_bridge_relevant_gw(self, bridge_id):
         """
         Returns relevant GW for sending actions to bridge
@@ -195,18 +200,16 @@
                 continue
             gw_id = gw['gatewayId']
             gw_dict = self.get_gateway(gw_id)
             if gw['connected'] and \
                     bridge_id in self.get_seen_bridges(gw_id) and \
                     self.check_gw_compatible_for_pwr_mgmt(gw_id):
                 if bridge_id in self.get_seen_bridges(gw['gatewayId']):
-                    potential_gws.append(gw['gatewayId'])
-        if len(potential_gws) == 0:
-            raise PowerManagementError(f'No relevant GW connected to bridge! Check deployment')
-        return potential_gws[0]
+                            return gw['gatewayId']
+        raise PowerManagementError(f'No relevant GW connected to bridge! Check deployment')
 
     def get_relevant_bridges(self, gateway_id):
         """
         Returns seen bridges by gateway that are associated to owner and have ble version with power management support
         :type gateway_id: str
         :param gateway_id: gateway ID
         :rtype: list
```

### Comparing `wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py` & `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from argparse import ArgumentParser
 import sys
 
 
 def main():
     # parser
     parser = ArgumentParser(prog='wlt-power-mgmt',
-                            usage='%(prog)s -o OwnerID -brg BridgeID (-t) [mode]',
                             description='Power Management - CLI Tool for using Wiliot Bridge power management functionality')
     required = parser.add_argument_group('required arguments')
     required.add_argument('-owner', type=str, help="Owner ID", required=True)
     parser.add_argument('-brg', type=str, help="Bridge ID", required=True)
     parser.add_argument('-test', action='store_true',
                         help='if flag used, use test environment (prod is used by default)')
 
@@ -39,22 +38,23 @@
 
 
     if len(sys.argv) == 1:
         parser.print_help(sys.stderr)
         sys.exit(1)
 
     args, unknown = parser.parse_known_args()
-    if args.t:
+    if args.test:
         env = 'test'
     else:
         env = 'prod'
-    owner_id = args.o
+    owner_id = args.owner
 
-
-    user_config_file_path, api_key, is_success = check_user_config_is_ok(owner_id, env, 'edge')
+    conf_env = env if env == 'prod' else 'non-prod'
+    user_config_file_path, api_key, is_success = check_user_config_is_ok(
+        owner_id, conf_env, 'edge')
     if is_success:
         print('credentials saved/upload from {}'.format(user_config_file_path))
     else:
         raise Exception('invalid credentials - please try again to login')
 
     args.pm = PowerManagementClient(api_key, owner_id, env)
     args.func(args)
```

### Comparing `wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/utils/get_version.py` & `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/utils/get_version.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.3/wiliot_deployment_tools.egg-info/PKG-INFO` & `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-deployment-tools
-Version: 4.0.3
+Version: 4.0.4
 Summary: A library for interacting with Wiliot's Deployment Tools
 Home-page: 
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Classifier: Programming Language :: Python :: 3
@@ -31,22 +31,22 @@
 
 ## Using wiliot-deployment-tools
 This package includes the following CLI Utilities:
 ### Automatic Configuration Tool
 Automatically connects to all Gateways / Bridges in the location specified, and configure them to optimal parameters.
 
 ```
-usage: wlt-config -owner OWNER -location LOCATION [-ota_upgrade] [-no_gp_zone] [-pacing_interval PACING_INTERVAL] [-ignore_bridges [IGNORE_BRIDGES [IGNORE_BRIDGES ...]]] [--expected_num_brgs EXPECTED_NUM_BRGS]
+usage: wlt-config -owner OWNER -location LOCATION [-ota] [-no_gp_zone] [-pacing_interval PACING_INTERVAL] [-ignore_bridges [IGNORE_BRIDGES [IGNORE_BRIDGES ...]]] [--expected_num_brgs EXPECTED_NUM_BRGS]
 
 required arguments:
   -owner OWNER         Platform owner id
   -location LOCATION   Location name in Wiliot platform. If location has ' ' in name, input location wrapped with double quotes: --location "LOCATION NAME"
 
 additional (optional) arguments:
-  -ota_upgrade         Updating FW version to latest for all devices
+  -ota         Updating FW version to latest for all devices
   -no_gp_zone          don't use Global pacing group by zone (all bridges will be GPG=0)
   -pacing_interval PACING_INTERVAL
                         Pacing interval for all devices
   -ignore_bridges [IGNORE_BRIDGES [IGNORE_BRIDGES ...]]
                         bridges to ignore in the tool - their configuration won't be changed
   -expected_num_brgs EXPECTED_NUM_BRGS
                         Number of expected bridges in location. The tool will try to connect to all bridges (excluding those specified in ignore bridges) until reaching expected number.
@@ -141,14 +141,17 @@
 ------------------
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.0.4:
+* Bugfixes, add relevant printouts to CLI to help understand errors.
+
 Version 4.0.3:
 * Initial release of CLI tools suite - Automatic Configuration Tool, Firmware Update, Power Management, Log Viewer.
 
 Version 4.0.0:
 * First version
```

### Comparing `wiliot-deployment-tools-4.0.3/wiliot_deployment_tools.egg-info/SOURCES.txt` & `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 wiliot_deployment_tools/common/analysis_data_bricks.py
 wiliot_deployment_tools/common/debug.py
 wiliot_deployment_tools/common/utils.py
 wiliot_deployment_tools/common/utils_defines.py
 wiliot_deployment_tools/firmware_update/__init__.py
 wiliot_deployment_tools/firmware_update/firmware_update.py
 wiliot_deployment_tools/firmware_update/firmware_update_cli.py
+wiliot_deployment_tools/log_viewer/__init__.py
 wiliot_deployment_tools/log_viewer/log_viewer_cli.py
 wiliot_deployment_tools/power_mgmt/__init__.py
 wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py
 wiliot_deployment_tools/power_mgmt/power_mgmt.py
 wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py
 wiliot_deployment_tools/utils/__init__.py
 wiliot_deployment_tools/utils/get_version.py
```

