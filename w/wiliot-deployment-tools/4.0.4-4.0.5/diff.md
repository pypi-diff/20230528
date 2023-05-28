# Comparing `tmp/wiliot-deployment-tools-4.0.4.tar.gz` & `tmp/wiliot-deployment-tools-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-deployment-tools-4.0.4.tar", last modified: Sun May 28 07:05:40 2023, max compression
+gzip compressed data, was "wiliot-deployment-tools-4.0.5.tar", last modified: Sun May 28 12:18:09 2023, max compression
```

## Comparing `wiliot-deployment-tools-4.0.4.tar` & `wiliot-deployment-tools-4.0.5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 07:05:40.224493 wiliot-deployment-tools-4.0.4/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 07:05:40.208492 wiliot-deployment-tools-4.0.4/.devcontainer/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 07:05:40.212493 wiliot-deployment-tools-4.0.4/.devcontainer/private/
--rw-rw-rw-   0 root         (0) root         (0)     1043 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/.devcontainer/private/devcontainer.json
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 07:05:40.212493 wiliot-deployment-tools-4.0.4/.devcontainer/public/
--rw-rw-rw-   0 root         (0) root         (0)     1057 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/.devcontainer/public/devcontainer.json
--rw-rw-rw-   0 root         (0) root         (0)      321 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5159 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     7307 2023-05-28 07:05:40.224493 wiliot-deployment-tools-4.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6816 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)     8812 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)     2625 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/ci.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/dep-tools-public.dockerfile
--rw-rw-rw-   0 root         (0) root         (0)      577 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/dep-tools.dockerfile
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-28 07:05:40.224493 wiliot-deployment-tools-4.0.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3457 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 07:05:40.216493 wiliot-deployment-tools-4.0.4/unittests/
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/unittests/test_debug_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2250 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/unittests/test_extended_api_edge.py
--rw-rw-rw-   0 root         (0) root         (0)     1196 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/unittests/test_extended_api_platform.py
--rw-rw-rw-   0 root         (0) root         (0)     2045 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/unittests/test_power_mgmt.py
--rw-rw-rw-   0 root         (0) root         (0)     2710 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/unittests/test_slack_alerts.py
--rw-rw-rw-   0 root         (0) root         (0)     1607 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/unittests/test_test_tool.py
--rw-rw-rw-   0 root         (0) root         (0)     2129 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/unittests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 07:05:40.216493 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 07:05:40.216493 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    41989 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/api/extended_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1187 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/api/gw_ssid.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 07:05:40.220493 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/automatic_configuration_tool/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/automatic_configuration_tool/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15257 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py
--rw-rw-rw-   0 root         (0) root         (0)     3178 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 07:05:40.220493 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/common/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    68575 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/common/analysis_data_bricks.py
--rw-rw-rw-   0 root         (0) root         (0)     2310 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/common/debug.py
--rw-rw-rw-   0 root         (0) root         (0)     6004 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/common/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3112 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/common/utils_defines.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 07:05:40.220493 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/firmware_update/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/firmware_update/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23066 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/firmware_update/firmware_update.py
--rw-rw-rw-   0 root         (0) root         (0)     4348 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/firmware_update/firmware_update_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 07:05:40.220493 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/log_viewer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/log_viewer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1956 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/log_viewer/log_viewer_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 07:05:40.224493 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/power_mgmt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/power_mgmt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4653 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py
--rw-rw-rw-   0 root         (0) root         (0)    26335 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/power_mgmt/power_mgmt.py
--rw-rw-rw-   0 root         (0) root         (0)     4143 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 07:05:40.224493 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6057 2023-05-28 07:05:18.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-28 07:05:40.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 07:05:40.216493 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     7307 2023-05-28 07:05:40.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2061 2023-05-28 07:05:40.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-28 07:05:40.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      345 2023-05-28 07:05:40.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-28 07:05:40.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      362 2023-05-28 07:05:40.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-28 07:05:40.000000 wiliot-deployment-tools-4.0.4/wiliot_deployment_tools.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 12:18:09.551898 wiliot-deployment-tools-4.0.5/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 12:18:09.539898 wiliot-deployment-tools-4.0.5/.devcontainer/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 12:18:09.543898 wiliot-deployment-tools-4.0.5/.devcontainer/private/
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/.devcontainer/private/devcontainer.json
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 12:18:09.543898 wiliot-deployment-tools-4.0.5/.devcontainer/public/
+-rw-rw-rw-   0 root         (0) root         (0)     1057 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/.devcontainer/public/devcontainer.json
+-rw-rw-rw-   0 root         (0) root         (0)      321 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     7307 2023-05-28 12:18:09.551898 wiliot-deployment-tools-4.0.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6816 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     8812 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2625 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/ci.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/dep-tools-public.dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)      577 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/dep-tools.dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-28 12:18:09.551898 wiliot-deployment-tools-4.0.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3457 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 12:18:09.543898 wiliot-deployment-tools-4.0.5/unittests/
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/unittests/test_debug_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2250 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/unittests/test_extended_api_edge.py
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/unittests/test_extended_api_platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     2045 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/unittests/test_power_mgmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     2710 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/unittests/test_slack_alerts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/unittests/test_test_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     2129 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/unittests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 12:18:09.543898 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 12:18:09.547898 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    41989 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/api/extended_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1187 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/api/gw_ssid.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 12:18:09.547898 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/automatic_configuration_tool/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/automatic_configuration_tool/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15257 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     3178 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 12:18:09.547898 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/common/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    68575 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/common/analysis_data_bricks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2310 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/common/debug.py
+-rw-rw-rw-   0 root         (0) root         (0)     6004 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/common/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3112 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/common/utils_defines.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 12:18:09.547898 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/firmware_update/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/firmware_update/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23066 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/firmware_update/firmware_update.py
+-rw-rw-rw-   0 root         (0) root         (0)     4348 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/firmware_update/firmware_update_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 12:18:09.547898 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/log_viewer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/log_viewer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1896 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/log_viewer/log_viewer_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 12:18:09.547898 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/power_mgmt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/power_mgmt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4653 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py
+-rw-rw-rw-   0 root         (0) root         (0)    26335 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/power_mgmt/power_mgmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     4143 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 12:18:09.547898 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6057 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-28 12:18:09.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 12:18:09.547898 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     7307 2023-05-28 12:18:09.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2061 2023-05-28 12:18:09.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-28 12:18:09.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      345 2023-05-28 12:18:09.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-28 12:18:09.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      362 2023-05-28 12:18:09.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-28 12:18:09.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools.egg-info/top_level.txt
```

### Comparing `wiliot-deployment-tools-4.0.4/.devcontainer/private/devcontainer.json` & `wiliot-deployment-tools-4.0.5/.devcontainer/private/devcontainer.json`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.4/.devcontainer/public/devcontainer.json` & `wiliot-deployment-tools-4.0.5/.devcontainer/public/devcontainer.json`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.4/LICENSE` & `wiliot-deployment-tools-4.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.4/PKG-INFO` & `wiliot-deployment-tools-4.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-deployment-tools
-Version: 4.0.4
+Version: 4.0.5
 Summary: A library for interacting with Wiliot's Deployment Tools
 Home-page: 
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wiliot-deployment-tools-4.0.4/README.md` & `wiliot-deployment-tools-4.0.5/README.md`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.4/bitbucket-pipelines.yml` & `wiliot-deployment-tools-4.0.5/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.4/ci.py` & `wiliot-deployment-tools-4.0.5/ci.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.4/dep-tools.dockerfile` & `wiliot-deployment-tools-4.0.5/dep-tools.dockerfile`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.4/setup.py` & `wiliot-deployment-tools-4.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.4/unittests/test_extended_api_edge.py` & `wiliot-deployment-tools-4.0.5/unittests/test_extended_api_edge.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.4/unittests/test_extended_api_platform.py` & `wiliot-deployment-tools-4.0.5/unittests/test_extended_api_platform.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.4/unittests/test_power_mgmt.py` & `wiliot-deployment-tools-4.0.5/unittests/test_power_mgmt.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.4/unittests/test_slack_alerts.py` & `wiliot-deployment-tools-4.0.5/unittests/test_slack_alerts.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.4/unittests/test_test_tool.py` & `wiliot-deployment-tools-4.0.5/unittests/test_test_tool.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.4/unittests/test_utils.py` & `wiliot-deployment-tools-4.0.5/unittests/test_utils.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/api/extended_api.py` & `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/api/extended_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/api/gw_ssid.py` & `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/api/gw_ssid.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py` & `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py` & `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/common/analysis_data_bricks.py` & `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/common/analysis_data_bricks.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/common/debug.py` & `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/common/debug.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/common/utils.py` & `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/common/utils.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/common/utils_defines.py` & `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/common/utils_defines.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/firmware_update/firmware_update.py` & `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/firmware_update/firmware_update.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/firmware_update/firmware_update_cli.py` & `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/firmware_update/firmware_update_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/log_viewer/log_viewer_cli.py` & `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/log_viewer/log_viewer_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,16 +9,15 @@
                             description='Log Viewer - CLI Tool to view Wiliot Gateway logs')
     required = parser.add_argument_group('required arguments')
     required.add_argument('-owner', type=str, help="Owner ID", required=True)
     required.add_argument('-gw', type=str, help="Gateway ID", required=True)
     parser.add_argument('-test', action='store_true',
                     help='If flag used, use test environment (prod is used by default)')
 
-    args = parser.parse_args(
-        ['-owner', '832742983939', '-gw', 'GW98F4AB14DB4C'])
+    args = parser.parse_args()
     if args.test:
         env = 'test'
     else:
         env = 'prod'
 
     owner_id = args.owner
     conf_env = env if env == 'prod' else 'non-prod'
```

### Comparing `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py` & `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/power_mgmt/power_mgmt.py` & `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/power_mgmt/power_mgmt.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py` & `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools/utils/get_version.py` & `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/utils/get_version.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools.egg-info/PKG-INFO` & `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-deployment-tools
-Version: 4.0.4
+Version: 4.0.5
 Summary: A library for interacting with Wiliot's Deployment Tools
 Home-page: 
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wiliot-deployment-tools-4.0.4/wiliot_deployment_tools.egg-info/SOURCES.txt` & `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

