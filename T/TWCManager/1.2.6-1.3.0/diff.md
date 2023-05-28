# Comparing `tmp/TWCManager-1.2.6.tar.gz` & `tmp/TWCManager-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/TWCManager-1.2.6.tar", last modified: Tue Mar  1 10:08:18 2022, max compression
+gzip compressed data, was "/__w/TWCManager/TWCManager/dist/.tmp-8ds4mo2u/TWCManager-1.3.0.tar", last modified: Sun May 28 05:09:09 2023, max compression
```

## Comparing `TWCManager-1.2.6.tar` & `TWCManager-1.3.0.tar`

### file list

```diff
@@ -1,98 +1,101 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 10:08:17.000000 TWCManager-1.2.6/
--rw-r--r--   0 root         (0) root         (0)       72 2022-03-01 10:00:57.000000 TWCManager-1.2.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      344 2022-03-01 10:08:17.000000 TWCManager-1.2.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9241 2022-03-01 10:00:57.000000 TWCManager-1.2.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 10:08:17.000000 TWCManager-1.2.6/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 10:08:17.000000 TWCManager-1.2.6/lib/TWCManager/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 10:08:17.000000 TWCManager-1.2.6/lib/TWCManager/Control/
--rw-r--r--   0 root         (0) root         (0)    54214 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/HTTPControl.py
--rw-r--r--   0 root         (0) root         (0)     4648 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/MQTTControl.py
--rw-r--r--   0 root         (0) root         (0)    19780 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/WebIPCControl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 10:08:17.000000 TWCManager-1.2.6/lib/TWCManager/Control/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 10:08:17.000000 TWCManager-1.2.6/lib/TWCManager/Control/static/css/
--rw-r--r--   0 root         (0) root         (0)      118 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/static/css/styles.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 10:08:17.000000 TWCManager-1.2.6/lib/TWCManager/Control/static/js/
--rw-r--r--   0 root         (0) root         (0)       79 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/static/js/commonUI.js
--rw-r--r--   0 root         (0) root         (0)     1156 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/static/js/debug.js
--rw-r--r--   0 root         (0) root         (0)     2062 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/static/js/settings.js
--rw-r--r--   0 root         (0) root         (0)      742 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/static/js/status.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 10:08:17.000000 TWCManager-1.2.6/lib/TWCManager/Control/themes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 10:08:17.000000 TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/
--rw-r--r--   0 root         (0) root         (0)     1151 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/bootstrap.html.j2
--rw-r--r--   0 root         (0) root         (0)     4883 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/debug.html.j2
--rw-r--r--   0 root         (0) root         (0)     3696 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/drawChart.html.j2
--rw-r--r--   0 root         (0) root         (0)      736 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/graphs.html.j2
--rw-r--r--   0 root         (0) root         (0)     1118 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/handle_teslalogin.html.j2
--rw-r--r--   0 root         (0) root         (0)     2493 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/jsrefresh.html.j2
--rw-r--r--   0 root         (0) root         (0)     1061 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/main.html.j2
--rw-r--r--   0 root         (0) root         (0)     1302 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/navbar.html.j2
--rw-r--r--   0 root         (0) root         (0)      165 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/policy.html.j2
--rw-r--r--   0 root         (0) root         (0)     1406 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/request_teslalogin.html.j2
--rw-r--r--   0 root         (0) root         (0)     3633 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/schedule.html.j2
--rw-r--r--   0 root         (0) root         (0)     5612 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/settings.html.j2
--rw-r--r--   0 root         (0) root         (0)     1327 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/showCommands.html.j2
--rw-r--r--   0 root         (0) root         (0)     4642 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/showStatus.html.j2
--rw-r--r--   0 root         (0) root         (0)       35 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/upgrade.html.j2
--rw-r--r--   0 root         (0) root         (0)      736 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/upgradePrompt.html.j2
--rw-r--r--   0 root         (0) root         (0)     4420 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/vehicleDetail.html.j2
--rw-r--r--   0 root         (0) root         (0)     2313 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/vehicles.html.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 10:08:17.000000 TWCManager-1.2.6/lib/TWCManager/Control/themes/Modern/
--rw-r--r--   0 root         (0) root         (0)      574 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/themes/Modern/bootstrap.js.html.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 10:08:17.000000 TWCManager-1.2.6/lib/TWCManager/Control/themes/Modern/css/
--rw-r--r--   0 root         (0) root         (0)      927 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/themes/Modern/css/styles.css
--rw-r--r--   0 root         (0) root         (0)     5410 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/themes/Modern/jsrefresh.html.j2
--rw-r--r--   0 root         (0) root         (0)    26177 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/themes/Modern/main.html.j2
--rw-r--r--   0 root         (0) root         (0)      559 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Control/themes/Modern/master.html.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 10:08:17.000000 TWCManager-1.2.6/lib/TWCManager/EMS/
--rw-r--r--   0 root         (0) root         (0)      903 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/EMS/DSMR.py
--rw-r--r--   0 root         (0) root         (0)     3385 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/EMS/Efergy.py
--rw-r--r--   0 root         (0) root         (0)     5275 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/EMS/EmonCMS.py
--rw-r--r--   0 root         (0) root         (0)     5370 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/EMS/Enphase.py
--rw-r--r--   0 root         (0) root         (0)     5438 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/EMS/Fronius.py
--rw-r--r--   0 root         (0) root         (0)     5271 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/EMS/Growatt.py
--rw-r--r--   0 root         (0) root         (0)     5433 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/EMS/HASS.py
--rw-r--r--   0 root         (0) root         (0)     5193 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/EMS/IotaWatt.py
--rw-r--r--   0 root         (0) root         (0)     6666 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/EMS/Kostal.py
--rw-r--r--   0 root         (0) root         (0)     5470 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/EMS/OpenHab.py
--rw-r--r--   0 root         (0) root         (0)     7133 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/EMS/OpenWeatherMap.py
--rw-r--r--   0 root         (0) root         (0)    11381 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/EMS/P1Monitor.py
--rw-r--r--   0 root         (0) root         (0)     4694 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/EMS/SmartMe.py
--rw-r--r--   0 root         (0) root         (0)     5260 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/EMS/SmartPi.py
--rw-r--r--   0 root         (0) root         (0)     9719 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/EMS/SolarEdge.py
--rw-r--r--   0 root         (0) root         (0)     7354 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/EMS/SolarLog.py
--rw-r--r--   0 root         (0) root         (0)     3429 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/EMS/TED.py
--rw-r--r--   0 root         (0) root         (0)    11466 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/EMS/TeslaPowerwall2.py
--rw-r--r--   0 root         (0) root         (0)     4913 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/EMS/URL.py
--rw-r--r--   0 root         (0) root         (0)     6820 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/EMS/Volkszahler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 10:08:17.000000 TWCManager-1.2.6/lib/TWCManager/Interface/
--rw-r--r--   0 root         (0) root         (0)     4551 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Interface/Dummy.py
--rw-r--r--   0 root         (0) root         (0)     3519 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Interface/RS485.py
--rw-r--r--   0 root         (0) root         (0)     2971 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Interface/TCP.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 10:08:17.000000 TWCManager-1.2.6/lib/TWCManager/Logging/
--rw-r--r--   0 root         (0) root         (0)     7732 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Logging/CSVLogging.py
--rw-r--r--   0 root         (0) root         (0)     2226 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Logging/ConsoleLogging.py
--rw-r--r--   0 root         (0) root         (0)     2148 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Logging/FileLogging.py
--rw-r--r--   0 root         (0) root         (0)    12067 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Logging/MySQLLogging.py
--rw-r--r--   0 root         (0) root         (0)     8420 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Logging/SQLiteLogging.py
--rw-r--r--   0 root         (0) root         (0)     1873 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Logging/SentryLogging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 10:08:17.000000 TWCManager-1.2.6/lib/TWCManager/Policy/
--rw-r--r--   0 root         (0) root         (0)    14552 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Policy/Policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 10:08:17.000000 TWCManager-1.2.6/lib/TWCManager/Protocol/
--rw-r--r--   0 root         (0) root         (0)     6714 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Protocol/TWCProtocol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 10:08:17.000000 TWCManager-1.2.6/lib/TWCManager/Status/
--rw-r--r--   0 root         (0) root         (0)     7374 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Status/HASSStatus.py
--rw-r--r--   0 root         (0) root         (0)     6648 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Status/MQTTStatus.py
--rwxr-xr-x   0 root         (0) root         (0)    70780 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/TWCManager.py
--rw-r--r--   0 root         (0) root         (0)    61141 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/TWCMaster.py
--rw-r--r--   0 root         (0) root         (0)    58158 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/TWCSlave.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 10:08:17.000000 TWCManager-1.2.6/lib/TWCManager/Vehicle/
--rw-r--r--   0 root         (0) root         (0)    63563 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Vehicle/TeslaAPI.py
--rw-r--r--   0 root         (0) root         (0)     9851 2022-03-01 10:00:58.000000 TWCManager-1.2.6/lib/TWCManager/Vehicle/TeslaMateVehicle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 10:08:17.000000 TWCManager-1.2.6/lib/TWCManager.egg-info/
--rw-r--r--   0 root         (0) root         (0)      344 2022-03-01 10:08:12.000000 TWCManager-1.2.6/lib/TWCManager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3085 2022-03-01 10:08:14.000000 TWCManager-1.2.6/lib/TWCManager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-01 10:08:12.000000 TWCManager-1.2.6/lib/TWCManager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      282 2022-03-01 10:08:12.000000 TWCManager-1.2.6/lib/TWCManager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-03-01 10:08:12.000000 TWCManager-1.2.6/lib/TWCManager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-03-01 10:08:17.000000 TWCManager-1.2.6/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1031 2022-03-01 10:00:58.000000 TWCManager-1.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 05:09:09.000000 TWCManager-1.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1210 2022-01-26 10:44:23.000000 TWCManager-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       72 2022-01-26 10:44:23.000000 TWCManager-1.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      426 2023-05-28 05:09:09.000000 TWCManager-1.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9336 2023-05-28 04:51:43.000000 TWCManager-1.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 05:09:09.000000 TWCManager-1.3.0/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 05:09:09.000000 TWCManager-1.3.0/lib/TWCManager/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 05:09:09.000000 TWCManager-1.3.0/lib/TWCManager/Control/
+-rw-r--r--   0 root         (0) root         (0)    56228 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/Control/HTTPControl.py
+-rw-r--r--   0 root         (0) root         (0)     4646 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/Control/MQTTControl.py
+-rw-r--r--   0 root         (0) root         (0)    19778 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/Control/WebIPCControl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 05:09:09.000000 TWCManager-1.3.0/lib/TWCManager/Control/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 05:09:09.000000 TWCManager-1.3.0/lib/TWCManager/Control/static/css/
+-rw-r--r--   0 root         (0) root         (0)      118 2022-01-26 10:44:23.000000 TWCManager-1.3.0/lib/TWCManager/Control/static/css/styles.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 05:09:09.000000 TWCManager-1.3.0/lib/TWCManager/Control/static/js/
+-rw-r--r--   0 root         (0) root         (0)       79 2022-01-26 10:44:23.000000 TWCManager-1.3.0/lib/TWCManager/Control/static/js/commonUI.js
+-rw-r--r--   0 root         (0) root         (0)     1156 2022-01-26 10:44:23.000000 TWCManager-1.3.0/lib/TWCManager/Control/static/js/debug.js
+-rw-r--r--   0 root         (0) root         (0)     2062 2022-01-26 10:44:23.000000 TWCManager-1.3.0/lib/TWCManager/Control/static/js/settings.js
+-rw-r--r--   0 root         (0) root         (0)      742 2022-01-26 10:44:23.000000 TWCManager-1.3.0/lib/TWCManager/Control/static/js/status.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 05:09:09.000000 TWCManager-1.3.0/lib/TWCManager/Control/themes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 05:09:09.000000 TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/
+-rw-r--r--   0 root         (0) root         (0)     1151 2022-01-26 10:44:23.000000 TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/bootstrap.html.j2
+-rw-r--r--   0 root         (0) root         (0)     4883 2022-02-25 04:03:23.000000 TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/debug.html.j2
+-rw-r--r--   0 root         (0) root         (0)     3696 2022-01-26 10:44:23.000000 TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/drawChart.html.j2
+-rw-r--r--   0 root         (0) root         (0)      736 2022-01-26 10:44:23.000000 TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/graphs.html.j2
+-rw-r--r--   0 root         (0) root         (0)     1118 2022-02-25 04:03:23.000000 TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/handle_teslalogin.html.j2
+-rw-r--r--   0 root         (0) root         (0)     2493 2022-01-26 10:44:23.000000 TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/jsrefresh.html.j2
+-rw-r--r--   0 root         (0) root         (0)     1061 2022-01-26 10:44:23.000000 TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/main.html.j2
+-rw-r--r--   0 root         (0) root         (0)     1302 2022-03-01 09:52:44.000000 TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/navbar.html.j2
+-rw-r--r--   0 root         (0) root         (0)      165 2022-01-26 10:44:23.000000 TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/policy.html.j2
+-rw-r--r--   0 root         (0) root         (0)     1406 2022-02-25 04:03:23.000000 TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/request_teslalogin.html.j2
+-rw-r--r--   0 root         (0) root         (0)     3633 2022-01-26 10:44:23.000000 TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/schedule.html.j2
+-rw-r--r--   0 root         (0) root         (0)     8080 2023-05-27 16:51:47.000000 TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/settings.html.j2
+-rw-r--r--   0 root         (0) root         (0)     1327 2022-01-26 10:44:23.000000 TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/showCommands.html.j2
+-rw-r--r--   0 root         (0) root         (0)     4642 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/showStatus.html.j2
+-rw-r--r--   0 root         (0) root         (0)       35 2022-03-01 09:52:44.000000 TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/upgrade.html.j2
+-rw-r--r--   0 root         (0) root         (0)      736 2022-03-01 09:52:44.000000 TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/upgradePrompt.html.j2
+-rw-r--r--   0 root         (0) root         (0)     4420 2022-01-26 10:44:23.000000 TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/vehicleDetail.html.j2
+-rw-r--r--   0 root         (0) root         (0)     2313 2022-01-26 10:44:23.000000 TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/vehicles.html.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 05:09:09.000000 TWCManager-1.3.0/lib/TWCManager/Control/themes/Modern/
+-rw-r--r--   0 root         (0) root         (0)      750 2022-03-01 12:03:52.000000 TWCManager-1.3.0/lib/TWCManager/Control/themes/Modern/bootstrap.js.html.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 05:09:09.000000 TWCManager-1.3.0/lib/TWCManager/Control/themes/Modern/css/
+-rw-r--r--   0 root         (0) root         (0)      927 2022-01-26 10:44:23.000000 TWCManager-1.3.0/lib/TWCManager/Control/themes/Modern/css/styles.css
+-rw-r--r--   0 root         (0) root         (0)     8122 2022-04-22 00:51:48.000000 TWCManager-1.3.0/lib/TWCManager/Control/themes/Modern/jsrefresh.html.j2
+-rw-r--r--   0 root         (0) root         (0)    26501 2023-05-27 16:51:47.000000 TWCManager-1.3.0/lib/TWCManager/Control/themes/Modern/main.html.j2
+-rw-r--r--   0 root         (0) root         (0)      441 2022-03-01 12:03:52.000000 TWCManager-1.3.0/lib/TWCManager/Control/themes/Modern/master.html.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 05:09:09.000000 TWCManager-1.3.0/lib/TWCManager/EMS/
+-rw-r--r--   0 root         (0) root         (0)      902 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/EMS/DSMR.py
+-rw-r--r--   0 root         (0) root         (0)     5348 2023-05-27 19:42:44.000000 TWCManager-1.3.0/lib/TWCManager/EMS/DSMRreader.py
+-rw-r--r--   0 root         (0) root         (0)     3380 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/EMS/Efergy.py
+-rw-r--r--   0 root         (0) root         (0)     5272 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/EMS/EmonCMS.py
+-rw-r--r--   0 root         (0) root         (0)     5365 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/EMS/Enphase.py
+-rw-r--r--   0 root         (0) root         (0)     5432 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/EMS/Fronius.py
+-rw-r--r--   0 root         (0) root         (0)     5267 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/EMS/Growatt.py
+-rw-r--r--   0 root         (0) root         (0)     5430 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/EMS/HASS.py
+-rw-r--r--   0 root         (0) root         (0)     5190 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/EMS/IotaWatt.py
+-rw-r--r--   0 root         (0) root         (0)     6665 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/EMS/Kostal.py
+-rw-r--r--   0 root         (0) root         (0)     4368 2023-05-27 14:19:19.000000 TWCManager-1.3.0/lib/TWCManager/EMS/MQTT.py
+-rw-r--r--   0 root         (0) root         (0)     5471 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/EMS/OpenHab.py
+-rw-r--r--   0 root         (0) root         (0)     7129 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/EMS/OpenWeatherMap.py
+-rw-r--r--   0 root         (0) root         (0)    11375 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/EMS/P1Monitor.py
+-rw-r--r--   0 root         (0) root         (0)     4691 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/EMS/SmartMe.py
+-rw-r--r--   0 root         (0) root         (0)     5257 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/EMS/SmartPi.py
+-rw-r--r--   0 root         (0) root         (0)    15245 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/EMS/SolarEdge.py
+-rw-r--r--   0 root         (0) root         (0)     7351 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/EMS/SolarLog.py
+-rw-r--r--   0 root         (0) root         (0)     3424 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/EMS/TED.py
+-rw-r--r--   0 root         (0) root         (0)    11458 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/EMS/TeslaPowerwall2.py
+-rw-r--r--   0 root         (0) root         (0)     4910 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/EMS/URL.py
+-rw-r--r--   0 root         (0) root         (0)     6815 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/EMS/Volkszahler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 05:09:09.000000 TWCManager-1.3.0/lib/TWCManager/Interface/
+-rw-r--r--   0 root         (0) root         (0)     4550 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/Interface/Dummy.py
+-rw-r--r--   0 root         (0) root         (0)     4063 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/Interface/RS485.py
+-rw-r--r--   0 root         (0) root         (0)     2970 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/Interface/TCP.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 05:09:09.000000 TWCManager-1.3.0/lib/TWCManager/Logging/
+-rw-r--r--   0 root         (0) root         (0)     7731 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/Logging/CSVLogging.py
+-rw-r--r--   0 root         (0) root         (0)     2457 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/Logging/ConsoleLogging.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/Logging/FileLogging.py
+-rw-r--r--   0 root         (0) root         (0)    12065 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/Logging/MySQLLogging.py
+-rw-r--r--   0 root         (0) root         (0)     8418 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/Logging/SQLiteLogging.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/Logging/SentryLogging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 05:09:09.000000 TWCManager-1.3.0/lib/TWCManager/Policy/
+-rw-r--r--   0 root         (0) root         (0)    15601 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/Policy/Policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 05:09:09.000000 TWCManager-1.3.0/lib/TWCManager/Protocol/
+-rw-r--r--   0 root         (0) root         (0)     6711 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/Protocol/TWCProtocol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 05:09:09.000000 TWCManager-1.3.0/lib/TWCManager/Status/
+-rw-r--r--   0 root         (0) root         (0)     7372 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/Status/HASSStatus.py
+-rw-r--r--   0 root         (0) root         (0)     6697 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/Status/MQTTStatus.py
+-rwxr-xr-x   0 root         (0) root         (0)    74675 2023-05-27 19:42:44.000000 TWCManager-1.3.0/lib/TWCManager/TWCManager.py
+-rw-r--r--   0 root         (0) root         (0)    61768 2023-05-27 19:42:44.000000 TWCManager-1.3.0/lib/TWCManager/TWCMaster.py
+-rw-r--r--   0 root         (0) root         (0)    59050 2023-05-27 16:51:47.000000 TWCManager-1.3.0/lib/TWCManager/TWCSlave.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 05:09:09.000000 TWCManager-1.3.0/lib/TWCManager/Vehicle/
+-rw-r--r--   0 root         (0) root         (0)    64120 2023-05-27 16:51:47.000000 TWCManager-1.3.0/lib/TWCManager/Vehicle/TeslaAPI.py
+-rw-r--r--   0 root         (0) root         (0)     9842 2023-05-27 06:35:34.000000 TWCManager-1.3.0/lib/TWCManager/Vehicle/TeslaMateVehicle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 05:09:09.000000 TWCManager-1.3.0/lib/TWCManager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      426 2023-05-28 05:09:09.000000 TWCManager-1.3.0/lib/TWCManager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3153 2023-05-28 05:09:09.000000 TWCManager-1.3.0/lib/TWCManager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 05:09:09.000000 TWCManager-1.3.0/lib/TWCManager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      306 2023-05-28 05:09:09.000000 TWCManager-1.3.0/lib/TWCManager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-28 05:09:09.000000 TWCManager-1.3.0/lib/TWCManager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-28 05:09:09.000000 TWCManager-1.3.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1205 2023-05-28 04:51:43.000000 TWCManager-1.3.0/setup.py
```

### Comparing `TWCManager-1.2.6/README.md` & `TWCManager-1.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # TWCManager
 
-[![Stable Release](https://img.shields.io/badge/Stable_Release-1.2.6-blue)](https://github.com/ngardiner/TWCManager/releases/tag/v1.2.6)
-[![Development Release](https://img.shields.io/badge/Devel_Release-1.3.0-green.svg)](https://github.com/ngardiner/TWCManager/tree/main)
+[![Stable Release](https://img.shields.io/badge/Stable_Release-1.3.0-blue)](https://github.com/ngardiner/TWCManager/releases/tag/v1.3.0)
+[![Development Release](https://img.shields.io/badge/Devel_Release-1.3.1-green.svg)](https://github.com/ngardiner/TWCManager/tree/main)
 ![Build Status](https://github.com/ngardiner/TWCManager/actions/workflows/test_suite.yml/badge.svg)
 ![GitHub commits](https://img.shields.io/github/commit-activity/m/ngardiner/TWCManager)
 ![Docker Pulls](https://img.shields.io/docker/pulls/twcmanager/twcmanager.svg)
 ![Contributors](https://img.shields.io/github/contributors/ngardiner/TWCManager)
 
 ## Screenshots
 ![Screenshot](docs/screenshot.png)
@@ -51,14 +51,15 @@
 ### EMS Interfaces
 
 EMS Interfaces read solar generation and/or consumption values from an external system. Current EMS interfaces are:
 
 | Platform                      | Status        | Details                 |
 | ----------------------------- | ------------- | ----------------------- |
 | Dutch SmartMeter | In Development | Supports DSMR Serial Protocol |
+| [DSMReader](docs/modules/DMS_DSMReader.md)      | Available | Supports DSM Reader via MQTT |
 | [Efergy](docs/modules/EMS_Efergy.md)            | Available | Supports Efergy Pro Sensors |
 | [Enphase](docs/modules/EMS_Enphase.md)          | Available | Supports Enphase Enlighten API |
 | [Fronius Inverter](docs/modules/EMS_Fronius.md) | Available | Supports Fronius Inverter API |
 | [Growatt](docs/modules/EMS_Growatt.md)          | Available | Support for Growatt Battery systems |
 | [HomeAssistant](docs/modules/EMS_HASS.md)       | Available | Supports HomeAssistant sensors |
 | [IoTaWatt](docs/modules/EMS_Iotawatt.md)       | Available | Supports Iotawatt outputs |
 | [Kostal (Pico/Plenticore)](docs/modules/EMS_Kostal.md) | Available | Support for Kostal Inverters via ModBus |
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/Control/HTTPControl.py` & `TWCManager-1.3.0/lib/TWCManager/Control/HTTPControl.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     configConfig = {}
     configHTTP = {}
     httpPort = 8080
     master = None
     status = False
 
     def __init__(self, master):
-
         self.master = master
         try:
             self.configConfig = master.config["config"]
         except KeyError:
             self.configConfig = {}
         try:
             self.configHTTP = master.config["control"]["HTTP"]
@@ -74,21 +73,27 @@
         post_data = ""
         templateEnv = None
         templateLoader = None
         timeList = []
         url = None
 
         def __init__(self, *args, **kwargs):
-
             # Populate ampsList so that any function which requires a list of supported
             # TWC amps can easily access it
             if not len(self.ampsList):
                 self.ampsList.append([0, "Disabled"])
                 for amp in range(
-                    5, (master.config["config"].get("wiringMaxAmpsPerTWC", 5)) + 1
+                    master.config["config"].get("minAmpsPerTWC", 5),
+                    (
+                        master.config["config"].get(
+                            "wiringMaxAmpsPerTWC",
+                            master.config["config"].get("minAmpsPerTWC", 5),
+                        )
+                    )
+                    + 1,
                 ):
                     self.ampsList.append([amp, str(amp) + "A"])
 
             # Populate list of hours
             if not len(self.hoursDurationList):
                 for hour in range(1, 25):
                     self.hoursDurationList.append([(hour * 3600), str(hour) + "h"])
@@ -335,14 +340,26 @@
 
                 json_data = json.dumps(data)
                 try:
                     self.wfile.write(json_data.encode("utf-8"))
                 except BrokenPipeError:
                     self.debugLogAPI("Connection Error: Broken Pipe")
 
+            elif self.url.path == "/api/getActivePolicyAction":
+                data = master.getModuleByName("Policy").getActivePolicyAction()
+                self.send_response(200)
+                self.send_header("Content-type", "application/json")
+                self.end_headers()
+
+                json_data = json.dumps(data)
+                try:
+                    self.wfile.write(json_data.encode("utf-8"))
+                except BrokenPipeError:
+                    self.debugLogAPI("Connection Error: Broken Pipe")
+
             elif self.url.path == "/api/getHistory":
                 output = []
                 now = datetime.now().replace(second=0, microsecond=0).astimezone()
                 startTime = now - timedelta(days=2) + timedelta(minutes=5)
                 endTime = now.replace(minute=math.floor(now.minute / 5) * 5)
                 startTime = startTime.replace(
                     minute=math.floor(startTime.minute / 5) * 5
@@ -394,15 +411,14 @@
                 self.send_response(404)
                 self.end_headers()
                 self.wfile.write("".encode("utf-8"))
 
             self.debugLogAPI("Ending API GET")
 
         def do_API_POST(self):
-
             self.debugLogAPI("Starting API POST")
 
             if self.url.path == "/api/addConsumptionOffset":
                 data = {}
                 try:
                     data = json.loads(self.post_data.decode("UTF-8"))
                 except (ValueError, UnicodeDecodeError):
@@ -497,15 +513,14 @@
                     del master.settings["consumptionOffset"][name]
 
                     self.send_response(204)
                     self.end_headers()
                     self.wfile.write("".encode("utf-8"))
 
                 else:
-
                     self.send_response(400)
                     self.end_headers()
                     self.wfile.write("".encode("utf-8"))
 
             elif self.url.path == "/api/saveSettings":
                 master.queue_background_task({"cmd": "saveSettings"})
                 self.send_response(204)
@@ -726,14 +741,16 @@
                 self.do_API_GET()
                 return
 
             webroutes = [
                 {"route": "/debug", "tmpl": "debug.html.j2"},
                 {"route": "/schedule", "tmpl": "schedule.html.j2"},
                 {"route": "/settings", "tmpl": "settings.html.j2"},
+                {"route": "/settings/homeLocation", "error": "insecure"},
+                {"route": "/settings/save", "error": "insecure"},
                 {"route": "/teslaAccount/saveToken", "error": "insecure"},
                 {"rstart": "/teslaAccount", "tmpl": "main.html.j2"},
                 {"route": "/upgradePrompt", "tmpl": "upgradePrompt.html.j2"},
                 {"rstart": "/vehicleDetail", "tmpl": "vehicleDetail.html.j2"},
                 {"route": "/vehicles", "tmpl": "vehicles.html.j2"},
             ]
 
@@ -748,14 +765,18 @@
                 # Set some values that we use within the template
                 # Check if we're able to access the Tesla API
                 self.apiAvailable = master.getModuleByName(
                     "TeslaAPI"
                 ).car_api_available()
                 self.scheduledAmpsMax = master.getScheduledAmpsMax()
 
+                self.activeAction = master.getModuleByName(
+                    "Policy"
+                ).getActivePolicyAction()
+
                 # Send the html message
                 page = self.template.render(vars(self))
 
                 self.wfile.write(page.encode("utf-8"))
                 return
 
             # Match web routes to defined webroutes routing
@@ -765,15 +786,14 @@
                     route = webroute
                     break
                 elif self.url.path.startswith(webroute.get("rstart", "INVALID")):
                     route = webroute
                     break
 
             if route and route.get("error", None):
-
                 if route["error"] == "insecure":
                     # For security, these details should be submitted via a POST request
                     # Send a 405 Method Not Allowed in response.
                     self.send_response(405)
                     page = (
                         "This function may only be requested via the POST HTTP method."
                     )
@@ -885,15 +905,14 @@
                 self.process_graphs(inicio, fin)
                 return
 
             # All other routes missed, return 404
             self.send_response(404)
 
         def do_POST(self):
-
             # Parse URL
             self.url = urllib.parse.urlparse(self.path)
 
             # Parse POST parameters
             self.fields.clear()
             length = int(self.headers.get("content-length"))
             self.post_data = self.rfile.read(length)
@@ -913,14 +932,19 @@
                 return
 
             if self.url.path == "/schedule/save":
                 # User has submitted schedule.
                 self.process_save_schedule()
                 return
 
+            if self.url.path == "/settings/homeLocation":
+                # User making changes to home location
+                self.process_home_location()
+                return
+
             if self.url.path == "/settings/save":
                 # User has submitted settings.
                 # Call dedicated function
                 self.process_save_settings()
                 return
 
             if self.url.path == "/graphs/dates":
@@ -930,25 +954,23 @@
 
                 if not objIni or not objEnd:
                     # Redirect back to graphs page if no Start or End time supplied
                     self.send_response(302)
                     self.send_header("Location", "/graphs")
 
                 else:
-
                     self.process_save_graphs(objIni, objEnd)
                     self.send_response(302)
                     self.send_header("Location", "/graphsP")
 
                 self.end_headers()
                 self.wfile.write("".encode("utf-8"))
                 return
 
             if self.url.path == "/teslaAccount/saveToken":
-
                 # Check if we are skipping Tesla Login submission
                 later = False
                 try:
                     later = len(self.fields["later"][0])
                 except KeyError:
                     later = False
 
@@ -956,26 +978,24 @@
                 url = self.getFieldValue("url")
 
                 if later:
                     master.teslaLoginAskLater = True
                     res = "later"
 
                 else:
-
                     res = master.getModuleByName("TeslaAPI").saveApiToken(url)
 
                 self.send_response(302)
                 self.send_header("Location", "/teslaAccount/" + res)
 
                 self.end_headers()
                 self.wfile.write("".encode("utf-8"))
                 return
 
             if self.url.path == "/vehicle/groupMgmt":
-
                 group = self.getFieldValue("group")
                 op = self.getFieldValue("operation")
                 vin = self.getFieldValue("vin")
 
                 if op == "add":
                     try:
                         master.settings["VehicleGroups"][group]["Members"].append(vin)
@@ -1028,15 +1048,14 @@
                 extrargs,
                 button_def[0],
                 button_def[1],
             )
             return page
 
         def chargeScheduleDay(self, day):
-
             # Fetch current settings
             sched = master.settings.get("Schedule", {})
             today = sched.get(day, {})
             suffix = day + "ChargeTime"
 
             # Render daily schedule options
             page = "<tr>"
@@ -1112,16 +1131,37 @@
                     sel,
                     option[1],
                 )
             page += "</select>"
             page += "</div>"
             return page
 
-        def process_save_schedule(self):
+        def process_home_location(self):
+            # If unset was selected, unset account
+            if "unset" in self.fields:
+                del master.settings["homeLat"]
+                del master.settings["homeLon"]
+
+            # If learn was selected, learn location
+            if "learn" in self.fields:
+                loc = self.getFieldValue("vehicle").split(",")
+                master.setHomeLon(loc[0])
+                master.setHomeLat(loc[1])
+
+            # Save Settings
+            master.queue_background_task({"cmd": "saveSettings"})
 
+            # Redirect to the index page
+            self.send_response(302)
+            self.send_header("Location", "/")
+            self.end_headers()
+            self.wfile.write("".encode("utf-8"))
+            return
+
+        def process_save_schedule(self):
             # Check that schedule dict exists within settings.
             # If not, this would indicate that this is the first time
             # we have saved the new schedule settings
             if master.settings.get("Schedule", None) == None:
                 master.settings["Schedule"] = {}
 
             # Slight issue with checkboxes, you have to default them all to
@@ -1208,20 +1248,18 @@
             self.send_response(302)
             self.send_header("Location", "/")
             self.end_headers()
             self.wfile.write("".encode("utf-8"))
             return
 
         def process_save_settings(self, page="settings"):
-
             # This function will write the settings submitted from the settings
             # page to the settings dict, before triggering a write of the settings
             # to file
             for key in self.fields:
-
                 # If the key relates to the car API tokens, we need to pass these
                 # to the appropriate module, rather than directly updating the
                 # configuration file (as it would just be overwritten)
                 if (
                     key == "carApiBearerToken" or key == "carApiRefreshToken"
                 ) and self.getFieldValue(key) != "":
                     carapi = master.getModuleByName("TeslaAPI")
@@ -1230,15 +1268,14 @@
                         # New tokens expire after 8 hours
                         carapi.setCarApiTokenExpireTime(time.time() + 8 * 60 * 60)
                     elif key == "carApiRefreshToken":
                         carapi.setCarApiRefreshToken(self.getFieldValue(key))
                         carapi.setCarApiTokenExpireTime(time.time() + 45 * 24 * 60 * 60)
 
                 else:
-
                     # Write setting to dictionary
                     master.settings[key] = self.getFieldValue(key)
 
             # If Non-Scheduled power action is either Do not Charge or
             # Track Green Energy, set Non-Scheduled power rate to 0
             if int(master.settings.get("nonScheduledAction", 1)) > 1:
                 master.settings["nonScheduledAmpsMax"] = 0
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/Control/MQTTControl.py` & `TWCManager-1.3.0/lib/TWCManager/Control/MQTTControl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 
 logger = logging.getLogger("\U0001F3AE MQTT")
 
 
 class MQTTControl:
-
     import paho.mqtt.client as mqtt
     import _thread
 
     brokerIP = None
     brokerPort = 1883
     __client = None
     config = None
@@ -77,15 +76,14 @@
     def mqttConnect(self, client, userdata, flags, rc):
         logger.log(logging.INFO5, "MQTT Connected.")
         logger.log(logging.INFO5, "Subscribe to " + self.topicPrefix + "/#")
         res = self.__client.subscribe(self.topicPrefix + "/#", qos=0)
         logger.log(logging.INFO5, "Res: " + str(res))
 
     def mqttMessage(self, client, userdata, message):
-
         # Takes an MQTT message which has a message body of the following format:
         # [Amps to charge at],[Seconds to charge for]
         # eg. 24,3600
         if message.topic == self.topicPrefix + "/control/chargeNow":
             payload = str(message.payload.decode("utf-8"))
             logger.log(
                 logging.INFO3, "MQTT Message called chargeNow with payload " + payload
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/Control/WebIPCControl.py` & `TWCManager-1.3.0/lib/TWCManager/Control/WebIPCControl.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import time
 import math
 
 logger = logging.getLogger(__name__.rsplit(".")[-1])
 
 
 class WebIPCControl:
-
     config = None
     configConfig = None
     configIPC = None
     debugLevel = 0
     master = None
     webIPCkey = None
     webIPCqueue = None
@@ -94,15 +93,14 @@
 
         if len(s) > makeLen:
             s = s[0:makeLen]
 
         return s
 
     def processIPC(self):
-
         ########################################################################
         # See if there's any message from the web interface.
         # If the message is longer than msgMaxSize, MSG_NOERROR tells it to
         # return what it can of the message and discard the rest.
         # When no message is available, IPC_NOWAIT tells msgrcv to return
         # msgResult = 0 and $! = 42 with description 'No message of desired
         # type'.
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/Control/static/js/debug.js` & `TWCManager-1.3.0/lib/TWCManager/Control/static/js/debug.js`

 * *Files identical despite different names*

### Comparing `TWCManager-1.2.6/lib/TWCManager/Control/static/js/settings.js` & `TWCManager-1.3.0/lib/TWCManager/Control/static/js/settings.js`

 * *Files identical despite different names*

### Comparing `TWCManager-1.2.6/lib/TWCManager/Control/static/js/status.js` & `TWCManager-1.3.0/lib/TWCManager/Control/static/js/status.js`

 * *Files identical despite different names*

### Comparing `TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/bootstrap.html.j2` & `TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/bootstrap.html.j2`

 * *Files identical despite different names*

### Comparing `TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/debug.html.j2` & `TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/debug.html.j2`

 * *Files identical despite different names*

### Comparing `TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/drawChart.html.j2` & `TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/drawChart.html.j2`

 * *Files identical despite different names*

### Comparing `TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/graphs.html.j2` & `TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/graphs.html.j2`

 * *Files identical despite different names*

### Comparing `TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/handle_teslalogin.html.j2` & `TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/handle_teslalogin.html.j2`

 * *Files identical despite different names*

### Comparing `TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/jsrefresh.html.j2` & `TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/jsrefresh.html.j2`

 * *Files identical despite different names*

### Comparing `TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/main.html.j2` & `TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/main.html.j2`

 * *Files identical despite different names*

### Comparing `TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/navbar.html.j2` & `TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/navbar.html.j2`

 * *Files identical despite different names*

### Comparing `TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/request_teslalogin.html.j2` & `TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/request_teslalogin.html.j2`

 * *Files identical despite different names*

### Comparing `TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/schedule.html.j2` & `TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/schedule.html.j2`

 * *Files identical despite different names*

### Comparing `TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/showCommands.html.j2` & `TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/showCommands.html.j2`

 * *Files identical despite different names*

### Comparing `TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/showStatus.html.j2` & `TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/showStatus.html.j2`

 * *Files identical despite different names*

### Comparing `TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/upgradePrompt.html.j2` & `TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/upgradePrompt.html.j2`

 * *Files identical despite different names*

### Comparing `TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/vehicleDetail.html.j2` & `TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/vehicleDetail.html.j2`

 * *Files identical despite different names*

### Comparing `TWCManager-1.2.6/lib/TWCManager/Control/themes/Default/vehicles.html.j2` & `TWCManager-1.3.0/lib/TWCManager/Control/themes/Default/vehicles.html.j2`

 * *Files identical despite different names*

### Comparing `TWCManager-1.2.6/lib/TWCManager/Control/themes/Modern/css/styles.css` & `TWCManager-1.3.0/lib/TWCManager/Control/themes/Modern/css/styles.css`

 * *Files identical despite different names*

### Comparing `TWCManager-1.2.6/lib/TWCManager/Control/themes/Modern/main.html.j2` & `TWCManager-1.3.0/lib/TWCManager/Control/themes/Modern/main.html.j2`

 * *Files 8% similar despite different names*

```diff
@@ -1,138 +1,161 @@
 {% extends "master.html.j2" %}
 {% block pagetitle %}TWCManager - Home{% endblock %}
 {% block content %}
     <! -- TODO -->
-    <table border='0' padding='0' margin='0' width='100%'>
-      <tr width='100%'>
-        <td valign='top' width='70%'>
+    <table border='0' style="padding='0'; margin='0'; width='100%';">
+      <tr style="width='100%';">
+        <td style="valign='top'; width='70%';">
           {% include 'handle_teslalogin.html.j2' %}
           {% if master.lastSaveFailed %}
              <font color=red>
                <b>We experienced an error trying to save your settings. This mea
 ns that while your current settings will be retained for the current session, th
 ey will not be saved if TWCManager exits. Please check the permissions on /etc/t
 wcmanager/settings.json and try saving your settings again.</b>
              </font>
           {% endif %}
         </td>
       </tr>
     </table>
 
 <!-- Home -->
-<div class="container-fluid pt-2">
+<div class="container-fluid pt-xl-3">
     <div class="row border-bottom mb-4">
         <h1 class="display-4">Home</h1>
     </div>
 
-    <div class="row justify-content-center">
-        <div class="col-sm-12 col-md-3 col-lg-3 mb-5 mb-md-0">
-            <div class="row justify-content-center">
-                <div>
-                    Generation
-                </div>
-                <div class="float-left ml-2" style="margin-top: -2px;">
-                    <svg width="1.5em" height="1.5em" viewBox="0 0 16 16" class="card-img-top bi bi-sun" fill="orange" xmlns="http://www.w3.org/2000/svg">
-                        <path d="M3.5 8a4.5 4.5 0 1 1 9 0 4.5 4.5 0 0 1-9 0z"/>
-                        <path fill-rule="evenodd" d="M8.202.28a.25.25 0 0 0-.404 0l-.91 1.255a.25.25 0 0 1-.334.067L5.232.79a.25.25 0 0 0-.374.155l-.36 1.508a.25.25 0 0 1-.282.19l-1.532-.245a.25.25 0 0 0-.286.286l.244 1.532a.25.25 0 0 1-.189.282l-1.509.36a.25.25 0 0 0-.154.374l.812 1.322a.25.25 0 0 1-.067.333l-1.256.91a.25.25 0 0 0 0 .405l1.256.91a.25.25 0 0 1 .067.334L.79 10.768a.25.25 0 0 0 .154.374l1.51.36a.25.25 0 0 1 .188.282l-.244 1.532a.25.25 0 0 0 .286.286l1.532-.244a.25.25 0 0 1 .282.189l.36 1.508a.25.25 0 0 0 .374.155l1.322-.812a.25.25 0 0 1 .333.067l.91 1.256a.25.25 0 0 0 .405 0l.91-1.256a.25.25 0 0 1 .334-.067l1.322.812a.25.25 0 0 0 .374-.155l.36-1.508a.25.25 0 0 1 .282-.19l1.532.245a.25.25 0 0 0 .286-.286l-.244-1.532a.25.25 0 0 1 .189-.282l1.508-.36a.25.25 0 0 0 .155-.374l-.812-1.322a.25.25 0 0 1 .067-.333l1.256-.91a.25.25 0 0 0 0-.405l-1.256-.91a.25.25 0 0 1-.067-.334l.812-1.322a.25.25 0 0 0-.155-.374l-1.508-.36a.25.25 0 0 1-.19-.282l.245-1.532a.25.25 0 0 0-.286-.286l-1.532.244a.25.25 0 0 1-.282-.189l-.36-1.508a.25.25 0 0 0-.374-.155l-1.322.812a.25.25 0 0 1-.333-.067L8.203.28zM8 2.5a5.5 5.5 0 1 0 0 11 5.5 5.5 0 0 0 0-11z"/>
-                    </svg>
+    <!-- main information row -->
+    <div class="d-flex flex-column flex-md-row flex-md-wrap justify-content-sm-between">
+        <!-- show solar generation -->
+        <div class="bd-highlight col-12 col-md-6 col-lg-3">
+            <div class="d-flex flex-column">
+                <div class="d-flex flex-row justify-content-center align-items-center">
+                    <div class="p-1">Generation</div>
+                    <div class="p-1">
+                        <svg width="1.5em" height="1.5em" viewBox="0 0 16 16" class="card-img-top bi bi-sun" fill="orange" xmlns="http://www.w3.org/2000/svg">
+                            <path d="M3.5 8a4.5 4.5 0 1 1 9 0 4.5 4.5 0 0 1-9 0z"/>
+                            <path fill-rule="evenodd" d="M8.202.28a.25.25 0 0 0-.404 0l-.91 1.255a.25.25 0 0 1-.334.067L5.232.79a.25.25 0 0 0-.374.155l-.36 1.508a.25.25 0 0 1-.282.19l-1.532-.245a.25.25 0 0 0-.286.286l.244 1.532a.25.25 0 0 1-.189.282l-1.509.36a.25.25 0 0 0-.154.374l.812 1.322a.25.25 0 0 1-.067.333l-1.256.91a.25.25 0 0 0 0 .405l1.256.91a.25.25 0 0 1 .067.334L.79 10.768a.25.25 0 0 0 .154.374l1.51.36a.25.25 0 0 1 .188.282l-.244 1.532a.25.25 0 0 0 .286.286l1.532-.244a.25.25 0 0 1 .282.189l.36 1.508a.25.25 0 0 0 .374.155l1.322-.812a.25.25 0 0 1 .333.067l.91 1.256a.25.25 0 0 0 .405 0l.91-1.256a.25.25 0 0 1 .334-.067l1.322.812a.25.25 0 0 0 .374-.155l.36-1.508a.25.25 0 0 1 .282-.19l1.532.245a.25.25 0 0 0 .286-.286l-.244-1.532a.25.25 0 0 1 .189-.282l1.508-.36a.25.25 0 0 0 .155-.374l-.812-1.322a.25.25 0 0 1 .067-.333l1.256-.91a.25.25 0 0 0 0-.405l-1.256-.91a.25.25 0 0 1-.067-.334l.812-1.322a.25.25 0 0 0-.155-.374l-1.508-.36a.25.25 0 0 1-.19-.282l.245-1.532a.25.25 0 0 0-.286-.286l-1.532.244a.25.25 0 0 1-.282-.189l-.36-1.508a.25.25 0 0 0-.374-.155l-1.322.812a.25.25 0 0 1-.333-.067L8.203.28zM8 2.5a5.5 5.5 0 1 0 0 11 5.5 5.5 0 0 0 0-11z"/>
+                        </svg>
+                    </div>
+                </div>
+                <div class="d-flex flex-row justify-content-center">
+                    <div class="d-flex flex-column">
+                        <div class="d-flex flex-row justify-content-center display-5 fw-light">
+                            <span id="generationWatts">0.0</span>
+                        </div>
+                        <div class="d-flex flex-row justify-content-center">
+                            <span id="generationAmps">0.00</span>&nbsp;<span class="text-muted">A</span>
+                        </div>
+                    </div>
                 </div>
             </div>
-            <div class="row justify-content-center">
-                <h1 class="meter"><span id="generationWatts">0.0</span></h1>
-            </div>
-            <div class="row justify-content-center display-watt text-muted">
-                <span id="generationAmps">0.00</span>&nbsp;A
-            </div>
         </div>
 
-        <div class="col-sm-12 col-md-3 col-lg-3 mb-5 mb-md-0">
-            <div class="row justify-content-center">
-                <div>
-                    <span class="text-danger">&#8675;</span>&nbsp;Consumption
-                </div>
-                <div class="float-left ml-2" style="margin-top: -2px;">
-                    <svg width="1.5em" height="1.5em" viewBox="0 0 16 16" class="bi bi-house" fill="dodgerblue" xmlns="http://www.w3.org/2000/svg">
-                        <path fill-rule="evenodd" d="M2 13.5V7h1v6.5a.5.5 0 0 0 .5.5h9a.5.5 0 0 0 .5-.5V7h1v6.5a1.5 1.5 0 0 1-1.5 1.5h-9A1.5 1.5 0 0 1 2 13.5zm11-11V6l-2-2V2.5a.5.5 0 0 1 .5-.5h1a.5.5 0 0 1 .5.5z"/>
-                        <path fill-rule="evenodd" d="M7.293 1.5a1 1 0 0 1 1.414 0l6.647 6.646a.5.5 0 0 1-.708.708L8 2.207 1.354 8.854a.5.5 0 1 1-.708-.708L7.293 1.5z"/>
-                    </svg>
+        <!-- show home consumption -->
+        <div class="d-highlight col-12 col-md-6 col-lg-3 mt-4 mt-lg-0">
+            <div class="d-flex flex-column">
+                <div class="d-flex flex-row justify-content-center align-items-center">
+                    <div class="p-1"><span class="text-danger">&#8675;</span>Consumption</div>
+                    <div class="p-1">
+                        <svg width="1.5em" height="1.5em" viewBox="0 0 16 16" class="bi bi-house" fill="dodgerblue" xmlns="http://www.w3.org/2000/svg">
+                            <path fill-rule="evenodd" d="M2 13.5V7h1v6.5a.5.5 0 0 0 .5.5h9a.5.5 0 0 0 .5-.5V7h1v6.5a1.5 1.5 0 0 1-1.5 1.5h-9A1.5 1.5 0 0 1 2 13.5zm11-11V6l-2-2V2.5a.5.5 0 0 1 .5-.5h1a.5.5 0 0 1 .5.5z"/>
+                            <path fill-rule="evenodd" d="M7.293 1.5a1 1 0 0 1 1.414 0l6.647 6.646a.5.5 0 0 1-.708.708L8 2.207 1.354 8.854a.5.5 0 1 1-.708-.708L7.293 1.5z"/>
+                        </svg>
+                    </div>
+                </div>
+                <div class="d-flex flex-row justify-content-center">
+                    <div class="d-flex flex-column">
+                        <div class="d-flex flex-row justify-content-center display-5 fw-light">
+                            <span id="consumptionWatts">0.0</span>
+                        </div>
+                        <div class="d-flex flex-row justify-content-center">
+                            <span id="consumptionAmps">0.00</span>&nbsp;<span class="text-muted">A</span>
+                        </div>
+                    </div>
                 </div>
             </div>
-            <div class="row justify-content-center">
-                <h1 class="meter"><span id="consumptionWatts">0.0</span></h1>
-            </div>
-            <div class="row justify-content-center display-watt text-muted">
-                <span id="consumptionAmps">0.00</span>&nbsp;A
-            </div>
         </div>
-
-
-        <div class="col-sm-12 col-md-3 col-lg-3 mb-5 mb-md-0">
-            <div class="row justify-content-center">
-                <div>
-                    Solar surplus
-                </div>
-                <div class="float-left ml-2" style="margin-top: -2px;">
-                    <svg width="1.5em" height="100%" viewBox="0 0 15 16" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" xml:space="preserve" xmlns:serif="http://www.serif.com/" style="fill-rule:evenodd;clip-rule:evenodd;stroke-linejoin:round;stroke-miterlimit:2;">
-                        <g transform="matrix(1,0,0,1,-9,-9.22827)">
-                        <g transform="matrix(0.031203,0,0,0.031203,8.71917,8.94032)">
-                            <path d="M9,522L9,499L32,499L32,476L45,476L45,176L9,176L9,152L34.5,152C56.8,152 59.9,151.8 59.4,150.5C58.5,148.2 60.8,143.4 63.3,142.3C64.5,141.8 68.5,140.5 72.2,139.5L78.8,137.6L70.7,134.2C61.8,130.6 60,129 60,125C60,120.4 62.4,118.4 71,115.9L79.2,113.6L75.8,112.4C69.7,110.3 62.3,106.1 61.6,104.5C59.3,98.3 62.1,94.7 71.4,92L78.9,89.7L71.1,86C63.1,82.1 62,80.9 62,76C62,72.2 65.3,69.8 73.5,67.5L80.2,65.7L75.3,63.6C72.6,62.4 68.8,60.5 66.7,59.3C63.4,57.3 63,56.6 63,53.1C63,47.9 64.6,46.5 73.1,43.9L80.1,41.8L72.8,38.1C64.4,34 62.4,31.1 64.1,26.2C64.8,24.1 66.3,22.7 69,21.6C79.1,17.6 102.8,12.2 120.4,9.9C128.6,8.9 129.4,8.9 131.9,10.7C133.7,12.1 134.6,13.8 134.8,16.3C135.2,21.4 132.7,23.6 125.4,24.4C116.8,25.4 96.9,29 95.6,29.7C93.4,31.1 105.1,33.2 116.5,33.4C130.4,33.7 132.3,34.1 133.8,37.6C135.5,41.2 135.3,42.6 132.8,45.4C130.9,47.5 129.1,48.1 122,48.9C110.1,50.3 95,53.2 95,54.1C95,55.6 105.8,57.3 117,57.6C123.3,57.7 128.8,57.9 129.3,57.9C131,58.1 134,62.2 134,64.4C134,68.7 130.5,71.7 124.8,72.5C114.6,73.7 95.6,77.1 94.2,77.9C91.9,79.2 104.3,81.3 116,81.6C121.8,81.8 127.1,81.9 127.8,82C130,82 133,85.9 133,88.8C133,93 129.8,95.8 124.3,96.5C112.4,98 94.4,101.2 93.7,101.9C92.3,103.3 106.4,105.3 117.8,105.4C127.4,105.5 128.3,105.7 130.1,107.9C134.4,113.1 130.9,119.5 123.2,120.5C110.3,122.1 93,125.4 93.7,126C95.2,127.4 107.7,129 117.3,129C125.7,129 127.3,129.3 129,131C131.6,133.6 131.5,138.3 128.7,141.5C126.8,143.7 125.2,144.3 118.5,145.1C110.2,146.1 88.7,150.3 83.5,151.9C81.5,152.5 93.8,152.9 119.2,152.9L157.9,153L157.4,150.2C156.5,145.6 159.8,142.6 169,140L177,137.6L168.8,134.2C159.9,130.5 158.1,128.9 158,124.8C158,120.7 160.9,118.4 169.1,116L176.4,113.8L168.3,110C160.4,106.3 159,104.9 159,100.6C159,96.5 161.6,94.4 169.7,92C174,90.7 176.8,89.5 176,89.2C172.1,88 162.4,82.7 161.3,81.3C159.6,79.1 159.7,74.9 161.4,72.4C162.3,71.1 165.9,69.4 170.7,68C175,66.7 177.8,65.5 177,65.2C173.1,64 163.4,58.7 162.3,57.3C161.6,56.4 161,54.2 161,52.4C161,48.2 164,45.8 172.2,43.5L178.5,41.8L173.2,39.4C164.2,35.4 162,33.4 162,29.1C162,26.6 162.7,24.7 163.9,23.6C167.8,20.1 194,13.4 215.4,10.5C227,8.9 227.4,8.9 229.9,10.8C231.8,12.2 232.6,13.8 232.8,16.8C233.2,22.2 231.1,23.5 220,25C208.4,26.5 194.7,29.1 193.7,30C192.1,31.5 203.5,33.3 215.1,33.6C221.5,33.7 227.7,34.1 228.8,34.4C231.9,35.4 233.5,40.3 232,44C230.5,47.6 228.7,48.1 211.5,50.4C204.9,51.3 197.7,52.5 195.5,53.2L191.5,54.3L197,55.7C200,56.5 208.3,57.4 215.4,57.7C229.6,58.4 232,59.4 232,64.8C232,69 228.8,71.8 223.3,72.5C213.3,73.7 193.4,77.2 192.1,78C189.8,79.2 207.6,82 217.8,82C228.2,82 231,83.5 231,88.9C231,94.2 228.4,95.9 219,97C208.2,98.3 194,100.9 192.2,101.9C189.8,103.3 202.8,105.3 214.9,105.4C225.5,105.6 226.4,105.7 228.1,107.9C232.2,112.9 229.4,119.4 222.8,120.4C209.5,122.3 192.5,125.1 192.1,125.5C191.9,125.8 191.9,126.2 192.1,126.4C193.2,127.5 206.4,129 215.3,129C226.3,129 229,130.4 229,136.1C229,142.5 226.1,144.4 215,145.5C207.9,146.2 185.1,150.6 181.7,152C180.4,152.5 194.6,152.9 216.8,152.9L254,153L254,149.9C254,144.6 255.5,143.2 264.6,140.4L273.2,137.7L265.7,134.6C256.1,130.6 255,129.6 255,125C255,120.2 256.8,118.7 265.8,116L273.2,113.7L266.4,110.9C258.1,107.4 255.7,105.1 255.7,101C255.7,96.8 258.2,94.7 266.3,92L273.1,89.8L265.6,86.3C257,82.2 254.9,79.2 257,74.1C258.2,71.1 259.4,70.4 268.8,67.5L274,65.8L266.2,62C258.3,58.2 257,56.9 257,52.5C257,49 260,46.4 266,44.5C269,43.6 272.2,42.6 273,42.3C273.9,42 272.1,40.7 268.4,39C265,37.5 261.3,35.3 260.1,34.1C257.5,31.5 257.4,27 259.8,24.2C262.9,20.5 290,13.4 311.9,10.6C321.7,9.3 323.7,9.3 326,10.5C330.6,12.9 331.3,17.4 327.8,21.4C325.9,23.5 324,24.1 317,25C306.4,26.3 292,29 290.1,30C287.6,31.3 298.8,33.2 312.8,33.9C327.4,34.6 329,35.3 329,41.1C329,46.3 326.3,48.1 317,49.1C307.4,50.1 293.1,52.7 289.8,53.9C286.3,55.2 303.7,58 315.1,58C326.1,58 328,59.1 328,65.2C328,70.6 326,71.7 311,73.9C303.6,75 295,76.4 292,77.1L286.5,78.3L291.5,79.7C294.3,80.5 302.6,81.4 310,81.7C325.4,82.3 327,83 327,89C327,94.6 324.8,95.9 312.6,97.5C300.1,99.1 290,101 288.1,102C285.8,103.2 298.9,105.3 310.8,105.6C324,105.9 326,106.9 326,113C326,118.3 323.6,120 314.8,121.1C303.4,122.5 289,125.2 288.5,126C287.7,127.3 300.1,129 310.7,129C322.8,129 325.4,130.3 325.4,136.5C325.4,141.3 321.5,145 316.5,145C312.2,145 292.6,148.4 283,150.9L275.5,152.8L350.7,153L350.2,150.2C349.6,145.7 353.2,142.6 362,140L369.5,137.8L361.6,134.5C353.2,131 351,129.1 351,125.2C351,120.9 352.8,119.2 359.7,117C363.5,115.8 367.2,114.6 368,114.3C369,114 368.6,113.5 366.5,112.6C353.6,107.1 352,105.7 352,100.6C352,96.9 355.1,94.3 361.7,92.4C364.9,91.5 367.9,90.5 368.4,90.2C368.9,89.9 366.4,88.4 362.9,86.8C354.5,83 353,81.5 353,77C353,72.3 354.9,70.6 362.5,68.5C365.8,67.5 368.9,66.5 369.3,66.3C369.7,66 367,64.4 363.3,62.6C355.5,58.8 353.7,57 353.7,53C353.7,48.7 356.3,46.5 363.6,44.4C367.1,43.4 370,42.2 370,41.8C370,41.5 367.9,40.4 365.4,39.4C359.8,37.3 354,32.1 354,29.2C354,24.8 358,22.1 369,18.9C384.4,14.5 402.2,11 413.1,10.3C422.4,9.7 422.7,9.8 424.3,12.1C426.5,15.1 426.5,19.2 424.3,21.9C422.9,23.6 420.6,24.3 414,25.1C404.8,26.2 386,29.7 385.3,30.4C384.2,31.5 395.8,33.2 408,33.7C415.4,34 422.1,34.7 422.9,35.3C427,38.7 426,46 421.2,47.8C419.7,48.3 414,49.3 408.5,49.9C403,50.5 395.1,51.9 391,52.8L383.5,54.6L392.5,56.3C397.5,57.2 405.9,58 411.2,58C420.4,58 420.9,58.1 422.9,60.6C425.3,63.6 425.5,64.9 423.9,68.4C422.5,71.4 419.4,72.6 411.5,73.4C408.2,73.8 400.3,75 394,76.2L382.5,78.3L387.5,79.7C390.3,80.5 398.7,81.4 406.3,81.7C419.5,82.2 420.1,82.4 422,84.8C424.5,87.9 424.5,91.1 422.3,93.9C420.8,95.7 418.5,96.3 409.3,97.6C398.6,99 384,101.7 383.3,102.4C382.4,103.3 396.8,105.3 407.8,105.9C418.5,106.4 420.4,106.8 421.6,108.4C424.3,112.2 422.5,118.2 418.1,119.8C416.7,120.4 410.1,121.5 403.5,122.4C396.9,123.3 389.7,124.5 387.5,125.1L383.5,126.3L386.5,127.2C388.2,127.7 396,128.4 403.8,128.8C417.3,129.5 418.3,129.6 420.1,131.9C423.8,136.4 421.3,143.6 415.7,144.4C397.1,147.2 385.3,149.4 379.5,150.9L372.5,152.8L416.3,152.9L460,153L460,177.2L443,176.8L426,176.5L426,476L438,476L438,499L461,499L461,522L9,522ZM239.8,380L320.7,318.5L250.3,317.5L281,267C297.9,239.2 311.6,216.3 311.4,216.2C311.3,216 274.5,243.6 229.7,277.7L148.3,339.5L183.6,339.8L218.9,340L203.3,365.8C194.7,379.9 180.8,402.9 172.3,416.8C163.8,430.8 157.4,442 157.9,441.8C158.4,441.7 195.3,413.8 239.8,380Z" style="fill:rgb(0,157,18);fill-rule:nonzero;"/>
-                        </g>
-                        </g>
-                    </svg>
+        <!-- show solar surplus generation -->
+        <div class="bd-highlight col-12 col-md-6 col-lg-3 mt-4 mt-lg-0">
+            <div class="d-flex flex-column">
+                <div class="d-flex flex-row justify-content-center align-items-center">
+                    <div class="p-1">Solar surplus</div>
+                    <div class="p-1">
+                        <svg height="100%" style="fill-rule:evenodd;clip-rule:evenodd;stroke-linejoin:round;stroke-miterlimit:2;" version="1.1" viewBox="0 0 15 16"
+                             width="1.5em" xml:space="preserve"
+                             xmlns="http://www.w3.org/2000/svg">
+                            <g transform="matrix(1,0,0,1,-9,-9.22827)">
+                            <g transform="matrix(0.031203,0,0,0.031203,8.71917,8.94032)">
+                                <path d="M9,522L9,499L32,499L32,476L45,476L45,176L9,176L9,152L34.5,152C56.8,152 59.9,151.8 59.4,150.5C58.5,148.2 60.8,143.4 63.3,142.3C64.5,141.8 68.5,140.5 72.2,139.5L78.8,137.6L70.7,134.2C61.8,130.6 60,129 60,125C60,120.4 62.4,118.4 71,115.9L79.2,113.6L75.8,112.4C69.7,110.3 62.3,106.1 61.6,104.5C59.3,98.3 62.1,94.7 71.4,92L78.9,89.7L71.1,86C63.1,82.1 62,80.9 62,76C62,72.2 65.3,69.8 73.5,67.5L80.2,65.7L75.3,63.6C72.6,62.4 68.8,60.5 66.7,59.3C63.4,57.3 63,56.6 63,53.1C63,47.9 64.6,46.5 73.1,43.9L80.1,41.8L72.8,38.1C64.4,34 62.4,31.1 64.1,26.2C64.8,24.1 66.3,22.7 69,21.6C79.1,17.6 102.8,12.2 120.4,9.9C128.6,8.9 129.4,8.9 131.9,10.7C133.7,12.1 134.6,13.8 134.8,16.3C135.2,21.4 132.7,23.6 125.4,24.4C116.8,25.4 96.9,29 95.6,29.7C93.4,31.1 105.1,33.2 116.5,33.4C130.4,33.7 132.3,34.1 133.8,37.6C135.5,41.2 135.3,42.6 132.8,45.4C130.9,47.5 129.1,48.1 122,48.9C110.1,50.3 95,53.2 95,54.1C95,55.6 105.8,57.3 117,57.6C123.3,57.7 128.8,57.9 129.3,57.9C131,58.1 134,62.2 134,64.4C134,68.7 130.5,71.7 124.8,72.5C114.6,73.7 95.6,77.1 94.2,77.9C91.9,79.2 104.3,81.3 116,81.6C121.8,81.8 127.1,81.9 127.8,82C130,82 133,85.9 133,88.8C133,93 129.8,95.8 124.3,96.5C112.4,98 94.4,101.2 93.7,101.9C92.3,103.3 106.4,105.3 117.8,105.4C127.4,105.5 128.3,105.7 130.1,107.9C134.4,113.1 130.9,119.5 123.2,120.5C110.3,122.1 93,125.4 93.7,126C95.2,127.4 107.7,129 117.3,129C125.7,129 127.3,129.3 129,131C131.6,133.6 131.5,138.3 128.7,141.5C126.8,143.7 125.2,144.3 118.5,145.1C110.2,146.1 88.7,150.3 83.5,151.9C81.5,152.5 93.8,152.9 119.2,152.9L157.9,153L157.4,150.2C156.5,145.6 159.8,142.6 169,140L177,137.6L168.8,134.2C159.9,130.5 158.1,128.9 158,124.8C158,120.7 160.9,118.4 169.1,116L176.4,113.8L168.3,110C160.4,106.3 159,104.9 159,100.6C159,96.5 161.6,94.4 169.7,92C174,90.7 176.8,89.5 176,89.2C172.1,88 162.4,82.7 161.3,81.3C159.6,79.1 159.7,74.9 161.4,72.4C162.3,71.1 165.9,69.4 170.7,68C175,66.7 177.8,65.5 177,65.2C173.1,64 163.4,58.7 162.3,57.3C161.6,56.4 161,54.2 161,52.4C161,48.2 164,45.8 172.2,43.5L178.5,41.8L173.2,39.4C164.2,35.4 162,33.4 162,29.1C162,26.6 162.7,24.7 163.9,23.6C167.8,20.1 194,13.4 215.4,10.5C227,8.9 227.4,8.9 229.9,10.8C231.8,12.2 232.6,13.8 232.8,16.8C233.2,22.2 231.1,23.5 220,25C208.4,26.5 194.7,29.1 193.7,30C192.1,31.5 203.5,33.3 215.1,33.6C221.5,33.7 227.7,34.1 228.8,34.4C231.9,35.4 233.5,40.3 232,44C230.5,47.6 228.7,48.1 211.5,50.4C204.9,51.3 197.7,52.5 195.5,53.2L191.5,54.3L197,55.7C200,56.5 208.3,57.4 215.4,57.7C229.6,58.4 232,59.4 232,64.8C232,69 228.8,71.8 223.3,72.5C213.3,73.7 193.4,77.2 192.1,78C189.8,79.2 207.6,82 217.8,82C228.2,82 231,83.5 231,88.9C231,94.2 228.4,95.9 219,97C208.2,98.3 194,100.9 192.2,101.9C189.8,103.3 202.8,105.3 214.9,105.4C225.5,105.6 226.4,105.7 228.1,107.9C232.2,112.9 229.4,119.4 222.8,120.4C209.5,122.3 192.5,125.1 192.1,125.5C191.9,125.8 191.9,126.2 192.1,126.4C193.2,127.5 206.4,129 215.3,129C226.3,129 229,130.4 229,136.1C229,142.5 226.1,144.4 215,145.5C207.9,146.2 185.1,150.6 181.7,152C180.4,152.5 194.6,152.9 216.8,152.9L254,153L254,149.9C254,144.6 255.5,143.2 264.6,140.4L273.2,137.7L265.7,134.6C256.1,130.6 255,129.6 255,125C255,120.2 256.8,118.7 265.8,116L273.2,113.7L266.4,110.9C258.1,107.4 255.7,105.1 255.7,101C255.7,96.8 258.2,94.7 266.3,92L273.1,89.8L265.6,86.3C257,82.2 254.9,79.2 257,74.1C258.2,71.1 259.4,70.4 268.8,67.5L274,65.8L266.2,62C258.3,58.2 257,56.9 257,52.5C257,49 260,46.4 266,44.5C269,43.6 272.2,42.6 273,42.3C273.9,42 272.1,40.7 268.4,39C265,37.5 261.3,35.3 260.1,34.1C257.5,31.5 257.4,27 259.8,24.2C262.9,20.5 290,13.4 311.9,10.6C321.7,9.3 323.7,9.3 326,10.5C330.6,12.9 331.3,17.4 327.8,21.4C325.9,23.5 324,24.1 317,25C306.4,26.3 292,29 290.1,30C287.6,31.3 298.8,33.2 312.8,33.9C327.4,34.6 329,35.3 329,41.1C329,46.3 326.3,48.1 317,49.1C307.4,50.1 293.1,52.7 289.8,53.9C286.3,55.2 303.7,58 315.1,58C326.1,58 328,59.1 328,65.2C328,70.6 326,71.7 311,73.9C303.6,75 295,76.4 292,77.1L286.5,78.3L291.5,79.7C294.3,80.5 302.6,81.4 310,81.7C325.4,82.3 327,83 327,89C327,94.6 324.8,95.9 312.6,97.5C300.1,99.1 290,101 288.1,102C285.8,103.2 298.9,105.3 310.8,105.6C324,105.9 326,106.9 326,113C326,118.3 323.6,120 314.8,121.1C303.4,122.5 289,125.2 288.5,126C287.7,127.3 300.1,129 310.7,129C322.8,129 325.4,130.3 325.4,136.5C325.4,141.3 321.5,145 316.5,145C312.2,145 292.6,148.4 283,150.9L275.5,152.8L350.7,153L350.2,150.2C349.6,145.7 353.2,142.6 362,140L369.5,137.8L361.6,134.5C353.2,131 351,129.1 351,125.2C351,120.9 352.8,119.2 359.7,117C363.5,115.8 367.2,114.6 368,114.3C369,114 368.6,113.5 366.5,112.6C353.6,107.1 352,105.7 352,100.6C352,96.9 355.1,94.3 361.7,92.4C364.9,91.5 367.9,90.5 368.4,90.2C368.9,89.9 366.4,88.4 362.9,86.8C354.5,83 353,81.5 353,77C353,72.3 354.9,70.6 362.5,68.5C365.8,67.5 368.9,66.5 369.3,66.3C369.7,66 367,64.4 363.3,62.6C355.5,58.8 353.7,57 353.7,53C353.7,48.7 356.3,46.5 363.6,44.4C367.1,43.4 370,42.2 370,41.8C370,41.5 367.9,40.4 365.4,39.4C359.8,37.3 354,32.1 354,29.2C354,24.8 358,22.1 369,18.9C384.4,14.5 402.2,11 413.1,10.3C422.4,9.7 422.7,9.8 424.3,12.1C426.5,15.1 426.5,19.2 424.3,21.9C422.9,23.6 420.6,24.3 414,25.1C404.8,26.2 386,29.7 385.3,30.4C384.2,31.5 395.8,33.2 408,33.7C415.4,34 422.1,34.7 422.9,35.3C427,38.7 426,46 421.2,47.8C419.7,48.3 414,49.3 408.5,49.9C403,50.5 395.1,51.9 391,52.8L383.5,54.6L392.5,56.3C397.5,57.2 405.9,58 411.2,58C420.4,58 420.9,58.1 422.9,60.6C425.3,63.6 425.5,64.9 423.9,68.4C422.5,71.4 419.4,72.6 411.5,73.4C408.2,73.8 400.3,75 394,76.2L382.5,78.3L387.5,79.7C390.3,80.5 398.7,81.4 406.3,81.7C419.5,82.2 420.1,82.4 422,84.8C424.5,87.9 424.5,91.1 422.3,93.9C420.8,95.7 418.5,96.3 409.3,97.6C398.6,99 384,101.7 383.3,102.4C382.4,103.3 396.8,105.3 407.8,105.9C418.5,106.4 420.4,106.8 421.6,108.4C424.3,112.2 422.5,118.2 418.1,119.8C416.7,120.4 410.1,121.5 403.5,122.4C396.9,123.3 389.7,124.5 387.5,125.1L383.5,126.3L386.5,127.2C388.2,127.7 396,128.4 403.8,128.8C417.3,129.5 418.3,129.6 420.1,131.9C423.8,136.4 421.3,143.6 415.7,144.4C397.1,147.2 385.3,149.4 379.5,150.9L372.5,152.8L416.3,152.9L460,153L460,177.2L443,176.8L426,176.5L426,476L438,476L438,499L461,499L461,522L9,522ZM239.8,380L320.7,318.5L250.3,317.5L281,267C297.9,239.2 311.6,216.3 311.4,216.2C311.3,216 274.5,243.6 229.7,277.7L148.3,339.5L183.6,339.8L218.9,340L203.3,365.8C194.7,379.9 180.8,402.9 172.3,416.8C163.8,430.8 157.4,442 157.9,441.8C158.4,441.7 195.3,413.8 239.8,380Z" style="fill:rgb(0,157,18);fill-rule:nonzero;"/>
+                            </g>
+                            </g>
+                        </svg>
+                    </div>
+                </div>
+                <div class="d-flex flex-row justify-content-center">
+                    <div class="d-flex flex-column">
+                        <div class="d-flex flex-row justify-content-center display-5 fw-light">
+                            <span id="surplusWatts">0.0</span>
+                        </div>
+                        <div class="d-flex flex-row justify-content-center">
+                            <span id="surplusAmps">0.00</span>&nbsp;<span class="text-muted">A</span>
+                        </div>
+                    </div>
                 </div>
             </div>
-            <div class="row justify-content-center">
-                <h1 class="meter"><span id="surplusWatts">0.0</span></h1>
-            </div>
-            <div class="row justify-content-center display-watt text-muted">
-                <span id="surplusAmps">0.00</span>&nbsp;A
-            </div>
         </div>
-
-        <div class="col-sm-12 col-md-3 col-lg-3 mb-5 mb-md-0">
-            <div class="row justify-content-center">
-                <div>
-                    <h6>Charging<span id="carsCharging" class="ml-1 badge badge-pill badge-grey">0</span></h6>
-                </div>
-                <div class="float-left ml-2" style="margin-top: -2px;">
-                    <svg width="1.5em" height="1.5em" viewBox="0 0 16 16" class="bi bi-plug" fill="limegreen" xmlns="http://www.w3.org/2000/svg">
-                        <path fill-rule="evenodd" d="M6 0a.5.5 0 0 1 .5.5V3h3V.5a.5.5 0 0 1 1 0V3h1a.5.5 0 0 1 .5.5v3A3.5 3.5 0 0 1 8.5 10c-.002.434-.01.845-.04 1.22-.041.514-.126 1.003-.317 1.424a2.083 2.083 0 0 1-.97 1.028C6.725 13.9 6.169 14 5.5 14c-.998 0-1.61.33-1.974.718A1.922 1.922 0 0 0 3 16H2c0-.616.232-1.367.797-1.968C3.374 13.42 4.261 13 5.5 13c.581 0 .962-.088 1.218-.219.241-.123.4-.3.514-.55.121-.266.193-.621.23-1.09.027-.34.035-.718.037-1.141A3.5 3.5 0 0 1 4 6.5v-3a.5.5 0 0 1 .5-.5h1V.5A.5.5 0 0 1 6 0zM5 4v2.5A2.5 2.5 0 0 0 7.5 9h1A2.5 2.5 0 0 0 11 6.5V4H5z"/>
-                    </svg>
+        <!-- show charging car(s) -->
+        <div class="bd-highlight col-12 col-md-6 col-lg-3 mt-4 mt-lg-0 text-center">
+            <div class="d-flex flex-column">
+                <div class="d-flex flex-row justify-content-center align-items-center">
+                    <div class="p-1">Charging
+                        <div class="badge rounded-pill badge-grey position-absolute ms-1 mt-0" id="carsCharging">0</div>
+                    </div>
+                    <div class="p-1 ms-3">
+                        <svg width="1.5em" height="1.5em" viewBox="0 0 16 16" class="bi bi-plug" fill="limegreen" xmlns="http://www.w3.org/2000/svg">
+                            <path fill-rule="evenodd" d="M6 0a.5.5 0 0 1 .5.5V3h3V.5a.5.5 0 0 1 1 0V3h1a.5.5 0 0 1 .5.5v3A3.5 3.5 0 0 1 8.5 10c-.002.434-.01.845-.04 1.22-.041.514-.126 1.003-.317 1.424a2.083 2.083 0 0 1-.97 1.028C6.725 13.9 6.169 14 5.5 14c-.998 0-1.61.33-1.974.718A1.922 1.922 0 0 0 3 16H2c0-.616.232-1.367.797-1.968C3.374 13.42 4.261 13 5.5 13c.581 0 .962-.088 1.218-.219.241-.123.4-.3.514-.55.121-.266.193-.621.23-1.09.027-.34.035-.718.037-1.141A3.5 3.5 0 0 1 4 6.5v-3a.5.5 0 0 1 .5-.5h1V.5A.5.5 0 0 1 6 0zM5 4v2.5A2.5 2.5 0 0 0 7.5 9h1A2.5 2.5 0 0 0 11 6.5V4H5z"/>
+                        </svg>
+                    </div>
+                </div>
+                <div class="d-flex flex-row justify-content-center">
+                    <div class="d-flex flex-column">
+                        <div class="d-flex flex-row justify-content-center display-5 fw-light">
+                            <span id="chargerLoadWatts">0.0</span>
+                        </div>
+                        <div class="d-flex flex-row justify-content-center">
+                            <span class="text-muted" id="chargerLoadAmps">0.0</span>&nbsp;A&nbsp;|&nbsp;<span class="text-muted" id="chargerAvailAmps">0</span>&nbsp;A&nbsp;offered
+                        </div>
+                    </div>
                 </div>
             </div>
-            <div class="row justify-content-center">
-                <h1 class="meter"><span id="chargerLoadWatts">0.0</span></h1>
-            </div>
-            <div class="row justify-content-center display-watt text-muted">
-                <span id="chargerLoadAmps">0.0</span>&nbsp;A&nbsp;|&nbsp;<span id="chargerAvailAmps">0</span>&nbsp;A&nbsp;<small class="mt-1">offered.</small>
-            </div>
         </div>
+    </div>
 
+    <div class="row justify-content-center">
         <!-- show active policy -->
         <div class="row w-100 justify-content-center mt-5">
             <div class="col-sm-11 col-md-10 col-lg-8">
                 <div class="jumbotron px-5 py-4 rounded-xl" style="background-color: #f0f0f0; pointer-events:none;">
                     <div class="form-group row" style="margin-bottom: -1em!important;">
-                        {% set active = master.settings.get("nonScheduledAction", 1) %}
-                        <label for="colBtns" class="col-lg-2 col-sm-12 col-form-label display-5">Charge Policy</label>
+                        <label for="colBtns" class="col-lg-2 col-sm-12 col-form-label display-6">Charge Policy</label>
                         <div class="col-lg-10 col-sm-12 btn-group" id="colBtns" role="group" style="flex-wrap: wrap;">
-                            <button type="button" class="btn btn-{% if active != 3 %}outline-{% endif %}primary" role="button" aria-describedby="helpText">Solar Surplus</button>
-                            <button type="button" class="btn btn-{% if active != 1 %}outline-{% endif %}primary" role="button" aria-describedby="helpText">Fixed Rate/Amps</button>
-                            <button type="button" class="btn btn-{% if active != 2 %}outline-{% endif %}primary" role="button" aria-describedby="helpText">Don't charge</button>
+                            <button id="policy_solar" type="button" class="btn btn-{% if activeAction != 3 %}outline-{% endif %}primary" role="button" aria-describedby="helpTextSolar">Solar Surplus</button>
+                            <button id="policy_fixed" type="button" class="btn btn-{% if activeAction != 1 %}outline-{% endif %}primary" role="button" aria-describedby="helpTextFixed">Fixed Rate/Amps</button>
+                            <button id="policy_dont" type="button" class="btn btn-{% if activeAction != 2 %}outline-{% endif %}primary" role="button" aria-describedby="helpTextDont">Don't charge</button>
                         </div>
                         <div class="col-lg-10 col-sm-12 offset-lg-2 offset-sm-0">
-                            <small id="helpText" class="form-text text-muted">
-                                {% if active == 1 %}
-                                    Charges a vehicle at a fixed rate of x Amps whenever it is plugged in
-                                {% elif active == 2 %}
-                                    Doesn't charge a vehicle when plugged in unless manually started (e.g. in the Tesla App)
-                                {% elif active == 3 %}
-                                    Charges a vehicle if Solar production is {{ master.settings.get("minAmpsPerTWC", 5) }} Amps or more than the current consumption
-                                {% endif %}
+                            <small id="helpTextFixed" class="form-text text-muted" {% if activeAction != 1 %}style="display: none;"{% endif %}>
+                                Charges a vehicle at a fixed rate of x Amps whenever it is plugged in
+                            </small>
+                            <small id="helpTextDont" class="form-text text-muted" {% if activeAction != 2 %}style="display: none;"{% endif %}>
+                                Doesn't charge a vehicle when plugged in unless manually started (e.g. in the Tesla App)
+                            </small>
+                            <small id="helpTextSolar" class="form-text text-muted" {% if activeAction != 3 %}style="display: none;"{% endif %}>
+                                Charges a vehicle if Solar production is at least {{ master.config["config"].get("minAmpsPerTWC", 5) }} Amps higher than the current consumption
                             </small>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
     </div>
@@ -140,174 +163,164 @@
 <!-- end Home -->
 
 <!-- Charge points -->
 <div class="container-fluid pt-4">
     <div class="row border-bottom mb-4">
         <h1 class="display-4">Charge Point{% if (slaves|count > 1) %}s{% endif %}</h1>
     </div>
+    {% set slaves = master.getSlaveTWCs() %}
+    {% for charger in slaves %}
+    {% set twcid = '%02x%02x' % (charger.TWCID[0], charger.TWCID[1]) %}
 
-    <div class="row pb-2 border-bottom text-center">
-        {% set slaves = master.getSlaveTWCs() %}
-        {% for charger in slaves %}
-        <div class="col-12">
-            <div class="row col-12">
-                <div class="col"><!-- icon column -->
-                    <div class="row">
-                        <div class="col">
-                            <svg height="4em" viewBox="0 0 78 142" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" xml:space="preserve" xmlns:serif="http://www.serif.com/" style="fill-rule:evenodd;clip-rule:evenodd;stroke-linecap:round;stroke-linejoin:round;stroke-miterlimit:1.5;">
-                                <g transform="matrix(1,0,0,1,-58.6302,-49.9425)">
-                                    <g transform="matrix(1.25227,0,0,0.981636,-34.4875,13.0036)">
-                                        <path d="M116.037,39.022C115.797,38.575 83.43,38.476 83.096,39.022C77.024,48.944 74.984,83.654 75.169,97.089C75.28,105.116 76.478,144.135 81.364,153.398C82.664,155.861 94.199,157.333 100.289,157.333C106.306,157.333 116.891,155.968 117.891,153.398C121.673,143.672 123.219,107.967 123.512,97.089C124.026,77.966 121.313,48.87 116.037,39.022Z" style="fill:none;"/>
-                                        <clipPath id="_clip1">
-                                            <path d="M116.037,39.022C115.797,38.575 83.43,38.476 83.096,39.022C77.024,48.944 74.984,83.654 75.169,97.089C75.28,105.116 76.478,144.135 81.364,153.398C82.664,155.861 94.199,157.333 100.289,157.333C106.306,157.333 116.891,155.968 117.891,153.398C121.673,143.672 123.219,107.967 123.512,97.089C124.026,77.966 121.313,48.87 116.037,39.022Z"/>
-                                        </clipPath>
-                                        <g clip-path="url(#_clip1)">
-                                            <g transform="matrix(0.988571,0,0,0.987743,1.07957,1.38293)">
-                                                <path d="M100,107.668L100,146.78" style="fill:none;stroke:rgb(94,159,40);stroke-width:1.8px;"/>
-                                            </g>
-                                        </g>
-                                        <path d="M116.037,39.022C115.797,38.575 83.43,38.476 83.096,39.022C77.024,48.944 74.984,83.654 75.169,97.089C75.28,105.116 76.478,144.135 81.364,153.398C82.664,155.861 94.199,157.333 100.289,157.333C106.306,157.333 116.891,155.968 117.891,153.398C121.673,143.672 123.219,107.967 123.512,97.089C124.026,77.966 121.313,48.87 116.037,39.022Z" style="fill:none;stroke:black;stroke-width:1.78px;"/>
-                                    </g>
-                                    <g transform="matrix(1,0,0,1,0.475625,-8.83563)">
-                                        <path d="M122.47,116.245C122.47,116.245 126.137,118.829 126.928,121.411C128.504,126.554 129.718,145.816 129.718,145.816L132.341,145.816C132.341,145.816 136.379,125.697 134.366,118.836C132.574,112.732 122.177,105.674 122.177,105.674C122.177,105.674 122.47,109.197 122.47,110.891L122.47,116.245Z" style="fill:none;stroke:black;stroke-width:2px;"/>
-                                    </g>
-                                    <g transform="matrix(1.01098,0,0,1.20996,-0.993229,-39.451)">
-                                        <path d="M90.658,170.995C92.296,189.853 129.911,210.487 131.271,145.981" style="fill:none;stroke:black;stroke-width:1.79px;stroke-linejoin:bevel;"/>
-                                    </g>
-                                </g>
-                            </svg>
-                        </div>
-                        <div class="col pt-1">
-                            {% set twcid = '%02x%02x' % (charger.TWCID[0], charger.TWCID[1]) %}
-                            <div class="row">
-                                <small>{{ twcid }}</small>
-                            </div>
-                            <div class="row">
-                                <small>Version <span id="{{ twcid }}_version"></span></small>
-                            </div>
-                            <div class="row">
-                                <small>State <span id="{{ twcid }}_state"></span></small>
-                            </div>
-                        </div>
-                    </div>
-                </div>
-                <div class="col"><!-- max Amps -->
-                    <div class="row">
-                        <div class="col-12">
-                            <span id="{{ twcid }}_chargeTime" class="meter">00:00:00</span>
-                        </div>
-                    </div>
-                    <div class="row">
-                        <div class="col-12">
-                            <small class="text-muted">Charging time counter</small>
-                        </div>
-                    </div>
-                </div>
-                <div class="col"><!-- Amps offered -->
-                    <div class="row">
-                        <div class="col-12">
-                            <span id="{{ twcid }}_lastAmpsOffered" class="meter amps"></span>
-                        </div>
-                    </div>
-                    <div class="row">
-                        <div class="col-12">
-                            <small class="text-muted">Amps offered</small>
-                        </div>
-                    </div>
-                </div>
-                <div class="col"><!-- Amps in use -->
-                    <div class="row">
-                        <div class="col-12">
-                            <span id="{{ twcid }}_reportedAmpsActual" class="meter amps"></span>
-                        </div>
-                    </div>
-                    <div class="row">
-                        <div class="col-12">
-                            <small class="text-muted">Amps in use</small>
-                        </div>
-                    </div>
-                </div>
-                <div class="col"><!-- Lifetime kWh -->
-                    <div class="row">
-                        <div class="col-12">
-                            <span id="{{ twcid }}_lifetimekWh" class="meter kwh"></span>
-                        </div>
-                    </div>
-                    <div class="row">
-                        <div class="col-12">
-                            <small class="text-muted">Lifetime kWh</small>
-                        </div>
-                    </div>
-                </div>
-                <div class="col"><!-- Voltage -->
-                    <div class="row" style="line-height: 0.9rem;">
-                        <div class="col-12">
-                            <div class="row justify-content-center">
-                                L<span class="phase">1</span><span id="{{ twcid }}_voltsPhaseA" class="volt"></span>
-                            </div>
-                            <div class="row justify-content-center">
-                                L<span class="phase">2</span><span id="{{ twcid }}_voltsPhaseB" class="volt"></span>
-                            </div>
-                            <div class="row justify-content-center">
-                                L<span class="phase">3</span><span id="{{ twcid }}_voltsPhaseC" class="volt"></span>
-                            </div>
-                        </div>
-                    </div>
-                    <div class="row">
-                        <div class="col-12">
-                            <small class="text-muted">Phase/Voltage</small>
-                        </div>
-                    </div>
-                </div>
-                <div class="col"><!-- Vehicle -->
-                    <div class="row">
-                        <div class="col-12 text-left" style="line-height: 1.37em;">
-                            <strong>Vehicle</strong>:<br>
-                            Current: <span id="{{ twcid }}_currentVIN" class='VINClick' onClick="loadVIN('{{ twcid }}','current');"></span><br>
-                            Last: <span id="{{ twcid }}_lastVIN" class='VINClick' onClick="loadVIN('{{ twcid }}','last');"></span>
-                            <span id="{{ twcid }}_socState"><br>SoC: <span id="{{ twcid }}_lastBatterySOC"></span>/<span id="{{ twcid }}_lastChargeLimit"></span>%</span>
-                        </div>
-                    </div>
-                </div>
+    <!-- charge point data in row -->
+    <div class="row mb-3 align-center">
+
+        <!-- TWC icon -->
+        <div class="col-1 text-center">
+            <svg height="4em" viewBox="0 0 78 142" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" xml:space="preserve" style="fill-rule:evenodd;clip-rule:evenodd;stroke-linecap:round;stroke-linejoin:round;stroke-miterlimit:1.5;">
+                <g transform="matrix(1,0,0,1,-58.6302,-49.9425)">
+                    <g transform="matrix(1.25227,0,0,0.981636,-34.4875,13.0036)">
+                        <path d="M116.037,39.022C115.797,38.575 83.43,38.476 83.096,39.022C77.024,48.944 74.984,83.654 75.169,97.089C75.28,105.116 76.478,144.135 81.364,153.398C82.664,155.861 94.199,157.333 100.289,157.333C106.306,157.333 116.891,155.968 117.891,153.398C121.673,143.672 123.219,107.967 123.512,97.089C124.026,77.966 121.313,48.87 116.037,39.022Z" style="fill:none;"/>
+                        <clipPath id="_clip1">
+                            <path d="M116.037,39.022C115.797,38.575 83.43,38.476 83.096,39.022C77.024,48.944 74.984,83.654 75.169,97.089C75.28,105.116 76.478,144.135 81.364,153.398C82.664,155.861 94.199,157.333 100.289,157.333C106.306,157.333 116.891,155.968 117.891,153.398C121.673,143.672 123.219,107.967 123.512,97.089C124.026,77.966 121.313,48.87 116.037,39.022Z"/>
+                        </clipPath>
+                        <g clip-path="url(#_clip1)">
+                            <g transform="matrix(0.988571,0,0,0.987743,1.07957,1.38293)">
+                                <path d="M100,107.668L100,146.78" style="fill:none;stroke:rgb(94,159,40);stroke-width:1.8px;"/>
+                            </g>
+                        </g>
+                        <path d="M116.037,39.022C115.797,38.575 83.43,38.476 83.096,39.022C77.024,48.944 74.984,83.654 75.169,97.089C75.28,105.116 76.478,144.135 81.364,153.398C82.664,155.861 94.199,157.333 100.289,157.333C106.306,157.333 116.891,155.968 117.891,153.398C121.673,143.672 123.219,107.967 123.512,97.089C124.026,77.966 121.313,48.87 116.037,39.022Z" style="fill:none;stroke:black;stroke-width:1.78px;"/>
+                    </g>
+                    <g transform="matrix(1,0,0,1,0.475625,-8.83563)">
+                        <path d="M122.47,116.245C122.47,116.245 126.137,118.829 126.928,121.411C128.504,126.554 129.718,145.816 129.718,145.816L132.341,145.816C132.341,145.816 136.379,125.697 134.366,118.836C132.574,112.732 122.177,105.674 122.177,105.674C122.177,105.674 122.47,109.197 122.47,110.891L122.47,116.245Z" style="fill:none;stroke:black;stroke-width:2px;"/>
+                    </g>
+                    <g transform="matrix(1.01098,0,0,1.20996,-0.993229,-39.451)">
+                        <path d="M90.658,170.995C92.296,189.853 129.911,210.487 131.271,145.981" style="fill:none;stroke:black;stroke-width:1.79px;stroke-linejoin:bevel;"/>
+                    </g>
+                </g>
+            </svg>
+        </div>
+
+        <!-- TWC status -->
+        <div class="col-lg-1 col-md-2 col-2 text-center">
+            <div class="row">
+                <small>ID {{ twcid }}</small>
+            </div>
+            <div class="row">
+                <small>Version <span id="{{ twcid }}_version"></span></small>
+            </div>
+            <div class="row">
+                <small>State <span id="{{ twcid }}_state"></span></small>
+            </div>
+        </div>
+
+        <!-- Charge timer -->
+        <div class="col-lg-2 col-md-3 col-5 text-center">
+            <div class="row-inline display-6 fw-light">
+                <span id="{{ twcid }}_chargeTime">--:--:--</span>
+            </div>
+            <div class="row">
+                <span class="text-muted">Charge time</span>
+            </div>
+        </div>
+
+        <!-- Amps offered -->
+        <div class="col-lg-1 col-md-3 col-2 text-center">
+            <div class="row display-6 fw-light">
+                <span class="text-body me-1" id="{{ twcid }}_lastAmpsOffered">0.0</span>
+            </div>
+            <div class="row">
+                <span class="text-muted">Amps offered</span>
+            </div>
+        </div>
+
+        <!-- Amps in used -->
+        <div class="col-lg-1 col-md-3 col-2 text-center">
+            <div class="row display-6 fw-light">
+                <span class="text-body me-1" id="{{ twcid }}_reportedAmpsActual">0.0</span>
+            </div>
+            <div class="row">
+                <span class="text-muted">Amps in use</span>
+            </div>
+        </div>
+
+        <!-- Lifetime Amps -->
+        <div class="col-lg-2 pt-lg-0 col-md-4 pt-3 col-4 text-center">
+            <div class="row-inline display-6 fw-light">
+                <span class="text-body me-1" id="{{ twcid }}_lifetimekWh">0000</span>
+            </div>
+            <div class="row">
+                <span class="text-muted">Lifetime kWh</span>
+            </div>
+        </div>
+
+        <!-- Phase/Voltage -->
+        <div class="col-lg-auto pt-lg-0 col-md-4 pt-3 col-4 text-center">
+            <div class="row">
+                <span class="text-muted">L<sub>1</sub> <span class="text-body me-1" id="{{ twcid }}_voltsPhaseA">230</span>V</span>
+            </div>
+            <div class="row">
+                <span class="text-muted">L<sub>2</sub> <span class="text-body me-1" id="{{ twcid }}_voltsPhaseB">230</span>V</span>
+            </div>
+            <div class="row">
+                <span class="text-muted">L<sub>3</sub> <span class="text-body me-1" id="{{ twcid }}_voltsPhaseC">230</span>V</span>
+            </div>
+            <div class="row">
+                <small class="text-muted">Phase/Voltage</small>
+            </div>
+        </div>
+
+        <!-- Vehicle/VIN -->
+        <div class="col-lg-2 pt-lg-0 col-md-4 pt-3 col-4 text-muted">
+            <div class="lh-sm">
+                <small>VIN: <span id="{{ twcid }}_currentVIN" class='VINClick' onClick="loadVIN('{{ twcid }}','current');"></span></small>
+            </div>
+            <div class="lh-sm">
+                <small>Last VIN: <span id="{{ twcid }}_lastVIN" class='VINClick' onClick="loadVIN('{{ twcid }}','last');"></span></small>
+            </div>
+            <div class="lh-sm">
+                <small>SoC: <span id="{{ twcid }}_socState"></span></small>
+            </div>
+            <div class="lh-sm">
+                <small>Last SoC: <span id="{{ twcid }}_lastBatterySOC"></span></small>
+            </div>
+            <div class="lh-sm">
+                <small>Last Limit: <span id="{{ twcid }}_lastChargeLimit"></span>%</small>
             </div>
         </div>
-        {% endfor %}
     </div>
+    {% endfor %}
 </div>
 <!-- end Charge Points -->
 
 <!--  Global Actions -->
-<div class="container-fluid pt-4">
-    <div class="row justify-content-center">
-        <div class="col-lg-3 col-sm-12">
-            <form>
-                <div class="form-group p-2">
-                    <label for="chargeNowDuration" class="text-muted mb-0">Charge duration <span class="text-dark font-weight-bold" id="{{ twcid }}_durationVal">1</span> hours</label>
-                    <input type="range" class="custom-range" id="chargeNowDuration" name="chargeNowDuration" min="1" max="24" step="1" value="1" onInput="$('#{{ twcid }}_durationVal').html($(this).val())">
-                </div>
-            </form>
+<div class="container-fluid py-3 bg-light border-top border-bottom mb-5">
+    <div class="row">
+        <div class="col-12 col-md-6 col-lg-4">
+            <label for="chargeNowDuration" class="form-label text-muted">Charge duration <span class="text-dark font-weight-bold" id="{{ twcid }}_durationVal">1</span> hour</label>
+            <input type="range" class="form-range" id="chargeNowDuration" name="chargeNowDuration" min="1" max="24" step="1" value="1" onInput="$('#{{ twcid }}_durationVal').html($(this).val())">
         </div>
-        <div class="col-lg-3 col-sm-12">
+        <hr class="d-block d-md-none my-md-0 my-4">
+        <div class="col-12 col-md-6 col-lg-4">
             {% set ampsMin = ampsList[1] %}
             {% set ampsMax = ampsList|last %}
-            <form>
-                <div class="form-group p-2">
-                    <label for="chargeNowRate" class="text-muted mb-0">Charge with <span class="text-dark font-weight-bold" id="{{ twcid }}_ampsVal">{{ ampsMin[0] }}</span> A</label>
-                    <input type="range" class="custom-range" id="chargeNowRate" name="chargeNowRate" min="{{ ampsMin[0]}}" max="{{ ampsMax[0] }}" step="1" value="{{ ampsMin[0] }}" onInput="$('#{{ twcid }}_ampsVal').html($(this).val())">
-                </div>
-            </form>
+            <label for="chargeNowRate" class="form-label text-muted">Charge with <span class="text-dark font-weight-bold" id="{{ twcid }}_ampsVal">{{ ampsMin[0] }}</span> A</label>
+            <input type="range" class="form-range" id="chargeNowRate" name="chargeNowRate" min="{{ ampsMin[0]}}" max="{{ ampsMax[0] }}" step="1" value="{{ ampsMin[0] }}" onInput="$('#{{ twcid }}_ampsVal').html($(this).val())">
         </div>
-            <div class="col-lg-2 col-sm-12 text-center">
-                <div class="form-group p-3 m-1">
-                    <button type="submit" class="btn btn-light btn-small border" id="start_chargenow" value="Charge now"></button>
+        <div class="col-12 col-lg-4">
+            <div class="row pt-3">
+                <div class="col-xl-6 col-lg-5 col-6">
+                    <div class="row px-2">
+                        <button type="submit" class="btn btn-block btn-primary" id="start_chargenow" value="Charge now"></button>
+                    </div>
                 </div>
-            </div>
-            <div class="col-lg-2 col-sm-12 text-center">
-                <div class="form-group p-3 m-1">
-                    <button type="submit" class="btn btn-light btn-small border" id="cancel_chargenow" value="Cancel Charge now">Cancel Charge Now</button>
+                <div class="col-xl-6 col-lg-7 col-6">
+                    <div class="row px-2">
+                        <button type="submit" class="btn btn-block btn-warning" disabled id="cancel_chargenow" value="Cancel Charge now">Cancel Charge now</button>
+                    </div>
                 </div>
             </div>
         </div>
     </div>
 </div>
 <!-- end Global Actions -->
 {% endblock %}
```

#### html2text {}

```diff
@@ -5,57 +5,67 @@
 experienced an error trying to save your settings. This mea ns that while your
 current settings will be retained for the current session, th ey will not be
 saved if TWCManager exits. Please check the permissions on /etc/t wcmanager/
 settings.json and try saving your settings again. {% endif %}
 ****** Home ******
 Generation
 
-****** 0.0 ******
+0.0
 0.00 A
-⇣ Consumption
+⇣Consumption
 
-****** 0.0 ******
+0.0
 0.00 A
 Solar surplus
 
-****** 0.0 ******
+0.0
 0.00 A
-* Charging0 *
+Charging
+0
 
-****** 0.0 ******
-0.0 A | 0 A offered.
-{% set active = master.settings.get("nonScheduledAction", 1) %} Charge Policy
+0.0
+0.0 A | 0 A offered
+Charge Policy
 Solar Surplus Fixed Rate/Amps Don't charge
-{% if active == 1 %} Charges a vehicle at a fixed rate of x Amps whenever it is
-plugged in {% elif active == 2 %} Doesn't charge a vehicle when plugged in
-unless manually started (e.g. in the Tesla App) {% elif active == 3 %} Charges
-a vehicle if Solar production is {{ master.settings.get("minAmpsPerTWC", 5) }}
-Amps or more than the current consumption {% endif %}
+% if activeAction != 1 %}style="display: none;"{% endif %}> Charges a vehicle
+at a fixed rate of x Amps whenever it is plugged in
+
+% if activeAction != 2 %}style="display: none;"{% endif %}> Doesn't charge a
+vehicle when plugged in unless manually started (e.g. in the Tesla App)
+
+% if activeAction != 3 %}style="display: none;"{% endif %}> Charges a vehicle
+if Solar production is at least {{ master.config["config"].get("minAmpsPerTWC",
+5) }} Amps higher than the current consumption
 
 ****** Charge Point{% if (slaves|count > 1) %}s{% endif %} ******
-{% set slaves = master.getSlaveTWCs() %} {% for charger in slaves %}
+{% set slaves = master.getSlaveTWCs() %} {% for charger in slaves %} {% set
+twcid = '%02x%02x' % (charger.TWCID[0], charger.TWCID[1]) %}
 
-{% set twcid = '%02x%02x' % (charger.TWCID[0], charger.TWCID[1]) %}
-{{ twcid }}
+ID {{ twcid }}
 Version
 State
-00:00:00
-Charging time counter
+--:--:--
+Charge time
+0.0
 Amps offered
+0.0
 Amps in use
+0000
 Lifetime kWh
-L1
-L2
-L3
+L1 230V
+L2 230V
+L3 230V
 Phase/Voltage
-Vehicle:
-Current:
-Last:
-SoC: /%
+VIN:
+Last VIN:
+SoC:
+Last SoC:
+Last Limit: %
 {% endfor %}
 
-Charge duration 1 hours [Unknown INPUT type]
-{% set ampsMin = ampsList[1] %} {% set ampsMax = ampsList|last %}
-Charge with {{ ampsMin[0] }} A [Unknown INPUT type]
-Cancel Charge Now
+Charge duration 1 hour [Unknown INPUT type]
+===============================================================================
+{% set ampsMin = ampsList[1] %} {% set ampsMax = ampsList|last %} Charge with {
+{ ampsMin[0] }} A [Unknown INPUT type]
+Cancel Charge now
  {% endblock %} {% block javascripts %}{% include "jsrefresh.html.j2" %}{%
 endblock %}
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/EMS/DSMR.py` & `TWCManager-1.3.0/lib/TWCManager/EMS/DSMR.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Dutch SmartMeter Serial Integration (DSMR)
 
 
 class DSMR:
-
     import time
 
     baudrate = 115200
     consumedW = 0
     generatedW = 0
     serial = None
     serialPort = "/dev/ttyUSB2"
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/EMS/Efergy.py` & `TWCManager-1.3.0/lib/TWCManager/EMS/Efergy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Efergy
 import time
 
 
 class Efergy:
-
     import requests
 
     cacheTime = 10
     config = None
     configConfig = None
     configEfergy = None
     consumedW = 0
@@ -40,41 +39,38 @@
 
         # Unload if this module is disabled or misconfigured
         if not self.status:
             self.master.releaseModule("lib.TWCManager.EMS", self.__class__.__name__)
             return None
 
     def getConsumption(self):
-
         if not self.status:
             logger.debug("Efergy EMS Module Disabled. Skipping getConsumption")
             return 0
 
         # Perform updates if necessary
         self.update()
 
         # Return consumption value
         return float(self.consumedW)
 
     def getGeneration(self):
-
         if not self.status:
             logger.debug("Efergy EMS Module Disabled. Skipping getGeneration")
             return 0
 
         # Perform updates if necessary
         self.update()
 
         # Return generation value
         if not self.generatedW:
             self.generatedW = 0
         return float(self.generatedW)
 
     def getValue(self, url):
-
         # Fetch the specified URL from the Efergy and return the data
         self.fetchFailed = False
 
         try:
             r = self.requests.get(url, timeout=self.timeout)
         except self.requests.exceptions.ConnectionError as e:
             logger.log(
@@ -93,15 +89,14 @@
             "https://engage.efergy.com/mobile_proxy/getCurrentValuesSummary?token="
             + self.token
         )
 
         return self.getValue(url)
 
     def update(self):
-
         if (int(time.time()) - self.lastFetch) > self.cacheTime:
             # Cache has expired. Fetch values from Efergy.
 
             meterData = self.getMeterData()
 
             if meterData:
                 try:
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/EMS/EmonCMS.py` & `TWCManager-1.3.0/lib/TWCManager/EMS/EmonCMS.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 
 logger = logging.getLogger(__name__.rsplit(".")[-1])
 
 
 class EmonCMS:
-
     # OpenEnergyMonitor (EmonCMS) Module
     # Fetches Consumption and Generation details from Open Energy Monitor
 
     import requests
     import time
 
     apiKey = None
@@ -53,27 +52,25 @@
 
         # Unload if this module is disabled or misconfigured
         if (not self.status) or (not self.serverIP) or (int(self.serverPort) < 1):
             self.master.releaseModule("lib.TWCManager.EMS", "EmonCMS")
             return None
 
     def getConsumption(self):
-
         if not self.status:
             logger.debug("Module Disabled. Skipping getConsumption")
             return 0
 
         # Perform updates if necessary
         self.update()
 
         # Return consumption value
         return self.consumedW
 
     def getGeneration(self):
-
         if not self.status:
             logger.debug("Module Disabled. Skipping getGeneration")
             return 0
 
         # Perform updates if necessary
         self.update()
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/EMS/Enphase.py` & `TWCManager-1.3.0/lib/TWCManager/EMS/Enphase.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import logging
 import time
 
 logger = logging.getLogger(__name__.rsplit(".")[-1])
 
 
 class Enphase:
-
     import requests
 
     apiKey = None
     # cacheTime is a bit higher than local EMS modules
     # because we're polling an external API
     cacheTime = 60
     config = None
@@ -56,27 +55,25 @@
             return None
 
         # Drop the cacheTime to 10 seconds if we use the local API
         if self.serverIP and self.serverPort:
             self.cacheTime = 10
 
     def getConsumption(self):
-
         if not self.status:
             logger.debug("Enphase EMS Module Disabled. Skipping getConsumption")
             return None
 
         # Perform updates if necessary
         self.update()
 
         # Return current consumption value
         return float(self.consumedW)
 
     def getGeneration(self):
-
         if not self.status:
             logger.debug("Enphase EMS Module Disabled. Skipping getGeneration")
             return 0
 
         # Perform updates if necessary
         self.update()
 
@@ -93,15 +90,14 @@
         elif self.serverIP and self.serverPort:
             url = "http://" + self.serverIP + ":" + str(self.serverPort)
             url += "/production.json?details=1&classic-1"
 
         return self.getPortalValue(url)
 
     def getPortalValue(self, url):
-
         # Fetch the specified URL from the Enphase Portal and return the data
         self.fetchFailed = False
 
         try:
             r = self.requests.get(url, timeout=self.timeout)
         except self.requests.exceptions.ConnectionError as e:
             logger.log(
@@ -122,15 +118,14 @@
                 + " connecting to Enphase Portal to fetch sensor value",
             )
             return ""
         else:
             return r.json()
 
     def update(self):
-
         if (int(time.time()) - self.lastFetch) > self.cacheTime:
             # Cache has expired. Fetch values from Portal.
 
             portalData = self.getPortalData()
             if portalData:
                 try:
                     # Determine if this is Local or Cloud API
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/EMS/Fronius.py` & `TWCManager-1.3.0/lib/TWCManager/EMS/Fronius.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import requests
 import time
 
 logger = logging.getLogger("\U000026C5 Fronius")
 
 
 class Fronius:
-
     cacheTime = 10
     config = None
     configConfig = None
     configFronius = None
     consumedW = 0
     fetchFailed = False
     generatedW = 0
@@ -46,27 +45,25 @@
 
         # Unload if this module is disabled or misconfigured
         if (not self.status) or (not self.serverIP) or (int(self.serverPort) < 1):
             self.master.releaseModule("lib.TWCManager.EMS", "Fronius")
             return None
 
     def getConsumption(self):
-
         if not self.status:
             logger.debug("Fronius EMS Module Disabled. Skipping getConsumption")
             return 0
 
         # Perform updates if necessary
         self.update()
 
         # Return consumption value (negated, as this is how it's presented)
         return float(self.consumedW) * -1
 
     def getGeneration(self):
-
         if not self.status:
             logger.debug("Fronius EMS Module Disabled. Skipping getGeneration")
             return 0
 
         # Perform updates if necessary
         self.update()
 
@@ -81,15 +78,14 @@
             url
             + "/solar_api/v1/GetInverterRealtimeData.cgi?Scope=Device&DeviceID=1&DataCollection=CommonInverterData"
         )
 
         return self.getInverterValue(url)
 
     def getInverterValue(self, url):
-
         # Fetch the specified URL from the Fronius Inverter and return the data
         self.fetchFailed = False
 
         try:
             r = requests.get(url, timeout=self.timeout)
         except requests.exceptions.ConnectionError as e:
             logger.log(
@@ -107,22 +103,20 @@
     def getMeterData(self, inverter):
         url = "http://" + inverter + ":" + self.serverPort
         url = url + "/solar_api/v1/GetPowerFlowRealtimeData.fcgi?Scope=System"
 
         return self.getInverterValue(url)
 
     def update(self):
-
         if (int(time.time()) - self.lastFetch) > self.cacheTime:
             # Cache has expired. Fetch values from Fronius inverter.
 
             con = 0
             gen = 0
             for inverter in self.serverIP:
-
                 inverterData = self.getInverterData(inverter)
                 if inverterData:
                     try:
                         if "UAC" in inverterData["Body"]["Data"]:
                             self.voltage = inverterData["Body"]["Data"]["UAC"]["Value"]
                     except (KeyError, TypeError) as e:
                         logger.log(
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/EMS/Growatt.py` & `TWCManager-1.3.0/lib/TWCManager/EMS/Growatt.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import datetime
 
 
 logger = logging.getLogger(__name__.rsplit(".")[-1])
 
 
 class Growatt:
-
     # Growatt EMS Module
     # Fetches Consumption and Generation details from Growatt API
 
     import requests
     import time
 
     cacheTime = 10
@@ -54,39 +53,36 @@
         self.now = datetime.datetime.now().time()
         # Unload if this module is disabled or misconfigured
         if (not self.status) or (not self.username or not self.password):
             self.master.releaseModule("lib.TWCManager.EMS", "Growatt")
             return None
 
     def getConsumption(self):  # gets called by TWCManager.py
-
         if not self.status:
             logger.debug("EMS Module Disabled. Skipping getConsumption")
             return 0
 
         # Perform updates if necessary
         self.update()
 
         # Return consumption value
         return self.consumedW
 
     def getGeneration(self):  # gets called by TWCManager.py
-
         if not self.status:
             logger.debug("EMS Module Disabled. Skipping getGeneration")
             return 0
 
         # Perform updates if necessary
         self.update()
 
         # Return generation value
         return self.generatedW
 
     def getGenerationValues(self):
-
         if not self.status:
             logger.debug("EMS Module Disabled. Skipping getGeneration")
             return 0
 
         api = growattServer.GrowattApi()
 
         try:
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/EMS/HASS.py` & `TWCManager-1.3.0/lib/TWCManager/EMS/HASS.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 
 logger = logging.getLogger(__name__.rsplit(".")[-1])
 
 
 class HASS:
-
     # HomeAssistant EMS Module
     # Fetches Consumption and Generation details from HomeAssistant
 
     import requests
     import time
 
     apiKey = None
@@ -50,27 +49,25 @@
 
         # Unload if this module is disabled or misconfigured
         if (not self.status) or (not self.serverIP) or (int(self.serverPort) < 1):
             self.master.releaseModule("lib.TWCManager.EMS", "HASS")
             return None
 
     def getConsumption(self):
-
         if not self.status:
             logger.debug("Module Disabled. Skipping getConsumption")
             return 0
 
         # Perform updates if necessary
         self.update()
 
         # Return consumption value
         return self.consumedW
 
     def getGeneration(self):
-
         if not self.status:
             logger.debug("Module Disabled. Skipping getGeneration")
             return 0
 
         # Perform updates if necessary
         self.update()
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/EMS/IotaWatt.py` & `TWCManager-1.3.0/lib/TWCManager/EMS/IotaWatt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 
 logger = logging.getLogger(__name__.rsplit(".")[-1])
 
 
 class IotaWatt:
-
     # IotaWatt EMS Module
     # Fetches Consumption and Generation details from IotaWatt
 
     import requests
     import time
 
     apiKey = None
@@ -49,27 +48,25 @@
 
         # Unload if this module is disabled or misconfigured
         if (not self.status) or (not self.serverIP):
             self.master.releaseModule("lib.TWCManager.EMS", "IotaWatt")
             return None
 
     def getConsumption(self):
-
         if not self.status:
             logger.debug("Module Disabled. Skipping getConsumption")
             return 0
 
         # Perform updates if necessary
         self.update()
 
         # Return consumption value
         return self.consumedW
 
     def getGeneration(self):
-
         if not self.status:
             logger.debug("Module Disabled. Skipping getGeneration")
             return 0
 
         # Perform updates if necessary
         self.update()
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/EMS/Kostal.py` & `TWCManager-1.3.0/lib/TWCManager/EMS/Kostal.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,14 @@
             self.modbus.close()
 
     #
     # Privat Method for reading Modbus values
     # read registers directly from the inverter via Modbus protocol
     #
     def __readModbus(self, address, data_format="Float"):
-
         # open the Modbus connection if neccessary
         if not self.modbus.is_open():
             self.modbus.open()
 
         # default data length is 1 ('U16')
         length = 1
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/EMS/OpenHab.py` & `TWCManager-1.3.0/lib/TWCManager/EMS/OpenHab.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import requests
 import time
 
 logger = logging.getLogger(__name__.rsplit(".")[-1])
 
 
 class OpenHab:
-
     # OpenHab EMS Module
     # Fetches Consumption and Generation details from OpenHab
 
     apiKey = None
     cacheTime = 10  # in seconds
     config = None
     configConfig = None
@@ -46,27 +45,25 @@
 
         # Unload if this module is disabled or misconfigured
         if (not self.status) or (not self.serverIP) or (int(self.serverPort) < 1):
             self.master.releaseModule("lib.TWCManager.EMS", "OpenHab")
             return None
 
     def getConsumption(self):
-
         if not self.status:
             logger.debug("OpenHab EMS Module Disabled. Skipping getConsumption")
             return 0
 
         # Perform updates if necessary
         self.update()
 
         # Return consumption value
         return self.consumedW
 
     def getGeneration(self):
-
         if not self.status:
             logger.debug("OpenHab EMS Module Disabled. Skipping getGeneration")
             return 0
 
         # Perform updates if necessary
         self.update()
 
@@ -107,15 +104,15 @@
             return False
 
         response = httpResponse.text
         response = response.strip()
 
         # Strip units like '12.3 W'
         if " " in response:
-            return response.split(" ")[0]
+            response = response.split(" ")[0]
 
         try:
             responseAsFloat = float(response)
             return responseAsFloat
         except ValueError:
             logger.log(logging.INFO4, "Fetched value from OpenHab item is not a number")
             logger.debug("Server response: " + str(response))
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/EMS/OpenWeatherMap.py` & `TWCManager-1.3.0/lib/TWCManager/EMS/OpenWeatherMap.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import requests
 import time
 
 logger = logging.getLogger(__name__.rsplit(".")[-1])
 
 
 class OpenWeatherMap:
-
     cacheTime = 60
     config = None
     configConfig = None
     configOpenWeatherMap = None
     fetchFailed = False
     generatedW = 0
     consumedW = 0
@@ -49,15 +48,14 @@
             return None
 
     def getConsumption(self):
         # since this is not knowing our consumption!
         return 0
 
     def getGeneration(self):
-
         if not self.status:
             logger.debug("OpenWeatherMap EMS Module Disabled. Skipping getGeneration")
             return 0
 
         # Perform updates if necessary
         self.update()
 
@@ -76,15 +74,14 @@
             + self.APIKey
             + "&exclude=minutely&units=metric"
         )
 
         return self.getOpenWeatherMapValue(url)
 
     def getOpenWeatherMapValue(self, url):
-
         # Fetch the specified URL from the OpenWeatherMap and return the data
         self.fetchFailed = False
 
         try:
             r = requests.get(url, timeout=self.timeout)
         except requests.exceptions.ConnectionError as e:
             logger.log(
@@ -120,15 +117,14 @@
                 if (dif == 0) or (cmp < dif):
                     dif = cmp
                     bestjson = subset
 
         return bestjson
 
     def update(self):
-
         month = int(time.strftime("%m"))
         dt = int(time.time())
         if (int(time.time()) - self.lastFetch) > self.cacheTime:
             # Cache has expired. Fetch values from OpenWeatherMap inverter.
             tmp = self.getOpenWeatherMapData()
             if tmp:
                 self.LastJson = tmp
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/EMS/P1Monitor.py` & `TWCManager-1.3.0/lib/TWCManager/EMS/P1Monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     import requests
 
     consumedW = 0
     generatedW = 0
     timeout = 10
 
     def __init__(self, master):
-
         self.p1monData = {}
         self.configP1Mon = master.config["sources"].get("P1Monitor", {})
         self.serverIP = self.configP1Mon.get("serverIP", None)
         self.samples = self.configP1Mon.get("samples", 1)
 
         # Unload if this module is disabled or misconfigured
         if not self.serverIP:
@@ -39,43 +38,40 @@
             logger.error(
                 "Cannot use P1Monitor module bacause the samples configured in config.json is not a value from 1 to 10!"
             )
             master.releaseModule("lib.TWCManager.EMS", "P1Monitor")
             return None
 
     def getConsumption(self):
-
         # Perform updates if necessary
         self.caller = "getConsumption"
         self.update()
 
         # Return current consumed value
         logger.log(logging.INFO2, "P1Monitor: consumedW (raw): " + str(self.consumedW))
         if self.consumedW > 0:
             return float(self.consumedW)
         else:
             return float(0)
 
     def getGeneration(self):
-
         # Perform updates if necessary
         self.caller = "getGeneration"
         self.update()
 
         # Return generation value
         logger.log(
             logging.INFO2, "P1Monitor: generatedW (raw): " + str(self.generatedW)
         )
         if self.generatedW > 0:
             return float(self.generatedW)
         else:
             return float(0)
 
     def getP1MonAPIData(self):
-
         # Fetch the specified data from the P1Monitor API and return the data
         self.fetchFailed = False
 
         url = (
             "http://"
             + self.serverIP
             + "/api/v1/phase?limit="
@@ -101,28 +97,26 @@
                 + str(e.response.status_code)
                 + " connecting to P1Monitor API to fetch sensor value"
             )
 
         return r.json()
 
     def update(self):
-
         if not self.p1monData or self.caller == "getConsumption":
             logger.log(
                 logging.INFO2, "P1Monitor: Refreshing data. Caller: " + self.caller
             )
             self.p1monData = self.getP1MonAPIData()
         else:
             logger.log(
                 logging.INFO2, "P1Monitor: Using existing data. Caller: " + self.caller
             )
 
         if self.p1monData:
             try:
-
                 logger.log(
                     logging.INFO3,
                     "P1Monitor: API Json Output: " + json.dumps(self.p1monData),
                 )
 
                 # Calculate the avarage trimming 10% of the highest and lowest values https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.trim_mean.html
                 CONSUMPTION_L1_W_Avg = scipy.stats.trim_mean(
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/EMS/SmartMe.py` & `TWCManager-1.3.0/lib/TWCManager/EMS/SmartMe.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 
 logger = logging.getLogger(__name__.rsplit(".")[-1])
 
 
 class SmartMe:
-
     # SmartMe EMS Module
     # Fetches Consumption and Generation details from SmartMe API
 
     import requests
     import time
 
     cacheTime = 10
@@ -41,28 +40,26 @@
         if (not self.status) or (
             not self.serialNumber or not self.username or not self.password
         ):
             self.master.releaseModule("lib.TWCManager.EMS", self.__class__.__name__)
             return None
 
     def getConsumption(self):
-
         if not self.status:
             logger.debug("EMS Module Disabled. Skipping getConsumption")
             return 0
 
         # While we don't have separate generation or consumption values, if
         # the value is a positive value we report it as consumption
         if self.generatedW < 0:
             return self.generatedW * -1
         else:
             return 0
 
     def getGeneration(self):
-
         if not self.status:
             logger.debug("EMS Module Disabled. Skipping getGeneration")
             return 0
 
         # Perform updates if necessary
         self.update()
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/EMS/SmartPi.py` & `TWCManager-1.3.0/lib/TWCManager/EMS/SmartPi.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import requests
 import time
 
 logger = logging.getLogger(__name__.rsplit(".")[-1])
 
 
 class SmartPi:
-
     # SmartPi EMS Module
     # Fetches Consumption and Generation details from SmartPi API
 
     cacheTime = 10
     config = None
     configConfig = None
     configSmartPi = None
@@ -37,28 +36,26 @@
 
         # Unload if this module is disabled or misconfigured
         if (not self.status) or (not self.serverIP):
             self.master.releaseModule("lib.TWCManager.EMS", self.__class__.__name__)
             return None
 
     def getConsumption(self):
-
         if not self.status:
             logger.debug("EMS Module Disabled. Skipping getConsumption")
             return 0
 
         # While we don't have separate generation or consumption values, if
         # the value is a positive value we report it as consumption
         if self.consumedW and self.showConsumption:
             return self.consumedW
         else:
             return 0
 
     def getGeneration(self):
-
         if not self.status:
             logger.debug("EMS Module Disabled. Skipping getGeneration")
             return 0
 
         # Perform updates if necessary
         self.update()
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/EMS/SolarLog.py` & `TWCManager-1.3.0/lib/TWCManager/EMS/SolarLog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 import time
 
 logger = logging.getLogger(__name__.rsplit(".")[-1])
 
 
 class SolarLog:
-
     # SolarLog EMS Module
     # Fetches Consumption and Generation details from SolarLog
 
     import requests
 
     cacheTime = 10
     config = None
@@ -40,27 +39,25 @@
 
         # Unload if this module is disabled or misconfigured
         if (not self.status) or (not self.serverIP):
             self.master.releaseModule("lib.TWCManager.EMS", "SolarLog")
             return None
 
     def getConsumption(self):
-
         if not self.status:
             logger.debug("SolarLog EMS Module Disabled. Skipping getConsumption")
             return 0
 
         # Perform updates if necessary
         self.update()
 
         # Return consumption value
         return self.consumedW - self.excludeConsumedW
 
     def getGeneration(self):
-
         if not self.status:
             logger.debug("SolarLog EMS Module Disabled. Skipping getGeneration")
             return 0
 
         # Perform updates if necessary
         self.update()
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/EMS/TED.py` & `TWCManager-1.3.0/lib/TWCManager/EMS/TED.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import time
 
 
 logger = logging.getLogger(__name__.rsplit(".")[-1])
 
 
 class TED:
-
     # I check solar panel generation using an API exposed by The
     # Energy Detective (TED). It's a piece of hardware available
     # at http://www.theenergydetective.com
 
     cacheTime = 10
     config = None
     configConfig = None
@@ -48,39 +47,36 @@
 
         # Unload if this module is disabled or misconfigured
         if (not self.status) or (not self.serverIP) or (int(self.serverPort) < 1):
             self.master.releaseModule("lib.TWCManager.EMS", "TED")
             return None
 
     def getConsumption(self):
-
         if not self.status:
             logger.debug("TED EMS Module Disabled. Skipping getConsumption")
             return 0
 
         # Perform updates if necessary
         self.update()
 
         # I don't believe this is implemented
         return float(0)
 
     def getGeneration(self):
-
         if not self.status:
             logger.debug("TED EMS Module Disabled. Skipping getGeneration")
             return 0
 
         # Perform updates if necessary
         self.update()
 
         # Return generation value
         return float(self.generatedW)
 
     def getTEDValue(self, url):
-
         # Fetch the specified URL from TED and return the data
         self.fetchFailed = False
 
         try:
             r = requests.get(url, timeout=self.timeout)
         except requests.exceptions.ConnectionError as e:
             logger.log(logging.INFO4, "Error connecting to TED to fetch solar data")
@@ -88,15 +84,14 @@
             self.fetchFailed = True
             return False
 
         r.raise_for_status()
         return r
 
     def update(self):
-
         if (int(time.time()) - self.lastFetch) > self.cacheTime:
             # Cache has expired. Fetch values from HomeAssistant sensor.
 
             url = "http://" + self.serverIP + ":" + self.serverPort
             url = url + "/history/export.csv?T=1&D=0&M=1&C=1"
 
             value = self.getTEDValue(url)
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/EMS/TeslaPowerwall2.py` & `TWCManager-1.3.0/lib/TWCManager/EMS/TeslaPowerwall2.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import logging
 import time
 
 logger = logging.getLogger(__name__.rsplit(".")[-1])
 
 
 class TeslaPowerwall2:
-
     import requests
     import urllib3
     import json as json
 
     cacheTime = 10
     cloudCacheTime = 1800
     config = None
@@ -157,24 +156,22 @@
                     logging.INFO6,
                     "Powerwall2 API token still valid for "
                     + str(self.tokenTimeout - time.time())
                     + " seconds.",
                 )
 
     def getConsumption(self):
-
         if not self.status:
             logger.debug("Powerwall2 EMS Module Disabled. Skipping getConsumption")
             return 0
 
         # Return consumption value
         return float(self.consumedW)
 
     def getGeneration(self):
-
         if not self.status:
             logger.debug("Powerwall2 EMS Module Disabled. Skipping getGeneration")
             return 0
 
         if self.batteryLevel > (self.minSOE * 1.05):
             self.suppressGeneration = False
         if self.batteryLevel < (self.minSOE * 0.95):
@@ -186,21 +183,19 @@
         if self.suppressGeneration:
             return 0
 
         # Return generation value
         return float(self.generatedW)
 
     def getPWJson(self, path):
-
         (lastTime, lastData) = (
             self.lastFetch[path] if path in self.lastFetch else (0, dict())
         )
 
         if (int(time.time()) - lastTime) > self.cacheTime:
-
             # Fetch the specified URL from Powerwall and return the data
 
             # Get a login token, if password authentication is enabled
             self.doPowerwallLogin()
 
             url = "https://" + self.serverIP + ":" + self.serverPort + path
             headers = dict()
@@ -247,15 +242,14 @@
         key = "CLOUD/live_status"
 
         (lastTime, lastData) = (
             self.lastFetch[key] if key in self.lastFetch else (0, dict())
         )
 
         if (int(time.time()) - lastTime) > self.cloudCacheTime:
-
             if token and now < expiry:
                 headers = {
                     "Authorization": "Bearer " + token,
                     "Content-Type": "application/json",
                 }
                 if not self.cloudID:
                     url = "https://owner-api.teslamotors.com/api/1/products"
@@ -278,15 +272,15 @@
                     if len(products) == 1:
                         (site, name) = products[0]
                         self.cloudID = site
                     elif len(products) > 1:
                         logger.info(
                             "Multiple Powerwall sites linked to your Tesla account.  Please specify the correct site ID in your config.json."
                         )
-                        for (site, name) in products:
+                        for site, name in products:
                             logger.info(f"   {site}: {name}")
                     else:
                         logger.info("Couldn't find a Powerwall on your Tesla account.")
 
                 if self.cloudID:
                     url = f"https://owner-api.teslamotors.com/api/1/energy_sites/{self.cloudID}/live_status"
                     bodyjson = None
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/EMS/URL.py` & `TWCManager-1.3.0/lib/TWCManager/EMS/URL.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import requests
 import time
 
 logger = logging.getLogger(__name__.rsplit(".")[-1])
 
 
 class URL:
-
     # URL EMS Module
     # Fetches Consumption and Generation details from URL
 
     apiKey = None
     cacheTime = 10  # in seconds
     config = None
     configConfig = None
@@ -44,27 +43,25 @@
 
         # Unload if this module is disabled or misconfigured
         if (not self.status) or (not self.URL):
             self.master.releaseModule("lib.TWCManager.EMS", "URL")
             return None
 
     def getConsumption(self):
-
         if not self.status:
             logger.debug("URL EMS Module Disabled. Skipping getConsumption")
             return 0
 
         # Perform updates if necessary
         self.update()
 
         # Return consumption value
         return self.consumedW
 
     def getGeneration(self):
-
         if not self.status:
             logger.debug("URL EMS Module Disabled. Skipping getGeneration")
             return 0
 
         # Perform updates if necessary
         self.update()
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/EMS/Volkszahler.py` & `TWCManager-1.3.0/lib/TWCManager/EMS/Volkszahler.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import time
 import re
 
 logger = logging.getLogger(__name__.rsplit(".")[-1])
 
 
 class Volkszahler:
-
     # Volkszahler EMS Module
     # Fetches Consumption and Generation details from Volkszahler API
 
     cacheTime = 10
     config = None
     configConfig = None
     configVolkszahler = None
@@ -40,15 +39,14 @@
 
         # Unload if this module is disabled or misconfigured
         if (not self.status) or (not self.serverIP) or (not self.uuidTotalGridW):
             self.master.releaseModule("lib.TWCManager.EMS", self.__class__.__name__)
             return None
 
     def getConsumption(self):
-
         if not self.status:
             logger.debug("EMS Module Disabled. Skipping getConsumption")
             return 0
 
         # Perform updates if necessary
         self.update()
 
@@ -56,15 +54,14 @@
         # negative 'TotalGridW' is 'Export to Grid'
         if (self.PhotovoltaikW + self.TotalGridW) > 0:
             return self.PhotovoltaikW + self.TotalGridW
         else:
             return 0
 
     def getGeneration(self):
-
         if not self.status:
             logger.debug("EMS Module Disabled. Skipping getGeneration")
             return 0
 
         # Perform updates if necessary
         self.update()
 
@@ -115,15 +112,14 @@
 
         if not httpResponse:
             logger.log(logging.INFO4, "Empty HTTP Response from Volkszahler API")
             self.fetchFailed = True
             return False
 
         else:
-
             msgMatch = re.search("^(.+) W$", httpResponse.text, re.DOTALL)
 
             if msgMatch:
                 self.PhotovoltaikW = float(msgMatch.group(1))
             else:
                 logger.log(
                     logging.INFO4,
@@ -171,15 +167,14 @@
 
         if not httpResponse:
             logger.log(logging.INFO4, "Empty HTTP Response from Volkszahler API")
             self.fetchFailed = True
             return False
 
         else:
-
             msgMatch = re.search("^(.+) W$", httpResponse.text, re.DOTALL)
 
             if msgMatch:
                 self.TotalGridW = float(msgMatch.group(1))
             else:
                 logger.log(
                     logging.INFO4,
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/Interface/Dummy.py` & `TWCManager-1.3.0/lib/TWCManager/Interface/Dummy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 import time
 
 logger = logging.getLogger(__name__.rsplit(".")[-1])
 
 
 class Dummy:
-
     enabled = False
     master = None
     msgBuffer = bytes()
     proto = None
     twcID = bytearray(b"\x12\x34")
     timeLastTx = 0
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/Interface/RS485.py` & `TWCManager-1.3.0/lib/TWCManager/Interface/RS485.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 import time
 
 logger = logging.getLogger("\U0001F50C RS485")
 
 
 class RS485:
-
     import serial
 
     baud = 9600
     enabled = True
     master = None
     port = None
     ser = None
@@ -44,29 +43,45 @@
         if "interface" in master.config:
             portb = master.config["interface"]["RS485"].get("port", "")
         if portb:
             self.port = portb
         elif porta:
             self.port = porta
 
+        self.connect()
+
+    def connect(self):
+        # Reset any Slave TWC last RX heartbeat counters in case serial reconnection has occurred
+        for slaveTWC in self.master.getSlaveTWCs():
+            slaveTWC.timeLastRx = time.time()
+
         # Connect to serial port
         self.ser = self.serial.serial_for_url(self.port, self.baud, timeout=0)
 
     def close(self):
         # Close the serial interface
         return self.ser.close()
 
     def getBufferLen(self):
         # This function returns the size of the recieve buffer.
         # This is used by read functions to determine if information is waiting
         return self.ser.inWaiting()
 
     def read(self, len):
         # Read the specified amount of data from the serial interface
-        return self.ser.read(len)
+        try:
+            return self.ser.read(len)
+        except serial.serialutil.SerialException as e:
+            logger.log(
+                logging.ERROR,
+                "Error reading from serial interface: {}. Will attempt re-connect.".format(
+                    e
+                ),
+            )
+            self.connect()
 
     def send(self, msg):
         # Send msg on the RS485 network. We'll escape bytes with a special meaning,
         # add a CRC byte to the message end, and add a C0 byte to the start and end
         # to mark where it begins and ends.
 
         msg = bytearray(msg)
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/Interface/TCP.py` & `TWCManager-1.3.0/lib/TWCManager/Interface/TCP.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import socket
 
 
 logger = logging.getLogger(__name__.rsplit(".")[-1])
 
 
 class TCP:
-
     import time
 
     config = None
     configTCP = None
     enabled = False
     master = None
     port = 6000
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/Logging/CSVLogging.py` & `TWCManager-1.3.0/lib/TWCManager/Logging/CSVLogging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # CSVLogging module. Provides output to CSV file for regular stats
 
 import logging
 
 
 class CSVLogging:
-
     capabilities = {"queryGreenEnergy": False}
     config = None
     configConfig = None
     configLogging = None
     openSessions = {}
     quoteColumns = True
     status = False
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/Logging/ConsoleLogging.py` & `TWCManager-1.3.0/lib/TWCManager/Logging/SentryLogging.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,53 @@
-# ConsoleLogging module. Provides output to console for logging.
+# SentryLogging module. Provides output to console for logging.
 import logging
 
-import sys
-from termcolor import colored
-
+import sentry_sdk
+from sentry_sdk.integrations.logging import LoggingIntegration
 
 logger = logging.getLogger(__name__.rsplit(".")[-1])
 
 
-class ColorFormatter(logging.Formatter):
-    def format(self, record):
-        if hasattr(record, "colored"):
-            old_args = record.args
-            record.args = tuple(colored(arg, record.colored) for arg in record.args)
-            s = super(ColorFormatter, self).format(record)
-            record.args = old_args
-        else:
-            s = super(ColorFormatter, self).format(record)
-        return s
-
-
-class ConsoleLogging:
-
+class SentryLogging:
     capabilities = {"queryGreenEnergy": False}
     config = None
     configConfig = None
     configLogging = None
     status = True
+    logger = None
+    mute = {}
+    muteDebugLogLevelGreaterThan = 1
 
     def __init__(self, master):
+        # raise ImportError
         self.master = master
         self.config = master.config
         try:
             self.configConfig = master.config["config"]
         except KeyError:
             self.configConfig = {}
         try:
-            self.configLogging = master.config["logging"]["Console"]
+            self.configLogging = master.config["logging"]["Sentry"]
         except KeyError:
             self.configLogging = {}
-        self.status = self.configLogging.get("enabled", True)
+        self.status = self.configLogging.get("enabled", False)
+        self.dsn = self.configLogging.get("DSN", False)
 
         # Unload if this module is disabled or misconfigured
-        if not self.status:
-            self.master.releaseModule("lib.TWCManager.Logging", "ConsoleLogging")
+        if not self.status or not self.dsn:
+            self.master.releaseModule("lib.TWCManager.Logging", "SentryLogging")
             return None
 
         # Initialize the mute config tree if it is not already
-        if not self.configLogging.get("mute", None):
-            self.configLogging["mute"] = {}
+        self.mute = self.configLogging.get("mute", {})
+        self.muteDebugLogLevelGreaterThan = self.mute.get("DebugLogLevelGreaterThan", 1)
 
         # Initialize Logger
-        color_formatter = ColorFormatter(
-            colored("%(asctime)s", "yellow")
-            + " "
-            + colored("%(name)-10.10s", "green")
-            + " "
-            + colored("%(levelno)d", "cyan")
-            + " %(message)s",
-            "%H:%M:%S",
+        sentry_logging = LoggingIntegration(
+            level=logging.INFO,  # Capture info and above as breadcrumbs
+            event_level=logging.ERROR,  # Send errors as events
         )
-        handler = logging.StreamHandler(sys.stdout)
-        handler.setFormatter(color_formatter)
-        # handler.setLevel(logging.INFO)
-        logging.getLogger("").addHandler(handler)
+        sentry_sdk.init(self.dsn, integrations=[sentry_logging], traces_sample_rate=1.0)
 
     def getCapabilities(self, capability):
         # Allows query of module capabilities when deciding which Logging module to use
         return self.capabilities.get(capability, False)
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/Logging/FileLogging.py` & `TWCManager-1.3.0/lib/TWCManager/Logging/FileLogging.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import re
 
 
 logger = logging.getLogger(__name__.rsplit(".")[-1])
 
 
 class FileLogging:
-
     capabilities = {"queryGreenEnergy": False}
     config = None
     configConfig = None
     configLogging = None
     status = True
     logger = None
     mute = {}
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/Logging/MySQLLogging.py` & `TWCManager-1.3.0/lib/TWCManager/Logging/MySQLLogging.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 logger = logging.getLogger(__name__.rsplit(".")[-1])
 
 
 class MySQLHandler(logging.Handler):
     slaveSession = {}
 
     def __init__(self, db):
-
         logging.Handler.__init__(self)
         self.db = db
 
     def emit(self, record):
         self.format(record)
         log_type = getattr(record, "logtype", "")
         if log_type == "charge_sessions":
@@ -170,15 +169,14 @@
                 # Issue, log message and rollback
                 logger.info("Error updating MySQL database. Rows = %d" % rows)
                 self.db.rollback()
             cur.close()
 
 
 class MySQLLogging:
-
     capabilities = {"queryGreenEnergy": True}
     config = None
     configConfig = None
     configLogging = None
     db = None
     status = False
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/Logging/SQLiteLogging.py` & `TWCManager-1.3.0/lib/TWCManager/Logging/SQLiteLogging.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import logging
 
 logger = logging.getLogger(__name__.rsplit(".")[-1])
 
 
 class SQLiteHandler(logging.Handler):
     def __init__(self, db):
-
         logging.Handler.__init__(self)
         self.db = db
         # Initialize the database schema for a database that does not
         # yet exist
         query_charge_sessions = """
           CREATE TABLE IF NOT EXISTS charge_sessions (
               chargeid int,
@@ -140,15 +139,14 @@
                 else:
                     # Issue, log message and rollback
                     logger.info("Error updating SQLite database. Rows = %d" % rows)
                     conn.rollback()
 
 
 class SQLiteLogging:
-
     capabilities = {"queryGreenEnergy": True}
     config = None
     configConfig = None
     configLogging = None
     db = None
     status = False
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/Policy/Policy.py` & `TWCManager-1.3.0/lib/TWCManager/Policy/Policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import time
 
 
 logger = logging.getLogger("\u26FD Policy")
 
 
 class Policy:
-
     active_policy = None
 
     # This is the default charge policy.  It can be overridden or extended.
     default_policy = [
         # The first policy table entry is for chargeNow. This will fire if
         # chargeNowAmps is set to a positive integer and chargeNowTimeEnd
         # is less than or equal to the current timestamp
@@ -92,37 +91,35 @@
                 # Policy override specified, just override in place without processing the
                 # extensions
                 self.charge_policy = config_policy.get("override")
             else:
                 config_extend = config_policy.get("extend", {})
 
                 # Get additional restrictions
-                for (name, restrictions) in config_extend.get(
-                    "restrictions", {}
-                ).items():
+                for name, restrictions in config_extend.get("restrictions", {}).items():
                     restricted = self.getPolicyByName(name)
                     for key in ("match", "condition", "value"):
                         restricted[key] += restrictions.get(key, [])
 
                 # Get webhooks
-                for (name, hooks) in config_extend.get("webhooks", {}).items():
+                for name, hooks in config_extend.get("webhooks", {}).items():
                     hooked = self.getPolicyByName(name)
                     hooked["webhooks"] = hooks
 
                 # Green Energy Latching
                 if "greenEnergyLatch" in self.config["config"]:
                     self.charge_policy[2]["latch_period"] = self.config["config"][
                         "greenEnergyLatch"
                     ]
 
                 # Insert optional policy extensions into policy list:
                 #   After - Inserted before Non-Scheduled Charging
                 #   Before - Inserted after Charge Now
                 #   Emergency - Inserted at the beginning
-                for (name, position) in [("after", 3), ("before", 1), ("emergency", 0)]:
+                for name, position in [("after", 3), ("before", 1), ("emergency", 0)]:
                     self.charge_policy[position:position] = config_extend.get(name, [])
 
             if config_policy.get("alwaysPollEMS", False):
                 for policy in self.charge_policy:
                     if policy.get("background_task", None) is None:
                         policy["background_task"] = "checkGreenEnergy"
 
@@ -149,15 +146,14 @@
         if (self.lastPolicyCheck + self.policyCheckInterval) > time.time():
             return
         else:
             # Update last policy check time
             self.lastPolicyCheck = time.time()
 
         for policy in self.charge_policy:
-
             # Check if the policy is within its latching period
             latched = False
             if "__latchTime" in policy:
                 if time.time() < policy["__latchTime"]:
                     latched = True
                 else:
                     del policy["__latchTime"]
@@ -229,27 +225,56 @@
             if currentCharge < 50:
                 currentCharge = 50
             limit = currentCharge if limit == -1 else min(limit, currentCharge)
         if not (limit >= 50 and limit <= 100):
             limit = -1
         self.master.queue_background_task({"cmd": "applyChargeLimit", "limit": limit})
 
+        # Report current policy via Status modules
+        for module in self.master.getModulesByType("Status"):
+            module["ref"].setStatus(
+                bytes("all", "UTF-8"),
+                "current_policy",
+                "currentPolicy",
+                policy["name"],
+                "",
+            )
+
     def fireWebhook(self, hook):
         policy = self.getPolicyByName(self.active_policy)
         if policy:
             url = policy.get("webhooks", {}).get(hook, None)
             if url:
                 self.master.queue_background_task({"cmd": "webhook", "url": url})
 
     def getPolicyByName(self, name):
         for policy in self.charge_policy:
             if policy["name"] == name:
                 return policy
         return None
 
+    def getActivePolicyAction(self):
+        # getActivePolicyAction returns an integer value depending on what
+        # charging action the currently active policy is following. Values
+        # correspond to nonScheduledAction values in settings.json:
+        # 1 ... fixed rate charging
+        # 2 ... do not charge
+        # 3 ... track green energy charging
+        # <None> will be returned if self.active_policy is not (yet) set
+        if self.active_policy == None:
+            return None
+        if self.policyIsGreen():
+            return 3
+        else:
+            policy = self.getPolicyByName(self.active_policy)
+            if int(self.policyValue(policy.get("charge_amps", 0))) > 0:
+                return 1
+            else:
+                return 2
+
     def policyValue(self, value):
         # policyValue is a macro to allow charging policy to refer to things
         # such as EMS module values or settings. This allows us to control
         # charging via policy.
         ltNow = time.localtime()
 
         # Anything other than a string can only be a literal value
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/Protocol/TWCProtocol.py` & `TWCManager-1.3.0/lib/TWCManager/Protocol/TWCProtocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 import re
 
 logger = logging.getLogger(__name__.rsplit(".")[-1])
 
 
 class TWCProtocol:
-
     # To avoid a situation where we would have to re-implement TWCManager logic to parse the
     # same messages both for the Dummy interface and for the Slave TWCManager mode, we break out
     # parsing of the protocol to this module.
 
     # The operationMode parameter determines which mode the parser operates in:
     #   1 = Slave
     #   2 = Master (not currently implemented)
@@ -20,15 +19,14 @@
 
     def __init__(self, master):
         self.master = master
         self.operationMode = 0
         classname = self.__class__.__name__
 
     def createMessage(self, packet):
-
         # We take some steps to be as autonomous as possible. One of these
         # steps is to automatically fill in fields where we can likely
         # determine the correct value
         if not packet.get("SenderID", None):
             packet["SenderID"] = bytearray(str(self.master.masterTWCID).encode("utf-8"))
         if packet.get("Command", "") != "SlaveLinkready":
             if not packet.get("RecieverID", None):
@@ -99,15 +97,14 @@
             )
             if self.master.protocolVersion == 2:
                 msg += bytearray(b"\x00\x00")
 
             return msg
 
     def parseMessage(self, msg):
-
         # Define protocol packet format
         packet = {"Command": None, "Errors": [], "SenderID": None, "Match": False}
 
         msgMatch = re.search(
             b"\xfc\xe1(..)(.)\x00\x00\x00\x00\x00\x00\x00\x00+?.*\Z",
             msg,
             re.DOTALL,
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/Status/HASSStatus.py` & `TWCManager-1.3.0/lib/TWCManager/Status/HASSStatus.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import time
 
 
 logger = logging.getLogger("\U0001F4CA HASS")
 
 
 class HASSStatus:
-
     import threading
     import requests
 
     apiKey = None
     config = None
     configConfig = None
     configHASS = None
@@ -191,15 +190,14 @@
 
     def settingRetryRate(self, msg):
         # Setting elapsing time to now + retryRateInSeconds
         self.msgQueue[msg.sensor].elapsingTime = time.time() + self.retryRateInSeconds
 
 
 class HASSMessage:
-
     elapsingTime = 0
     sensor = ""
     twcid = ""
     key_underscore = ""
     key_camelcase = ""
     value = None
     unit = ""
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/Status/MQTTStatus.py` & `TWCManager-1.3.0/lib/TWCManager/Status/MQTTStatus.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import time
 
 
 logger = logging.getLogger("\U0001F4CA MQTT")
 
 
 class MQTTStatus:
-
     import paho.mqtt.client as mqtt
 
     brokerIP = None
     brokerPort = 1883
     __carsCharging = {}
     __config = None
     __configConfig = None
@@ -59,15 +58,14 @@
         if self.__carsCharging.get(twident, "0") != str(value):
             if str(value) == "0":
                 self.setStatus(twc, "amps_in_use", "ampsInUse", 0, "A")
         self.__carsCharging[twident] = str(value)
 
     def setStatus(self, twcid, key_underscore, key_camelcase, value, unit):
         if self.status:
-
             # Format TWCID nicely
             twident = None
             if len(twcid) == 2:
                 twident = "%02X%02X" % (twcid[0], twcid[1])
             else:
                 twident = str(twcid.decode("utf-8"))
             topic = self.topicPrefix + "/" + twident
@@ -149,15 +147,17 @@
                 "Publishing MQTT Topic "
                 + str(msg["topic"])
                 + " (value is "
                 + str(msg["payload"])
                 + ")",
             )
             try:
-                pub = client.publish(msg["topic"], payload=msg["payload"], qos=0)
+                pub = client.publish(
+                    msg["topic"], payload=msg["payload"], qos=0, retain=True
+                )
             except e:
                 logger.log(logging.INFO4, "Error publishing MQTT Topic Status")
                 logger.debug(str(e))
 
         client.loop_stop()
         self.msgQueueBuffer.clear()
         self.connectionState = 0
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/TWCManager.py` & `TWCManager-1.3.0/lib/TWCManager/TWCManager.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,22 +82,24 @@
     "Policy.Policy",
     "Vehicle.TeslaAPI",
     "Vehicle.TeslaMateVehicle",
     "Control.WebIPCControl",
     "Control.HTTPControl",
     "Control.MQTTControl",
     #    "Control.OCPPControl",
+    "EMS.DSMRreader",
     "EMS.Efergy",
     "EMS.EmonCMS",
     "EMS.Enphase",
     "EMS.Fronius",
     "EMS.Growatt",
     "EMS.HASS",
     "EMS.IotaWatt",
     "EMS.Kostal",
+    "EMS.MQTT",
     "EMS.OpenHab",
     "EMS.OpenWeatherMap",
     "EMS.P1Monitor",
     "EMS.SmartMe",
     "EMS.SmartPi",
     "EMS.SolarEdge",
     "EMS.SolarLog",
@@ -355,102 +357,94 @@
 
     # Set max amps iff charge_amps isn't specified on the policy.
     if master.getModuleByName("Policy").policyIsGreen():
         master.setMaxAmpsToDivideAmongSlaves(master.getMaxAmpsToDivideGreenEnergy())
 
 
 def update_statuses():
-
     # Print a status update if we are on track green energy showing the
     # generation and consumption figures
     maxamps = master.getMaxAmpsToDivideAmongSlaves()
     maxampsDisplay = f"{maxamps:.2f}A"
+    subtractChargerLoad = config["config"].get("subtractChargerLoad", False)
+    treatGenerationAsGridDelivery = config["config"].get(
+        "treatGenerationAsGridDelivery", False
+    )
     if master.getModuleByName("Policy").policyIsGreen():
         genwatts = master.getGeneration()
         conwatts = master.getConsumption()
         conoffset = master.getConsumptionOffset()
         chgwatts = master.getChargerLoad()
         othwatts = 0
 
-        if config["config"]["subtractChargerLoad"]:
+        if subtractChargerLoad:
             if conwatts > 0:
                 othwatts = conwatts - chgwatts
 
             if conoffset > 0:
                 othwatts -= conoffset
 
+        if treatGenerationAsGridDelivery:
+            # Calculate total generation when it is already consumed by TWC
+            genwatts = max(0, genwatts + chgwatts - conwatts)
+
         # Extra parameters to send with logs
         logExtra = {
             "logtype": "green_energy",
             "genWatts": genwatts,
             "conWatts": conwatts,
             "chgWatts": chgwatts,
             "colored": "magenta",
         }
 
         if (genwatts or conwatts) and (not conoffset and not othwatts):
-
             logger.info(
                 "Green energy Generates %s, Consumption %s (Charger Load %s)",
                 f"{genwatts:.0f}W",
                 f"{conwatts:.0f}W",
                 f"{chgwatts:.0f}W",
                 extra=logExtra,
             )
 
         elif (genwatts or conwatts) and othwatts and not conoffset:
-
             logger.info(
                 "Green energy Generates %s, Consumption %s (Charger Load %s, Other Load %s)",
                 f"{genwatts:.0f}W",
                 f"{conwatts:.0f}W",
                 f"{chgwatts:.0f}W",
                 f"{othwatts:.0f}W",
                 extra=logExtra,
             )
 
         elif (genwatts or conwatts) and othwatts and conoffset > 0:
-
             logger.info(
                 "Green energy Generates %s, Consumption %s (Charger Load %s, Other Load %s, Offset %s)",
                 f"{genwatts:.0f}W",
                 f"{conwatts:.0f}W",
                 f"{chgwatts:.0f}W",
                 f"{othwatts:.0f}W",
                 f"{conoffset:.0f}W",
                 extra=logExtra,
             )
 
         elif (genwatts or conwatts) and othwatts and conoffset < 0:
-
             logger.info(
                 "Green energy Generates %s (Offset %s), Consumption %s (Charger Load %s, Other Load %s)",
                 f"{genwatts:.0f}W",
                 f"{(-1 * conoffset):.0f}W",
                 f"{conwatts:.0f}W",
                 f"{chgwatts:.0f}W",
                 f"{othwatts:.0f}W",
                 extra=logExtra,
             )
 
         nominalOffer = master.convertWattsToAmps(
             genwatts
-            + (
-                chgwatts
-                if (config["config"]["subtractChargerLoad"] and conwatts == 0)
-                else 0
-            )
-            - (
-                conwatts
-                - (
-                    chgwatts
-                    if (config["config"]["subtractChargerLoad"] and conwatts > 0)
-                    else 0
-                )
-            )
+            + (chgwatts if (subtractChargerLoad and conwatts == 0) else 0)
+            - (conwatts - (chgwatts if (subtractChargerLoad and conwatts > 0) else 0))
         )
         if abs(maxamps - nominalOffer) > 0.005:
             nominalOfferDisplay = f"{nominalOffer:.2f}A"
             logger.debug(
                 f"Offering {maxampsDisplay} instead of {nominalOfferDisplay} to compensate for inexact current draw"
             )
             conwatts = genwatts - master.convertAmpsToWatts(maxamps)
@@ -491,15 +485,14 @@
             "maxAmpsForSlaves",
             master.getMaxAmpsToDivideAmongSlaves(),
             "A",
         )
 
 
 def update_sunrise_sunset():
-
     ltNow = time.localtime()
     latlong = master.getHomeLatLon()
     if latlong[0] == 10000:
         # We don't know where home is; keep defaults
         master.settings["sunrise"] = 6
         master.settings["sunset"] = 20
     else:
@@ -698,15 +691,17 @@
                 # as long as no slave was connected, but since real slaves send
                 # linkready once every 10 seconds till they're connected to a
                 # master, we'll just wait for that.
                 if time.time() - master.getTimeLastTx() >= 1.0:
                     # It's been about a second since our last heartbeat.
                     if master.countSlaveTWC() > 0:
                         slaveTWC = master.getSlaveTWC(idxSlaveToSendNextHeartbeat)
-                        if time.time() - slaveTWC.timeLastRx > 26:
+                        if time.time() - slaveTWC.timeLastRx > config.get(
+                            "interfaces", {}
+                        ).get("RS485", {}).get("slaveTimeout", 26):
                             # A real master stops sending heartbeats to a slave
                             # that hasn't responded for ~26 seconds. It may
                             # still send the slave a heartbeat every once in
                             # awhile but we're just going to scratch the slave
                             # from our little black book and add them again if
                             # they ever send us a linkready.
                             logger.info(
@@ -1168,14 +1163,23 @@
                             "logtype": "slave_status",
                             "TWCID": senderID,
                             "kWh": kWh,
                             "voltsPerPhase": [voltsPhaseA, voltsPhaseB, voltsPhaseC],
                         },
                     )
 
+                    # Set minAmpsTWCSupports to 1A for 3 phase chargers
+                    if voltsPhaseA >= 200 and voltsPhaseB >= 200 and voltsPhaseC >= 200:
+                        slaveTWC.minAmpsTWCSupports = 1
+                        logger.debug(
+                            "Slave TWC %02X%02X: Set minAmpsTWCSupports to 1A",
+                            senderID[0],
+                            senderID[1],
+                        )
+
                     # Update the timestamp of the last reciept of this message
                     master.lastkWhMessage = time.time()
 
                     # Every time we get this message, we re-queue the query
                     master.queue_background_task({"cmd": "getLifetimekWh"})
 
                     # Update this detail for the Slave TWC
@@ -1226,15 +1230,95 @@
                                 "vinPart": str(vinPart),
                             }
                         )
                     else:
                         potentialVIN = "".join(slaveTWC.VINData)
 
                         # Ensure we have a valid VIN
-                        if len(potentialVIN) == 17:
+                        vinValid = True
+
+                        if len(potentialVIN) != 17 and len(potentialVIN) != 0:
+                            vinValid = False
+
+                        if vinValid and len(potentialVIN) == 17:
+                            potentialVIN = potentialVIN.upper()
+                            check = potentialVIN[8]
+                            if check == "X":
+                                check = 10
+                            elif check.isdigit():
+                                check = int(check)
+                            else:
+                                vinValid = False
+
+                        if vinValid and len(potentialVIN) == 17:
+                            weights = [
+                                8,
+                                7,
+                                6,
+                                5,
+                                4,
+                                3,
+                                2,
+                                10,
+                                0,
+                                9,
+                                8,
+                                7,
+                                6,
+                                5,
+                                4,
+                                3,
+                                2,
+                            ]
+                            replaceValues = {
+                                "A": 1,
+                                "B": 2,
+                                "C": 3,
+                                "D": 4,
+                                "E": 5,
+                                "F": 6,
+                                "G": 7,
+                                "H": 8,
+                                "J": 1,
+                                "K": 2,
+                                "L": 3,
+                                "M": 4,
+                                "N": 5,
+                                "P": 7,
+                                "R": 9,
+                                "S": 2,
+                                "T": 3,
+                                "U": 4,
+                                "V": 5,
+                                "W": 6,
+                                "X": 7,
+                                "Y": 8,
+                                "Z": 9,
+                                "1": 1,
+                                "2": 2,
+                                "3": 3,
+                                "4": 4,
+                                "5": 5,
+                                "6": 6,
+                                "7": 7,
+                                "8": 8,
+                                "9": 9,
+                                "0": 0,
+                            }
+
+                            sum = 0
+                            for digit, weight in zip(potentialVIN, weights):
+                                if digit not in replaceValues:
+                                    vinValid = False
+                                    break
+                                sum += replaceValues[digit] * weight
+                            if sum % 11 != check:
+                                vinValid = False
+
+                        if vinValid:
                             # Record Vehicle VIN
                             slaveTWC.currentVIN = potentialVIN
 
                             # Clear VIN retry timer
                             slaveTWC.lastVINQuery = 0
                             slaveTWC.vinQueryAttempt = 0
 
@@ -1251,15 +1335,15 @@
                                     "cmd": "checkVINEntitlement",
                                     "subTWC": slaveTWC,
                                 }
                             )
 
                             vinPart += 1
                         else:
-                            # Unfortunately the VIN was not the right length.
+                            # Unfortunately the VIN was not received correctly.
                             # Re-request VIN
                             master.queue_background_task(
                                 {
                                     "cmd": "getVehicleVIN",
                                     "slaveTWC": slaveTWC.TWCID,
                                     "vinPart": 0,
                                 }
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/TWCMaster.py` & `TWCManager-1.3.0/lib/TWCManager/TWCMaster.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import requests
 import bisect
 
 logger = logging.getLogger("\u26FD Master")
 
 
 class TWCMaster:
-
     allowed_flex = 0
     backgroundTasksQueue = queue.Queue()
     backgroundTasksCmds = {}
     backgroundTasksLock = threading.Lock()
     backgroundTasksDelayed = []
     config = None
     consumptionValues = {}
@@ -60,33 +59,37 @@
         [0x01, 0x0F, 0xA0, 0x0F, 0xA0, 0x00, 0x00, 0x00, 0x00]
     )
     slaveTWCs = {}
     slaveTWCRoundRobin = []
     stopTimeout = datetime.max
     spikeAmpsToCancel6ALimit = 16
     subtractChargerLoad = False
+    treatGenerationAsGridDelivery = False
     teslaLoginAskLater = False
     TWCID = None
     updateVersion = False
-    version = "1.2.6"
+    version = "1.3.0"
 
     # TWCs send a seemingly-random byte after their 2-byte TWC id in a number of
     # messages. I call this byte their "Sign" for lack of a better term. The byte
     # never changes unless the TWC is reset or power cycled. We use hard-coded
     # values for now because I don't know if there are any rules to what values can
     # be chosen. I picked 77 because it's easy to recognize when looking at logs.
     # These shouldn't need to be changed.
     masterSign = bytearray(b"\x77")
     slaveSign = bytearray(b"\x77")
 
     def __init__(self, TWCID, config):
         self.config = config
         self.debugOutputToFile = config["config"].get("debugOutputToFile", False)
         self.TWCID = TWCID
-        self.subtractChargerLoad = config["config"]["subtractChargerLoad"]
+        self.subtractChargerLoad = config["config"].get("subtractChargerLoad", False)
+        self.treatGenerationAsGridDelivery = config["config"].get(
+            "treatGenerationAsGridDelivery", False
+        )
         self.advanceHistorySnap()
 
         # Register ourself as a module, allows lookups via the Module architecture
         self.registerModule({"name": "master", "ref": self, "type": "Master"})
 
     def addkWhDelivered(self, kWh):
         self.settings["kWhDelivered"] = self.settings.get("kWhDelivered", 0) + kWh
@@ -159,15 +162,14 @@
         for module in self.getModulesByType(type):
             if module["ref"].getCapabilities(capability):
                 match = True
 
         return match
 
     def checkScheduledCharging(self):
-
         # Check if we're within the hours we must use scheduledAmpsMax instead
         # of nonScheduledAmpsMax
         blnUseScheduledAmps = 0
         ltNow = time.localtime()
         hourNow = ltNow.tm_hour + (ltNow.tm_min / 60)
         timeSettings = self.getScheduledAmpsTimeFlex()
         startHour = timeSettings[0]
@@ -253,15 +255,14 @@
             task["cmd"] in self.backgroundTasksCmds
             and self.backgroundTasksCmds[task["cmd"]] == task
         ):
             del self.backgroundTasksCmds[task["cmd"]]["cmd"]
             del self.backgroundTasksCmds[task["cmd"]]
 
     def doneBackgroundTask(self, task):
-
         # Delete task['cmd'] from backgroundTasksCmds such that
         # queue_background_task() can queue another task['cmd'] in the future.
         if "cmd" in task:
             del self.backgroundTasksCmds[task["cmd"]]
 
         # task_done() must be called to let the queue know the task is finished.
         # backgroundTasksQueue.join() can then be used to block until all tasks
@@ -421,15 +422,14 @@
     def getScheduledAmpsEndHour(self):
         return self.settings.get("scheduledAmpsEndHour", -1)
 
     def getScheduledAmpsFlexStart(self):
         return int(self.settings.get("scheduledAmpsFlexStart", False))
 
     def getSlaveLifetimekWh(self):
-
         # This function is called from a Scheduled Task
         # If it's been at least 1 minute, then query all known Slave TWCs
         # to determine their lifetime kWh and per-phase voltages
         now = time.time()
         if now >= self.lastkWhPoll + 60:
             for slaveTWC in self.getSlaveTWCs():
                 self.getInterfaceModule().send(
@@ -591,35 +591,37 @@
             generationVal += float(self.generationValues[key])
 
         if generationVal < 0:
             generationVal = 0
 
         offset = self.getConsumptionOffset()
         if offset < 0:
-            generationVal += -1 * offset
+            generationVal -= offset
 
         return float(generationVal)
 
     def getGenerationOffset(self):
         # Returns the number of watts to subtract from the solar generation stats
         # This is consumption + charger load if subtractChargerLoad is enabled
         # Or simply consumption if subtractChargerLoad is disabled
         generationOffset = self.getConsumption()
         if self.subtractChargerLoad:
             generationOffset -= self.getChargerLoad()
-        if generationOffset < 0:
+        # Allow negative offset when EMS reports grid delivery instead of
+        # generation. This means the offset increases the total generation.
+        if generationOffset < 0 and not self.treatGenerationAsGridDelivery:
             generationOffset = 0
         return float(generationOffset)
 
     def getHomeLatLon(self):
         # Returns Lat/Lon coordinates to check if car location is
         # at home
         latlon = [10000, 10000]
-        latlon[0] = self.settings.get("homeLat", 10000)
-        latlon[1] = self.settings.get("homeLon", 10000)
+        latlon[0] = float(self.settings.get("homeLat", 10000))
+        latlon[1] = float(self.settings.get("homeLon", 10000))
         return latlon
 
     def getMasterHeartbeatOverride(self):
         return self.overrideMasterHeartbeatData
 
     def getMaxAmpsToDivideGreenEnergy(self):
         # Calculate our current generation and consumption in watts
@@ -629,15 +631,15 @@
         # Calculate what we should offer to align with green energy
         #
         # The current offered shouldn't increase more than / must
         # decrease at least the current gap between generation and
         # consumption.
 
         currentOffer = max(
-            self.getMaxAmpsToDivideAmongSlaves(),
+            int(self.getMaxAmpsToDivideAmongSlaves()),
             self.num_cars_charging_now() * self.config["config"]["minAmpsPerTWC"],
         )
         newOffer = currentOffer + self.convertWattsToAmps(generationW - consumptionW)
 
         # This is the *de novo* calculation of how much we can offer
         #
         # Fetches and uses consumptionW separately
@@ -650,14 +652,18 @@
         return round(amps, 2)
 
     def getNormalChargeLimit(self, ID):
         if "chargeLimits" in self.settings and str(ID) in self.settings["chargeLimits"]:
             result = self.settings["chargeLimits"][str(ID)]
             if type(result) is int:
                 result = (result, 0)
+            if result[0] is None:
+                result[0] = 0
+            if result[1] is None:
+                result[1] = 0
             return (True, result[0], result[1])
         return (False, None, None)
 
     def getSlaveByID(self, twcid):
         return self.slaveTWCs[twcid]
 
     def getSlaveTWCID(self, twc):
@@ -677,47 +683,56 @@
             totalAmps += slaveTWC.reportedAmpsActual
 
         logger.debug("Total amps all slaves are using: " + str(totalAmps))
         return totalAmps
 
     def getVoltageMeasurement(self):
         slavesWithVoltage = [
-            slave for slave in self.getSlaveTWCs() if slave.voltsPhaseA > 0
+            slave
+            for slave in self.getSlaveTWCs()
+            if (slave.voltsPhaseA > 0 or slave.voltsPhaseB > 0 or slave.voltsPhaseC > 0)
         ]
         if len(slavesWithVoltage) == 0:
             # No slaves support returning voltage
             return (
                 self.config["config"].get("defaultVoltage", 240),
                 self.config["config"].get("numberOfPhases", 1),
             )
 
         total = 0
         phases = 0
-        if any([slave.voltsPhaseC > 0 for slave in slavesWithVoltage]):
-            # Three-phase system
-            phases = 3
-            if all([slave.voltsPhaseC > 0 for slave in slavesWithVoltage]):
-                total = sum(
-                    [
-                        (slave.voltsPhaseA + slave.voltsPhaseB + slave.voltsPhaseC)
-                        for slave in slavesWithVoltage
-                    ]
-                )
+
+        # Detect number of active phases
+        for slave in slavesWithVoltage:
+            localPhases = 0
+            if slave.voltsPhaseA:
+                localPhases += 1
+            if slave.voltsPhaseB:
+                localPhases += 1
+            if slave.voltsPhaseC:
+                localPhases += 1
+
+            if phases:
+                if localPhases != phases:
+                    logger.info(
+                        "FATAL:  Mix of multi-phase TWC configurations not currently supported."
+                    )
+                    return (
+                        self.config["config"].get("defaultVoltage", 240),
+                        self.config["config"].get("numberOfPhases", 1),
+                    )
             else:
-                logger.info(
-                    "FATAL:  Mix of three-phase and single-phase not currently supported."
-                )
-                return (
-                    self.config["config"].get("defaultVoltage", 240),
-                    self.config["config"].get("numberOfPhases", 1),
-                )
-        else:
-            # Single-phase system
-            total = sum([slave.voltsPhaseA for slave in slavesWithVoltage])
-            phases = 1
+                phases = localPhases
+
+        total = sum(
+            [
+                (slave.voltsPhaseA + slave.voltsPhaseB + slave.voltsPhaseC)
+                for slave in slavesWithVoltage
+            ]
+        )
 
         return (total / (phases * len(slavesWithVoltage)), phases)
 
     def hex_str(self, s: str):
         return " ".join("{:02X}".format(ord(c)) for c in s)
 
     def hex_str(self, ba: bytearray):
@@ -816,15 +831,14 @@
                 + "."
             )
             self.deleteSlaveTWC(self.getSlaveTWCID(0))
 
         return slaveTWC
 
     def num_cars_charging_now(self):
-
         carsCharging = 0
         for slaveTWC in self.getSlaveTWCs():
             if slaveTWC.reportedAmpsActual >= 1.0:
                 if slaveTWC.isCharging == 0:
                     # We have detected that a vehicle has started charging on this Slave TWC
                     # Attempt to request the vehicle's VIN
                     slaveTWC.isCharging = 1
@@ -875,15 +889,14 @@
 
         if carsCharging == 0:
             self.stopTimeout = datetime.max
 
         return carsCharging
 
     def queue_background_task(self, task, delay=0):
-
         if delay > 0:
             bisect.insort(
                 self.backgroundTasksDelayed,
                 (datetime.now() + timedelta(seconds=delay), task),
             )
             return
 
@@ -1112,15 +1125,14 @@
             self.lastSaveFailed = 1
         except TypeError as e:
             logger.info("Exception raised while attempting to save settings file:")
             logger.info(str(e))
             self.lastSaveFailed = 1
 
     def send_master_linkready1(self):
-
         logger.log(logging.INFO8, "Send master linkready1")
 
         # When master is powered on or reset, it sends 5 to 7 copies of this
         # linkready1 message followed by 5 copies of linkready2 (I've never seen
         # more or less than 5 of linkready2).
         #
         # This linkready1 message advertises master's TWCID to other slaves on the
@@ -1169,15 +1181,14 @@
             bytearray(b"\xFC\xE1")
             + self.TWCID
             + self.masterSign
             + bytearray(b"\x00\x00\x00\x00\x00\x00\x00\x00")
         )
 
     def send_master_linkready2(self):
-
         logger.log(logging.INFO8, "Send master linkready2")
 
         # This linkready2 message is also sent 5 times when master is booted/reset
         # and then not sent again if no other TWCs are heard from on the network.
         # If the master has ever seen a slave on the network, linkready2 is sent at
         # long intervals.
         # Slaves always ignore the first linkready2, but respond to the second
@@ -1283,15 +1294,14 @@
 
     def setMasterTWCID(self, twcid):
         # This is called when TWCManager is in Slave mode, to track the
         # master's TWCID
         self.masterTWCID = twcid
 
     def setMaxAmpsToDivideAmongSlaves(self, amps):
-
         # Use backgroundTasksLock to prevent changing maxAmpsToDivideAmongSlaves
         # if the main thread is in the middle of examining and later using
         # that value.
         self.getBackgroundTasksLock()
 
         if amps > self.config["config"]["wiringMaxAmpsAllTWCs"]:
             # Never tell the slaves to draw more amps than the physical charger
@@ -1507,10 +1517,10 @@
             ) + realPowerFactorMinAmps
 
     def rotl(self, num, bits):
         bit = num & (1 << (bits - 1))
         num <<= 1
         if bit:
             num |= 1
-        num &= 2 ** bits - 1
+        num &= 2**bits - 1
 
         return num
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/TWCSlave.py` & `TWCManager-1.3.0/lib/TWCManager/TWCSlave.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import time
 
 
 logger = logging.getLogger("\u26FD Slave")
 
 
 class TWCSlave:
-
     config = None
     configConfig = None
     TWCID = None
     __lastAPIAmpsValue = 0
     __lastAPIAmpsRequest = time.time() + 30
     __lastAPIAmpsRepeat = 0
     lastVINQuery = 0
@@ -73,23 +72,23 @@
 
     def __init__(self, TWCID, maxAmps, config, master):
         self.config = config
         self.configConfig = self.config.get("config", {})
         self.master = master
         self.TWCID = TWCID
         self.maxAmps = maxAmps
+        self.APIcontrol = False
 
         self.wiringMaxAmps = self.configConfig.get("wiringMaxAmpsPerTWC", 6)
         self.useFlexAmpsToStartCharge = self.configConfig.get(
             "useFlexAmpsToStartCharge", False
         )
         self.startStopDelay = self.configConfig.get("startStopDelay", 60)
 
     def print_status(self, heartbeatData):
-
         try:
             debugOutput = "SHB %02X%02X: %02X %05.2f/%05.2fA %02X%02X" % (
                 self.TWCID[0],
                 self.TWCID[1],
                 heartbeatData[0],
                 (((heartbeatData[3] << 8) + heartbeatData[4]) / 100),
                 (((heartbeatData[1] << 8) + heartbeatData[2]) / 100),
@@ -534,21 +533,21 @@
                     # car_api_charge() will prevent telling the car to start or stop
                     # more than once per minute. Once the car gets the message to
                     # stop, reportedAmpsActualSignificantChangeMonitor should drop
                     # to near zero within a few seconds.
                     self.master.stopCarsCharging()
             elif (
                 self.lastAmpsOffered >= self.config["config"]["minAmpsPerTWC"]
-                and self.reportedAmpsActual < 2.0
+                and self.reportedAmpsActual < 1.0
                 and self.reportedState != 0x02
             ):
                 # Car is not charging and is not reporting an error state, so
                 # try starting charge via car api.
                 self.master.startCarsCharging()
-            elif self.reportedAmpsActual > 4.0:
+            elif self.reportedAmpsActual >= 1.0:
                 # At least one plugged in car is successfully charging. We don't
                 # know which car it is, so we must set
                 # vehicle.stopAskingToStartCharging = False on all vehicles such
                 # that if any vehicle is not charging without us calling
                 # car_api_charge(False), we'll try to start it charging again at
                 # least once. This probably isn't necessary but might prevent
                 # some unexpected case from never starting a charge. It also
@@ -657,14 +656,20 @@
         self.master.getModuleByName("Policy").setChargingPerPolicy()
 
         # Determine how many cars are charging and how many amps they're using
         numCarsCharging = self.master.num_cars_charging_now()
         desiredAmpsOffered = self.master.getMaxAmpsToDivideAmongSlaves()
         flex = self.master.getAllowedFlex()
 
+        # Get charge rate control mode from settings
+        # 1 = Use TWC Exclusively to control Charge Rate
+        # 2 = Use Tesla API Exclusively to control Charge Rate
+        # 3 = Use TWC >= 6A + Tesla API < 6A to control Charge Rate
+        chargeRateControl = int(self.master.settings.get("chargeRateControl", 1))
+
         if numCarsCharging > 0:
             desiredAmpsOffered -= sum(
                 slaveTWC.reportedAmpsActual
                 for slaveTWC in self.master.getSlaveTWCs()
                 if slaveTWC.TWCID != self.TWCID
             )
             flex = self.master.getAllowedFlex() / numCarsCharging
@@ -797,17 +802,20 @@
                     desiredAmpsOffered = 0
 
             else:
                 # no cars are charging, and desiredAmpsOffered < minAmpsToOffer
                 # so we need to set desiredAmpsOffered to 0
                 logger.debug("no cars charging, setting desiredAmpsOffered to 0")
                 desiredAmpsOffered = 0
-        elif int(self.master.settings.get("chargeRateControl", 1)) == 2:
-            # Exclusive control is given to the Tesla API to control Charge Rate
+        elif chargeRateControl == 2 or (
+            chargeRateControl == 3 and desiredAmpsOffered < 6
+        ):
+            # Control is given to the Tesla API to control Charge Rate
             # We offer the maximum wiring amps from the TWC, and ask the API to control charge rate
+            self.APIcontrol = True
 
             # Call the Tesla API to set the charge rate for vehicle connected to this TWC
             # TODO: Identify vehicle
             if (
                 int(desiredAmpsOffered) == self.__lastAPIAmpsValue
                 and (
                     self.__lastAPIAmpsRepeat > 50 or self.__lastAPIAmpsRepeat % 10 != 0
@@ -828,17 +836,25 @@
                     None if self.getLastVehicle() is None else self.getLastVehicle()
                 )
 
                 self.master.getModuleByName("TeslaAPI").setChargeRate(
                     int(desiredAmpsOffered), targetVehicle
                 )
 
-            desiredAmpsOffered = int(self.configConfig.get("wiringMaxAmpsPerTWC", 6))
+            desiredAmpsOffered = self.wiringMaxAmps
 
         else:
+            # If we just switched from API to TWC make sure the car is set to a
+            # high enough charge rate so it is not limiting the TWC control
+            if chargeRateControl == 3 and self.APIcontrol:
+                self.master.getModuleByName("TeslaAPI").setChargeRate(
+                    self.wiringMaxAmps, self.getLastVehicle()
+                )
+                self.APIcontrol = False
+
             # We can tell the TWC how much power to use in 0.01A increments, but
             # the car will only alter its power in larger increments (somewhere
             # between 0.5 and 0.6A). The car seems to prefer being sent whole
             # amps and when asked to adjust between certain values like 12.6A
             # one second and 12.0A the next second, the car reduces its power
             # use to ~5.14-5.23A and refuses to go higher. So it seems best to
             # stick with whole amps.
@@ -967,16 +983,20 @@
                 logger.debug(
                     "Reduce amps: time - self.timeLastAmpsOfferedChanged "
                     + str(int(now - self.timeLastAmpsOfferedChanged))
                 )
                 if now - self.timeLastAmpsOfferedChanged < 5:
                     desiredAmpsOffered = self.lastAmpsOffered
 
-        if (self.lastAmpsDesired <= 0 and desiredAmpsOffered > 0) or (
-            self.lastAmpsDesired > 0 and desiredAmpsOffered == 0
+        if (
+            self.lastAmpsDesired < minAmpsToOffer
+            and desiredAmpsOffered >= minAmpsToOffer
+        ) or (
+            self.lastAmpsDesired >= minAmpsToOffer
+            and desiredAmpsOffered < minAmpsToOffer
         ):
             self.lastAmpsDesired = desiredAmpsOffered
             self.timeLastAmpsDesiredFlipped = now
             logger.debug("lastAmpsDesired flipped - now " + str(desiredAmpsOffered))
 
         # Keep charger on if dampening changes. See reasoning above where
         # I don't turn the charger off till it's been on for a bit.
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/Vehicle/TeslaAPI.py` & `TWCManager-1.3.0/lib/TWCManager/Vehicle/TeslaAPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import time
 from urllib.parse import parse_qs
 
 logger = logging.getLogger("\U0001F697 TeslaAPI")
 
 
 class TeslaAPI:
-
     __apiChallenge = None
     __apiVerifier = None
     __apiState = None
     __authURL = "https://auth.tesla.com/oauth2/v3/token"
     __callbackURL = "https://auth.tesla.com/void/callback"
     carApiLastErrorTime = 0
     carApiBearerToken = ""
@@ -72,15 +71,14 @@
         self.generateChallenge()
 
     def addVehicle(self, json):
         self.carApiVehicles.append(CarApiVehicle(json, self, self.config))
         return True
 
     def apiDebugInterface(self, command, vehicleID, parameters):
-
         # Provides an interface from the Web UI to allow commands to be run interactively
 
         # Map vehicle ID back to vehicle object
         vehicle = self.getVehicleByID(int(vehicleID))
 
         # Get parameters
         params = {}
@@ -510,15 +508,14 @@
         return (
             self.__apiChallenge.decode("UTF-8"),
             self.__apiState,
             self.__apiVerifier,
         )
 
     def is_location_home(self, lat, lon):
-
         if self.master.getHomeLatLon()[0] == 10000:
             logger.info(
                 "Home location for vehicles has never been set.  "
                 + "We'll assume home is where we found the first vehicle currently parked.  "
                 + "Home set to lat="
                 + str(lat)
                 + ", lon="
@@ -540,17 +537,23 @@
         # I originally tried using 0.00548 (~2000 feet) but one night the car
         # consistently reported being 2839 feet away from home despite being
         # parked in the exact spot I always park it.  This is very odd because
         # GPS is supposed to be accurate to within 12 feet.  Tesla phone app
         # also reports the car is not at its usual address.  I suspect this
         # is another case of a bug that's been causing car GPS to freeze  the
         # last couple months.
+        # Desired maximum destination from home is now configurable. As the
+        # parameter may not be set, we catch the key error and use the default
+        # value documented above.
+        atHomeRadius = (
+            1 / 364488.888 * float(self.config["config"].get("atHomeRadius", 10560))
+        )
         if (
-            abs(self.master.getHomeLatLon()[0] - lat) > 0.0289
-            or abs(self.master.getHomeLatLon()[1] - lon) > 0.0289
+            abs(self.master.getHomeLatLon()[0] - lat) > atHomeRadius
+            or abs(self.master.getHomeLatLon()[1] - lon) > atHomeRadius
         ):
             return False
 
         return True
 
     def car_api_charge(self, charge):
         # Do not call this function directly.  Call by using background thread:
@@ -561,15 +564,14 @@
         if not charge:
             # Whenever we are going to tell vehicles to stop charging, set
             # vehicle.stopAskingToStartCharging = False on all vehicles.
             for vehicle in self.getCarApiVehicles():
                 vehicle.stopAskingToStartCharging = False
 
         if now - self.getLastStartOrStopChargeTime() < 60:
-
             # Don't start or stop more often than once a minute
             logger.log(
                 logging.DEBUG2,
                 "car_api_charge return because not long enough since last carApiLastStartOrStopChargeTime",
             )
             return "error"
 
@@ -607,41 +609,36 @@
                 continue
 
             # Only update carApiLastStartOrStopChargeTime if car_api_available() managed
             # to wake cars.  Setting this prevents any command below from being sent
             # more than once per minute.
             self.updateLastStartOrStopChargeTime()
 
-            if (
-                self.config["config"]["onlyChargeMultiCarsAtHome"]
-                and self.getVehicleCount() > 1
-            ):
-                # When multiple cars are enrolled in the car API, only start/stop
-                # charging cars parked at home.
+            # only start/stop charging cars parked at home.
 
-                if vehicle.update_location() is False:
-                    result = "error"
-                    continue
+            if vehicle.update_location() is False:
+                result = "error"
+                continue
 
-                if not vehicle.atHome:
-                    # Vehicle is not at home, so don't change its charge state.
-                    logger.info(
-                        vehicle.name
-                        + " is not at home.  Do not "
-                        + startOrStop
-                        + " charge."
-                    )
-                    continue
+            if not vehicle.atHome:
+                # Vehicle is not at home, so don't change its charge state.
+                logger.info(
+                    vehicle.name
+                    + " is not at home.  Do not "
+                    + startOrStop
+                    + " charge."
+                )
+                continue
 
-                # If you send charge_start/stop less than 1 second after calling
-                # update_location(), the charge command usually returns:
-                #   {'response': {'result': False, 'reason': 'could_not_wake_buses'}}
-                # Waiting 2 seconds seems to consistently avoid the error, but let's
-                # wait 5 seconds in case of hardware differences between cars.
-                time.sleep(5)
+            # If you send charge_start/stop less than 1 second after calling
+            # update_location(), the charge command usually returns:
+            #   {'response': {'result': False, 'reason': 'could_not_wake_buses'}}
+            # Waiting 2 seconds seems to consistently avoid the error, but let's
+            # wait 5 seconds in case of hardware differences between cars.
+            time.sleep(5)
 
             if charge:
                 self.applyChargeLimit(self.lastChargeLimitApplied, checkArrival=True)
 
             url = "https://owner-api.teslamotors.com/api/1/vehicles/"
             url = url + str(vehicle.ID) + "/command/charge_" + startOrStop
             headers = {
@@ -701,29 +698,36 @@
                         # carApiErrorRetryMins mins.
                         self.updateCarApiLastErrorTime(vehicle)
                     else:
                         if apiResponseDict["response"]["result"] == True:
                             self.resetCarApiLastErrorTime(vehicle)
                         elif charge:
                             reason = apiResponseDict["response"]["reason"]
-                            if reason == "complete" or reason == "charging":
+                            if reason in [
+                                "complete",
+                                "charging",
+                                "is_charging",
+                                "disconnected",
+                            ]:
                                 # We asked the car to charge, but it responded that
                                 # it can't, either because it's reached target
                                 # charge state (reason == 'complete'), or it's
-                                # already trying to charge (reason == 'charging').
+                                # already trying to charge (reason == 'charging') or
+                                # it's not connected to a charger (reason == 'charging').
                                 # In these cases, it won't help to keep asking it to
                                 # charge, so set vehicle.stopAskingToStartCharging =
                                 # True.
                                 #
                                 # Remember, this only means at least one car in the
                                 # list wants us to stop asking and we don't know
                                 # which car in the list is connected to our TWC.
                                 logger.info(
                                     vehicle.name
-                                    + " is done charging or already trying to charge.  Stop asking to start charging."
+                                    + " is done charging or already trying to charge or not connected to a charger."
+                                    + "  Stop asking to start charging."
                                 )
                                 vehicle.stopAskingToStartCharging = True
                                 self.resetCarApiLastErrorTime(vehicle)
                             elif reason == "could_not_wake_buses":
                                 # This error often happens if you call
                                 # charge_start too quickly after another command
                                 # like drive_state. Even if you delay 5 seconds
@@ -779,15 +783,14 @@
 
         if self.getLastStartOrStopChargeTime() == now:
             logger.info("Car API " + startOrStop + " charge result: " + result)
 
         return result
 
     def applyChargeLimit(self, limit, checkArrival=False, checkDeparture=False):
-
         if limit != -1 and (limit < 50 or limit > 100):
             logger.log(logging.INFO8, "applyChargeLimit skipped")
             return "error"
 
         if not self.car_api_available():
             logger.log(
                 logging.INFO8,
@@ -861,31 +864,35 @@
         self.carApiLastChargeLimitApplyTime = now
 
         needSleep = False
         for vehicle in self.carApiVehicles:
             if vehicle.stopTryingToApplyLimit or not vehicle.ready():
                 continue
 
-            located = vehicle.update_location()
             (wasAtHome, outside, lastApplied) = self.master.getNormalChargeLimit(
                 vehicle.ID
             )
             forgetVehicle = False
-            if not vehicle.update_charge():
-                # We failed to read the "normal" limit; don't risk changing it.
+            if not vehicle.update_charge() or not vehicle.update_location():
+                # We failed to read the "normal" limit or locate the car; don't
+                # risk changing the charge limit yet.
+                continue
+
+            if not wasAtHome and not vehicle.atHome:
+                # If the vehicle was away and is still away, nothing to do.
                 continue
 
-            if not wasAtHome and located and vehicle.atHome:
+            if not wasAtHome and vehicle.atHome:
                 logger.log(logging.INFO2, vehicle.name + " has arrived")
                 outside = vehicle.chargeLimit
-            elif wasAtHome and located and not vehicle.atHome:
+            elif wasAtHome and not vehicle.atHome:
                 logger.log(logging.INFO2, vehicle.name + " has departed")
                 forgetVehicle = True
 
-            if limit == -1 or (located and not vehicle.atHome):
+            if limit == -1 or not vehicle.atHome:
                 # We're removing any applied limit, provided it hasn't been manually changed
                 #
                 # If lastApplied == -1, the manual-change path is always selected.
                 if wasAtHome and vehicle.chargeLimit == lastApplied:
                     if vehicle.apply_charge_limit(outside):
                         logger.log(
                             logging.INFO2,
@@ -1086,44 +1093,55 @@
         self.carApiRefreshToken = token
         return True
 
     def setCarApiTokenExpireTime(self, value):
         self.carApiTokenExpireTime = value
         return True
 
-    def setChargeRate(self, charge_rate, vehicle=None):
-
+    def setChargeRate(self, charge_rate, vehicle=None, set_again=False):
         # As a fallback to allow initial implementation of the charge rate functionality for single car installs,
         # If no vehcle is specified, we take the first returned to us.
 
         if not vehicle:
             vehicle = self.getCarApiVehicles()[0]
 
+        # Do not set charge_rate to 0 as this will effectively stop the car from charging all together
+        if charge_rate < 1:
+            charge_rate = 1
+
         vehicle.lastAPIAccessTime = time.time()
 
         url = "https://owner-api.teslamotors.com/api/1/vehicles/"
         url = url + str(vehicle.ID) + "/command/set_charging_amps"
 
         headers = {
             "accept": "application/json",
             "Authorization": "Bearer " + self.getCarApiBearerToken(),
         }
 
         body = {"charging_amps": charge_rate}
 
         try:
             req = requests.post(url, headers=headers, json=body)
-            logger.log(logging.INFO8, "Car API cmd set_charging_amps" + str(req))
+            logger.log(
+                logging.INFO8,
+                f"Car API cmd set_charging_amps {charge_rate}A {str(req)}",
+            )
             apiResponseDict = json.loads(req.text)
         except requests.exceptions.RequestException:
             return False
         except json.decoder.JSONDecodeError:
             return False
 
-        return apiResponseDict
+        # Set charge rates < 5 twice, see https://github.com/tdorssers/TeslaPy/pull/42
+        if charge_rate < 5 and not set_again:
+            time.sleep(5)
+            return self.setChargeRate(charge_rate, vehicle, set_again=True)
+        else:
+            return apiResponseDict
 
     def updateCarApiLastErrorTime(self, vehicle=None):
         timestamp = time.time()
         logger.log(
             logging.INFO8,
             "updateCarApiLastErrorTime() called due to Tesla API Error. Updating timestamp from "
             + str(self.carApiLastErrorTime)
@@ -1182,15 +1200,14 @@
         return min(
             [car.batteryLevel for car in self.carApiVehicles if car.atHome],
             default=10000,
         )
 
 
 class CarApiVehicle:
-
     carapi = None
     __config = None
     debuglevel = 0
     ID = None
     name = ""
     syncSource = "TeslaAPI"
     VIN = ""
@@ -1198,16 +1215,15 @@
     firstWakeAttemptTime = 0
     lastAPIAccessTime = 0
     delayNextWakeAttempt = 0
     lastLimitAttemptTime = 0
 
     errorCount = 0
     lastErrorTime = 0
-    lastDriveStatusTime = 0
-    lastChargeStatusTime = 0
+    lastVehicleStatusTime = 0
     stopAskingToStartCharging = False
     stopTryingToApplyLimit = False
 
     batteryLevel = 10000
     chargeLimit = -1
     lat = 10000
     lon = 10000
@@ -1364,74 +1380,59 @@
 
             return (True, response)
         else:
             self.carapi.updateCarApiLastErrorTime(self)
             return (False, None)
 
     def update_location(self, cacheTime=60):
-
         if self.syncSource == "TeslaAPI":
-            url = "https://owner-api.teslamotors.com/api/1/vehicles/"
-            url = url + str(self.ID) + "/data_request/drive_state"
-
-            now = time.time()
-
-            if now - self.lastDriveStatusTime < cacheTime:
-                return True
-
-            try:
-                (result, response) = self.get_car_api(url)
-            except TypeError:
-                logger.log(logging.error, "Got None response from get_car_api()")
-                return False
-
-            if result:
-                self.lastDriveStatusTime = now
-                self.lat = response["latitude"]
-                self.lon = response["longitude"]
-                self.atHome = self.carapi.is_location_home(self.lat, self.lon)
-
-            return result
+            return self.update_vehicle_data(cacheTime)
 
         else:
-
             self.lat = self.syncLat
             self.lon = self.syncLon
             self.atHome = self.carapi.is_location_home(self.lat, self.lon)
 
             return True
 
-    def update_charge(self):
+    def update_vehicle_data(self, cacheTime=60):
+        url = "https://owner-api.teslamotors.com/api/1/vehicles/"
+        url = url + str(self.ID) + "/vehicle_data"
 
-        if self.syncSource == "TeslaAPI":
+        now = time.time()
 
-            url = "https://owner-api.teslamotors.com/api/1/vehicles/"
-            url = url + str(self.ID) + "/data_request/charge_state"
+        if now - self.lastVehicleStatusTime < cacheTime:
+            return True
 
-            now = time.time()
+        try:
+            (result, response) = self.get_car_api(url)
+        except TypeError:
+            logger.log(logging.error, "Got None response from get_car_api()")
+            return False
 
-            if now - self.lastChargeStatusTime < 60:
-                return True
+        if result:
+            drive = response["drive_state"]
+            self.lat = drive["latitude"]
+            self.lon = drive["longitude"]
+            self.atHome = self.carapi.is_location_home(self.lat, self.lon)
 
-            try:
-                (result, response) = self.get_car_api(url)
-            except TypeError:
-                logger.log(logging.error, "Got None response from get_car_api()")
-                return False
+            charge = response["charge_state"]
+            self.chargeLimit = charge["charge_limit_soc"]
+            self.batteryLevel = charge["battery_level"]
+            self.timeToFullCharge = charge["time_to_full_charge"]
 
-            if result:
-                self.lastChargeStatusTime = time.time()
-                self.chargeLimit = response["charge_limit_soc"]
-                self.batteryLevel = response["battery_level"]
-                self.timeToFullCharge = response["time_to_full_charge"]
+            self.lastVehicleStatusTime = now
 
-            return result
+        return result
 
-        else:
+    def update_charge(self):
+        if self.syncSource == "TeslaAPI":
+            return self.update_vehicle_data()
 
+        else:
             return True
 
     def apply_charge_limit(self, limit):
         if self.stopTryingToApplyLimit:
             return True
 
         now = time.time()
```

### Comparing `TWCManager-1.2.6/lib/TWCManager/Vehicle/TeslaMateVehicle.py` & `TWCManager-1.3.0/lib/TWCManager/Vehicle/TeslaMateVehicle.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import threading
 import time
 
 logger = logging.getLogger("\U0001F697 TeslaMate")
 
 
 class TeslaMateVehicle:
-
     __db_host = None
     __db_name = None
     __db_pass = None
     __db_user = None
     __client = None
     __config = None
     __configConfig = None
@@ -106,15 +105,14 @@
 
         self.__client.loop_start()
 
     def doSyncTokens(self, firstrun=False):
         # Connect to TeslaMate database and synchronize API tokens
 
         if self.__db_host and self.__db_name and self.__db_user and self.__db_pass:
-
             conn = None
 
             try:
                 conn = psycopg2.connect(
                     host=self.__db_host,
                     database=self.__db_name,
                     user=self.__db_user,
@@ -147,28 +145,26 @@
                 # We don't want to refresh the token - let the source handle that.
                 carapi.setCarApiTokenExpireTime(99999 * 99999 * 99999)
                 carapi.setCarApiBearerToken(result[0])
                 carapi.setCarApiRefreshToken(result[1])
                 self.lastSync = time.time()
 
             else:
-
                 logger.log(
                     logging.ERROR,
                     "Failed to connect to TeslaMate database. Disabling Token Sync",
                 )
 
                 # Connection failed. Turn off token sync
                 if firstrun:
                     # If this is the first time we try to fetch, disable token sync.
                     # On subsequent fetches, we don't want to disable token sync as it could be a transient connectivity issue
                     self.syncTokens = False
 
         else:
-
             logger.log(
                 logging.ERROR,
                 "TeslaMate Database connection settings not specified. Disabling Token Sync",
             )
 
             # Required database details not provided. Turn off token sync
             self.syncTokens = False
@@ -176,20 +172,18 @@
     def mqttConnect(self, client, userdata, flags, rc):
         logger.log(logging.INFO5, "MQTT Connected.")
         logger.log(logging.INFO5, "Subscribe to " + self.__mqtt_prefix + "/cars/#")
         res = client.subscribe(self.__mqtt_prefix + "/cars/#", qos=0)
         logger.log(logging.INFO5, "Res: " + str(res))
 
     def mqttMessage(self, client, userdata, message):
-
         topic = str(message.topic).split("/")
         payload = str(message.payload.decode("utf-8"))
 
         if topic[0] == self.__mqtt_prefix and topic[1] == "cars":
-
             if topic[3] == "battery_level":
                 if self.vehicles.get(topic[2], None):
                     self.vehicles[topic[2]].batteryLevel = int(payload)
                     self.vehicles[topic[2]].lastChargeStatusTime = time.time()
                     self.vehicles[topic[2]].syncTimestamp = time.time()
 
             elif topic[3] == "charge_limit_soc":
@@ -200,27 +194,24 @@
 
             elif topic[3] == "display_name":
                 # We can map the car ID in TeslaMate to the vehicle
                 # in the Tesla API module
                 self.updateVehicles(topic[2], payload)
 
             elif topic[3] == "latitude":
-
                 if self.vehicles.get(topic[2], None):
                     self.vehicles[topic[2]].syncLat = float(payload)
                     self.vehicles[topic[2]].syncTimestamp = time.time()
 
             elif topic[3] == "longitude":
-
                 if self.vehicles.get(topic[2], None):
                     self.vehicles[topic[2]].syncLon = float(payload)
                     self.vehicles[topic[2]].syncTimestamp = time.time()
 
             elif topic[3] == "state":
-
                 if self.vehicles.get(topic[2], None):
                     self.vehicles[topic[2]].syncState = payload
                     self.vehicles[topic[2]].syncTimestamp = time.time()
 
             elif topic[3] == "time_to_full_charge":
                 if self.vehicles.get(topic[2], None):
                     self.vehicles[topic[2]].timeToFullCharge = int(float(payload))
```

### Comparing `TWCManager-1.2.6/lib/TWCManager.egg-info/SOURCES.txt` & `TWCManager-1.3.0/lib/TWCManager.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.py
 lib/TWCManager/TWCManager.py
 lib/TWCManager/TWCMaster.py
 lib/TWCManager/TWCSlave.py
 lib/TWCManager.egg-info/PKG-INFO
@@ -37,22 +38,24 @@
 lib/TWCManager/Control/themes/Default/vehicles.html.j2
 lib/TWCManager/Control/themes/Modern/bootstrap.js.html.j2
 lib/TWCManager/Control/themes/Modern/jsrefresh.html.j2
 lib/TWCManager/Control/themes/Modern/main.html.j2
 lib/TWCManager/Control/themes/Modern/master.html.j2
 lib/TWCManager/Control/themes/Modern/css/styles.css
 lib/TWCManager/EMS/DSMR.py
+lib/TWCManager/EMS/DSMRreader.py
 lib/TWCManager/EMS/Efergy.py
 lib/TWCManager/EMS/EmonCMS.py
 lib/TWCManager/EMS/Enphase.py
 lib/TWCManager/EMS/Fronius.py
 lib/TWCManager/EMS/Growatt.py
 lib/TWCManager/EMS/HASS.py
 lib/TWCManager/EMS/IotaWatt.py
 lib/TWCManager/EMS/Kostal.py
+lib/TWCManager/EMS/MQTT.py
 lib/TWCManager/EMS/OpenHab.py
 lib/TWCManager/EMS/OpenWeatherMap.py
 lib/TWCManager/EMS/P1Monitor.py
 lib/TWCManager/EMS/SmartMe.py
 lib/TWCManager/EMS/SmartPi.py
 lib/TWCManager/EMS/SolarEdge.py
 lib/TWCManager/EMS/SolarLog.py
```

### Comparing `TWCManager-1.2.6/setup.py` & `TWCManager-1.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 #!/usr/bin/python3
 
 from setuptools import setup, find_namespace_packages
 
 setup(
     name="TWCManager",
-    version="1.2.6",
+    version="1.3.0",
     package_dir={"": "lib"},
     packages=find_namespace_packages(where="lib"),
     python_requires=">= 3.6",
     include_package_data=True,
+    long_description="Controls the charge rate of certain versions of Tesla Wall Connector (TWC) via the built-in Load Sharing protocol.",
     # Dependencies
     install_requires=[
         "cryptography<3.4",
         "growattServer>=1.0.0",
         "jinja2>=2.11.2",
         "ocpp",
         "paho_mqtt>=1.5.0",
         "psycopg2",
         "pyModbusTCP>=0.1.8",
         "pymysql",
         "pyserial>=3.4",
         "pyyaml",
         "requests>=2.23.0",
         "sentry_sdk>=0.11.2",
+        "solaredge_modbus>=0.7.0",
         "sysv_ipc",
         "termcolor>=1.1.0",
         "websockets<=9.1; python_version == '3.6'",
         "websockets>=9.1; python_version >= '3.7'",
     ],
     # Package Metadata
     author="Nathan Gardiner",
```

