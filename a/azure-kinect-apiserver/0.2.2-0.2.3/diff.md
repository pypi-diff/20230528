# Comparing `tmp/azure-kinect-apiserver-0.2.2.tar.gz` & `tmp/azure-kinect-apiserver-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/azure-kinect-apiserver/azure-kinect-apiserver/dist/.tmp-kl64orx7/azure-kinect-apiserver-0.2.2.tar", last modified: Sun May 21 19:38:04 2023, max compression
+gzip compressed data, was "/home/runner/work/azure-kinect-apiserver/azure-kinect-apiserver/dist/.tmp-1rqsu5u4/azure-kinect-apiserver-0.2.3.tar", last modified: Sun May 28 14:46:44 2023, max compression
```

## Comparing `azure-kinect-apiserver-0.2.2.tar` & `azure-kinect-apiserver-0.2.3.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/apiserver/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/apiserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14960 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/apiserver/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/apiserver/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/default/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/default/get_status_v1_azure_status_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/default/root_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/default/single_shot_v1_azure_single_shot_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/default/start_recording_v1_azure_start_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/default/stop_recording_v1_azure_stop_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/default/stop_single_shot_v1_azure_single_shot_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/models/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/models/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/models/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17413 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/cmd/analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/cmd/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/cmd/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/cmd/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)    17441 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/cmd/multical.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/common/
--rw-r--r--   0 runner    (1001) docker     (123)    16228 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/common/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/common/DataModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/common/MulticalCamera.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19671 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/common/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/common/point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/decoder/
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/decoder/StateMachine.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/decoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/decoder/aruco.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/decoder/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33269 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/_k4a.py
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/_k4atypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/capture.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/imu_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/_k4abt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/_k4abtTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/body2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/joint2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/_k4arecord.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/_k4arecordTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/datablock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/playback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/record_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/pykinect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/plot3dUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/postProcessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_aruco.py
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_chroma_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_client_restful.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_color_picker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_colored_pc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_decode_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_decode_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_examine_multical_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_filter_chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_filter_chroma_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_multical_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_open3d_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_sync_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_window_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:46:44.000000 azure-kinect-apiserver-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-28 14:46:44.000000 azure-kinect-apiserver-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:46:44.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:46:44.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/apiserver/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/apiserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14960 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/apiserver/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/apiserver/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:46:44.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:46:44.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/restful/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/restful/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:46:44.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/restful/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/restful/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:46:44.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/restful/api/default/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/restful/api/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/restful/api/default/get_status_v1_azure_status_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/restful/api/default/root_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/restful/api/default/single_shot_v1_azure_single_shot_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/restful/api/default/start_recording_v1_azure_start_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/restful/api/default/stop_recording_v1_azure_stop_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/restful/api/default/stop_single_shot_v1_azure_single_shot_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/restful/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/restful/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:46:44.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/restful/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/restful/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/restful/models/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/restful/models/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/restful/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:46:44.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17413 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/cmd/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/cmd/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/cmd/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/cmd/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17441 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/cmd/multical.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:46:44.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/common/
+-rw-r--r--   0 runner    (1001) docker     (123)    16228 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/common/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/common/DataModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/common/MulticalCamera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19671 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/common/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/common/point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:46:44.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/decoder/
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/decoder/StateMachine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/decoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/decoder/aruco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/decoder/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:46:44.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:46:44.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:46:44.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:46:44.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33269 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/_k4a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/_k4atypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/imu_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:46:44.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/_k4abt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/_k4abtTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/body2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/joint2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:46:44.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/_k4arecord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/_k4arecordTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/datablock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/playback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/record_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/pykinect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:46:44.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/plot3dUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/postProcessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-28 14:46:31.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:46:44.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-28 14:46:44.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-05-28 14:46:44.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 14:46:44.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-28 14:46:44.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-28 14:46:44.000000 azure-kinect-apiserver-0.2.3/azure_kinect_apiserver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 14:46:44.000000 azure-kinect-apiserver-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:46:44.000000 azure-kinect-apiserver-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/tests/test_aruco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/tests/test_chroma_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/tests/test_client_restful.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/tests/test_color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/tests/test_colored_pc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/tests/test_decode_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/tests/test_decode_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/tests/test_examine_multical_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/tests/test_filter_chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/tests/test_filter_chroma_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/tests/test_multical_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/tests/test_open3d_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/tests/test_sync_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/tests/test_window_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-28 14:46:30.000000 azure-kinect-apiserver-0.2.3/tests/test_wrapper.py
```

### Comparing `azure-kinect-apiserver-0.2.2/PKG-INFO` & `azure-kinect-apiserver-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: azure-kinect-apiserver
-Version: 0.2.2
+Version: 0.2.3
 Summary: Azure Kinect APIServer
 Author: davidliyutong
 Author-email: davidliyutong@sjtu.edu.cn
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Azure Kinect APIServer
 
 ## Get Started
 
 Clone and change directory into this directory
 
 ```shell
-git clone https://gihub.com/mvig-robotflow/azure-kinect-apiserver.git
+git clone --recursive https://gihub.com/mvig-robotflow/azure-kinect-apiserver.git
 cd azure-kinect-apiserver
 ```
 
 Run setup.py to install the package
 ```shell
 python setup.py install
 ```
@@ -71,17 +71,20 @@
     Navigate to `http://localhost:<api_port>` to view the Swagger UI.
     
 
 - Decode MKV files to synchronized images and depth map sequences:
     ```shell
     python -m azure_kinect_apiserver decode <path_to_recording>
     ```
+
+    > please put your mkvs under <path_to_recording>/kinect
+
     This will create corresponding folders for each camera in the same directory as the recording.
     ```
-    <path_to_recording>
+    <path_to_recording>/kinect
     ├─000673513312
     │  ├─color
     │  └─depth
     ├─000700713312
     │  ├─color
     │  └─depth
     ├─000729313312
```

### Comparing `azure-kinect-apiserver-0.2.2/README.md` & `azure-kinect-apiserver-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Azure Kinect APIServer
 
 ## Get Started
 
 Clone and change directory into this directory
 
 ```shell
-git clone https://gihub.com/mvig-robotflow/azure-kinect-apiserver.git
+git clone --recursive https://gihub.com/mvig-robotflow/azure-kinect-apiserver.git
 cd azure-kinect-apiserver
 ```
 
 Run setup.py to install the package
 ```shell
 python setup.py install
 ```
@@ -62,17 +62,20 @@
     Navigate to `http://localhost:<api_port>` to view the Swagger UI.
     
 
 - Decode MKV files to synchronized images and depth map sequences:
     ```shell
     python -m azure_kinect_apiserver decode <path_to_recording>
     ```
+
+    > please put your mkvs under <path_to_recording>/kinect
+
     This will create corresponding folders for each camera in the same directory as the recording.
     ```
-    <path_to_recording>
+    <path_to_recording>/kinect
     ├─000673513312
     │  ├─color
     │  └─depth
     ├─000700713312
     │  ├─color
     │  └─depth
     ├─000729313312
```

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/__main__.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/__main__.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/apiserver/app.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/apiserver/app.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/apiserver/server.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/apiserver/server.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/default/get_status_v1_azure_status_get.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/restful/api/default/get_status_v1_azure_status_get.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/default/root_get.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/restful/api/default/root_get.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/default/single_shot_v1_azure_single_shot_get.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/restful/api/default/single_shot_v1_azure_single_shot_get.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/default/start_recording_v1_azure_start_post.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/restful/api/default/start_recording_v1_azure_start_post.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/default/stop_recording_v1_azure_stop_post.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/restful/api/default/stop_recording_v1_azure_stop_post.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/default/stop_single_shot_v1_azure_single_shot_delete.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/restful/api/default/stop_single_shot_v1_azure_single_shot_delete.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/client.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/restful/client.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/models/http_validation_error.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/restful/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/models/validation_error.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/restful/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/types.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/client/restful/types.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/cmd/analyze.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/cmd/analyze.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/cmd/calibration.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/cmd/calibration.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/cmd/decode.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/cmd/decode.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,22 +43,23 @@
                                       cam_name: str,
                                       examine_n_frames: int = 600,
                                       maximum_no_detect_count: int = 30,
                                       debug: bool = True) -> Tuple[float, float, Optional[Exception]]:
     # Read metadata and check if all color images are present
     _color_img_path_collection = sorted(glob.glob(os.path.join(tagged_path, cam_name, 'color', '*.jpg')), key=lambda x: int(osp.splitext(osp.basename(x))[0]))
     color_img_meta = pd.read_csv(os.path.join(tagged_path, cam_name, 'meta.csv'))
-    assert len(color_img_meta) == len(_color_img_path_collection), f"len(color_img_meta)={len(color_img_meta)}"
+    assert len(color_img_meta) == len(_color_img_path_collection), f"len(color_img_meta)={len(color_img_meta)} but len(_color_img_path_collection)={len(_color_img_path_collection)}"
     color_img_path_collection = [osp.join(tagged_path, cam_name, 'color', str(filename_no_ext) + '.jpg') for filename_no_ext in color_img_meta['basename']]
     assert all([osp.exists(x) for x in color_img_path_collection]), f"some color images are missing"
 
     decoder = cv2.QRCodeDetector()
     calibration_pairs = []
     last_qrcode_data = None
     no_detect_count = 0
+    logger.info(f"examine {cam_name} for {examine_n_frames} frames, maximum no detect count is {maximum_no_detect_count}")
 
     with tqdm.tqdm(total=len(color_img_path_collection)) as pbar:
         for img_idx, img_path in enumerate(color_img_path_collection):
             # Read color image
             if img_idx >= examine_n_frames or no_detect_count >= maximum_no_detect_count:
                 break
             color_img = cv2.imread(img_path)
@@ -92,14 +93,25 @@
         logger.info(f"found {len(calibration_pairs)} calibration pairs, timestamp offset is {timestamp_offset}")
         return timestamp_offset, datetime.datetime.strptime(calibration_pairs[-1][-1], "%Y-%m-%d_%H:%M:%S.%f").timestamp(), None
 
 
 def mkv_worker(kinect_dir: str):
     files = glob.glob(kinect_dir + "/*.mkv")
     names = [osp.basename(f).split('.')[0] for f in files]
+    metadata = {'recordings': {names[i]: get_mkv_record_meta(file)[0] for i, file in enumerate(files)}}
+    master_camera_candidates = list(filter(lambda x: x[1]['is_master'] is True, metadata['recordings'].items()))
+    if len(master_camera_candidates) == 0:
+        logger.warning("no master camera found, using first camera as master")
+        master_camera = names[0]
+    else:
+        master_camera = master_camera_candidates[0][0]
+    
+    names = [master_camera] + list(filter(lambda x: x != master_camera, names))
+    logger.info(f"master_camera: {names[0]}, all_cameras: {names}", )
+        
     wrappers = [
         mkv_record_wrapper(f) for f in files
     ]
     m = StateMachine(names)
     t = threading.Thread(target=state_machine_save_thread_v1, args=(m, kinect_dir, names))
     t.start()
     with tqdm.tqdm() as pbar:
@@ -113,40 +125,40 @@
                     if err is not None:
                         raise err
                 except StopIteration:
                     num_closed += 1
                     continue
 
             frames = {k: frame_futures[k].result() for k in names if frame_futures[k] is not None}
+            # print({k: v['color_dev_ts_usec'] if v is not None else None for k, v in frames.items()})
 
             for stream_id, frame in frames.items():
                 if frame is not None:
                     m.push(stream_id, frame)
-                    pbar.set_description(f"pressure: {len(m.frame_buffer[names[1]])}")
+                    pbar.set_description(f"pressure: {len(m.frame_buffer[names[-1]])}")
                     pbar.update(1)
-
         m.close()
         t.join()
 
     for i, file in enumerate(files):
         with open(osp.join(kinect_dir, names[i], f"calibration.kinect.json"), "w") as f:
             json.dump(get_mkv_record_calibration(file)[0], f, indent=4, sort_keys=True)
 
-    metadata = {'recordings': {names[i]: get_mkv_record_meta(file)[0] for i, file in enumerate(files)}}
-    master_camera = list(filter(lambda x: x[1]['is_master'] is True, metadata['recordings'].items()))[0][0]
-    ts, ts_action_start, err = get_timestamp_offset_from_decoded(tagged_path=kinect_dir, cam_name=master_camera, debug=False)
-    ret: Optional[Exception] = None
-    if err is not None:
-        logging.error(str(err))
-        ret = Exception("failed to get timestamp offset")
-        metadata['system_timestamp_offset'] = 0
-        metadata['system_action_start_timestamp'] = 0
-    else:
-        metadata['system_timestamp_offset'] = ts
-        metadata['system_action_start_timestamp'] = ts_action_start
+    ret: Optional[Exception] = Exception("failed to get timestamp offset")
+    metadata['system_timestamp_offset'] = 0
+    metadata['system_action_start_timestamp'] = 0
+    for cam_name in names:
+        ts, ts_action_start, err = get_timestamp_offset_from_decoded(tagged_path=kinect_dir, cam_name=cam_name, debug=False)
+        ret= None
+        if err is not None:
+            logging.error(str(err))
+            continue
+        else:
+            metadata['system_timestamp_offset'] = ts
+            metadata['system_action_start_timestamp'] = ts_action_start
 
     with open(osp.join(kinect_dir, "meta.json"), "w") as f:
         json.dump(metadata, f, indent=4, sort_keys=True)
 
     return ret
```

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/cmd/multical.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/cmd/multical.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/common/Config.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/common/Config.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/common/DataModel.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/common/DataModel.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/common/MulticalCamera.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/common/MulticalCamera.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/common/functional.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/common/functional.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/common/point.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/common/point.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/decoder/StateMachine.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/decoder/StateMachine.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,18 @@
     def try_pop(self):
         self.mutex.acquire()
         if len(self.frame_buffer[self.master_id]) == 0:
             self.mutex.release()
             return None
         else:
             master_frame = self.frame_buffer[self.master_id].popleft()
+            if len(self.subordinate_ids) == 0:
+                self.mutex.release()
+                return {self.master_id: master_frame}
+
             while len(self.frame_buffer[self.master_id]) > 0:
                 if any([abs(self.frame_buffer[subordinate_id][0]['color_dev_ts_usec'] - master_frame['color_dev_ts_usec']) for subordinate_id in self.subordinate_ids]):
                     break
                 else:
                     master_frame = self.frame_buffer[self.master_id].popleft()
                     continue
 
@@ -87,27 +91,28 @@
                 while len(self.frame_buffer[subordinate_id]) > 0:
                     subordinate_frame = self.frame_buffer[subordinate_id].popleft()
 
                     if abs(subordinate_frame['color_dev_ts_usec'] - master_frame['color_dev_ts_usec']) < self.criteria_sec * 1e6:
                         subordinate_frames[subordinate_id] = subordinate_frame  # save frame
                         break
                     elif subordinate_frame['color_dev_ts_usec'] > master_frame['color_dev_ts_usec']:
+                        # print(subordinate_id, abs(subordinate_frame['color_dev_ts_usec'] - master_frame['color_dev_ts_usec']))
+                        self.frame_buffer[subordinate_id].appendleft(subordinate_frame)
                         flag_master_not_synced = True
                         break
                     else:
+                        # print(subordinate_id, abs(subordinate_frame['color_dev_ts_usec'] - master_frame['color_dev_ts_usec']))
                         continue
 
                 if flag_master_not_synced:
                     break
 
             if flag_master_not_synced or any([x is None for x in subordinate_frames.values()]):
-                for stream_id, frame in subordinate_frames.items():
-                    if frame is not None:
-                        self.frame_buffer[stream_id].appendleft(frame)
                 self.mutex.release()
+                # print(flag_master_not_synced, [x is None for x in subordinate_frames.values()])
                 return None
             else:
                 self.mutex.release()
                 return {self.master_id: master_frame, **subordinate_frames}
 
 
 def state_machine_save_thread_v1(m: StateMachine, data_dir: str, camera_names: List[str]):
@@ -123,15 +128,17 @@
             os.makedirs(osp.join(data_dir, stream_id, 'depth'), exist_ok=True)
 
     meta_handles = {s: open(osp.join(data_dir, s, 'meta.csv'), 'w') for s in camera_names}
     for stream_id in camera_names:
         meta_handles[stream_id].write('basename,index,color_dev_ts_usec,depth_dev_ts_usec,color_sys_ts_nsec,depth_sys_ts_nsec\n')
 
     pool = ThreadPoolExecutor(max_workers=4)
-    while not m.closed:
+    while True:
+        if m.closed and not m.ready:
+            break
         if m.ready:
             frames = m.try_pop()
             if frames is not None:
                 for stream_id, frame in frames.items():
                     color_path = osp.join(data_dir, stream_id, 'color', f'{frame["color_dev_ts_usec"]}.jpg')
                     depth_path = osp.join(data_dir, stream_id, 'depth', f'{frame["color_dev_ts_usec"]}.png')
                     pool.submit(cv2.imwrite, color_path, frame['color'])
@@ -139,8 +146,11 @@
                     meta_handles[stream_id].write(
                         f'{frame["color_dev_ts_usec"]},{frame["index"]},{frame["color_dev_ts_usec"]},{frame["depth_dev_ts_usec"]},{frame["color_sys_ts_nsec"]},{frame["depth_sys_ts_nsec"]}\n'
                     )
                     # cv2.imwrite(osp.join(data_dir, stream_id, 'color', f'{frame["color_dev_ts_usec"]}.jpg'), frame['color'])
                     # cv2.imwrite(osp.join(data_dir, stream_id, 'depth', f'{frame["color_dev_ts_usec"]}.png'), frame['depth'])
         else:
             time.sleep(2)  # Must be an enough long duration
+
+    for stream_id, handle in meta_handles.items():
+        handle.close()
     pool.shutdown(wait=True)
```

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/decoder/aruco.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/decoder/aruco.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/decoder/wrapper.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/decoder/wrapper.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/_k4a.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/_k4a.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/_k4atypes.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/_k4atypes.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/calibration.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/calibration.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/capture.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/capture.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/configuration.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/configuration.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/device.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/device.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/image.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/image.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/imu_sample.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/imu_sample.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/transformation.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/transformation.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/_k4abt.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/_k4abt.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/_k4abtTypes.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/_k4abtTypes.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/body.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/body.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/body2d.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/body2d.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/frame.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/frame.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/joint.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/joint.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/joint2d.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/joint2d.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/tracker.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/tracker.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/_k4arecord.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/_k4arecord.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/_k4arecordTypes.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/_k4arecordTypes.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/datablock.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/datablock.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/playback.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/playback.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/record.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/record.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/record_configuration.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/record_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/pykinect.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/pykinect.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/plot3dUtils.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/plot3dUtils.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/postProcessing.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/postProcessing.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/utils.py` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/utils.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver.egg-info/PKG-INFO` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: azure-kinect-apiserver
-Version: 0.2.2
+Version: 0.2.3
 Summary: Azure Kinect APIServer
 Author: davidliyutong
 Author-email: davidliyutong@sjtu.edu.cn
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Azure Kinect APIServer
 
 ## Get Started
 
 Clone and change directory into this directory
 
 ```shell
-git clone https://gihub.com/mvig-robotflow/azure-kinect-apiserver.git
+git clone --recursive https://gihub.com/mvig-robotflow/azure-kinect-apiserver.git
 cd azure-kinect-apiserver
 ```
 
 Run setup.py to install the package
 ```shell
 python setup.py install
 ```
@@ -71,17 +71,20 @@
     Navigate to `http://localhost:<api_port>` to view the Swagger UI.
     
 
 - Decode MKV files to synchronized images and depth map sequences:
     ```shell
     python -m azure_kinect_apiserver decode <path_to_recording>
     ```
+
+    > please put your mkvs under <path_to_recording>/kinect
+
     This will create corresponding folders for each camera in the same directory as the recording.
     ```
-    <path_to_recording>
+    <path_to_recording>/kinect
     ├─000673513312
     │  ├─color
     │  └─depth
     ├─000700713312
     │  ├─color
     │  └─depth
     ├─000729313312
```

### Comparing `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver.egg-info/SOURCES.txt` & `azure-kinect-apiserver-0.2.3/azure_kinect_apiserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/setup.py` & `azure-kinect-apiserver-0.2.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages
 
 requires = open("requirements.txt", "r").readlines() if os.path.exists("requirements.txt") else open("./azure_kinect_apiserver.egg-info/requires.txt", "r").readlines()
 print("#-------------------    ", str(os.listdir("./")))
 setup(
     name="azure-kinect-apiserver",
-    version="0.2.2",
+    version="0.2.3",
     author="davidliyutong",
     author_email="davidliyutong@sjtu.edu.cn",
     description="Azure Kinect APIServer",
     packages=find_packages() + ["azure_kinect_apiserver.thirdparty.pyKinectAzure." + pkg for pkg in find_packages('azure_kinect_apiserver/thirdparty/pyKinectAzure')],
     python_requires=">=3.7",
     install_requires=requires,
     long_description=open('README.md', encoding='utf-8').read(),
```

### Comparing `azure-kinect-apiserver-0.2.2/tests/test_aruco.py` & `azure-kinect-apiserver-0.2.3/tests/test_aruco.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/tests/test_chroma_filter.py` & `azure-kinect-apiserver-0.2.3/tests/test_chroma_filter.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/tests/test_colored_pc.py` & `azure-kinect-apiserver-0.2.3/tests/test_colored_pc.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/tests/test_decode_file.py` & `azure-kinect-apiserver-0.2.3/tests/test_decode_file.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/tests/test_filter_chroma.py` & `azure-kinect-apiserver-0.2.3/tests/test_filter_chroma.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/tests/test_filter_chroma_gui.py` & `azure-kinect-apiserver-0.2.3/tests/test_filter_chroma_gui.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/tests/test_open3d_reader.py` & `azure-kinect-apiserver-0.2.3/tests/test_open3d_reader.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/tests/test_window_gui.py` & `azure-kinect-apiserver-0.2.3/tests/test_window_gui.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.2/tests/test_wrapper.py` & `azure-kinect-apiserver-0.2.3/tests/test_wrapper.py`

 * *Files identical despite different names*

