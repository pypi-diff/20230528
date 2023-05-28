# Comparing `tmp/pyalarmdotcomajax-0.5.0b5.tar.gz` & `tmp/pyalarmdotcomajax-0.5.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalarmdotcomajax-0.5.0b5.tar", last modified: Mon May 22 20:21:26 2023, max compression
+gzip compressed data, was "pyalarmdotcomajax-0.5.0b6.tar", last modified: Sun May 28 04:00:39 2023, max compression
```

## Comparing `pyalarmdotcomajax-0.5.0b5.tar` & `pyalarmdotcomajax-0.5.0b6.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:21:26.834513 pyalarmdotcomajax-0.5.0b5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17973 2023-05-22 20:21:26.834513 pyalarmdotcomajax-0.5.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:21:26.826513 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/
--rw-r--r--   0 runner    (1001) docker     (123)    47148 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20770 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:21:26.830513 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/
--rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/garage_door.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/image_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)    14474 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/water_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:21:26.830513 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:21:26.834513 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/garage_door.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/water_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:21:26.826513 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17973 2023-05-22 20:21:26.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-22 20:21:26.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 20:21:26.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-22 20:21:26.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-22 20:21:26.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-22 20:21:26.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 20:21:26.000000 pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-22 20:21:26.834513 pyalarmdotcomajax-0.5.0b5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:21:26.834513 pyalarmdotcomajax-0.5.0b5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:21:26.834513 pyalarmdotcomajax-0.5.0b5/tests/responses/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/tests/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/tests/test_device_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/tests/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/tests/test_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-22 20:21:06.000000 pyalarmdotcomajax-0.5.0b5/tests/test_thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:00:39.127723 pyalarmdotcomajax-0.5.0b6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18040 2023-05-28 04:00:39.131723 pyalarmdotcomajax-0.5.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:00:39.123723 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/
+-rw-r--r--   0 runner    (1001) docker     (123)    46317 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20995 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:00:39.127723 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/garage_door.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/image_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14829 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/water_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22829 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:00:39.127723 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:00:39.127723 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/garage_door.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/water_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:00:39.127723 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18040 2023-05-28 04:00:39.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-28 04:00:39.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 04:00:39.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-28 04:00:39.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-28 04:00:39.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-28 04:00:39.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 04:00:38.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-28 04:00:39.131723 pyalarmdotcomajax-0.5.0b6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:00:39.127723 pyalarmdotcomajax-0.5.0b6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:00:39.127723 pyalarmdotcomajax-0.5.0b6/tests/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/tests/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-28 04:00:28.000000 pyalarmdotcomajax-0.5.0b6/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-05-28 04:00:28.000000 pyalarmdotcomajax-0.5.0b6/tests/test_device_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-28 04:00:28.000000 pyalarmdotcomajax-0.5.0b6/tests/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-28 04:00:28.000000 pyalarmdotcomajax-0.5.0b6/tests/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-28 04:00:28.000000 pyalarmdotcomajax-0.5.0b6/tests/test_thermostat.py
```

### Comparing `pyalarmdotcomajax-0.5.0b5/LICENSE` & `pyalarmdotcomajax-0.5.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b5/PKG-INFO` & `pyalarmdotcomajax-0.5.0b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalarmdotcomajax
-Version: 0.5.0b5
+Version: 0.5.0b6
 Summary: Python Interface for Alarm.com
 Home-page: https://github.com/pyalarmdotcom/pyalarmdotcomajax
 Author: Justin Wong
 Author-email: 46082645+uvjustin@users.noreply.github.com
 Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com, 466460+elahd@users.noreply.github.com
 License: MIT
@@ -34,16 +34,16 @@
 </p>
 <p align="center">
   <!-- <a href="https://www.codacy.com/gh/pyalarmdotcom/pyalarmdotcomajax/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=pyalarmdotcom/pyalarmdotcomajax&amp;utm_campaign=Badge_Grade"><img src="https://app.codacy.com/project/badge/Grade/c58b00c68f9542aea1554d160997e5cd"/></a> -->
   <!-- <a href="https://www.codacy.com/gh/pyalarmdotcom/pyalarmdotcomajax/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=pyalarmdotcom/pyalarmdotcomajax&amp;utm_campaign=Badge_Coverage"><img src="https://app.codacy.com/project/badge/Coverage/c58b00c68f9542aea1554d160997e5cd"/></a> -->
   <a href="https://results.pre-commit.ci/latest/github/pyalarmdotcom/pyalarmdotcomajax/master"><img src="https://results.pre-commit.ci/badge/github/pyalarmdotcom/pyalarmdotcomajax/master.svg" /></a>
   <a href="https://pypi.org/project/pyalarmdotcomajax/"><img alt="PyPI" src="https://img.shields.io/pypi/v/pyalarmdotcomajax"></a>
   <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" /></a>
-  <a href="https://github.com/PyCQA/pylint"><img src="https://img.shields.io/badge/linting-pylint-yellowgreen" /></a>
-  <a href="https://github.com/pyalarmdotcom/pyalarmdotcomajax/blob/master/LICENSE"><img alt="GitHub" src="https://img.shields.io/github/license/pyalarmdotcom/pyalarmdotcomajax"></a>
+  <a href="https://github.com/charliermarsh/ruff"><img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json" /></a>
+  <a href="https://github.com/pyalarmdotcom/pyalarmdotcomajax/blob/master/LICENSE"><img alt="GitHub" src="https://img.shields.io/github/license/pyalarmdotcom/pyalarmdotcomajax" /></a>
 </p>
 
 ## Installation / Usage
 
 To install use pip:
 
 ```bash
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.0b5 Summary: Python
+Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.0b6 Summary: Python
 Interface for Alarm.com Home-page: https://github.com/pyalarmdotcom/
 pyalarmdotcomajax Author: Justin Wong Author-email:
 46082645+uvjustin@users.noreply.github.com Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com,
 466460+elahd@users.noreply.github.com License: MIT Keywords: Alarm.com,Security
 System,Home Assistant Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English Classifier: Environment :: Web
@@ -19,15 +19,16 @@
      This is an unofficial project that is not affiliated with Alarm.com.
                     Forked from Daren Lord's pyalarmdotcom.
 
   [https://img.shields.io/badge/Creator-Justin%20Wong%20(%40uvjustin)-blue]
  [https://img.shields.io/badge/Maintainer-Elahd%20Bar--Shai%20(%40elahd)-blue]
   [https://results.pre-commit.ci/badge/github/pyalarmdotcom/pyalarmdotcomajax/
 master.svg] [PyPI] [https://img.shields.io/badge/code%20style-black-000000.svg]
-      [https://img.shields.io/badge/linting-pylint-yellowgreen] [GitHub]
+    [https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/
+            charliermarsh/ruff/main/assets/badge/v2.json] [GitHub]
 ## Installation / Usage To install use pip: ```bash pip install
 pyalarmdotcomajax ``` Or clone the repo: ```bash git clone https://github.com/
 uvjustin/pyalarmdotcomajax.git python setup.py install ``` ## Usage See
 `examples/basic_sensor_data.py` for a basic usage example. ## Device Support
 (Core Functions) Pyalarmdotcomajax supports core features (monitoring and using
 actions) of the device types listed below. - As of v0.2, multiples of all
 devices are supported. - All devices include the attributes: `name`, `id_`,
```

### Comparing `pyalarmdotcomajax-0.5.0b5/README.md` & `pyalarmdotcomajax-0.5.0b6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 </p>
 <p align="center">
   <!-- <a href="https://www.codacy.com/gh/pyalarmdotcom/pyalarmdotcomajax/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=pyalarmdotcom/pyalarmdotcomajax&amp;utm_campaign=Badge_Grade"><img src="https://app.codacy.com/project/badge/Grade/c58b00c68f9542aea1554d160997e5cd"/></a> -->
   <!-- <a href="https://www.codacy.com/gh/pyalarmdotcom/pyalarmdotcomajax/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=pyalarmdotcom/pyalarmdotcomajax&amp;utm_campaign=Badge_Coverage"><img src="https://app.codacy.com/project/badge/Coverage/c58b00c68f9542aea1554d160997e5cd"/></a> -->
   <a href="https://results.pre-commit.ci/latest/github/pyalarmdotcom/pyalarmdotcomajax/master"><img src="https://results.pre-commit.ci/badge/github/pyalarmdotcom/pyalarmdotcomajax/master.svg" /></a>
   <a href="https://pypi.org/project/pyalarmdotcomajax/"><img alt="PyPI" src="https://img.shields.io/pypi/v/pyalarmdotcomajax"></a>
   <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" /></a>
-  <a href="https://github.com/PyCQA/pylint"><img src="https://img.shields.io/badge/linting-pylint-yellowgreen" /></a>
-  <a href="https://github.com/pyalarmdotcom/pyalarmdotcomajax/blob/master/LICENSE"><img alt="GitHub" src="https://img.shields.io/github/license/pyalarmdotcom/pyalarmdotcomajax"></a>
+  <a href="https://github.com/charliermarsh/ruff"><img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json" /></a>
+  <a href="https://github.com/pyalarmdotcom/pyalarmdotcomajax/blob/master/LICENSE"><img alt="GitHub" src="https://img.shields.io/github/license/pyalarmdotcom/pyalarmdotcomajax" /></a>
 </p>
 
 ## Installation / Usage
 
 To install use pip:
 
 ```bash
```

#### html2text {}

```diff
@@ -5,15 +5,16 @@
      This is an unofficial project that is not affiliated with Alarm.com.
                     Forked from Daren Lord's pyalarmdotcom.
 
   [https://img.shields.io/badge/Creator-Justin%20Wong%20(%40uvjustin)-blue]
  [https://img.shields.io/badge/Maintainer-Elahd%20Bar--Shai%20(%40elahd)-blue]
   [https://results.pre-commit.ci/badge/github/pyalarmdotcom/pyalarmdotcomajax/
 master.svg] [PyPI] [https://img.shields.io/badge/code%20style-black-000000.svg]
-      [https://img.shields.io/badge/linting-pylint-yellowgreen] [GitHub]
+    [https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/
+            charliermarsh/ruff/main/assets/badge/v2.json] [GitHub]
 ## Installation / Usage To install use pip: ```bash pip install
 pyalarmdotcomajax ``` Or clone the repo: ```bash git clone https://github.com/
 uvjustin/pyalarmdotcomajax.git python setup.py install ``` ## Usage See
 `examples/basic_sensor_data.py` for a basic usage example. ## Device Support
 (Core Functions) Pyalarmdotcomajax supports core features (monitoring and using
 actions) of the device types listed below. - As of v0.2, multiples of all
 devices are supported. - All devices include the attributes: `name`, `id_`,
```

### Comparing `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/__init__.py` & `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,81 +1,66 @@
 """Alarmdotcom API Controller."""
 from __future__ import annotations
 
 import asyncio
-import contextlib
 import json
 import logging
 import re
 from collections.abc import Callable, Coroutine
 from contextlib import suppress
 from datetime import datetime, timedelta
-from enum import Enum
 from typing import Any, TypedDict
 
 import aiohttp
 from bs4 import BeautifulSoup
 
 from pyalarmdotcomajax import const as c
+from pyalarmdotcomajax.const import OtpType
 from pyalarmdotcomajax.devices import (
     BaseDevice,
     DeviceTypeSpecificData,
     TroubleCondition,
 )
 from pyalarmdotcomajax.devices.partition import Partition
 from pyalarmdotcomajax.devices.registry import (
     AllDevices_t,
     AttributeRegistry,
     DeviceRegistry,
     DeviceType,
 )
-from pyalarmdotcomajax.errors import (
+from pyalarmdotcomajax.exceptions import (
     AuthenticationFailed,
-    DataFetchFailed,
+    ConfigureTwoFactorAuthentication,
+    NotAuthorized,
+    OtpRequired,
     SessionTimeout,
     TryAgain,
-    TwoFactor_ConfigurationRequired,
-    UnexpectedDataStructure,
-    UnsupportedDevice,
+    UnexpectedResponse,
+    UnsupportedDeviceType,
 )
 from pyalarmdotcomajax.extensions import (
     CameraSkybellControllerExtension,
     ConfigurationOption,
     ControllerExtensions_t,
     ExtendedProperties,
 )
 from pyalarmdotcomajax.websockets.client import WebSocketClient, WebSocketState
 
-# TODO: Use error handler and exception handlers in _async_get_system_devices on other request functions.
-# TODO: Fix get raw server response function.
-
-__version__ = "0.5.0-beta.5"
+__version__ = "0.5.0-beta.6"
 
 log = logging.getLogger(__name__)
 
 
 class ExtensionResults(TypedDict):
     """Results of multi-device extension calls."""
 
     settings: dict[str, ConfigurationOption]
     controller: ControllerExtensions_t
 
 
-class OtpType(Enum):
-    """Alarm.com two factor authentication type."""
-
-    # https://www.alarm.com/web/system/assets/customer-ember/enums/TwoFactorAuthenticationType.js
-    # Keep these lowercase. Strings.json in Home Assistant requires lowercase values.
-
-    disabled = 0
-    app = 1
-    sms = 2
-    email = 4
-
-
 class AlarmController:
     """Base class for communicating with Alarm.com via API."""
 
     AJAX_HEADERS_TEMPLATE = {
         "Accept": "application/vnd.api+json",
         "ajaxrequestuniquekey": None,
     }
@@ -217,27 +202,37 @@
     #
     ####################
     # PUBLIC FUNCTIONS #
     ####################
     #
     #
 
-    async def async_update(self) -> None:  # noqa: C901
-        """Fetch latest device data."""
+    async def async_update(self) -> None:
+        """Pull latest device data from Alarm.com.
+
+        Raises:
+            OtpRequired: Username and password are correct. User now needs to begin two-factor authentication workflow.
+            ConfigureTwoFactorAuthentication: Alarm.com requires that the user set up two-factor authentication for their account.
+            UnexpectedResponse: Server returned status code >=400 or response object was not as expected.
+            aiohttp.ClientError: Connection error.
+            asyncio.TimeoutError: Connection error due to timeout.
+            NotAuthorized: User doesn't have permission to perform the action requested.
+            AuthenticationFailed: User could not be logged in, likely due to invalid credentials.
+            UnsupportedDeviceType: Device type is not supported by this library.
+        """
 
         log.debug("Calling update on Alarm.com")
 
         has_image_sensors: bool = False
 
         if not self._active_system_id:
             self._active_system_id = await self._async_get_active_system()
             has_image_sensors = await self._async_has_image_sensors(self._active_system_id)
 
-        with contextlib.suppress(DataFetchFailed, UnexpectedDataStructure):
-            await self._async_get_trouble_conditions()
+        await self._async_get_trouble_conditions()
 
         #
         # GET CORE DEVICE ATTRIBUTES
         #
 
         device_instances: dict[str, AllDevices_t] = {}
         raw_devices: list[dict] = await self._async_get_system(self._active_system_id)
@@ -268,129 +263,123 @@
 
         #
         # BUILD PARTITIONS
         #
 
         # Ensure that partition map is built before devices are built.
 
-        for device in [
-            device
-            for device in raw_devices
-            if device["type"] == AttributeRegistry.get_relationship_id_from_devicetype(DeviceType.PARTITION)
+        for partition_raw in [
+            partition_raw
+            for partition_raw in raw_devices
+            if partition_raw["type"] == AttributeRegistry.get_relationship_id_from_devicetype(DeviceType.PARTITION)
         ]:
             partition_instance: AllDevices_t = await self._async_update__build_device(
-                device, device_type_specific_data, extension_results
+                partition_raw, device_type_specific_data, extension_results
             )
 
             for child, _ in partition_instance.children:
                 self._partition_map[child] = partition_instance.id_
 
             device_instances.update({partition_instance.id_: partition_instance})
 
-            raw_devices.remove(device)
+            raw_devices.remove(partition_raw)
 
             #
             # BUILD ALL DEVICES IN PARTITION
             #
             # This ensures that partition map is built before devices are built.
 
-            for device in raw_devices:
+            for device_raw in raw_devices:
                 try:
                     device_instance: AllDevices_t = await self._async_update__build_device(
-                        device, device_type_specific_data, extension_results
+                        device_raw, device_type_specific_data, extension_results
                     )
 
                     device_instances.update({device_instance.id_: device_instance})
 
-                except UnsupportedDevice:
+                except UnsupportedDeviceType:
                     continue
 
         self.devices.update(device_instances, purge=True)
 
     async def async_send_command(
         self,
         device_type: DeviceType,
         event: BaseDevice.Command,
-        device_id: str | None = None,  # ID corresponds to device_type
+        device_id: str,  # ID corresponds to device_type
         msg_body: dict = {},  # Body of request. No abstractions here.
         retry_on_failure: bool = True,  # Set to prevent infinite loops when function calls itself
     ) -> bool:
         """Send commands to Alarm.com."""
         log.info("Sending %s to Alarm.com.", event)
 
         msg_body["statePollOnly"] = False
 
         try:
             url = (
                 f"{AttributeRegistry.get_endpoints(device_type)['primary'].format(c.URL_BASE, device_id)}/{event.value}"
             )
         except KeyError as err:
-            raise UnsupportedDevice from err
+            raise UnsupportedDeviceType(device_type, device_id) from err
 
         log.debug("Url %s", url)
 
-        async with self._websession.post(url=url, json=msg_body, headers=self._ajax_headers) as resp:
-            log.debug("Response from Alarm.com %s", resp.status)
+        try:
+            async with self._websession.post(url=url, json=msg_body, headers=self._ajax_headers) as resp:
+                log.debug("Response from Alarm.com %s", resp.status)
 
-            match str(resp.status):
-                case "200":
-                    # Update entities after calling state change.
-                    # TODO: Confirm that we can remove this call because of webhook support.
-                    # await self.async_update()
-                    return True
+                json_rsp = await resp.json()
 
-                case "423":
-                    # User has read-only permission to the entity.
-                    err_msg = (
-                        f"{__name__}: User {self.user_email} has read-only access to"
-                        f" {device_type.name.lower()} {device_id}."
+                # Special handling of 422 status.
+                # 422 sometimes occurs when forceBypass is True but there's nothing to bypass.
+                if (
+                    str(resp.status) == "422"
+                    and isinstance(event, Partition.Command)
+                    and (msg_body.get("forceBypass") is True)
+                ):
+                    log.debug(
+                        "Error executing %s, trying again without force bypass...",
+                        event.value,
                     )
-                    raise PermissionError(err_msg)
 
-                case "422":
-                    if isinstance(event, Partition.Command) and (msg_body.get("forceBypass") is True):
-                        # 422 sometimes occurs when forceBypass is True but there's nothing to bypass.
-                        log.debug(
-                            "Error executing %s, trying again without force bypass...",
-                            event.value,
-                        )
-
-                        # Not changing retry_on_failure. Changing forcebypass means that we won't re-enter this block.
-
-                        msg_body["forceBypass"] = False
-
-                        return await self.async_send_command(
-                            device_type=device_type,
-                            event=event,
-                            device_id=device_id,
-                            msg_body=msg_body,
-                        )
-
-                case "403":
-                    # Session may have expired. Log back in and try again.
-                    log.warning(
-                        "Error executing %s. Session. probably expired. Logging in and trying again...",
-                        event.value,
+                    # Not changing retry_on_failure. Changing forcebypass means that we won't re-enter this block.
+
+                    msg_body["forceBypass"] = False
+
+                    return await self.async_send_command(
+                        device_type=device_type,
+                        event=event,
+                        device_id=device_id,
+                        msg_body=msg_body,
                     )
 
-                    if retry_on_failure:
-                        await self.async_login()
-                        return await self.async_send_command(
-                            device_type,
-                            event,
-                            device_id,
-                            msg_body,
-                            False,
-                        )
-
-        log.error(
-            f"{event.value} failed with HTTP code {resp.status}. URL: {url}\nJSON: {msg_body}\nHeaders:"
-            f" {self._ajax_headers}"
-        )
-        raise ConnectionError
+                # Run standard server response checks.
+                await self._async_handle_server_errors(json_rsp, "send_command", retry_on_failure)
+
+                # If above pass and we have a 200, we're good.
+                if str(resp.status) == "200":
+                    return True
+
+        except aiohttp.ClientResponseError as err:
+            log.exception("Failed to send command.")
+            raise UnexpectedResponse from err
+        except TryAgain:
+            return await self.async_send_command(
+                device_type=device_type,
+                event=event,
+                device_id=device_id,
+                msg_body=msg_body,
+                retry_on_failure=False,
+            )
+        else:
+            log.exception(
+                f"{event.value} failed with HTTP code {resp.status}. URL: {url}\nJSON: {msg_body}\nHeaders:"
+                f" {self._ajax_headers}"
+            )
+            raise UnexpectedResponse
 
     async def start_session_nudger(self) -> None:
         """Start task to nudge user sessions to keep from timing out."""
 
         self._session_timer = SessionTimer(self.keep_alive, self.KEEP_ALIVE_SIGNAL_INTERVAL_S)
         await self._session_timer.start()
 
@@ -422,178 +411,294 @@
 
     #
     # AUTHENTICATION FUNCTIONS
     #
 
     async def async_login(
         self,
-    ) -> list[OtpType] | None:
-        """Login to Alarm.com."""
+    ) -> None:
+        """Log in to Alarm.com.
+
+        Raises:
+            OtpRequired: Username and password are correct. User now needs to begin two-factor authentication workflow.
+            ConfigureTwoFactorAuthentication: Alarm.com requires that the user set up two-factor authentication for their account.
+            UnexpectedResponse: Server returned status code >=400 or response object was not as expected.
+            aiohttp.ClientError: Connection error.
+            asyncio.TimeoutError: Connection error due to timeout.
+            NotAuthorized: User doesn't have permission to perform the action requested.
+            AuthenticationFailed: User could not be logged in, likely due to invalid credentials.
+        """
         log.debug("Attempting to log in to Alarm.com")
 
+        #
+        # Step 1: Get login page and cookies
+        #
+
         try:
-            await self._async_login_and_get_key()
-            await self._async_get_identity_info()
+            # load login page once and grab VIEWSTATE/cookies
+            async with self._websession.get(url=self.LOGIN_URL, cookies=self._two_factor_cookie) as resp:
+                text = await resp.text()
+                log.debug("Response status from Alarm.com: %s", resp.status)
+                tree = BeautifulSoup(text, "html.parser")
+                login_info = {
+                    self.VIEWSTATE_FIELD: tree.select(f"#{self.VIEWSTATE_FIELD}")[0].attrs.get("value"),
+                    self.VIEWSTATEGENERATOR_FIELD: tree.select(f"#{self.VIEWSTATEGENERATOR_FIELD}")[0].attrs.get(
+                        "value"
+                    ),
+                    self.EVENTVALIDATION_FIELD: tree.select(f"#{self.EVENTVALIDATION_FIELD}")[0].attrs.get(
+                        "value"
+                    ),
+                    self.PREVIOUSPAGE_FIELD: tree.select(f"#{self.PREVIOUSPAGE_FIELD}")[0].attrs.get("value"),
+                }
 
-            log.info("Logged in successfully.")
+        except aiohttp.ClientResponseError as err:
+            log.exception("Failed to load login page.")
+            raise UnexpectedResponse from err
+        except (AttributeError, IndexError) as err:
+            log.exception("Unable to extract login info from Alarm.com")
+            raise UnexpectedResponse from err
 
-            return await self._get_2fa_requirements()
+        #
+        # Step 2: Log in and save anti-forgery key
+        #
 
-        except (DataFetchFailed, UnexpectedDataStructure) as err:
-            raise ConnectionError from err
-        except (AuthenticationFailed, PermissionError) as err:
-            raise AuthenticationFailed from err
+        try:
+            # login and grab ajax key
+            async with self._websession.post(
+                url=self.LOGIN_POST_URL,
+                data={
+                    self.LOGIN_USERNAME_FIELD: self._username,
+                    self.LOGIN_PASSWORD_FIELD: self._password,
+                    self.VIEWSTATE_FIELD: login_info[self.VIEWSTATE_FIELD],
+                    self.VIEWSTATEGENERATOR_FIELD: login_info[self.VIEWSTATEGENERATOR_FIELD],
+                    self.EVENTVALIDATION_FIELD: login_info[self.EVENTVALIDATION_FIELD],
+                    self.PREVIOUSPAGE_FIELD: login_info[self.PREVIOUSPAGE_FIELD],
+                    self.LOGIN_REMEMBERME_FIELD: "on",
+                    "IsFromNewSite": "1",
+                },
+                cookies=self._two_factor_cookie,
+                raise_for_status=True,
+            ) as resp:
+                if re.search("m=login_fail", str(resp.url)) is not None:
+                    log.exception("Login failed.")
+                    log.exception("\nResponse URL:\n%s\n", str(resp.url))
+                    log.exception("\nRequest Headers:\n%s\n", str(resp.request_info.headers))
+                    raise AuthenticationFailed("Invalid username and password.")
 
-    async def _get_2fa_requirements(self) -> list[OtpType] | None:
-        """Get list of two factor authentication methods enabled on account."""
+                # Update anti-forgery cookie
+                self._ajax_headers["ajaxrequestuniquekey"] = resp.cookies["afg"].value
+
+        except (aiohttp.ClientResponseError, KeyError) as err:
+            log.exception("Failed to get AJAX key from Alarm.com.")
+            raise UnexpectedResponse from err
+
+        self._last_session_refresh = datetime.now()
+
+        log.debug("Logged in to Alarm.com.")
+
+        #
+        # Step 3: Get user's profile.
+        #
 
         async with self._websession.get(
-            url=self.LOGIN_2FA_DETAIL_URL_TEMPLATE.format(c.URL_BASE, self._user_id),
+            url=c.IDENTITIES_URL_TEMPLATE.format(c.URL_BASE, ""),
             headers=self._ajax_headers,
+            cookies=self._two_factor_cookie,
         ) as resp:
             json_rsp = await resp.json()
 
-            if not (data := json_rsp.get("data", {})):
-                raise UnexpectedDataStructure("Could not find expected data in two-factor authentication details.")
+            try:
+                self._user_id = json_rsp["data"][0]["id"]
+                self._provider_name = json_rsp["data"][0]["attributes"]["logoName"]
+                self._provider_name = json_rsp["data"][0]["attributes"]["logoName"]
 
-            if data.get("showSuggestedSetup") is True:
-                raise TwoFactor_ConfigurationRequired(
-                    "Got 2FA nag screen. 2FA must be configured on this account before proceeding."
+                for inclusion in json_rsp["included"]:
+                    if inclusion["id"] == self._user_id and inclusion["type"] == "profile/profile":
+                        self._user_email = inclusion["attributes"]["loginEmailAddress"]
+
+                if not self._user_email:
+                    raise UnexpectedResponse("Failed to get user's email address.")
+            except KeyError as err:
+                log.exception(f"{__name__} _async_get_identity_info: Failed to get user's identity info.")
+                log.debug(
+                    f"{__name__} _async_get_identity_info: Server Response:\n{json.dumps(json_rsp, indent=4)}"
                 )
+                raise AuthenticationFailed from err
+
+            try:
+                self._session_refresh_interval_ms = json_rsp["data"][0]["attributes"][
+                    "applicationSessionProperties"
+                ]["inactivityWarningTimeoutMs"]
+
+                if not self._session_refresh_interval_ms:
+                    raise KeyError
+
+            except KeyError:
+                self._session_refresh_interval_ms = self.SESSION_REFRESH_DEFAULT_INTERVAL_MS
+
+            try:
+                self._keep_alive_url = json_rsp["data"][0]["attributes"]["applicationSessionProperties"][
+                    "keepAliveUrl"
+                ]
+
+                if not self._keep_alive_url:
+                    raise KeyError
+
+            except KeyError:
+                self._keep_alive_url = self.KEEP_ALIVE_DEFAULT_URL
+
+            log.debug("*** START IDENTITY INFO ***")
+            log.debug(f"Provider: {self._provider_name}")
+            log.debug(f"User: {self._user_id} {self._user_email}")
+            log.debug(f"Keep Alive Interval: {self._session_refresh_interval_ms}")
+            log.debug(f"Keep Alive URL: {self._keep_alive_url}")
+            log.debug("*** END IDENTITY INFO ***")
+
+        #
+        # Step 4: Determine whether OTP is required
+        #
+
+        try:
+            async with self._websession.get(
+                url=self.LOGIN_2FA_DETAIL_URL_TEMPLATE.format(c.URL_BASE, self._user_id),
+                headers=self._ajax_headers,
+            ) as resp:
+                json_rsp = await resp.json()
+
+            await self._async_handle_server_errors(json_rsp, "2FA requirements", False)
+
+        except aiohttp.ClientResponseError as err:
+            log.exception("Failed to get 2FA requirements.")
+            raise UnexpectedResponse from err
+
+        if not (attribs := json_rsp.get("data", {}).get("attributes")):
+            raise UnexpectedResponse("Could not find expected data in two-factor authentication details.")
+
+        if attribs.get("showSuggestedSetup") is True:
+            raise ConfigureTwoFactorAuthentication
 
-            enabled_otp_types_bitmask = json_rsp.get("data", {}).get("attributes", {}).get("enabledTwoFactorTypes")
-            enabled_2fa_methods = [
-                otp_type for otp_type in OtpType if bool(enabled_otp_types_bitmask & otp_type.value)
-            ]
-
-            if OtpType.disabled in enabled_2fa_methods or data.get("isCurrentDeviceTrusted") is True:
-                # 2FA is disabled, we can skip 2FA altogether.
-                return None
+        enabled_otp_types_bitmask = attribs.get("enabledTwoFactorTypes")
+        enabled_2fa_methods = [
+            otp_type for otp_type in OtpType if bool(enabled_otp_types_bitmask & otp_type.value)
+        ]
 
-            log.info(f"Requires two-factor authentication. Enabled methods are {enabled_2fa_methods}")
-            return enabled_2fa_methods
+        if (OtpType.disabled in enabled_2fa_methods) or (attribs.get("isCurrentDeviceTrusted") is True):
+            # 2FA is disabled, we can skip 2FA altogether.
+            return
+
+        log.info(f"Requires two-factor authentication. Enabled methods are {enabled_2fa_methods}")
+
+        raise OtpRequired(enabled_2fa_methods)
 
     async def async_request_otp(self, method: OtpType | None) -> None:
         """Request SMS/email OTP code from Alarm.com."""
 
+        log.debug("Requesting OTP code...")
+
         if method not in (OtpType.email, OtpType.sms):
-            return None
+            return
 
+        request_url = (
+            self.LOGIN_2FA_REQUEST_OTP_EMAIL_URL_TEMPLATE
+            if method == OtpType.email
+            else self.LOGIN_2FA_REQUEST_OTP_SMS_URL_TEMPLATE
+        )
         try:
-            log.debug("Requesting OTP code...")
-
-            request_url = (
-                self.LOGIN_2FA_REQUEST_OTP_EMAIL_URL_TEMPLATE
-                if method == OtpType.email
-                else self.LOGIN_2FA_REQUEST_OTP_SMS_URL_TEMPLATE
-            )
-
             async with self._websession.post(
                 url=request_url.format(c.URL_BASE, self._user_id),
                 headers=self._ajax_headers,
-            ) as resp:
-                if resp.status != 200:
-                    raise DataFetchFailed("Failed to request 2FA code.")
-
-        except (asyncio.TimeoutError, aiohttp.ClientError) as err:
-            log.error("Can not load 2FA submission page from Alarm.com")
-            raise DataFetchFailed from err
-
-        return None
+                raise_for_status=True,
+            ):
+                pass
+
+        except aiohttp.ClientResponseError as err:
+            log.exception("Failed to get available systems.")
+            raise UnexpectedResponse from err
 
     async def async_submit_otp(
         self, code: str, method: OtpType, device_name: str | None = None, remember_me: bool = False
-    ) -> str | None:
+    ) -> None:
         """Submit two factor authentication code.
 
         Register device and return 2FA code if device_name is not None.
         """
 
         # Submit code
         try:
             log.debug("Submitting OTP code...")
 
-            if not method:
-                raise AuthenticationFailed("Missing OTP type.")
-
             async with self._websession.post(
                 url=self.LOGIN_2FA_POST_URL_TEMPLATE.format(c.URL_BASE, self._user_id),
                 headers=self._ajax_headers,
                 json={"code": code, "typeOf2FA": method.value},
+                raise_for_status=True,
             ) as resp:
                 json_rsp = await resp.json()
 
-        except (asyncio.TimeoutError, aiohttp.ClientError) as err:
-            log.error("Can not load 2FA submission page from Alarm.com")
-            raise DataFetchFailed from err
-
-        if resp.status == 422:
-            raise AuthenticationFailed("Wrong code.")
-        if resp.status > 400:
-            log.error(
-                "Failed 2FA submission with status %s: %s",
-                resp.status,
-                await resp.text(),
-            )
-            raise DataFetchFailed("Unknown error.")
+        except aiohttp.ClientResponseError as err:
+            if err.status == 422:
+                raise AuthenticationFailed("Wrong code.") from err
+            raise UnexpectedResponse from err
 
         log.debug("Submitted OTP code.")
 
         if not device_name and not remember_me:
             log.debug('Skipping "Remember Me".')
-            return None
+            return
 
         # Submit device name for "remember me" function.
         if suggested_device_name := json_rsp.get("value", {}).get("deviceName"):
             try:
                 log.debug("Registering device...")
 
                 async with self._websession.post(
                     url=self.LOGIN_2FA_TRUST_URL_TEMPLATE.format(c.URL_BASE, self._user_id),
                     headers=self._ajax_headers,
                     json={"deviceName": device_name if device_name else suggested_device_name},
+                    raise_for_status=True,
                 ) as resp:
                     json_rsp = await resp.json()
-            except (asyncio.TimeoutError, aiohttp.ClientError) as err:
-                log.error("Can not load device trust page from Alarm.com")
-                raise DataFetchFailed from err
+            except aiohttp.ClientResponseError as err:
+                log.exception("Failed to send command.")
+                raise UnexpectedResponse from err
 
             log.debug("Registered device.")
 
         # Save 2FA cookie value.
         for cookie in self._websession.cookie_jar:
             if cookie.key == self.LOGIN_TWO_FACTOR_COOKIE_NAME:
                 log.debug("Found two-factor authentication cookie: %s", cookie.value)
                 self._two_factor_cookie = {"twoFactorAuthenticationId": cookie.value} if cookie.value else {}
-                return str(cookie.value)
+                return
 
-        log.error("Failed to find two-factor authentication cookie.")
-        return None
+        raise UnexpectedResponse("Failed to find two-factor authentication cookie.")
 
     async def is_logged_in(self, throw: bool = False) -> bool:
         """Check if we are still logged in."""
 
         url = f"{c.URL_BASE[:-1]}{self._keep_alive_url}{self.KEEP_ALIVE_URL_PARAM_TEMPLATE.format(int(round(datetime.now().timestamp())))}"
 
-        async with self._websession.get(
-            url=url,
-            headers=self._ajax_headers,
-        ) as resp:
-            text_rsp = await resp.text()
+        try:
+            async with self._websession.get(
+                url=url,
+                headers=self._ajax_headers,
+                raise_for_status=True,
+            ) as resp:
+                text_rsp = await resp.text()
 
-        if resp.status == 403:
-            log.debug("Session expired.")
+        except aiohttp.ClientResponseError as err:
+            if err.status == 403:
+                log.debug("Session expired.")
 
-            if throw:
-                raise SessionTimeout
+                if throw:
+                    raise SessionTimeout
 
-            return False
+                return False
 
-        elif resp.status >= 400:
-            raise DataFetchFailed(f"Failed to send keep alive signal. Response: {text_rsp}")
+            raise UnexpectedResponse(f"Failed to send keep alive signal. Response: {text_rsp}") from err
 
         return True
 
     async def keep_alive(self) -> None:
         """Keep session alive. Handle if not (optionally).
 
         Should be called once per minute to keep session alive.
@@ -637,20 +742,18 @@
             url=self.KEEP_ALIVE_RENEW_SESSION_URL_TEMPLATE.format(c.URL_BASE, self._user_id),
             headers=self._ajax_headers,
             data=json.dumps({"included": [], "meta": {"transformer_version": "1.1"}}),
         ) as resp:
             json_rsp = await resp.json()
 
             if resp.status >= 400:
-                raise DataFetchFailed(f"Failed to reload session context. Response: {json_rsp}")
+                raise UnexpectedResponse(f"Failed to reload session context. Response: {json_rsp}")
 
             self._last_session_refresh = datetime.now()
 
-        return None
-
     async def _async_update__build_device(
         self,
         raw_device: dict,
         device_type_specific_data: dict[str, DeviceTypeSpecificData],
         extension_results: dict[str, ExtensionResults],
     ) -> AllDevices_t:
         """Build device instance."""
@@ -665,15 +768,15 @@
         # SKIP UNSUPPORTED DEVICE TYPES
         #
         # There is a hack here for cameras. We don't really support cameras (no images / streaming), we only support settings for the Skybell HD.
         if not AttributeRegistry.is_supported(device_type) or (
             (device_type == DeviceType.CAMERA)
             and (raw_device.get("attributes", {}).get("deviceModel") != "SKYBELLHD")
         ):
-            raise UnsupportedDevice(f"Unsupported device type: {device_type}")
+            raise UnsupportedDeviceType(device_type, raw_device.get("id"))
 
         children: list[tuple[str, DeviceType]] = []
 
         # Get child elements for partitions and systems if function called using a device_type.
         if device_type in [DeviceType.PARTITION, DeviceType.SYSTEM]:
             for family_name, family_data in raw_device["relationships"].items():
                 if DeviceType.has_value(family_name):
@@ -684,15 +787,15 @@
         # BUILD DEVICE INSTANCE
         #
 
         device_extension_results: ExtensionResults | dict = extension_results.get(
             entity_id := raw_device["id"], {}
         )
 
-        device_instance = device_class(
+        return device_class(
             id_=entity_id,
             raw_device_data=raw_device,
             children=children,
             device_type_specific_data=device_type_specific_data.get(entity_id),
             send_action_callback=self.async_send_command,
             config_change_callback=(
                 extension_controller.submit_change
@@ -700,16 +803,14 @@
                 else None
             ),
             trouble_conditions=self._trouble_conditions.get(entity_id),
             partition_id=self._partition_map.get(entity_id),
             settings=device_extension_results.get("settings"),
         )
 
-        return device_instance
-
     async def _async_update__query_multi_device_extensions(
         self, raw_devices: list[dict]
     ) -> dict[str, ExtensionResults]:
         """Query device extensions that request data for multiple devices at once.
 
         Args:
             raw_devices: A list of devices to query.
@@ -730,19 +831,21 @@
         for raw_device in raw_devices:
             device_type: DeviceType = AttributeRegistry.get_devicetype_from_relationship_id(raw_device["type"])
 
             #
             # Camera Skybell HD Extension
             # Skybell HD extension pulls data for all cameras at once.
             #
-            if device_type == DeviceType.CAMERA:
-                if raw_device.get("attributes", {}).get("deviceModel") == "SKYBELLHD":
-                    required_extensions.append(CameraSkybellControllerExtension)
-                    # Stop searching at the first hit since once we have a Skybell, we know that we need to query the extension.
-                    break
+            if (
+                device_type == DeviceType.CAMERA
+                and raw_device.get("attributes", {}).get("deviceModel") == "SKYBELLHD"
+            ):
+                required_extensions.append(CameraSkybellControllerExtension)
+                # Stop searching at the first hit since once we have a Skybell, we know that we need to query the extension.
+                break
 
         if not required_extensions:
             return {}
 
         #
         # Build map of device names -> device ids.
         #
@@ -762,15 +865,15 @@
                 websession=self._websession,
                 headers=self._ajax_headers,
             )
 
             try:
                 # Fetch from Alarm.com
                 extended_properties_by_device: list[ExtendedProperties] = await extension_controller.fetch()
-            except UnexpectedDataStructure:
+            except UnexpectedResponse:
                 continue
 
             # Match extended properties to devices by name, then add to storage.
 
             for device_properties in extended_properties_by_device:
                 if (device_name := device_properties.device_name) in name_id_map:
                     device_id = name_id_map[device_name]
@@ -795,22 +898,22 @@
 
                 await self._async_handle_server_errors(json_rsp, "active system", retry_on_failure)
 
                 return str(
                     [system["id"] for system in json_rsp.get("data", []) if system["attributes"]["isSelected"]][0]
                 )
 
-        except (asyncio.TimeoutError, aiohttp.ClientError, aiohttp.ClientResponseError, KeyError) as err:
-            log.error("Failed to get available systems.")
-            raise DataFetchFailed from err
-        except TryAgain as err:
+        except (aiohttp.ClientResponseError, KeyError) as err:
+            log.exception("Failed to get active system.")
+            raise UnexpectedResponse from err
+        except TryAgain:
             if retry_on_failure:
                 return await self._async_get_active_system(retry_on_failure=False)
-            else:
-                raise err
+
+            raise
 
     async def _async_get_recent_images(self) -> dict[str, DeviceTypeSpecificData]:
         """Get recent images."""
 
         try:
             log.info("Getting recent images.")
 
@@ -829,19 +932,20 @@
             device_type_specific_data: dict[str, DeviceTypeSpecificData] = {}
 
             for image in json_rsp["data"]:
                 device_type_specific_data.setdefault(
                     str(image["relationships"]["imageSensor"]["data"]["id"]), {}
                 ).setdefault("raw_recent_images", []).append(image)
 
-            return device_type_specific_data
+        except (aiohttp.ClientResponseError, KeyError) as err:
+            log.exception("Failed to get recent images.")
+            raise UnexpectedResponse from err
 
-        except (asyncio.TimeoutError, aiohttp.ClientError, KeyError) as err:
-            log.error("Failed to get available systems.")
-            raise DataFetchFailed from err
+        else:
+            return device_type_specific_data
 
     async def _async_has_image_sensors(self, system_id: str, retry_on_failure: bool = True) -> bool:
         """Check whether image sensors are present in system.
 
         Check is required because image sensors are not shown in the device catalog endpoint.
         """
 
@@ -858,22 +962,22 @@
             ) as resp:
                 json_rsp = await resp.json()
 
                 await self._async_handle_server_errors(json_rsp, "image sensors", retry_on_failure)
 
                 return len(json_rsp["data"].get("relationships", {}).get("imageSensors", {}).get("data", [])) > 0
 
-        except (asyncio.TimeoutError, aiohttp.ClientError, aiohttp.ClientResponseError, KeyError) as err:
-            log.error("Failed to get image sensors.")
-            raise DataFetchFailed from err
-        except TryAgain as err:
+        except (aiohttp.ClientResponseError, KeyError) as err:
+            log.exception("Failed to get image sensors.")
+            raise UnexpectedResponse from err
+        except TryAgain:
             if retry_on_failure:
                 return await self._async_has_image_sensors(system_id, retry_on_failure=False)
-            else:
-                raise err
+
+            raise
 
     async def _async_get_system(self, system_id: str, retry_on_failure: bool = True) -> list[dict]:
         """Get all devices present in system."""
 
         try:
             log.info(f"Getting system data for {system_id}.")
 
@@ -886,17 +990,17 @@
                 # Used by adc CLI.
                 self.raw_system = json_rsp
 
                 await self._async_handle_server_errors(json_rsp, "system", retry_on_failure)
 
                 return [json_rsp["data"]]
 
-        except (asyncio.TimeoutError, aiohttp.ClientError, aiohttp.ClientResponseError, KeyError) as err:
-            log.error("Failed to get system devices.")
-            raise DataFetchFailed from err
+        except (aiohttp.ClientResponseError, KeyError) as err:
+            log.exception("Failed to get system metadata.")
+            raise UnexpectedResponse from err
         except TryAgain:
             return await self._async_get_system(system_id=system_id, retry_on_failure=False)
 
     async def _async_get_system_devices(self, system_id: str, retry_on_failure: bool = True) -> list[dict]:
         """Get all devices present in system."""
 
         try:
@@ -915,17 +1019,17 @@
 
                 return [
                     device
                     for device in json_rsp["included"]
                     if device.get("type") in AttributeRegistry.all_relationship_ids
                 ]
 
-        except (asyncio.TimeoutError, aiohttp.ClientError, aiohttp.ClientResponseError, KeyError) as err:
-            log.error("Failed to get system devices.")
-            raise DataFetchFailed from err
+        except (aiohttp.ClientResponseError, KeyError) as err:
+            log.exception("Failed to get system devices.")
+            raise UnexpectedResponse from err
         except TryAgain:
             return await self._async_get_system_devices(system_id=system_id, retry_on_failure=False)
 
     async def _async_get_devices_by_device_type(
         self, device_type: DeviceType, retry_on_failure: bool = True
     ) -> list[dict]:
         """Get all devices of the specified type."""
@@ -943,74 +1047,20 @@
                 if device_type == DeviceType.IMAGE_SENSOR:
                     self.raw_image_sensors = json_rsp
 
                 await self._async_handle_server_errors(json_rsp, f"get all {device_type.value}", retry_on_failure)
 
                 return list(json_rsp["data"])
 
-        except (asyncio.TimeoutError, aiohttp.ClientError, aiohttp.ClientResponseError, KeyError) as err:
-            log.error(f"Failed to get {device_type.value}.")
-            raise DataFetchFailed from err
+        except (aiohttp.ClientResponseError, KeyError) as err:
+            log.exception(f"Failed to get devices of type {device_type}.")
+            raise UnexpectedResponse from err
         except TryAgain:
             return await self._async_get_devices_by_device_type(device_type=device_type, retry_on_failure=False)
 
-    async def _async_get_identity_info(self) -> None:
-        """Get user id, email address, provider name, etc."""
-
-        async with self._websession.get(
-            url=c.IDENTITIES_URL_TEMPLATE.format(c.URL_BASE, ""),
-            headers=self._ajax_headers,
-            cookies=self._two_factor_cookie,
-        ) as resp:
-            json_rsp = await resp.json()
-
-            try:
-                self._user_id = json_rsp["data"][0]["id"]
-                self._provider_name = json_rsp["data"][0]["attributes"]["logoName"]
-                self._provider_name = json_rsp["data"][0]["attributes"]["logoName"]
-
-                for inclusion in json_rsp["included"]:
-                    if inclusion["id"] == self._user_id and inclusion["type"] == "profile/profile":
-                        self._user_email = inclusion["attributes"]["loginEmailAddress"]
-
-                if not self._user_email:
-                    raise KeyError("Failed to get user's email address.")
-            except KeyError as err:
-                log.error(f"{__name__} _async_get_identity_info: Failed to get user's identity info.")
-                log.debug(
-                    f"{__name__} _async_get_identity_info: Server Response:\n{json.dumps(json_rsp, indent=4)}"
-                )
-                raise AuthenticationFailed from err
-
-            try:
-                self._session_refresh_interval_ms = json_rsp["data"][0]["attributes"][
-                    "applicationSessionProperties"
-                ]["inactivityWarningTimeoutMs"]
-
-                if not self._session_refresh_interval_ms:
-                    raise KeyError
-            except KeyError:
-                self._session_refresh_interval_ms = self.SESSION_REFRESH_DEFAULT_INTERVAL_MS
-
-            try:
-                self._keep_alive_url = json_rsp["data"][0]["attributes"]["applicationSessionProperties"][
-                    "keepAliveUrl"
-                ]
-                if not self._keep_alive_url:
-                    raise KeyError
-            except KeyError:
-                self._keep_alive_url = self.KEEP_ALIVE_DEFAULT_URL
-
-            log.debug("*** START IDENTITY INFO ***")
-            log.debug(f"Provider: {self._provider_name}")
-            log.debug(f"User: {self._user_id} {self._user_email}")
-            log.debug(f"Keep Alive Interval: {self._session_refresh_interval_ms}")
-            log.debug(f"Keep Alive URL: {self._keep_alive_url}")
-            log.debug("*** END IDENTITY INFO ***")
-
     async def _async_get_trouble_conditions(self, retry_on_failure: bool = True) -> None:
         """Get trouble conditions for all devices."""
 
         # TODO: Trouble condition dict should be flagged, not None, when library encounters an error retrieving trouble conditions.
 
         try:
             async with self._websession.get(
@@ -1037,164 +1087,95 @@
                     trouble_single_device.append(new_trouble)
                     trouble_all_devices[device_id] = trouble_single_device
 
                 self._trouble_conditions = trouble_all_devices
 
         except aiohttp.ContentTypeError as err:
             self._trouble_conditions = {}
-            log.error(
+            log.exception(
                 "Server returned wrong content type. Response: %s\n\nResponse Text:\n\n%s\n\n",
                 resp,
                 resp.text(),
             )
-            raise DataFetchFailed from err
+            raise UnexpectedResponse from err
 
-        except (asyncio.TimeoutError, aiohttp.ClientError) as err:
-            self._trouble_conditions = {}
-            log.error("Connection error while fetching trouble conditions.")
-            raise DataFetchFailed from err
+        except aiohttp.ClientResponseError as err:
+            log.exception("Failed to get trouble conditions.")
+            raise UnexpectedResponse from err
 
         except KeyError as err:
             self._trouble_conditions = {}
-            log.error("Failed processing trouble conditions.")
-            raise UnexpectedDataStructure from err
+            log.exception("Failed processing trouble conditions.")
+            raise UnexpectedResponse from err
 
-        except TryAgain as err:
-            if retry_on_failure:
-                return await self._async_get_trouble_conditions(retry_on_failure=False)
-            else:
-                raise err
+        except TryAgain:
+            return await self._async_get_trouble_conditions(retry_on_failure=False)
 
     async def _async_handle_server_errors(
         self, json_rsp: dict, request_name: str, retry_on_failure: bool = False
     ) -> None:
         """Handle errors returned by the server."""
 
         log.debug(
-            f"\n==============================\nServer Response:\n{json_rsp}\n=============================="
+            "\n==============================\nServer"
+            f" Response:\n{json.dumps(json_rsp)}\n=============================="
         )
 
         if not len(rsp_errors := json_rsp.get("errors", [])):
             return
 
         log.debug(
             error_msg := f"{__name__}: Request error. Status: {rsp_errors[0].get('status')}. Response: {json_rsp}"
         )
 
         match rsp_errors[0].get("status"):
             case "423":  # Processing Error
-                log.error(
+                log.exception(
                     f"Got a processing error when trying to request {request_name}. This may be caused by missing"
                     " permissions, being on an Alarm.com plan without support for a particular device type, or"
                     " having a device type disabled for this system."
                 )
                 log.debug(error_msg := f"{request_name} failed.\nResponse:\n{json_rsp}.")
-                raise PermissionError
+                raise NotAuthorized
 
             case "403":  # Invalid Anti-Forgery Token
                 # 403 means that either the user doesn't have access to this class of device or that the user has logged out.
                 # Unsupported device types should be stripped out in async_update(), so assume logged out.
                 # If logged out, try logging in again, then give up by pretending that we couldn't find any devices of this type.
 
                 if not retry_on_failure:
-                    log.error(
+                    log.exception(
                         "Error fetching data from Alarm.com. Got 403 status when"
                         f" fetching {request_name}. Logging in"
                         " again didn't help. Giving up on device type."
                     )
-                    raise DataFetchFailed(error_msg)
+                    raise UnexpectedResponse(error_msg)
 
                 if not self.is_logged_in():
                     log.debug(
                         "Error fetching data from Alarm.com. Got 403 status"
                         f" when requesting {request_name}. Trying to"
                         " refresh auth tokens by logging in again."
                     )
 
                     await self.async_login()
 
                     raise TryAgain
 
             case "409":
-                log.error(
+                log.exception(
                     error_msg := f"Failed to request {request_name}. Two factor authentication cookie is incorrect."
                 )
                 log.debug(error_msg := f"{request_name} failed.\nResponse:\n{json_rsp}.")
                 raise AuthenticationFailed(error_msg)
 
             case _:
-                log.error(f"Unknown error while requesting {request_name}.")
+                log.exception(f"Unknown error while requesting {request_name}.")
                 log.debug(error_msg := f"{request_name} failed.\nResponse:\n{json_rsp}.")
-                raise DataFetchFailed(error_msg)
-
-    async def _async_login_and_get_key(self) -> None:
-        """Load hidden fields from login page."""
-        try:
-            # load login page once and grab VIEWSTATE/cookies
-            async with self._websession.get(url=self.LOGIN_URL, cookies=self._two_factor_cookie) as resp:
-                text = await resp.text()
-                log.debug("Response status from Alarm.com: %s", resp.status)
-                tree = BeautifulSoup(text, "html.parser")
-                login_info = {
-                    self.VIEWSTATE_FIELD: tree.select(f"#{self.VIEWSTATE_FIELD}")[0].attrs.get("value"),
-                    self.VIEWSTATEGENERATOR_FIELD: tree.select(f"#{self.VIEWSTATEGENERATOR_FIELD}")[0].attrs.get(
-                        "value"
-                    ),
-                    self.EVENTVALIDATION_FIELD: tree.select(f"#{self.EVENTVALIDATION_FIELD}")[0].attrs.get(
-                        "value"
-                    ),
-                    self.PREVIOUSPAGE_FIELD: tree.select(f"#{self.PREVIOUSPAGE_FIELD}")[0].attrs.get("value"),
-                }
-
-        except (
-            asyncio.TimeoutError,
-            aiohttp.ClientError,
-            asyncio.exceptions.CancelledError,
-        ) as err:
-            log.error("Can not load login page from Alarm.com")
-
-            raise err
-        except (AttributeError, IndexError) as err:
-            log.error("Unable to extract login info from Alarm.com")
-            raise UnexpectedDataStructure from err
-        try:
-            # login and grab ajax key
-            async with self._websession.post(
-                url=self.LOGIN_POST_URL,
-                data={
-                    self.LOGIN_USERNAME_FIELD: self._username,
-                    self.LOGIN_PASSWORD_FIELD: self._password,
-                    self.VIEWSTATE_FIELD: login_info[self.VIEWSTATE_FIELD],
-                    self.VIEWSTATEGENERATOR_FIELD: login_info[self.VIEWSTATEGENERATOR_FIELD],
-                    self.EVENTVALIDATION_FIELD: login_info[self.EVENTVALIDATION_FIELD],
-                    self.PREVIOUSPAGE_FIELD: login_info[self.PREVIOUSPAGE_FIELD],
-                    self.LOGIN_REMEMBERME_FIELD: "on",
-                    "IsFromNewSite": "1",
-                },
-                cookies=self._two_factor_cookie,
-            ) as resp:
-                if re.search("m=login_fail", str(resp.url)) is not None:
-                    log.error("Login failed.")
-                    log.error("\nResponse URL:\n%s\n", str(resp.url))
-                    log.error("\nRequest Headers:\n%s\n", str(resp.request_info.headers))
-                    raise AuthenticationFailed("Invalid username and password.")
-
-                # Update anti-forgery cookie
-                self._ajax_headers["ajaxrequestuniquekey"] = resp.cookies["afg"].value
-
-        except (asyncio.TimeoutError, aiohttp.ClientError) as err:
-            log.error("Can not login to Alarm.com")
-            raise DataFetchFailed from err
-        except KeyError as err:
-            log.error("Unable to extract ajax key from Alarm.com. Response:\n%s", resp)
-            raise DataFetchFailed from err
-
-        self._last_session_refresh = datetime.now()
-
-        log.debug("Logged in to Alarm.com.")
+                raise UnexpectedResponse(error_msg)
 
 
 class SessionTimer:
     """Run keep_alive function periodically to keep session alive."""
 
     # https://stackoverflow.com/a/37514633
```

### Comparing `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/cli.py` & `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,24 +18,27 @@
 from enum import Enum
 from typing import Any
 
 import aiohttp
 from termcolor import colored, cprint
 
 import pyalarmdotcomajax
+from pyalarmdotcomajax.const import OtpType
 from pyalarmdotcomajax.devices.registry import AllDevices_t, AttributeRegistry
 
-from . import AlarmController, OtpType
+from . import AlarmController
 from .devices import BaseDevice, DeviceType
-from .devices.light import Light
 from .devices.sensor import Sensor
-from .errors import (
+from .exceptions import (
+    AuthenticationFailed,
+    ConfigureTwoFactorAuthentication,
     InvalidConfigurationOption,
-    TwoFactor_ConfigurationRequired,
-    UnexpectedDataStructure,
+    NotAuthorized,
+    OtpRequired,
+    UnexpectedResponse,
 )
 from .extensions import ConfigurationOption
 from .helpers import ExtendedEnumMixin, slug_to_title
 from .websockets.client import WebSocketState
 
 CLI_CARD_BREAK = ""  # "--------"
 
@@ -216,23 +219,33 @@
             username=args.get("username", ""),
             password=args.get("password", ""),
             websession=session,
             twofactorcookie=args.get("cookie"),
         )
 
         try:
-            if enabled_2fa_methods := await alarm.async_login():
-                await async_handle_otp_workflow(alarm, args, enabled_2fa_methods)
-        except TwoFactor_ConfigurationRequired:
+            await alarm.async_login()
+        except ConfigureTwoFactorAuthentication:
             cprint(
                 "Unable to log in. Please set up two-factor authentication for this account.",
                 "red",
             )
             sys.exit()
 
+        except (aiohttp.ClientError, asyncio.TimeoutError, UnexpectedResponse, NotAuthorized):
+            cprint("Could not connect to Alarm.com.", "red")
+            sys.exit()
+
+        except AuthenticationFailed:
+            cprint("Invalid credentials.", "red")
+            sys.exit()
+
+        except OtpRequired as exc:
+            await async_handle_otp_workflow(alarm, args, exc.enabled_2fa_methods)
+
         #######################
         # REFRESH DEVICE DATA #
         #######################
 
         await alarm.async_update()
 
         device_type_output: dict = {}
@@ -355,15 +368,15 @@
             except asyncio.TimeoutError:
                 cprint("Timed out while connecting to Alarm.com.")
             except (
                 aiohttp.ClientError,
                 asyncio.exceptions.CancelledError,
             ):
                 cprint("Failed to connect to Alarm.com.")
-            except UnexpectedDataStructure:
+            except UnexpectedResponse:
                 cprint("Couldn't find settings on device configuration page.")
             except InvalidConfigurationOption:
                 cprint(f"Couldn't load pyalarmdotcomajax configuration extension for {setting_slug}.")
             except TypeError as err:
                 cprint(str(err), "red")
                 sys.exit(0)
 
@@ -456,15 +469,15 @@
 
         output[slug_to_title(device_type.name)] = device_type_output
 
     return output
 
 
 def _print_element_tearsheet(
-    element: BaseDevice,
+    element: AllDevices_t,
 ) -> str:
     output_str: str = ""
 
     # DEVICE NAME
     output_str += colored(f"\n{element.name} ({element.id_})", attrs=["bold", "underline"])
 
     if element.malfunction:
@@ -494,20 +507,16 @@
 
         if battery:
             output_str += f"[BATTERY: {battery}] "
 
         if element.read_only:
             output_str += f"[READ ONLY: {element.read_only}] "
 
-        if isinstance(element, Light):
-            # Disabling. Boring stat.
-            # attribute_str += f"[REPORTS STATE: {element.supports_state_tracking}] "
-
-            if element.brightness:
-                output_str += f"[BRIGHTNESS: {element.brightness}%] "
+        if hasattr(element, "brightness") and element.brightness:
+            output_str += f"[BRIGHTNESS: {element.brightness}%] "
 
         # ENTITIES WITH "ATTRIBUTES" PROPERTY
         if isinstance(element.attributes, BaseDevice.DeviceAttributes):
             for name, value in asdict(element.attributes).items():
                 output_str += f"[{str(name).upper()}: {value}] "
     else:
         output_str += "(none)"
```

### Comparing `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/__init__.py` & `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """Alarm.com device base devices."""
 from __future__ import annotations
 
-import asyncio
 import logging
 from abc import ABC
 from collections.abc import Callable
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any, TypedDict
 
-import aiohttp
-
-from pyalarmdotcomajax.errors import InvalidConfigurationOption, UnexpectedDataStructure
+from pyalarmdotcomajax.exceptions import (
+    InvalidConfigurationOption,
+)
 from pyalarmdotcomajax.extensions import (
     CameraSkybellControllerExtension,
     ConfigurationOption,
 )
 from pyalarmdotcomajax.helpers import CastingMixin, ExtendedEnumMixin
 
 log = logging.getLogger(__name__)
@@ -241,15 +240,15 @@
     # #
     # FUNCTIONS
     # #
 
     async def async_handle_external_state_change(self, raw_state: int) -> None:
         """Update device state when notified of externally-triggered change."""
 
-        self._attribs_raw[self._ATTRIB_STATE] = raw_state
+        self._attribs_raw.update({self._ATTRIB_STATE: raw_state})
 
         log.info(f"{__name__} Got async update for {self.name} ({self.id_}) with new state: {self.state}.")
 
         for external_callback in self.external_update_callback:
             external_callback()
 
     async def async_handle_external_attribute_change(self, new_attribute: dict) -> None:
@@ -301,21 +300,21 @@
     @property
     def attributes(self) -> DeviceAttributes | None:
         """Hold non-primary device state attributes. To be overridden by children."""
 
     def process_device_type_specific_data(self) -> None:
         """Process element specific data. To be overridden by children."""
 
-        return None
+        return
 
     async def async_change_setting(self, slug: str, new_value: Any) -> None:
         """Update specified configuration setting via extension."""
 
         if not self._config_change_callback:
-            log.error(
+            log.exception(
                 "async_change_setting called for %s, which does not have a config_change_callback set.",
                 self.name,
             )
             return
 
         config_option: ConfigurationOption | None = self.settings.get(slug)
         extension: type[CameraSkybellControllerExtension] | None = (
@@ -329,26 +328,15 @@
             "BaseDevice -> async_change_setting: Calling change setting function for %s %s (%s) via extension %s.",
             type(self).__name__,
             self.name,
             self.id_,
             extension,
         )
 
-        try:
-            updated_option = await self._config_change_callback(
-                camera_name=self.name, slug=slug, new_value=new_value
-            )
-        except (
-            asyncio.TimeoutError,
-            aiohttp.ClientError,
-            asyncio.exceptions.CancelledError,
-        ) as err:
-            raise err
-        except UnexpectedDataStructure as err:
-            raise err
+        updated_option = await self._config_change_callback(camera_name=self.name, slug=slug, new_value=new_value)
 
         self._settings["slug"] = updated_option
 
     # #
     # CASTING FUNCTIONS
     # #
```

### Comparing `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/garage_door.py` & `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/garage_door.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/gate.py` & `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/gate.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/image_sensor.py` & `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/image_sensor.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/light.py` & `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/light.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,17 +61,16 @@
             return supports
 
         return None
 
     async def async_turn_on(self, brightness: int | None = None) -> None:
         """Send turn on command with optional brightness."""
 
-        msg_body: dict | None = None
+        msg_body: dict = {}
         if brightness:
-            msg_body = {}
             msg_body["dimmerLevel"] = brightness
 
         await self._send_action_callback(
             device_type=DeviceType.LIGHT,
             event=self.Command.ON,
             device_id=self.id_,
             msg_body=msg_body,
```

### Comparing `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/lock.py` & `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/lock.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/partition.py` & `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/partition.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         no_entry_delay: bool | None = None,
         silent_arming: bool | None = None,
         night_arming: bool | None = None,
     ) -> None:
         """Arm alarm system."""
 
         if arm_type == self.Command.DISARM:
-            log.error("Invalid arm type.")
+            log.exception("Invalid arm type.")
             return
 
         msg_body = {}
 
         if force_bypass and Partition.ExtendedArmingOption.BYPASS_SENSORS in extended_arming_options:
             msg_body.update({"forceBypass": force_bypass})
```

### Comparing `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/registry.py` & `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/registry.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from pyalarmdotcomajax.devices.light import Light
 from pyalarmdotcomajax.devices.lock import Lock
 from pyalarmdotcomajax.devices.partition import Partition
 from pyalarmdotcomajax.devices.sensor import Sensor
 from pyalarmdotcomajax.devices.system import System
 from pyalarmdotcomajax.devices.thermostat import Thermostat
 from pyalarmdotcomajax.devices.water_sensor import WaterSensor
-from pyalarmdotcomajax.errors import UnkonwnDevice, UnsupportedDevice
+from pyalarmdotcomajax.exceptions import UnkonwnDevice, UnsupportedDeviceType
 from pyalarmdotcomajax.helpers import classproperty
 
 log = logging.getLogger(__name__)
 
 AllDeviceTypes_t = (
     type[Camera]
     | type[GarageDoor]
@@ -32,28 +32,44 @@
     | type[Partition]
     | type[Sensor]
     | type[System]
     | type[Thermostat]
     | type[WaterSensor]
 )
 
+AllCommands_t = (
+    Camera.Command
+    | GarageDoor.Command
+    | Gate.Command
+    | ImageSensor.Command
+    | Light.Command
+    | Lock.Command
+    | Partition.Command
+    | Sensor.Command
+    | System.Command
+    | Thermostat.Command
+    | WaterSensor.Command
+)
+
+
 AllDevices_t = (
     Camera
     | GarageDoor
     | Gate
     | ImageSensor
     | Light
     | Lock
     | Partition
     | Sensor
     | System
     | Thermostat
     | WaterSensor
 )
 
+
 AllDevicesLists_t = (
     list[Camera]
     | list[GarageDoor]
     | list[Gate]
     | list[ImageSensor]
     | list[Light]
     | list[Lock]
@@ -112,16 +128,16 @@
         return self._devices
 
     def get(self, device_id: str) -> AllDevices_t:
         """Get device by id."""
 
         try:
             return self._devices[device_id]
-        except KeyError:
-            raise UnkonwnDevice(f"Device with id {device_id} not found.")
+        except KeyError as err:
+            raise UnkonwnDevice(device_id) from err
 
     def update(self, payload: dict[str, AllDevices_t], purge: bool = False) -> None:
         """Store device or list of devices."""
 
         if purge:
             self._devices = payload
         else:
@@ -337,24 +353,24 @@
 
     @staticmethod
     def get_endpoints(device_type: DeviceType) -> DeviceTypeEndpoints:
         """Return primary endpoint for device type."""
         try:
             return AttributeRegistry._ATTRIBUTES.get(device_type, {})["endpoints"]
         except KeyError as err:
-            raise UnsupportedDevice from err
+            raise UnsupportedDeviceType(device_type) from err
 
     @staticmethod
     def get_class(device_type: DeviceType) -> type[AllDevices_t]:
         """Return primary endpoint for device type."""
 
         try:
             return AttributeRegistry._ATTRIBUTES[device_type]["class_"]
         except KeyError as err:
-            raise UnsupportedDevice from err
+            raise UnsupportedDeviceType(device_type) from err
 
     @staticmethod
     def get_storage_name(device_type: DeviceType | type) -> str:
         """Return primary endpoint for device type."""
 
         try:
             if isinstance(device_type, DeviceType):
@@ -363,32 +379,32 @@
             return next(
                 attributes["device_registry_property"]
                 for attributes in AttributeRegistry._ATTRIBUTES.values()
                 if attributes.get("class_") == device_type
             )
 
         except KeyError as err:
-            raise UnsupportedDevice from err
+            raise UnsupportedDeviceType(str(device_type)) from err
 
     @staticmethod
     def get_devicetype_from_relationship_id(relationship_id: str) -> DeviceType:
         """Return device type from relationship id."""
         for device_type, attributes in AttributeRegistry._ATTRIBUTES.items():
             if attributes.get("rel_id") == relationship_id:
                 return device_type
 
-        raise UnsupportedDevice
+        raise UnsupportedDeviceType(relationship_id)
 
     @staticmethod
     def get_relationship_id_from_devicetype(device_type: DeviceType) -> str:
         """Return device type from relationship id."""
         try:
             return AttributeRegistry._ATTRIBUTES[device_type]["rel_id"]
         except KeyError as err:
-            raise UnsupportedDevice from err
+            raise UnsupportedDeviceType(device_type) from err
 
     @classproperty
     def supported_device_types(cls) -> list[DeviceType]:  # pylint: disable=no-self-argument
         """Return list of supported devices."""
         return [device_type for device_type in cls._ATTRIBUTES if cls._ATTRIBUTES[device_type].get("class_")]
 
     @classproperty
```

### Comparing `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/sensor.py` & `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/sensor.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/system.py` & `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/system.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/devices/thermostat.py` & `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/thermostat.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 
 import logging
 from dataclasses import dataclass
 from enum import Enum
 
 from pyalarmdotcomajax.devices import DeviceType
-from pyalarmdotcomajax.errors import UnexpectedDataStructure
+from pyalarmdotcomajax.exceptions import UnexpectedResponse
 
 from . import BaseDevice
 
 log = logging.getLogger(__name__)
 
 
 class Thermostat(BaseDevice):
@@ -185,15 +185,15 @@
 
         msg_body: dict[str, float | int] = {}
 
         # Make sure we're only being asked to set one attribute at a time.
         if (attrib_list := [state, fan, cool_setpoint, heat_setpoint, schedule_mode]).count(None) < len(
             attrib_list
         ) - 1:
-            raise UnexpectedDataStructure
+            raise UnexpectedResponse
 
         # Build the request body.
         if state:
             msg_body = {self._ATTRIB_STATE: state.value}
         elif fan:
             msg_body = {
                 self.ATTRIB_DESIRED_FAN_MODE: self.FanMode(fan[0]).value,
```

### Comparing `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/extensions.py` & `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/extensions.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from enum import Enum, auto
 from typing import Any
 
 import aiohttp
 from bs4 import BeautifulSoup, Tag
 
 from pyalarmdotcomajax import const as c
-from pyalarmdotcomajax.errors import UnexpectedDataStructure
+from pyalarmdotcomajax.exceptions import UnexpectedResponse
 
 from .helpers import ExtendedEnumMixin, extract_field_value
 
 log = logging.getLogger(__name__)
 
 # #################
 # ### UNIVERSAL ###
@@ -289,31 +289,31 @@
                         # Add to camera config retrieval queue
                         additional_camera_config_ids.append(camera_config_id)
 
         except (
             asyncio.TimeoutError,
             aiohttp.ClientError,
             asyncio.exceptions.CancelledError,
-        ) as err:
-            log.error("Can not load settings page from Alarm.com")
-            raise err
+        ):
+            log.exception("Can not load settings page from Alarm.com")
+            raise
         except (AttributeError, IndexError) as err:
-            log.error("Unable to extract page info from Alarm.com.")
+            log.exception("Unable to extract page info from Alarm.com.")
             log.debug("====== HTTP DUMP BEGIN ======\n%s\n====== HTTP DUMP END ======", text)
-            raise UnexpectedDataStructure from err
+            raise UnexpectedResponse from err
 
         #
         # Get data for additional cameras.
         #
         try:
             for config_id in additional_camera_config_ids:
                 # Build payload to request config page for next camera
 
                 if not (postback_form_data := current_form_data.raw_attribs):
-                    raise UnexpectedDataStructure
+                    raise UnexpectedResponse
 
                 postback_form_data["__EVENTTARGET"] = "ctl00$phBody$CamSelector$ddlCams"
                 postback_form_data["ctl00$phBody$CamSelector$ddlCams"] = config_id
 
                 async with self._websession.post(
                     url=self.ENDPOINT,
                     data=postback_form_data,
@@ -325,21 +325,21 @@
 
                     # Pull data for camera on current page
                     camera_return_data.append(current_form_data := self._extract_fields(config_id, tree))
         except (
             asyncio.TimeoutError,
             aiohttp.ClientError,
             asyncio.exceptions.CancelledError,
-        ) as err:
-            log.error("Can not load settings page for additional camera from Alarm.com")
+        ):
+            log.exception("Can not load settings page for additional camera from Alarm.com")
 
-            raise err
-        except UnexpectedDataStructure as err:
+            raise
+        except UnexpectedResponse:
             log.debug("HTTP Response Status %s, Body:\n%s", resp.status, text)
-            raise err
+            raise
 
         return camera_return_data
 
     async def submit_change(
         self,
         camera_name: str,
         slug: str,
@@ -369,15 +369,15 @@
             for config_option_field_name, config_option in self._form_field_settings:
                 if config_option.slug == slug:
                     field_name = config_option_field_name
                     field_value_type = config_option.value_type
                     field_config_options = config_option
 
         except KeyError as err:
-            raise UnexpectedDataStructure("Slug not found.") from err
+            raise UnexpectedResponse("Slug not found.") from err
 
         log.debug("CameraSkybellControllerExtension -> submit_change(): Validating input.")
 
         #
         # VALIDATE INPUT
         #
 
@@ -385,44 +385,43 @@
         # Currently only supports enums. In the future, should be expanded to also support native types.
 
         if field_value_type and not isinstance(new_value, field_value_type):
             raise TypeError(f"New value {new_value} is not of type {field_value_type}")
 
         # Validation for ints
 
-        if field_value_type == int:
-            if (
-                ((value_max := field_config_options.value_max) and new_value > value_max)
-                or ((value_min := field_config_options.value_min) and new_value < value_min)
-                or not (isinstance(new_value, int))
-            ):
-                raise ValueError
+        if field_value_type == int and (
+            ((value_max := field_config_options.value_max) and new_value > value_max)
+            or ((value_min := field_config_options.value_min) and new_value < value_min)
+            or not (isinstance(new_value, int))
+        ):
+            raise ValueError
 
         # Validation for strings
 
-        if field_value_type == str:
-            if (
-                (value_regex := field_config_options.value_regex) and not re.search(value_regex, new_value)
-            ) or not isinstance(new_value, str):
-                raise ValueError
+        if field_value_type == str and (
+            ((value_regex := field_config_options.value_regex) and not re.search(value_regex, new_value))
+            or not isinstance(new_value, str)
+        ):
+            raise ValueError
 
         log.debug("CameraSkybellControllerExtension -> submit_change(): Refreshing settings.")
 
         #
         # Refresh settings data to prime submission payload.
         #
 
         results = await self.fetch(
             camera_names=[camera_name],
         )
 
         if not (payload := results[0].raw_attribs) or not (
             (config_id := results[0].config_id) or not isinstance(payload, dict)
         ):
-            raise UnexpectedDataStructure("Failed to refresh settings data for device.")
+            raise UnexpectedResponse("Failed to refresh settings data for device.")
 
         log.debug("CameraSkybellControllerExtension -> submit_change(): Creating response payload.")
 
         #
         # Process into response payload.
         #
 
@@ -510,18 +509,17 @@
                 # Pull data for camera on current page
                 camera_return_data = self._extract_fields(config_id, tree)
 
         except (
             asyncio.TimeoutError,
             aiohttp.ClientError,
             asyncio.exceptions.CancelledError,
-        ) as err:
-            log.error("Can not load settings page for additional camera from Alarm.com")
-
-            raise err
+        ):
+            log.exception("Can not load settings page for additional camera from Alarm.com")
+            raise
 
         return camera_return_data.settings[slug]
 
     def _build_submit_payload(self, response_data: dict) -> dict:
         """Build POST for new setting submission or for getting other camera data."""
 
         # Pre-populate static fields.
@@ -558,44 +556,44 @@
         try:
             for field_name in self._FORM_FIELDS_BYPASSABLE:
                 if not (field := tree.find(attrs={"name": field_name})):
                     raw_attribs[field_name] = ""
                 else:
                     try:
                         value = extract_field_value(field)
-                    except UnexpectedDataStructure:
+                    except ValueError:
                         log.warning("Couldn't find field %s", field)
                         value = ""
                     raw_attribs[field_name] = value
 
             for field_name in self._FORM_FIELDS_GENERIC:
                 field = tree.find(attrs={"name": field_name})
                 try:
                     value = extract_field_value(field)
-                except UnexpectedDataStructure:
+                except ValueError:
                     log.warning("Couldn't find field %s", field)
                     value = ""
                 raw_attribs[field_name] = value
 
             for field_name, property_name in self._FORM_FIELDS_META:
                 field = tree.find(attrs={"name": field_name})
                 try:
                     value = extract_field_value(field)
-                except UnexpectedDataStructure:
+                except ValueError:
                     log.warning("Couldn't find field %s", field)
                     value = ""
                 raw_attribs[field_name] = value
                 setattr(properties, property_name, value)
 
             for field_name, config_option in self._form_field_settings:
                 field = tree.find(attrs={"name": field_name})
 
                 try:
                     value = extract_field_value(field)
-                except UnexpectedDataStructure:
+                except ValueError:
                     log.warning("Couldn't find field %s", field)
                     value = ""
 
                 typed_value: Any
 
                 #
                 # CONVERSIONS
@@ -618,57 +616,48 @@
 
                 if config_value_type in [
                     self.ChimeAdjustableVolume,
                     self.MotionSensitivity,
                 ]:
                     raw_attribs[field_name] = value
 
-                    if not value:
-                        raise ValueError
-
                     typed_value = config_value_type(int(value))
 
                 #
                 # Conversions for ints.
                 #
 
                 # Preprocessing for colors
 
                 if config_option_type == ConfigurationOptionType.COLOR and (
                     value_regex := config_option.value_regex
                 ):
-                    if not value:
-                        raise ValueError
-
                     match = re.search(value_regex, value)
                     typed_value = str(value)
 
                     if not match:
                         raise ValueError
 
                     raw_attribs[field_name] = match.group()
 
                 # Ints
 
                 if config_value_type == int:
-                    if not value:
-                        raise ValueError
-
                     typed_value = int(value)
                     raw_attribs[field_name] = typed_value
 
                 # Wrap Up
 
                 config_option.current_value = typed_value
 
                 properties.settings[config_option.slug] = config_option
 
-        except (KeyError, ValueError, UnexpectedDataStructure) as err:
-            log.error("Unable to extract field. Failed on field %s.", field_name)
-            raise UnexpectedDataStructure from err
+        except (KeyError, ValueError, UnexpectedResponse) as err:
+            log.exception("Unable to extract field. Failed on field %s.", field_name)
+            raise UnexpectedResponse from err
 
         properties.raw_attribs = raw_attribs
 
         return properties
 
 
 ControllerExtensions_t = CameraSkybellControllerExtension
```

### Comparing `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/helpers.py` & `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 
 import logging
 from enum import Enum
 from typing import Any
 
 from bs4 import Tag
 
-from pyalarmdotcomajax.errors import UnexpectedDataStructure
-
 log = logging.getLogger(__name__)
 
 
 class CastingMixin:
     """Functions used for pulling data from JSON in standardized format."""
 
     def _safe_int_from_dict(self, src_dict: dict, key: str) -> int | None:
@@ -50,17 +48,18 @@
     def _safe_list_from_dict(self, src_dict: dict, key: str, value_type: type) -> list | None:
         """Cast raw value to list. Satisfies mypy."""
 
         try:
             extracted_list: list = list(src_dict.get(key))  # type: ignore
             for duration in extracted_list:
                 value_type(duration)
-            return extracted_list
         except (ValueError, TypeError):
             pass
+        else:
+            return extracted_list
 
         return None
 
     def _safe_special_from_dict(self, src_dict: dict, key: str, value_type: type) -> Any | None:
         """Cast raw value to specified type. Satisfies mypy."""
 
         try:
@@ -111,34 +110,36 @@
     @classmethod
     def names(cls) -> list[str]:
         """Return list of all enum members."""
 
         return cls._member_names_
 
 
-def extract_field_value(field: Tag) -> str | None:
+def extract_field_value(field: Tag) -> str:
     """Extract value from BeautifulSoup4 text, checkbox, and dropdown fields."""
 
     # log.debug("Extracting field: %s", field)
 
-    value: str | None = None
+    value = None
+
     try:
         if field.attrs.get("name") and field.name == "select":
             value = field.findChild(attrs={"selected": "selected"}).attrs["value"]
-        elif field.attrs.get("checked") and (is_checked := field.attrs["checked"]):
-            value = is_checked == "checked"
+        elif field.attrs.get("checked") and field.attrs.get("checked"):
+            value = field.attrs["checked"] == "checked"
         elif field.attrs.get("value"):
             value = field.attrs["value"]
-        else:
-            pass
 
     except (KeyError, AttributeError) as err:
-        raise UnexpectedDataStructure from err
+        raise ValueError from err
+
+    if not value:
+        raise ValueError("Value not found.")
 
-    return value
+    return str(value)
 
 
 def slug_to_title(slug: str) -> str:
     """Convert slug to title case."""
 
     return slug.replace("_", " ").title()
```

### Comparing `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/client.py` & `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Functions for communicating with Alarm.com over WebSockets."""
 
-# noqa: T201
 
 from __future__ import annotations
 
 import asyncio
 import json
 import logging
 from collections.abc import Callable
@@ -18,15 +17,15 @@
 from pyalarmdotcomajax.devices.gate import Gate
 from pyalarmdotcomajax.devices.light import Light
 from pyalarmdotcomajax.devices.partition import Partition
 from pyalarmdotcomajax.devices.registry import DeviceRegistry
 from pyalarmdotcomajax.devices.sensor import Sensor
 from pyalarmdotcomajax.devices.thermostat import Thermostat
 from pyalarmdotcomajax.devices.water_sensor import WaterSensor
-from pyalarmdotcomajax.errors import AuthenticationFailed, DataFetchFailed
+from pyalarmdotcomajax.exceptions import AuthenticationFailed, UnexpectedResponse
 from pyalarmdotcomajax.websockets.handler.garage_door import GarageDoorWebSocketHandler
 from pyalarmdotcomajax.websockets.handler.gate import GateWebSocketHandler
 from pyalarmdotcomajax.websockets.handler.light import LightWebSocketHandler
 from pyalarmdotcomajax.websockets.handler.partition import PartitionWebSocketHandler
 from pyalarmdotcomajax.websockets.handler.sensor import SensorWebSocketHandler
 from pyalarmdotcomajax.websockets.handler.thermostat import ThermostatWebSocketHandler
 from pyalarmdotcomajax.websockets.handler.water_sensor import (
@@ -96,19 +95,20 @@
 
     async def _connect(self) -> None:
         """Connect to Alarm.com WebSocket."""
 
         # Get authentication token for websocket communication
         try:
             self._ws_auth_token = await self._async_get_websocket_token()
-            if not self._ws_auth_token:
-                raise AuthenticationFailed("async_connect(): Failed to get WebSocket authentication token.")
-        except (DataFetchFailed, AuthenticationFailed) as err:
+        except (UnexpectedResponse, AuthenticationFailed) as err:
             raise AuthenticationFailed from err
 
+        if not self._ws_auth_token:
+            raise AuthenticationFailed("async_connect(): Failed to get WebSocket authentication token.")
+
         try:
             # Connect to websocket endpoint
             async with self._websession.ws_connect(
                 self.WEBSOCKET_ENDPOINT_TEMPLATE.format(self._ws_auth_token),
                 headers=self._ajax_headers,
                 timeout=30,
             ) as websocket:
@@ -122,32 +122,32 @@
                     if msg.type != aiohttp.WSMsgType.TEXT:
                         pass
                     elif msg.type == aiohttp.WSMsgType.CLOSED:
                         log.warning("AIOHTTP websocket connection closed")
                         break
 
                     elif msg.type == aiohttp.WSMsgType.ERROR:
-                        log.error("AIOHTTP websocket error: '%s'", msg.data)
+                        log.exception("AIOHTTP websocket error: '%s'", msg.data)
                         break
 
                     try:
                         await self._async_handle_message(json.loads(msg.data))
                     except (TypeError, ValueError):
                         log.warning("Unable to parse message from Alarm.com: %s", msg.data)
                         # TODO: On failure, refresh everything synchronous HTTP endpoints.
                         pass
 
         except aiohttp.ClientConnectorError:
             if self.state != WebSocketState.STOPPED:
-                log.error("WebSocket client connection error")
+                log.exception("WebSocket client connection error")
                 self.state = WebSocketState.DISCONNECTED
 
-        except Exception as err:
+        except Exception:
             if self.state != WebSocketState.STOPPED:
-                log.error("Unexpected WebSocket error %s", err)
+                log.exception("Unexpected WebSocket error")
                 self.state = WebSocketState.DISCONNECTED
 
         else:
             if self.state != WebSocketState.STOPPED:
                 self.state = WebSocketState.DISCONNECTED
 
     def start(self) -> None:
@@ -216,12 +216,12 @@
             log.debug(
                 (
                     "async_get_websocket_token(): Received errors while requesting WebSocket authentication token."
                     " Response: %s"
                 ),
                 resp,
             )
-            raise DataFetchFailed(
+            raise UnexpectedResponse(
                 "async_get_websocket_token(): Received errors while requesting WebSocket authentication token."
             )
 
         return str(token_value)
```

### Comparing `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/const.py` & `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/const.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/__init__.py` & `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/garage_door.py` & `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/garage_door.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/gate.py` & `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/gate.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/light.py` & `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/light.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
                     case PropertyChangeType.LightColor:
                         # RGBW light not currently supported by library.
                         pass
             case StatusChangeMessage():
                 if message.new_state in self.STATE_MAP:
                     await message.device.async_handle_external_state_change(self.STATE_MAP[message.new_state])
                 else:
-                    log.error(
+                    log.exception(
                         f"{self.__class__.__name__}: Failed to update"
                         f" {message.device.name} ({message.device.id_}). Unknown state: {message.new_state}."
                     )
             case EventMessage():
                 match message.event_type:
                     case EventType.SwitchLevelChanged:
                         if message.value:
```

### Comparing `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/lock.py` & `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/lock.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/partition.py` & `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/partition.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/sensor.py` & `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/sensor.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/thermostat.py` & `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/thermostat.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/handler/water_sensor.py` & `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/water_sensor.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax/websockets/messages.py` & `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/messages.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,66 +4,60 @@
 
 import logging
 from datetime import datetime
 
 from dateutil import parser
 
 from pyalarmdotcomajax.devices.registry import AllDevices_t, DeviceRegistry
-from pyalarmdotcomajax.errors import UnkonwnDevice, UnsupportedAction
+from pyalarmdotcomajax.exceptions import UnsupportedWebSocketMessage
 from pyalarmdotcomajax.helpers import CastingMixin
 from pyalarmdotcomajax.websockets.const import (
     SUPPORTED_MONITORING_EVENT_TYPES,
     SUPPORTED_PROPERY_CHANGE_TYPES,
     EventType,
     PropertyChangeType,
 )
 
 log = logging.getLogger(__name__)
 
 
 def process_raw_message(message: dict, device_registry: DeviceRegistry) -> WebSocketMessage:
     """Create websocket message object from raw message."""
 
-    try:
-        if not (device := device_registry.get(f"{message['UnitId']}-{message['DeviceId']}")):
-            log.warning(f"Got message for unknown device: {message['UnitId']}-{message['DeviceId']}")
-            raise UnkonwnDevice(device)
-    except KeyError:
-        log.warning("Got message for unknown device: %s", message)
-        raise UnkonwnDevice(device)
+    device = device_registry.get(f"{message['UnitId']}-{message['DeviceId']}")
 
-    if {"EventType", "EventValue", "QstringForExtraData"} <= set(message.keys()):
+    if {"FenceId", "IsInsideNow"} <= set(message.keys()):
+        # Geofence Event (Not Yet Supported)
+        pass
+    elif {"EventType", "EventValue", "QstringForExtraData"} <= set(message.keys()):
         # Event
         log.debug("WebSocket Message Type: Event")
         return EventMessage(message, device)
     elif {"EventType", "CorrelatedId"} <= set(message.keys()):
         # Monitoring Event
         log.debug("WebSocket Message Type: Monitoring Event")
         return MonitoringEventMessage(message, device)
     elif {"Property", "PropertyValue"} <= set(message.keys()):
         # Property Change
         log.debug("WebSocket Message Type: Property Change")
         return PropertyChangeMessage(message, device)
-    elif {"FenceId", "IsInsideNow"} <= set(message.keys()):
-        # Geofence Event (Not Yet Supported)
-        pass
     elif {"NewState", "FlagMask"} <= set(message.keys()):
         # State Change
         log.debug("WebSocket Message Type: State Change")
         return StatusChangeMessage(message, device)
 
-    raise UnsupportedAction(message)
+    raise UnsupportedWebSocketMessage(message)
 
 
 class WebSocketMessage(CastingMixin):
     """Alarm.com websocket message base class."""
 
     def __init__(self, message: dict, device: AllDevices_t):
         """Initialize."""
-        self.id_: str = f"{str(message.get('UnitId', ''))}-{str(message.get('DeviceId', ''))}"
+        self.id_: str = f"{message.get('UnitId', '')!s}-{message.get('DeviceId', '')!s}"
         self.device: AllDevices_t = device
 
 
 class EventMessage(WebSocketMessage):
     """Alarm.com event websocket message class."""
 
     def __init__(self, message: dict, device: AllDevices_t):
```

### Comparing `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax.egg-info/PKG-INFO` & `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalarmdotcomajax
-Version: 0.5.0b5
+Version: 0.5.0b6
 Summary: Python Interface for Alarm.com
 Home-page: https://github.com/pyalarmdotcom/pyalarmdotcomajax
 Author: Justin Wong
 Author-email: 46082645+uvjustin@users.noreply.github.com
 Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com, 466460+elahd@users.noreply.github.com
 License: MIT
@@ -34,16 +34,16 @@
 </p>
 <p align="center">
   <!-- <a href="https://www.codacy.com/gh/pyalarmdotcom/pyalarmdotcomajax/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=pyalarmdotcom/pyalarmdotcomajax&amp;utm_campaign=Badge_Grade"><img src="https://app.codacy.com/project/badge/Grade/c58b00c68f9542aea1554d160997e5cd"/></a> -->
   <!-- <a href="https://www.codacy.com/gh/pyalarmdotcom/pyalarmdotcomajax/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=pyalarmdotcom/pyalarmdotcomajax&amp;utm_campaign=Badge_Coverage"><img src="https://app.codacy.com/project/badge/Coverage/c58b00c68f9542aea1554d160997e5cd"/></a> -->
   <a href="https://results.pre-commit.ci/latest/github/pyalarmdotcom/pyalarmdotcomajax/master"><img src="https://results.pre-commit.ci/badge/github/pyalarmdotcom/pyalarmdotcomajax/master.svg" /></a>
   <a href="https://pypi.org/project/pyalarmdotcomajax/"><img alt="PyPI" src="https://img.shields.io/pypi/v/pyalarmdotcomajax"></a>
   <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" /></a>
-  <a href="https://github.com/PyCQA/pylint"><img src="https://img.shields.io/badge/linting-pylint-yellowgreen" /></a>
-  <a href="https://github.com/pyalarmdotcom/pyalarmdotcomajax/blob/master/LICENSE"><img alt="GitHub" src="https://img.shields.io/github/license/pyalarmdotcom/pyalarmdotcomajax"></a>
+  <a href="https://github.com/charliermarsh/ruff"><img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json" /></a>
+  <a href="https://github.com/pyalarmdotcom/pyalarmdotcomajax/blob/master/LICENSE"><img alt="GitHub" src="https://img.shields.io/github/license/pyalarmdotcom/pyalarmdotcomajax" /></a>
 </p>
 
 ## Installation / Usage
 
 To install use pip:
 
 ```bash
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.0b5 Summary: Python
+Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.0b6 Summary: Python
 Interface for Alarm.com Home-page: https://github.com/pyalarmdotcom/
 pyalarmdotcomajax Author: Justin Wong Author-email:
 46082645+uvjustin@users.noreply.github.com Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com,
 466460+elahd@users.noreply.github.com License: MIT Keywords: Alarm.com,Security
 System,Home Assistant Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English Classifier: Environment :: Web
@@ -19,15 +19,16 @@
      This is an unofficial project that is not affiliated with Alarm.com.
                     Forked from Daren Lord's pyalarmdotcom.
 
   [https://img.shields.io/badge/Creator-Justin%20Wong%20(%40uvjustin)-blue]
  [https://img.shields.io/badge/Maintainer-Elahd%20Bar--Shai%20(%40elahd)-blue]
   [https://results.pre-commit.ci/badge/github/pyalarmdotcom/pyalarmdotcomajax/
 master.svg] [PyPI] [https://img.shields.io/badge/code%20style-black-000000.svg]
-      [https://img.shields.io/badge/linting-pylint-yellowgreen] [GitHub]
+    [https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/
+            charliermarsh/ruff/main/assets/badge/v2.json] [GitHub]
 ## Installation / Usage To install use pip: ```bash pip install
 pyalarmdotcomajax ``` Or clone the repo: ```bash git clone https://github.com/
 uvjustin/pyalarmdotcomajax.git python setup.py install ``` ## Usage See
 `examples/basic_sensor_data.py` for a basic usage example. ## Device Support
 (Core Functions) Pyalarmdotcomajax supports core features (monitoring and using
 actions) of the device types listed below. - As of v0.2, multiples of all
 devices are supported. - All devices include the attributes: `name`, `id_`,
```

### Comparing `pyalarmdotcomajax-0.5.0b5/pyalarmdotcomajax.egg-info/SOURCES.txt` & `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 README.md
 pyproject.toml
 setup.cfg
 pyalarmdotcomajax/__init__.py
 pyalarmdotcomajax/__main__.py
 pyalarmdotcomajax/cli.py
 pyalarmdotcomajax/const.py
-pyalarmdotcomajax/errors.py
+pyalarmdotcomajax/exceptions.py
 pyalarmdotcomajax/extensions.py
 pyalarmdotcomajax/helpers.py
 pyalarmdotcomajax.egg-info/PKG-INFO
 pyalarmdotcomajax.egg-info/SOURCES.txt
 pyalarmdotcomajax.egg-info/dependency_links.txt
 pyalarmdotcomajax.egg-info/entry_points.txt
 pyalarmdotcomajax.egg-info/requires.txt
```

### Comparing `pyalarmdotcomajax-0.5.0b5/setup.cfg` & `pyalarmdotcomajax-0.5.0b6/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b5/tests/__init__.py` & `pyalarmdotcomajax-0.5.0b6/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b5/tests/conftest.py` & `pyalarmdotcomajax-0.5.0b6/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -81,21 +81,14 @@
         response_mocker.get(
             url=AttributeRegistry.get_endpoints(DeviceType.SYSTEM)["primary"].format(c.URL_BASE, "id-system"),
             status=200,
             body=get_http_body_json("system_ok"),
             repeat=repeat,
         )
 
-        # response_mocker.get(
-        #     url=AttributeRegistry.get_endpoints(DeviceType.SYSTEM)["primary"].format(c.URL_BASE, ""),
-        #     status=200,
-        #     body=get_http_body_json("systems_ok"),
-        #     repeat=repeat,
-        # )
-
         response_mocker.get(
             url=AttributeRegistry.get_endpoints(DeviceType.IMAGE_SENSOR)["primary"].format(c.URL_BASE, ""),
             status=200,
             body=get_http_body_json("image_sensors_ok"),
             repeat=repeat,
         )
 
@@ -124,28 +117,14 @@
             repeat=True,
         )
 
     return _load_mocks
 
 
 @pytest.fixture
-def device_catalog_no_permission(response_mocker: aioresponses, all_base_ok_responses_callable: Callable) -> None:
-    """No permission to view devices."""
-
-    response_mocker.get(
-        url=AlarmController.ALL_DEVICES_URL_TEMPLATE.format(c.URL_BASE, "id-system"),
-        status=200,
-        body=get_http_body_json("no_permissions_or_invalid_antiforgery"),
-        repeat=True,
-    )
-
-    all_base_ok_responses_callable()
-
-
-@pytest.fixture
 def image_sensors_no_permission(response_mocker: aioresponses, all_base_ok_responses_callable: Callable) -> None:
     """No permission to view devices."""
 
     response_mocker.get(
         url=AlarmController.ALL_RECENT_IMAGES_TEMPLATE.format(c.URL_BASE, ""),
         status=200,
         body=get_http_body_json("processing_error"),
```

### Comparing `pyalarmdotcomajax-0.5.0b5/tests/test_controller.py` & `pyalarmdotcomajax-0.5.0b6/tests/test_controller.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,30 @@
 """Tests for main controller."""
 
 # pylint: disable=protected-access
-
+# ruff: noqa: SLF001, S105
 
 import aiohttp
 import pytest
 
 from pyalarmdotcomajax import AlarmController
-from pyalarmdotcomajax.errors import DataFetchFailed
+from pyalarmdotcomajax.exceptions import UnexpectedResponse
 
 
 def test_property__initial_state(adc_client: AlarmController) -> None:
     """Ensure that login data is ingested correctly."""
-    assert adc_client._password == "hunter2"  # noqa: S105
+    assert adc_client._password == "hunter2"
     assert adc_client._username == "test-username"
     assert adc_client.two_factor_cookie == "test-cookie"
     assert isinstance(adc_client._websession, aiohttp.ClientSession)
 
     assert adc_client.provider_name is None
     assert adc_client.user_id is None
 
-    assert not adc_client.devices.systems.values()
-    assert not adc_client.devices.partitions.values()
-    assert not adc_client.devices.sensors.values()
-    assert not adc_client.devices.locks.values()
-    assert not adc_client.devices.garage_doors.values()
-    assert not adc_client.devices.image_sensors.values()
-    assert not adc_client.devices.lights.values()
-    assert not adc_client.devices.thermostats.values()
-    assert not adc_client.devices.cameras.values()
-    assert not adc_client.devices.water_sensors.values()
+    assert not adc_client.devices.all.values()
 
 
 @pytest.mark.asyncio
 async def test__device_storage(
     all_base_ok_responses: str,
     adc_client: AlarmController,
 ) -> None:
@@ -55,15 +46,15 @@
 @pytest.mark.asyncio
 async def test___async_update__refresh_failure(
     device_catalog_no_permissions: str,
     adc_client: AlarmController,
 ) -> None:
     """Test for when devices initialize but fail to refresh. Ensure that devices are wiped on update failure."""
 
-    with pytest.raises(DataFetchFailed):
+    with pytest.raises(UnexpectedResponse):
         await adc_client.async_update()
 
 
 @pytest.mark.asyncio
 async def test__async_has_image_sensors(
     image_sensors_no_permission: str,
     all_base_ok_responses: str,
```

### Comparing `pyalarmdotcomajax-0.5.0b5/tests/test_device_extensions.py` & `pyalarmdotcomajax-0.5.0b6/tests/test_device_extensions.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b5/tests/test_partition.py` & `pyalarmdotcomajax-0.5.0b6/tests/test_partition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Test partition device."""
 
+# ruff: noqa: PLR2004
+
 from collections import Counter
 
 import pytest
 
 from pyalarmdotcomajax import AlarmController
 from pyalarmdotcomajax.cli import _print_element_tearsheet
 from pyalarmdotcomajax.devices.partition import Partition
```

### Comparing `pyalarmdotcomajax-0.5.0b5/tests/test_sensors.py` & `pyalarmdotcomajax-0.5.0b6/tests/test_sensors.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b5/tests/test_thermostat.py` & `pyalarmdotcomajax-0.5.0b6/tests/test_thermostat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Test thermostat device."""
 
+# ruff: noqa: PLR2004
 
 import pytest
 
 from pyalarmdotcomajax import AlarmController
 from pyalarmdotcomajax.cli import _print_element_tearsheet
 from pyalarmdotcomajax.devices.thermostat import Thermostat
```

