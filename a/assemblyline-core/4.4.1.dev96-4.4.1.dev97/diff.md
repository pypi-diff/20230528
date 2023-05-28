# Comparing `tmp/assemblyline-core-4.4.1.dev96.tar.gz` & `tmp/assemblyline-core-4.4.1.dev97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assemblyline-core-4.4.1.dev96.tar", last modified: Fri May 26 15:59:07 2023, max compression
+gzip compressed data, was "assemblyline-core-4.4.1.dev97.tar", last modified: Sun May 28 06:56:01 2023, max compression
```

## Comparing `assemblyline-core-4.4.1.dev96.tar` & `assemblyline-core-4.4.1.dev97.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-26 15:59:07.887010 assemblyline-core-4.4.1.dev96/
--rw-r--r--   0 vsts      (1001) docker     (122)     1396 2023-05-26 15:58:52.000000 assemblyline-core-4.4.1.dev96/LICENCE.md
--rw-r--r--   0 vsts      (1001) docker     (122)     1681 2023-05-26 15:59:07.887010 assemblyline-core-4.4.1.dev96/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      860 2023-05-26 15:58:52.000000 assemblyline-core-4.4.1.dev96/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-26 15:59:07.859008 assemblyline-core-4.4.1.dev96/assemblyline_core/
--rw-r--r--   0 vsts      (1001) docker     (122)       12 2023-05-26 15:59:06.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/VERSION
--rw-r--r--   0 vsts      (1001) docker     (122)       49 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-26 15:59:07.859008 assemblyline-core-4.4.1.dev96/assemblyline_core/alerter/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-26 15:58:52.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/alerter/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15689 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/alerter/processing.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4871 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/alerter/run_alerter.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-26 15:59:07.859008 assemblyline-core-4.4.1.dev96/assemblyline_core/archiver/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/archiver/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8210 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/archiver/run_archiver.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-26 15:59:07.863008 assemblyline-core-4.4.1.dev96/assemblyline_core/dispatching/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-26 15:58:52.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/dispatching/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      122 2023-05-26 15:58:52.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/dispatching/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    16929 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/dispatching/client.py
--rw-r--r--   0 vsts      (1001) docker     (122)    83163 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/dispatching/dispatcher.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7289 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/dispatching/schedules.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2050 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/dispatching/timeout.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-26 15:59:07.863008 assemblyline-core-4.4.1.dev96/assemblyline_core/expiry/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-26 15:58:52.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/expiry/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13558 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/expiry/run_expiry.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-26 15:59:07.863008 assemblyline-core-4.4.1.dev96/assemblyline_core/ingester/
--rw-r--r--   0 vsts      (1001) docker     (122)       54 2023-05-26 15:58:52.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/ingester/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      113 2023-05-26 15:58:52.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/ingester/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      182 2023-05-26 15:58:52.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/ingester/constants.py
--rw-r--r--   0 vsts      (1001) docker     (122)    35958 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/ingester/ingester.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-26 15:59:07.875009 assemblyline-core-4.4.1.dev96/assemblyline_core/metrics/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-26 15:58:52.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/metrics/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    30681 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/metrics/es_metrics.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13019 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/metrics/heartbeat_formatter.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7559 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/metrics/helper.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17144 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/metrics/metrics_server.py
--rw-r--r--   0 vsts      (1001) docker     (122)      256 2023-05-26 15:58:52.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/metrics/run_heartbeat_manager.py
--rw-r--r--   0 vsts      (1001) docker     (122)      250 2023-05-26 15:58:52.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/metrics/run_metrics_aggregator.py
--rw-r--r--   0 vsts      (1001) docker     (122)      274 2023-05-26 15:58:52.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/metrics/run_statistics_aggregator.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-26 15:59:07.875009 assemblyline-core-4.4.1.dev96/assemblyline_core/plumber/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-26 15:58:52.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/plumber/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6434 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/plumber/run_plumber.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-26 15:59:07.875009 assemblyline-core-4.4.1.dev96/assemblyline_core/replay/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/replay/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12345 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/replay/client.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-26 15:59:07.875009 assemblyline-core-4.4.1.dev96/assemblyline_core/replay/creator/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/replay/creator/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2168 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/replay/creator/run.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4743 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/replay/creator/run_worker.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-26 15:59:07.875009 assemblyline-core-4.4.1.dev96/assemblyline_core/replay/loader/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/replay/loader/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3533 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/replay/loader/run.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2999 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/replay/loader/run_worker.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2577 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/replay/replay.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2498 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/safelist_client.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-26 15:59:07.875009 assemblyline-core-4.4.1.dev96/assemblyline_core/scaler/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-26 15:58:52.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/scaler/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1858 2023-05-26 15:58:52.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/scaler/collection.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-26 15:59:07.875009 assemblyline-core-4.4.1.dev96/assemblyline_core/scaler/controllers/
--rw-r--r--   0 vsts      (1001) docker     (122)       90 2023-05-26 15:58:52.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/scaler/controllers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    24018 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/scaler/controllers/docker_ctl.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2174 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/scaler/controllers/interface.py
--rw-r--r--   0 vsts      (1001) docker     (122)    53877 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/scaler/controllers/kubernetes_ctl.py
--rw-r--r--   0 vsts      (1001) docker     (122)      160 2023-05-26 15:58:52.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/scaler/run_scaler.py
--rw-r--r--   0 vsts      (1001) docker     (122)    48567 2023-05-26 15:58:53.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/scaler/scaler_server.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12219 2023-05-26 15:58:54.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/server_base.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10353 2023-05-26 15:58:54.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/submission_client.py
--rw-r--r--   0 vsts      (1001) docker     (122)    22003 2023-05-26 15:58:54.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/tasking_client.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-26 15:59:07.875009 assemblyline-core-4.4.1.dev96/assemblyline_core/updater/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-26 15:58:52.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/updater/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8093 2023-05-26 15:58:54.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/updater/helper.py
--rw-r--r--   0 vsts      (1001) docker     (122)    32152 2023-05-26 15:58:54.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/updater/run_updater.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-26 15:59:07.875009 assemblyline-core-4.4.1.dev96/assemblyline_core/vacuum/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-26 15:58:54.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/vacuum/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5628 2023-05-26 15:58:54.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/vacuum/crawler.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2675 2023-05-26 15:58:54.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/vacuum/department_map.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3478 2023-05-26 15:58:54.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/vacuum/safelist.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3136 2023-05-26 15:58:54.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/vacuum/stream_map.py
--rw-r--r--   0 vsts      (1001) docker     (122)    29284 2023-05-26 15:58:54.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/vacuum/worker.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-26 15:59:07.875009 assemblyline-core-4.4.1.dev96/assemblyline_core/workflow/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-26 15:58:52.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9532 2023-05-26 15:58:54.000000 assemblyline-core-4.4.1.dev96/assemblyline_core/workflow/run_workflow.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-26 15:59:07.859008 assemblyline-core-4.4.1.dev96/assemblyline_core.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1681 2023-05-26 15:59:07.000000 assemblyline-core-4.4.1.dev96/assemblyline_core.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     2975 2023-05-26 15:59:07.000000 assemblyline-core-4.4.1.dev96/assemblyline_core.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-26 15:59:07.000000 assemblyline-core-4.4.1.dev96/assemblyline_core.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       66 2023-05-26 15:59:07.000000 assemblyline-core-4.4.1.dev96/assemblyline_core.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       18 2023-05-26 15:59:07.000000 assemblyline-core-4.4.1.dev96/assemblyline_core.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       70 2023-05-26 15:59:07.887010 assemblyline-core-4.4.1.dev96/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     1870 2023-05-26 15:58:54.000000 assemblyline-core-4.4.1.dev96/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-26 15:59:07.887010 assemblyline-core-4.4.1.dev96/test/
--rw-r--r--   0 vsts      (1001) docker     (122)     5768 2023-05-26 15:58:52.000000 assemblyline-core-4.4.1.dev96/test/test_alerter.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15228 2023-05-26 15:58:54.000000 assemblyline-core-4.4.1.dev96/test/test_dispatcher.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2043 2023-05-26 15:58:54.000000 assemblyline-core-4.4.1.dev96/test/test_expiry.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2506 2023-05-26 15:58:54.000000 assemblyline-core-4.4.1.dev96/test/test_plumber.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6995 2023-05-26 15:58:54.000000 assemblyline-core-4.4.1.dev96/test/test_replay.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2006 2023-05-26 15:58:52.000000 assemblyline-core-4.4.1.dev96/test/test_scaler.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5313 2023-05-26 15:58:54.000000 assemblyline-core-4.4.1.dev96/test/test_scheduler.py
--rw-r--r--   0 vsts      (1001) docker     (122)    38685 2023-05-26 15:58:54.000000 assemblyline-core-4.4.1.dev96/test/test_simulation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4419 2023-05-26 15:58:54.000000 assemblyline-core-4.4.1.dev96/test/test_vacuum.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6792 2023-05-26 15:58:54.000000 assemblyline-core-4.4.1.dev96/test/test_worker_ingest.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4780 2023-05-26 15:58:54.000000 assemblyline-core-4.4.1.dev96/test/test_worker_submit.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-28 06:56:01.778700 assemblyline-core-4.4.1.dev97/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1396 2023-05-28 06:55:50.000000 assemblyline-core-4.4.1.dev97/LICENCE.md
+-rw-r--r--   0 vsts      (1001) docker     (122)     1681 2023-05-28 06:56:01.778700 assemblyline-core-4.4.1.dev97/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      860 2023-05-28 06:55:50.000000 assemblyline-core-4.4.1.dev97/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-28 06:56:01.714699 assemblyline-core-4.4.1.dev97/assemblyline_core/
+-rw-r--r--   0 vsts      (1001) docker     (122)       12 2023-05-28 06:56:00.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/VERSION
+-rw-r--r--   0 vsts      (1001) docker     (122)       49 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-28 06:56:01.722699 assemblyline-core-4.4.1.dev97/assemblyline_core/alerter/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-28 06:55:50.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/alerter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15689 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/alerter/processing.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4871 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/alerter/run_alerter.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-28 06:56:01.722699 assemblyline-core-4.4.1.dev97/assemblyline_core/archiver/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/archiver/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8210 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/archiver/run_archiver.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-28 06:56:01.726699 assemblyline-core-4.4.1.dev97/assemblyline_core/dispatching/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-28 06:55:50.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/dispatching/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      122 2023-05-28 06:55:50.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/dispatching/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    16929 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/dispatching/client.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    83163 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/dispatching/dispatcher.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7289 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/dispatching/schedules.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2050 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/dispatching/timeout.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-28 06:56:01.726699 assemblyline-core-4.4.1.dev97/assemblyline_core/expiry/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-28 06:55:50.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/expiry/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13558 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/expiry/run_expiry.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-28 06:56:01.738699 assemblyline-core-4.4.1.dev97/assemblyline_core/ingester/
+-rw-r--r--   0 vsts      (1001) docker     (122)       54 2023-05-28 06:55:50.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/ingester/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      113 2023-05-28 06:55:50.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/ingester/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      182 2023-05-28 06:55:50.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/ingester/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    35958 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/ingester/ingester.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-28 06:56:01.742699 assemblyline-core-4.4.1.dev97/assemblyline_core/metrics/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-28 06:55:50.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/metrics/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    30681 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/metrics/es_metrics.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13019 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/metrics/heartbeat_formatter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7559 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/metrics/helper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17144 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/metrics/metrics_server.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      256 2023-05-28 06:55:50.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/metrics/run_heartbeat_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      250 2023-05-28 06:55:50.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/metrics/run_metrics_aggregator.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      274 2023-05-28 06:55:50.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/metrics/run_statistics_aggregator.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-28 06:56:01.750699 assemblyline-core-4.4.1.dev97/assemblyline_core/plumber/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-28 06:55:50.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/plumber/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6434 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/plumber/run_plumber.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-28 06:56:01.750699 assemblyline-core-4.4.1.dev97/assemblyline_core/replay/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/replay/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12345 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/replay/client.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-28 06:56:01.754700 assemblyline-core-4.4.1.dev97/assemblyline_core/replay/creator/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/replay/creator/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2168 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/replay/creator/run.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4743 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/replay/creator/run_worker.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-28 06:56:01.754700 assemblyline-core-4.4.1.dev97/assemblyline_core/replay/loader/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/replay/loader/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3533 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/replay/loader/run.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2999 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/replay/loader/run_worker.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2577 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/replay/replay.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2498 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/safelist_client.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-28 06:56:01.758700 assemblyline-core-4.4.1.dev97/assemblyline_core/scaler/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-28 06:55:50.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/scaler/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1858 2023-05-28 06:55:50.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/scaler/collection.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-28 06:56:01.758700 assemblyline-core-4.4.1.dev97/assemblyline_core/scaler/controllers/
+-rw-r--r--   0 vsts      (1001) docker     (122)       90 2023-05-28 06:55:50.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/scaler/controllers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    24018 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/scaler/controllers/docker_ctl.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2174 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/scaler/controllers/interface.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    54253 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/scaler/controllers/kubernetes_ctl.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      160 2023-05-28 06:55:50.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/scaler/run_scaler.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    48567 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/scaler/scaler_server.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12219 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/server_base.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10353 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/submission_client.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    22003 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/tasking_client.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-28 06:56:01.762699 assemblyline-core-4.4.1.dev97/assemblyline_core/updater/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-28 06:55:50.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/updater/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9293 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/updater/helper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    32180 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/updater/run_updater.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-28 06:56:01.762699 assemblyline-core-4.4.1.dev97/assemblyline_core/vacuum/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/vacuum/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5628 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/vacuum/crawler.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2675 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/vacuum/department_map.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3478 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/vacuum/safelist.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3136 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/vacuum/stream_map.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    29284 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/vacuum/worker.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-28 06:56:01.766700 assemblyline-core-4.4.1.dev97/assemblyline_core/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-28 06:55:50.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9532 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/assemblyline_core/workflow/run_workflow.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-28 06:56:01.718699 assemblyline-core-4.4.1.dev97/assemblyline_core.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1681 2023-05-28 06:56:01.000000 assemblyline-core-4.4.1.dev97/assemblyline_core.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     2975 2023-05-28 06:56:01.000000 assemblyline-core-4.4.1.dev97/assemblyline_core.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-28 06:56:01.000000 assemblyline-core-4.4.1.dev97/assemblyline_core.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       66 2023-05-28 06:56:01.000000 assemblyline-core-4.4.1.dev97/assemblyline_core.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       18 2023-05-28 06:56:01.000000 assemblyline-core-4.4.1.dev97/assemblyline_core.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       70 2023-05-28 06:56:01.778700 assemblyline-core-4.4.1.dev97/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     1870 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-28 06:56:01.774700 assemblyline-core-4.4.1.dev97/test/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5768 2023-05-28 06:55:50.000000 assemblyline-core-4.4.1.dev97/test/test_alerter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15228 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/test/test_dispatcher.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2043 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/test/test_expiry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2506 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/test/test_plumber.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6995 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/test/test_replay.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2006 2023-05-28 06:55:50.000000 assemblyline-core-4.4.1.dev97/test/test_scaler.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5313 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/test/test_scheduler.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    38685 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/test/test_simulation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4419 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/test/test_vacuum.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6792 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/test/test_worker_ingest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4780 2023-05-28 06:55:51.000000 assemblyline-core-4.4.1.dev97/test/test_worker_submit.py
```

### Comparing `assemblyline-core-4.4.1.dev96/LICENCE.md` & `assemblyline-core-4.4.1.dev97/LICENCE.md`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/PKG-INFO` & `assemblyline-core-4.4.1.dev97/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyline-core
-Version: 4.4.1.dev96
+Version: 4.4.1.dev97
 Summary: Assemblyline 4 - Core components
 Home-page: https://github.com/CybercentreCanada/assemblyline-core/
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Keywords: assemblyline automated malware analysis gc canada cse-cst cse cst cyber cccs
 Platform: UNKNOWN
```

### Comparing `assemblyline-core-4.4.1.dev96/README.md` & `assemblyline-core-4.4.1.dev97/README.md`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/alerter/processing.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/alerter/processing.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/alerter/run_alerter.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/alerter/run_alerter.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/archiver/run_archiver.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/archiver/run_archiver.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/dispatching/client.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/dispatching/client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/dispatching/dispatcher.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/dispatching/dispatcher.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/dispatching/schedules.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/dispatching/schedules.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/dispatching/timeout.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/dispatching/timeout.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/expiry/run_expiry.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/expiry/run_expiry.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/ingester/ingester.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/ingester/ingester.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/metrics/es_metrics.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/metrics/es_metrics.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/metrics/heartbeat_formatter.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/metrics/heartbeat_formatter.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/metrics/helper.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/metrics/helper.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/metrics/metrics_server.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/metrics/metrics_server.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/plumber/run_plumber.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/plumber/run_plumber.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/replay/client.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/replay/client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/replay/creator/run.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/replay/creator/run.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/replay/creator/run_worker.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/replay/creator/run_worker.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/replay/loader/run.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/replay/loader/run.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/replay/loader/run_worker.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/replay/loader/run_worker.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/replay/replay.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/replay/replay.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/safelist_client.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/safelist_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/scaler/collection.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/scaler/collection.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/scaler/controllers/docker_ctl.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/scaler/controllers/docker_ctl.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/scaler/controllers/interface.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/scaler/controllers/interface.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/scaler/controllers/kubernetes_ctl.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/scaler/controllers/kubernetes_ctl.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from collections import OrderedDict, defaultdict
 from typing import List, Optional, Tuple
 from time import sleep
 
 
 from kubernetes import client, config, watch
 from kubernetes.client import V1Deployment, V1DeploymentSpec, V1PodTemplateSpec, V1DeploymentStrategy, \
-    V1PodSpec, V1ObjectMeta, V1Volume, V1Container, V1VolumeMount, V1EnvVar, V1ConfigMapVolumeSource, \
+    V1PodSpec, V1PodOS, V1ObjectMeta, V1Volume, V1Container, V1VolumeMount, V1EnvVar, V1ConfigMapVolumeSource, \
     V1PersistentVolumeClaimVolumeSource, V1LabelSelector, V1ResourceRequirements, V1PersistentVolumeClaim, \
     V1PersistentVolumeClaimSpec, V1NetworkPolicy, V1NetworkPolicySpec, V1NetworkPolicyEgressRule, V1NetworkPolicyPeer, \
     V1NetworkPolicyIngressRule, V1Secret, V1SecretVolumeSource, V1LocalObjectReference, V1Service, V1ServiceSpec, V1ServicePort, V1PodSecurityContext, \
     V1Probe, V1ExecAction, V1SecurityContext
 from kubernetes.client.rest import ApiException
 from assemblyline.odm.models.service import DependencyConfig, DockerConfig, PersistentVolume
 
@@ -710,23 +710,35 @@
                 name="chown-mounts",
                 image=docker_config.image,
                 command=['chown', '-R', '1000:1000'] + [m.mount_path for m in chown_mounts],
                 security_context=V1SecurityContext(run_as_user=0),
                 volume_mounts=chown_mounts
             ))
 
+        pod_os = None
+        security_context = V1PodSecurityContext(fs_group=1000)
+        if docker_config.operating_system:
+            #  Allow Kubernetes to schedule the pod to a compatible node
+            pod_os = V1PodOS(name=docker_config.operating_system)
+
+        if docker_config.operating_system == 'windows':
+            security_context = None
+
+
         pod = V1PodSpec(
             init_containers=init_containers,
             volumes=all_volumes,
             containers=self._create_containers(service_name, deployment_name, docker_config,
                                                all_mounts, core_container=core_mounts),
+            os=pod_os,
             priority_class_name=self.dependency_priority if high_priority else self.priority,
             termination_grace_period_seconds=shutdown_seconds,
-            security_context=V1PodSecurityContext(fs_group=1000),
+            security_context=security_context,
             service_account_name=service_account,
+
         )
 
         if use_pull_secret:
             pod.image_pull_secrets = [V1LocalObjectReference(name=pull_secret_name)]
 
         template = V1PodTemplateSpec(
             metadata=metadata,
```

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/scaler/scaler_server.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/scaler/scaler_server.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/server_base.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/server_base.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/submission_client.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/submission_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/tasking_client.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/tasking_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/updater/helper.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/updater/helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,84 +8,122 @@
 from assemblyline.odm.models.config import Config as SystemConfig
 from assemblyline.odm.models.service import Service as ServiceConfig
 
 from base64 import b64encode
 from collections import defaultdict
 from logging import Logger
 from packaging.version import parse, Version
+from typing import Any, Dict, List, Tuple
 
 DEFAULT_DOCKER_REGISTRY = "registry.hub.docker.com"
 
 
 class ContainerRegistry():
-    # Provide a means of obtaining a list of tags from a container registry
-    def _get_proprietary_registry_tags(self, server, image_name, auth, verify):
-        raise NotImplementedError()
-
-
-class DockerRegistry(ContainerRegistry):
-    def _get_proprietary_registry_tags(self, server, image_name, auth, verify, proxies=None):
-        # Find latest tag for each types
-        url = f"https://{server}/v2/{image_name}/tags/list"
-
-        # Get tag list
-        headers = {}
-        if auth:
-            headers["Authorization"] = auth
+    def __init__(self, server, headers: Dict[str, str] = None, verify: bool = True,
+                 proxies: Dict[str, str] = None, *args, **kwargs):
+        self.server = server
+        self.session = requests.Session()
+        self.session.headers = headers
+        self.session.verify = verify
+        self.session.proxies = proxies
 
+    def _make_request(self, path: str) -> Dict[str, Any]:
+        request_path = f"{self.server}{path}"
         resp = None
         try:
-            resp = requests.get(url, headers=headers, verify=verify, proxies=proxies)
+            resp = self.session.get(f"https://{request_path}")
         except requests.exceptions.SSLError:
             # Connect to insecure registry over HTTP (development only)
-            if not verify:
-                url = f"http://{server}/v2/{image_name}/tags/list"
-                resp = requests.get(url, headers=headers, verify=verify, proxies=proxies)
-
+            if not self.session.verify:
+                resp = self.session.get(f"http://{request_path}")
         # Test for valid response
         if resp and resp.ok:
-            # Test for positive list of tags
-            resp_data = resp.json()
-            return resp_data['tags'] or []
+            return resp.json()
+        return None
+
+    # Provide a means of obtaining a list of tags from a container registry
+    def get_image_tags(self, image_name) -> List[str]:
+        raise NotImplementedError()
+
+    # Provide a means of obtaining the compatible operating system for the container image
+    def get_image_os(self, image_name, image_tag) -> str:
+        raise NotImplementedError()
+
+
+class DockerHub(ContainerRegistry):
+    def __init__(self, update_channel, proxies: Dict[str, str] = None, *args, **kwargs):
+        super().__init__(DEFAULT_DOCKER_REGISTRY, None, True, proxies)
+        self.update_channel = update_channel
+
+    def get_image_tags(self, image_name) -> List[str]:
+        resp = self._make_request(f"/v2/repositories/{image_name}/tags?page_size=5&page=1&name={self.update_channel}")
+        if resp:
+            return [x['name'] for x in resp['results']]
+        return []
+
+    def get_image_os(self, image_name, image_tag) -> str:
+        resp = self._make_request(f"/v2/repositories/{image_name}/tags/{image_tag}")
+        if resp:
+            return resp['images'][0]['os']
+        return None
+
+
+# Ref: https://docs.docker.com/registry/spec/api/#detail
+class DockerRegistry(ContainerRegistry):
+    def get_image_tags(self, image_name) -> List[str]:
+        # Find latest tag for each types
+        resp = self._make_request(f"/v2/{image_name}/tags/list")
+        if resp:
+            return resp['tags'] or []
         return []
 
+    def get_image_os(self, image_name, image_tag) -> str:
+        resp = self._make_request(f"/v2/{image_name}/manifests/{image_tag}")
+        if resp:
+            # Retrieve OS compatibilty from historical record
+            return json.loads(resp['history'][0]['v1Compatibility'])['os']
+
+        # Unable to determine the OS compatibility
+        return None
 
+
+# Ref: https://github.com/goharbor/harbor/blob/main/api/v2.0/swagger.yaml
 class HarborRegistry(ContainerRegistry):
-    def _get_proprietary_registry_tags(self, server, image_name, auth, verify, proxies=None):
+    def _get_project_repo_ids(self, image_name) -> Tuple[str, str]:
         # Determine project/repo IDs from image name
         project_id, repo_id = image_name.split('/', 1)
         repo_id = repo_id.replace('/', "%2F")
-        url = f"https://{server}/api/v2.0/projects/{project_id}/repositories/{repo_id}/artifacts?page_size=0"
+        return project_id, repo_id
 
-        headers = {}
-        if auth:
-            headers["Authorization"] = auth
+    def get_image_tags(self, image_name) -> List[str]:
+        project_id, repo_id = self._get_project_repo_ids(image_name)
+        resp = self._make_request(f"/api/v2.0/projects/{project_id}/repositories/{repo_id}/artifacts?page_size=0")
+        if resp:
+            return [tag['name'] for image in resp if image['tags'] for tag in image['tags']]
+        return []
 
-        resp = None
-        try:
-            resp = requests.get(url, headers=headers, verify=verify, proxies=proxies)
-        except requests.exceptions.SSLError:
-            # Connect to insecure registry over HTTP (development only)
-            if not verify:
-                url = f"http://{server}/api/v2.0/projects/{project_id}/repositories/{repo_id}/artifacts"
-                resp = requests.get(url, headers=headers, verify=verify, proxies=proxies)
+    def get_image_os(self, image_name, image_tag) -> str:
+        project_id, repo_id = self._get_project_repo_ids(image_name)
+        resp = self._make_request(f"/api/v2.0/projects/{project_id}/repositories/{repo_id}/artifacts/{image_tag}")
+        if resp:
+            # Retrieve OS compatibilty from reference
+            return resp['references'][0]['platform']['os']
 
-        if resp and resp.ok:
-            return [tag['name'] for image in resp.json() if image['tags'] for tag in image['tags']]
-        return []
+        # Unable to determine the OS compatibility
+        return None
 
 
 REGISTRY_TYPE_MAPPING = {
-    'docker': DockerRegistry(),
-    'harbor': HarborRegistry()
+    'dockerhub': DockerHub,
+    'docker': DockerRegistry,
+    'harbor': HarborRegistry
 }
 
 
-def get_latest_tag_for_service(
-        service_config: ServiceConfig, system_config: SystemConfig, logger: Logger, prefix: str = ""):
+def get_latest_tag_for_service(service_config: ServiceConfig, system_config: SystemConfig, logger: Logger, prefix: str = ""):
     def process_image(image):
         # Find which server to search in
         server = image.split("/")[0]
         if server != "cccs":
             if ":" in server:
                 image_name = image[len(server) + 1:]
             else:
@@ -134,29 +172,33 @@
         auth_config = {
             'username': service_config.docker_config.registry_username,
             'password': service_config.docker_config.registry_password
         }
         upass = f"{service_config.docker_config.registry_username}:{service_config.docker_config.registry_password}"
         auth = f"Basic {b64encode(upass.encode()).decode()}"
 
-    registry = REGISTRY_TYPE_MAPPING[service_config.docker_config.registry_type]
     proxies = None
     for reg_conf in system_config.core.updater.registry_configs:
         if reg_conf.name == server:
             proxies = reg_conf.proxies or None
             break
 
-    if server == DEFAULT_DOCKER_REGISTRY:
-        tags = _get_dockerhub_tags(image_name, update_channel, proxies)
-    else:
-        tags = registry._get_proprietary_registry_tags(server, image_name, auth,
-                                                       not system_config.services.allow_insecure_registry, proxies)
+    registry_type = 'dockerhub' if server == DEFAULT_DOCKER_REGISTRY else service_config.docker_config.registry_type
+    registry_args = {
+        'server': server,
+        'headers': {'Authorization': auth},
+        'verify': not system_config.services.allow_insecure_registry,
+        'proxies': proxies,
+        'update_channel': update_channel
+    }
 
-    tag_name = None
+    registry: ContainerRegistry = REGISTRY_TYPE_MAPPING[registry_type](**registry_args)
+    tags = registry.get_image_tags(image_name)
 
+    tag_name = None
     # Pre-filter tags to only consider 'compatible' tags relative to the running system
     tags = [t for t in tags
             if re.match(f"({FRAMEWORK_VERSION})[.]({SYSTEM_VERSION})[.]\\d+[.]({update_channel})\\d+", t)]
 
     if not tags:
         logger.warning(f"{prefix}Cannot fetch latest tag for service {service_name} - {image_name}"
                        f" => [server: {server}, repo_name: {image_name}, channel: {update_channel}]")
@@ -172,32 +214,14 @@
 
         logger.info(f"{prefix}Latest {service_name} tag on {update_channel.upper()} channel is: {tag_name}")
 
     # Fix service image for use in Kubernetes
     image_variables = defaultdict(str)
     image_variables.update(system_config.services.image_variables)
     image = string.Template(image).safe_substitute(image_variables)
-    server, image_name = process_image(image)
+    os = registry.get_image_os(image_name, tag_name)
 
     # Append server to image if not the default server
-    if server != "registry.hub.docker.com":
+    if server != DEFAULT_DOCKER_REGISTRY:
         image_name = "/".join([server, image_name])
 
-    return image_name, tag_name, auth_config
-
-
-# Default for obtaining tags from DockerHub
-def _get_dockerhub_tags(image_name, update_channel, proxies=None):
-    # Find latest tag for each types
-    url = f"https://{DEFAULT_DOCKER_REGISTRY}/v2/repositories/{image_name}/tags" \
-        f"?page_size=5&page=1&name={update_channel}"
-
-    # Get tag list
-    resp = requests.get(url, proxies=proxies)
-
-    # Test for valid response
-    if resp.ok:
-        # Test for positive list of tags
-        resp_data = resp.json()
-        return [x['name'] for x in resp_data['results']]
-
-    return []
+    return image_name, tag_name, auth_config, os
```

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/updater/run_updater.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/updater/run_updater.py`

 * *Files 1% similar despite different names*

```diff
@@ -474,18 +474,18 @@
                 try:
                     service = Service(
                         {'name': service_name,
                          'update_channel': self.config.services.preferred_update_channel,
                          'version': tag,
                          'docker_config': {'image': install_data.get('image')}})
 
-                    image_name, tag_name, auth = get_latest_tag_for_service(
+                    image_name, tag_name, auth, os = get_latest_tag_for_service(
                         service,  self.config, self.log, prefix="[CI] ")
 
-                    docker_config = dict(image=f"{image_name}:{tag_name}")
+                    docker_config = dict(image=f"{image_name}:{tag_name}", operating_system=os)
                     if auth:
                         docker_config.update(dict(registry_username=auth['username'],
                                                   registry_password=auth['password']))
 
                     # Apply any container configuration changes specifically for jobs
                     docker_config.update(self.job_dockerconfig)
 
@@ -634,15 +634,15 @@
         while self.running:
             self.log.info("[CV] Checking for new versions of all service containers...")
             existing_services = set(self.container_update.keys()) | set(self.latest_service_tags.keys())
             discovered_services: list[str] = []
 
             for service in self.datastore.list_all_services(full=True):
                 discovered_services.append(service.name)
-                image_name, tag_name, auth = get_latest_tag_for_service(service, self.config, self.log, prefix="[CV] ")
+                image_name, tag_name, auth, _ = get_latest_tag_for_service(service, self.config, self.log, prefix="[CV] ")
                 self.latest_service_tags.set(service.name,
                                              {'auth': auth, 'image': image_name, service.update_channel: tag_name})
 
             # Remove services we have locally or in redis that have been deleted from the database
             for stray_service in existing_services - set(discovered_services):
                 self.log.info(f"[CV] Service updates disabled for {stray_service}")
                 self._service_stage_hash.pop(stray_service)
```

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/vacuum/crawler.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/vacuum/crawler.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/vacuum/department_map.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/vacuum/department_map.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/vacuum/safelist.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/vacuum/safelist.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/vacuum/stream_map.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/vacuum/stream_map.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/vacuum/worker.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/vacuum/worker.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core/workflow/run_workflow.py` & `assemblyline-core-4.4.1.dev97/assemblyline_core/workflow/run_workflow.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core.egg-info/PKG-INFO` & `assemblyline-core-4.4.1.dev97/assemblyline_core.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyline-core
-Version: 4.4.1.dev96
+Version: 4.4.1.dev97
 Summary: Assemblyline 4 - Core components
 Home-page: https://github.com/CybercentreCanada/assemblyline-core/
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Keywords: assemblyline automated malware analysis gc canada cse-cst cse cst cyber cccs
 Platform: UNKNOWN
```

### Comparing `assemblyline-core-4.4.1.dev96/assemblyline_core.egg-info/SOURCES.txt` & `assemblyline-core-4.4.1.dev97/assemblyline_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/setup.py` & `assemblyline-core-4.4.1.dev97/setup.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/test/test_alerter.py` & `assemblyline-core-4.4.1.dev97/test/test_alerter.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/test/test_dispatcher.py` & `assemblyline-core-4.4.1.dev97/test/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/test/test_expiry.py` & `assemblyline-core-4.4.1.dev97/test/test_expiry.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/test/test_plumber.py` & `assemblyline-core-4.4.1.dev97/test/test_plumber.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/test/test_replay.py` & `assemblyline-core-4.4.1.dev97/test/test_replay.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/test/test_scaler.py` & `assemblyline-core-4.4.1.dev97/test/test_scaler.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/test/test_scheduler.py` & `assemblyline-core-4.4.1.dev97/test/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/test/test_simulation.py` & `assemblyline-core-4.4.1.dev97/test/test_simulation.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/test/test_vacuum.py` & `assemblyline-core-4.4.1.dev97/test/test_vacuum.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/test/test_worker_ingest.py` & `assemblyline-core-4.4.1.dev97/test/test_worker_ingest.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev96/test/test_worker_submit.py` & `assemblyline-core-4.4.1.dev97/test/test_worker_submit.py`

 * *Files identical despite different names*

