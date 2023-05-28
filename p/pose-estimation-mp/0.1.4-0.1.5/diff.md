# Comparing `tmp/pose_estimation_mp-0.1.4-py3-none-any.whl.zip` & `tmp/pose_estimation_mp-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 9807 bytes, number of entries: 13
+Zip file size: 9992 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-28 04:45 Body_Tracking/__init__.py
 -rw-rw-rw-  2.0 fat     3309 b- defN 23-May-27 14:42 Body_Tracking/body_tracking_module.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-28 04:45 Face_Tracking/__init__.py
 -rw-rw-rw-  2.0 fat     3415 b- defN 23-May-27 14:49 Face_Tracking/face_mesh_detection_module.py
 -rw-rw-rw-  2.0 fat     3953 b- defN 23-May-27 14:49 Face_Tracking/face_tracking_module.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-28 04:46 Hand_Tacking/__init__.py
 -rw-rw-rw-  2.0 fat     3743 b- defN 23-May-27 14:44 Hand_Tacking/hand_tracking_module.py
--rw-rw-rw-  2.0 fat       71 b- defN 23-May-28 03:57 pose_estimation_mp-0.1.4.data/scripts/pose_estimation_mp
--rw-rw-rw-  2.0 fat     1086 b- defN 23-May-28 05:11 pose_estimation_mp-0.1.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4486 b- defN 23-May-28 05:11 pose_estimation_mp-0.1.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-28 05:11 pose_estimation_mp-0.1.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       41 b- defN 23-May-28 05:11 pose_estimation_mp-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1169 b- defN 23-May-28 05:11 pose_estimation_mp-0.1.4.dist-info/RECORD
-13 files, 21365 bytes uncompressed, 7803 bytes compressed:  63.5%
+-rw-rw-rw-  2.0 fat       71 b- defN 23-May-28 03:57 pose_estimation_mp-0.1.5.data/scripts/pose_estimation_mp
+-rw-rw-rw-  2.0 fat     1086 b- defN 23-May-28 05:57 pose_estimation_mp-0.1.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     5603 b- defN 23-May-28 05:57 pose_estimation_mp-0.1.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-28 05:57 pose_estimation_mp-0.1.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       41 b- defN 23-May-28 05:57 pose_estimation_mp-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1169 b- defN 23-May-28 05:57 pose_estimation_mp-0.1.5.dist-info/RECORD
+13 files, 22482 bytes uncompressed, 7988 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: Hand_Tacking/__init__.py
 Comment: 
 
 Filename: Hand_Tacking/hand_tracking_module.py
 Comment: 
 
-Filename: pose_estimation_mp-0.1.4.data/scripts/pose_estimation_mp
+Filename: pose_estimation_mp-0.1.5.data/scripts/pose_estimation_mp
 Comment: 
 
-Filename: pose_estimation_mp-0.1.4.dist-info/LICENSE
+Filename: pose_estimation_mp-0.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: pose_estimation_mp-0.1.4.dist-info/METADATA
+Filename: pose_estimation_mp-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: pose_estimation_mp-0.1.4.dist-info/WHEEL
+Filename: pose_estimation_mp-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: pose_estimation_mp-0.1.4.dist-info/top_level.txt
+Filename: pose_estimation_mp-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: pose_estimation_mp-0.1.4.dist-info/RECORD
+Filename: pose_estimation_mp-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pose_estimation_mp-0.1.4.dist-info/LICENSE` & `pose_estimation_mp-0.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pose_estimation_mp-0.1.4.dist-info/METADATA` & `pose_estimation_mp-0.1.5.dist-info/METADATA`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pose-estimation-mp
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Body, Hand, Face tracking utility
 Home-page: https://github.com/REZ3LIET/Pose_Estimations
 Author: Samar Kale
 Author-email: rz.samar.kale@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -28,93 +28,133 @@
 
 ## Installation
 
 To use this repo use
 ```bash
 git clone https://github.com/REZ3LIET/Pose_Estimations.git
 ```
+or
+```bash
+pip3 install pose-estimation-mp
+```
 
 ## Body_Estimations
 
 <img src="https://github.com/REZ3LIET/Pose_Estimations/blob/main/Results/body_tracking_result.jpg"  width=25% height=25%> <br>
-This contains the module [body_estimation_module.py](./Body_Estimation/Codes/body_tracking_module.py) which can be used to track the landmarks on a human body. It is limited to tracking a single person at a time and gives 33 unique landmarks on the body.
+This contains the module [body_estimation_module.py](./Body_Tracking/body_tracking_module.py) which can be used to track the landmarks on a human body. It is limited to tracking a single person at a time and gives 33 unique landmarks on the body.
 
 ### Usage
 
-To use the [body_estimation_module.py](./Body_Estimation/Codes/body_tracking_module.py) go to `Body_Estimation` directory in terminal
+To use [body_estimation_module.py](./Body_Tracking/body_tracking_module.py) in your code simply import one of the following ways:
+```bash
+import Body_Tracking
+from Body_Tracking import body_tracking_module as btm
+from Body_Tracking.body_tracking_module import BodyPoseDetect
+```
+
+### Example
+
+To use the [body_estimation_module.py](./Body_Tracking/body_tracking_module.py) go to `Body_Tracking` directory in terminal
 - For default execution:  
 ```bash
-python3 Codes/bodytracking_module.py
+python3 bodytracking_module.py
 ```
 - To execute with an image  
 ```bash
-python3 Codes/bodytracking_module.py -p Data/Images/handstand.jpg
+python3 bodytracking_module.py -p Data/Images/handstand.jpg
 ```
 - To execute on a video  
 ```bash
-python3 Codes/bodytracking_module.py -v -p Data/Videos/dance.mp4
+python3 bodytracking_module.py -v -p Data/Videos/dance.mp4
 ```
 
 ## Hand_Estimation
 
 <img src="https://github.com/REZ3LIET/Pose_Estimations/blob/main/Results/hand_track_result.jpg"  width=25% height=25%> <br>
-This contains the module [hand_tracking_module.py](./Hand_Estimation/Codes/hand_tracking_module.py) which can be used to track the landmarks on hand(s) and also display them. It can track maximum of 2 handas at an instant.
+This contains the module [hand_tracking_module.py](./Hand_Tacking/hand_tracking_module.py) which can be used to track the landmarks on hand(s) and also display them. It can track maximum of 2 handas at an instant.
 
 ### Usage
 
-To use the [hand_tracking_module.py](./Hand_Estimation/Codes/hand_tracking_module.py) go to `Hand_Estimation` directory in terminal
+To use [hand_tracking_module.py](./Hand_Tacking/hand_tracking_module.py) in your code simply import one of the following ways:
+```bash
+import Hand_Tacking
+from Hand_Tacking import hand_tracking_module as htm
+from Hand_Tacking.hand_tracking_module import HandPoseDetect
+```
+
+### Example
+
+To use the [hand_tracking_module.py](./Hand_Tacking/hand_tracking_module.py) go to `Hand_Tacking` directory in terminal
 - For default execution:  
 ```bash
-python3 Codes/hand_tracking_module.py
+python3 hand_tracking_module.py
 ```
 - To execute with an image  
 ```bash
-python3 Codes/hand_tracking_module.py -p Data/Images/covered_face.jpg
+python3 hand_tracking_module.py -p Data/Images/covered_face.jpg
 ```
 - To execute on a video  
 ```bash
-python3 Codes/hand_tracking_module.py -v -p Data/Videos/piano_playing.mp4
+python3 hand_tracking_module.py -v -p Data/Videos/piano_playing.mp4
 ```
 
 ## Face_Tracking
 
 <img src="https://github.com/REZ3LIET/Pose_Estimations/blob/main/Results/face_track_result.jpg"  width=25% height=25%> <br>
-This contains the module [face_tracking_module.py](./Face_Estimation/Codes/face_tracking_module.py) which can be used to detect and track the face by drawing a bounding box around it. To detect faces at farther range set model type to 1.
+This contains the module [face_tracking_module.py](./Face_Tracking/face_tracking_module.py) which can be used to detect and track the face by drawing a bounding box around it. To detect faces at farther range set model type to 1.
 
 ### Usage
 
-To use the [face_tracking_module.py](./Face_Estimation/Codes/face_tracking_module.py) go to `Face_Estimation` directory in terminal
+To use [face_tracking_module.py](./Face_Tracking/face_tracking_module.py) in your code simply import one of the following ways:
+```bash
+import Face_Tracking
+from Face_Tracking import face_tracking_module as ftm
+from Face_Tracking.face_tracking_module import FaceTrack
+```
+
+### Example
+
+To use the [face_tracking_module.py](./Face_Tracking/face_tracking_module.py) go to `Face_Tracking` directory in terminal
 - For default execution:  
 ```bash
-python3 Codes/face_tracking_module.py
+python3 face_tracking_module.py
 ```
 - To execute with an image  
 ```bash
-python3 Codes/face_tracking_module.py -p Data/Images/human_3.jpg
+python3 face_tracking_module.py -p Data/Images/human_3.jpg
 ```
 - To execute on a video  
 ```bash
-python3 Codes/face_tracking_module.py -v -p Data/Videos/humans_1.mp4
+python3 face_tracking_module.py -v -p Data/Videos/humans_1.mp4
 ```
 
 ## Face_Mesh_Detection
 
 <img src="https://github.com/REZ3LIET/Pose_Estimations/blob/main/Results/face_mesh_result.jpg"  width=25% height=25%> <br>
-This contains the module [face_mesh_detection_module.py](./Face_Estimation/Codes/face_mesh_detection_module.py) which can be used to detect and track the face by drawing a mesh on it around it. Max 2 faces can be detected.
+This contains the module [face_mesh_detection_module.py](./Face_Tracking/face_mesh_detection_module.py) which can be used to detect and track the face by drawing a mesh on it around it. Max 2 faces can be detected.
 
 ### Usage
 
-To use the [face_mesh_detection_module.py](./Face_Estimation/Codes/face_mesh_detection_module.py) go to `Face_Estimation` directory in terminal
+To use [face_mesh_detection_module.py](./Face_Tracking/face_mesh_detection_module.py) in your code simply import one of the following ways:
+```bash
+import Face_Tracking
+from Face_Tracking import face_mesh_detection_module as ftm
+from Face_Tracking.face_mesh_detection_module import FaceDetect
+```
+
+### Example
+
+To use the [face_mesh_detection_module.py](./Face_Tracking/face_mesh_detection_module.py) go to `Face_Tracking` directory in terminal
 - For default execution:  
 ```bash
-python3 Codes/face_mesh_detection_module.py
+python3 face_mesh_detection_module.py
 ```
 - To execute with an image  
 ```bash
-python3 Codes/face_mesh_detection_module.py -p Data/Images/human_2.jpg
+python3 face_mesh_detection_module.py -p Data/Images/human_2.jpg
 ```
 - To execute on a video  
 ```bash
-python3 Codes/face_mesh_detection_module.py -v -p Data/Videos/humans_2.mp4
+python3 face_mesh_detection_module.py -v -p Data/Videos/humans_2.mp4
 ```
```

## Comparing `pose_estimation_mp-0.1.4.dist-info/RECORD` & `pose_estimation_mp-0.1.5.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Body_Tracking/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 Body_Tracking/body_tracking_module.py,sha256=2VkmzFJ7KCWLFH3cspCLP5D310cs3fcesI1gOv4t_Ro,3309
 Face_Tracking/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 Face_Tracking/face_mesh_detection_module.py,sha256=Jei1BRCjB85tsJX0pg1g-qgB6WQrU7QnUepHzvAI5r0,3415
 Face_Tracking/face_tracking_module.py,sha256=dY-ZYXZiVFWgIPAqo_kjUXl6W0VPKDjL8VZKXN-rw8s,3953
 Hand_Tacking/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 Hand_Tacking/hand_tracking_module.py,sha256=WNK1gvzIDfrcslN1YAj3uOegXIPjChOkKn4yu-nGuvY,3743
-pose_estimation_mp-0.1.4.data/scripts/pose_estimation_mp,sha256=CAjPiRBgYX91PPZu6oNXjpNuPIZuiQhnGQAiMEPSbWg,71
-pose_estimation_mp-0.1.4.dist-info/LICENSE,sha256=KmxvWy0nPYGdv2-FZTEKSXqRgr6zr3l05vzZVLm-ecA,1086
-pose_estimation_mp-0.1.4.dist-info/METADATA,sha256=Ljb0h1Ivd8iLIMw-T7hLWNCBi7PVugFnK6lnEMlBIyw,4486
-pose_estimation_mp-0.1.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pose_estimation_mp-0.1.4.dist-info/top_level.txt,sha256=V7-v4FeS13VKt3XmzpPtqJMyVtlTG-HKlw41KK9fm-c,41
-pose_estimation_mp-0.1.4.dist-info/RECORD,,
+pose_estimation_mp-0.1.5.data/scripts/pose_estimation_mp,sha256=CAjPiRBgYX91PPZu6oNXjpNuPIZuiQhnGQAiMEPSbWg,71
+pose_estimation_mp-0.1.5.dist-info/LICENSE,sha256=KmxvWy0nPYGdv2-FZTEKSXqRgr6zr3l05vzZVLm-ecA,1086
+pose_estimation_mp-0.1.5.dist-info/METADATA,sha256=aAzmgy_YyjwqvdX-bBu0zpe0tt3ed4idBd1jSY6fPX0,5603
+pose_estimation_mp-0.1.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pose_estimation_mp-0.1.5.dist-info/top_level.txt,sha256=V7-v4FeS13VKt3XmzpPtqJMyVtlTG-HKlw41KK9fm-c,41
+pose_estimation_mp-0.1.5.dist-info/RECORD,,
```

