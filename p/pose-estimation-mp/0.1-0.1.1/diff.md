# Comparing `tmp/pose_estimation_mp-0.1-py3-none-any.whl.zip` & `tmp/pose_estimation_mp-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3320 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat       71 b- defN 23-May-28 03:57 pose_estimation_mp-0.1.data/scripts/pose_estimation_mp
--rw-rw-rw-  2.0 fat     1086 b- defN 23-May-28 04:08 pose_estimation_mp-0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4272 b- defN 23-May-28 04:08 pose_estimation_mp-0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-28 04:08 pose_estimation_mp-0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-May-28 04:08 pose_estimation_mp-0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      539 b- defN 23-May-28 04:08 pose_estimation_mp-0.1.dist-info/RECORD
-6 files, 6061 bytes uncompressed, 2326 bytes compressed:  61.6%
+Zip file size: 3357 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat       71 b- defN 23-May-28 03:57 pose_estimation_mp-0.1.1.data/scripts/pose_estimation_mp
+-rw-rw-rw-  2.0 fat     1086 b- defN 23-May-28 04:25 pose_estimation_mp-0.1.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4486 b- defN 23-May-28 04:25 pose_estimation_mp-0.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-28 04:25 pose_estimation_mp-0.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 23-May-28 04:25 pose_estimation_mp-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      551 b- defN 23-May-28 04:25 pose_estimation_mp-0.1.1.dist-info/RECORD
+6 files, 6287 bytes uncompressed, 2339 bytes compressed:  62.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: pose_estimation_mp-0.1.data/scripts/pose_estimation_mp
+Filename: pose_estimation_mp-0.1.1.data/scripts/pose_estimation_mp
 Comment: 
 
-Filename: pose_estimation_mp-0.1.dist-info/LICENSE
+Filename: pose_estimation_mp-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: pose_estimation_mp-0.1.dist-info/METADATA
+Filename: pose_estimation_mp-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: pose_estimation_mp-0.1.dist-info/WHEEL
+Filename: pose_estimation_mp-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: pose_estimation_mp-0.1.dist-info/top_level.txt
+Filename: pose_estimation_mp-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pose_estimation_mp-0.1.dist-info/RECORD
+Filename: pose_estimation_mp-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pose_estimation_mp-0.1.dist-info/LICENSE` & `pose_estimation_mp-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pose_estimation_mp-0.1.dist-info/METADATA` & `pose_estimation_mp-0.1.1.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pose-estimation-mp
-Version: 0.1
+Version: 0.1.1
 Summary: A Body, Hand, Face tracking utility
 Home-page: https://github.com/REZ3LIET/Pose_Estimations
 Author: Samar Kale
 Author-email: rz.samar.kale@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -31,15 +31,15 @@
 To use this repo use
 ```bash
 git clone https://github.com/REZ3LIET/Pose_Estimations.git
 ```
 
 ## Body_Estimations
 
-<img src="./Results/body_tracking_result.jpg"  width=25% height=25%> <br>
+<img src="https://github.com/REZ3LIET/Pose_Estimations/blob/main/Results/body_tracking_result.jpg"  width=25% height=25%> <br>
 This contains the module [body_estimation_module.py](./Body_Estimation/Codes/body_tracking_module.py) which can be used to track the landmarks on a human body. It is limited to tracking a single person at a time and gives 33 unique landmarks on the body.
 
 ### Usage
 
 To use the [body_estimation_module.py](./Body_Estimation/Codes/body_tracking_module.py) go to `Body_Estimation` directory in terminal
 - For default execution:  
 ```bash
@@ -52,15 +52,15 @@
 - To execute on a video  
 ```bash
 python3 Codes/bodytracking_module.py -v -p Data/Videos/dance.mp4
 ```
 
 ## Hand_Estimation
 
-<img src="./Results/hand_track_result.jpg"  width=25% height=25%> <br>
+<img src="https://github.com/REZ3LIET/Pose_Estimations/blob/main/Results/hand_track_result.jpg"  width=25% height=25%> <br>
 This contains the module [hand_tracking_module.py](./Hand_Estimation/Codes/hand_tracking_module.py) which can be used to track the landmarks on hand(s) and also display them. It can track maximum of 2 handas at an instant.
 
 ### Usage
 
 To use the [hand_tracking_module.py](./Hand_Estimation/Codes/hand_tracking_module.py) go to `Hand_Estimation` directory in terminal
 - For default execution:  
 ```bash
@@ -73,15 +73,15 @@
 - To execute on a video  
 ```bash
 python3 Codes/hand_tracking_module.py -v -p Data/Videos/piano_playing.mp4
 ```
 
 ## Face_Tracking
 
-<img src="./Results/face_track_result.jpg"  width=25% height=25%> <br>
+<img src="https://github.com/REZ3LIET/Pose_Estimations/blob/main/Results/face_track_result.jpg"  width=25% height=25%> <br>
 This contains the module [face_tracking_module.py](./Face_Estimation/Codes/face_tracking_module.py) which can be used to detect and track the face by drawing a bounding box around it. To detect faces at farther range set model type to 1.
 
 ### Usage
 
 To use the [face_tracking_module.py](./Face_Estimation/Codes/face_tracking_module.py) go to `Face_Estimation` directory in terminal
 - For default execution:  
 ```bash
@@ -94,15 +94,15 @@
 - To execute on a video  
 ```bash
 python3 Codes/face_tracking_module.py -v -p Data/Videos/humans_1.mp4
 ```
 
 ## Face_Mesh_Detection
 
-<img src="./Results/face_mesh_result.jpg"  width=25% height=25%> <br>
+<img src="https://github.com/REZ3LIET/Pose_Estimations/blob/main/Results/face_mesh_result.jpg"  width=25% height=25%> <br>
 This contains the module [face_mesh_detection_module.py](./Face_Estimation/Codes/face_mesh_detection_module.py) which can be used to detect and track the face by drawing a mesh on it around it. Max 2 faces can be detected.
 
 ### Usage
 
 To use the [face_mesh_detection_module.py](./Face_Estimation/Codes/face_mesh_detection_module.py) go to `Face_Estimation` directory in terminal
 - For default execution:  
 ```bash
```

## Comparing `pose_estimation_mp-0.1.dist-info/RECORD` & `pose_estimation_mp-0.1.1.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-pose_estimation_mp-0.1.data/scripts/pose_estimation_mp,sha256=CAjPiRBgYX91PPZu6oNXjpNuPIZuiQhnGQAiMEPSbWg,71
-pose_estimation_mp-0.1.dist-info/LICENSE,sha256=KmxvWy0nPYGdv2-FZTEKSXqRgr6zr3l05vzZVLm-ecA,1086
-pose_estimation_mp-0.1.dist-info/METADATA,sha256=9Rf_huec5wQ9GQHteTEa0YPeni9P4LiSTuLoxJgG2Cs,4272
-pose_estimation_mp-0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pose_estimation_mp-0.1.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-pose_estimation_mp-0.1.dist-info/RECORD,,
+pose_estimation_mp-0.1.1.data/scripts/pose_estimation_mp,sha256=CAjPiRBgYX91PPZu6oNXjpNuPIZuiQhnGQAiMEPSbWg,71
+pose_estimation_mp-0.1.1.dist-info/LICENSE,sha256=KmxvWy0nPYGdv2-FZTEKSXqRgr6zr3l05vzZVLm-ecA,1086
+pose_estimation_mp-0.1.1.dist-info/METADATA,sha256=Wt-k1j7vMWXBPE6hZGdL7ggFZoUpM9iTN9wbwkhOVXI,4486
+pose_estimation_mp-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pose_estimation_mp-0.1.1.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+pose_estimation_mp-0.1.1.dist-info/RECORD,,
```

