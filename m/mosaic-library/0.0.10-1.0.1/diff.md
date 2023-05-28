# Comparing `tmp/mosaic-library-0.0.10.tar.gz` & `tmp/mosaic-library-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaic-library-0.0.10.tar", last modified: Thu Jun 16 13:45:57 2022, max compression
+gzip compressed data, was "mosaic-library-1.0.1.tar", last modified: Sun May 28 16:23:50 2023, max compression
```

## Comparing `mosaic-library-0.0.10.tar` & `mosaic-library-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxrwxr-x   0 fft       (1000) fft       (1000)        0 2022-06-16 13:45:57.283186 mosaic-library-0.0.10/
--rw-rw-r--   0 fft       (1000) fft       (1000)       82 2022-06-16 13:45:57.283186 mosaic-library-0.0.10/PKG-INFO
-drwxrwxr-x   0 fft       (1000) fft       (1000)        0 2022-06-16 13:45:57.283186 mosaic-library-0.0.10/mosaic_library.egg-info/
--rw-rw-r--   0 fft       (1000) fft       (1000)       82 2022-06-16 13:45:56.000000 mosaic-library-0.0.10/mosaic_library.egg-info/PKG-INFO
--rw-rw-r--   0 fft       (1000) fft       (1000)      429 2022-06-16 13:45:57.000000 mosaic-library-0.0.10/mosaic_library.egg-info/SOURCES.txt
--rw-rw-r--   0 fft       (1000) fft       (1000)        1 2022-06-16 13:45:56.000000 mosaic-library-0.0.10/mosaic_library.egg-info/dependency_links.txt
--rw-rw-r--   0 fft       (1000) fft       (1000)       53 2022-06-16 13:45:56.000000 mosaic-library-0.0.10/mosaic_library.egg-info/entry_points.txt
--rw-rw-r--   0 fft       (1000) fft       (1000)       79 2022-06-16 13:45:56.000000 mosaic-library-0.0.10/mosaic_library.egg-info/requires.txt
--rw-rw-r--   0 fft       (1000) fft       (1000)       11 2022-06-16 13:45:57.000000 mosaic-library-0.0.10/mosaic_library.egg-info/top_level.txt
-drwxrwxr-x   0 fft       (1000) fft       (1000)        0 2022-06-16 13:45:57.283186 mosaic-library-0.0.10/mosaicking/
--rw-rw-r--   0 fft       (1000) fft       (1000)        0 2021-06-12 17:59:45.000000 mosaic-library-0.0.10/mosaicking/__init__.py
--rw-rw-r--   0 fft       (1000) fft       (1000)     2221 2021-06-20 14:52:59.000000 mosaic-library-0.0.10/mosaicking/calibration.py
--rw-rw-r--   0 fft       (1000) fft       (1000)    22538 2022-03-13 15:24:07.000000 mosaic-library-0.0.10/mosaicking/mosaic.py
--rw-rw-r--   0 fft       (1000) fft       (1000)     2966 2022-06-16 13:43:42.000000 mosaic-library-0.0.10/mosaicking/preprocessing.py
--rw-rw-r--   0 fft       (1000) fft       (1000)    12901 2022-03-13 15:24:07.000000 mosaic-library-0.0.10/mosaicking/registration.py
--rw-rw-r--   0 fft       (1000) fft       (1000)    15664 2022-03-13 15:24:07.000000 mosaic-library-0.0.10/mosaicking/transformations.py
--rw-rw-r--   0 fft       (1000) fft       (1000)    11228 2022-03-13 15:24:07.000000 mosaic-library-0.0.10/mosaicking/utils.py
--rw-rw-r--   0 fft       (1000) fft       (1000)       89 2021-06-18 15:24:15.000000 mosaic-library-0.0.10/pyproject.toml
--rw-rw-r--   0 fft       (1000) fft       (1000)      376 2022-06-16 13:45:57.283186 mosaic-library-0.0.10/setup.cfg
+drwxrwxr-x   0 fft       (1000) fft       (1000)        0 2023-05-28 16:23:50.971173 mosaic-library-1.0.1/
+-rw-rw-r--   0 fft       (1000) fft       (1000)     1083 2023-05-28 16:07:39.000000 mosaic-library-1.0.1/LICENSE
+-rw-rw-r--   0 fft       (1000) fft       (1000)    18654 2023-05-28 16:23:50.971173 mosaic-library-1.0.1/PKG-INFO
+-rw-rw-r--   0 fft       (1000) fft       (1000)    18072 2023-05-28 16:07:39.000000 mosaic-library-1.0.1/README.MD
+drwxrwxr-x   0 fft       (1000) fft       (1000)        0 2023-05-28 16:23:50.971173 mosaic-library-1.0.1/mosaic_library.egg-info/
+-rw-rw-r--   0 fft       (1000) fft       (1000)    18654 2023-05-28 16:23:50.000000 mosaic-library-1.0.1/mosaic_library.egg-info/PKG-INFO
+-rw-rw-r--   0 fft       (1000) fft       (1000)      475 2023-05-28 16:23:50.000000 mosaic-library-1.0.1/mosaic_library.egg-info/SOURCES.txt
+-rw-rw-r--   0 fft       (1000) fft       (1000)        1 2023-05-28 16:23:50.000000 mosaic-library-1.0.1/mosaic_library.egg-info/dependency_links.txt
+-rw-rw-r--   0 fft       (1000) fft       (1000)       98 2023-05-28 16:23:50.000000 mosaic-library-1.0.1/mosaic_library.egg-info/entry_points.txt
+-rw-rw-r--   0 fft       (1000) fft       (1000)       86 2023-05-28 16:23:50.000000 mosaic-library-1.0.1/mosaic_library.egg-info/requires.txt
+-rw-rw-r--   0 fft       (1000) fft       (1000)       11 2023-05-28 16:23:50.000000 mosaic-library-1.0.1/mosaic_library.egg-info/top_level.txt
+drwxrwxr-x   0 fft       (1000) fft       (1000)        0 2023-05-28 16:23:50.971173 mosaic-library-1.0.1/mosaicking/
+-rw-rw-r--   0 fft       (1000) fft       (1000)        0 2023-05-19 14:29:07.000000 mosaic-library-1.0.1/mosaicking/__init__.py
+-rw-rw-r--   0 fft       (1000) fft       (1000)     5067 2023-05-28 16:07:39.000000 mosaic-library-1.0.1/mosaicking/calibration.py
+-rw-rw-r--   0 fft       (1000) fft       (1000)    22678 2023-05-28 16:07:39.000000 mosaic-library-1.0.1/mosaicking/mosaic.py
+-rw-rw-r--   0 fft       (1000) fft       (1000)     6135 2023-05-28 16:07:39.000000 mosaic-library-1.0.1/mosaicking/preprocessing.py
+-rw-rw-r--   0 fft       (1000) fft       (1000)     2156 2023-05-28 16:07:39.000000 mosaic-library-1.0.1/mosaicking/registration.py
+-rw-rw-r--   0 fft       (1000) fft       (1000)    16557 2023-05-28 16:07:39.000000 mosaic-library-1.0.1/mosaicking/transformations.py
+-rw-rw-r--   0 fft       (1000) fft       (1000)    11706 2023-05-28 16:07:39.000000 mosaic-library-1.0.1/mosaicking/utils.py
+-rw-rw-r--   0 fft       (1000) fft       (1000)      656 2023-05-28 16:21:44.000000 mosaic-library-1.0.1/pyproject.toml
+-rw-rw-r--   0 fft       (1000) fft       (1000)      427 2023-05-28 16:23:50.971173 mosaic-library-1.0.1/setup.cfg
+drwxrwxr-x   0 fft       (1000) fft       (1000)        0 2023-05-28 16:23:50.971173 mosaic-library-1.0.1/tests/
+-rw-rw-r--   0 fft       (1000) fft       (1000)     2727 2023-05-28 16:07:39.000000 mosaic-library-1.0.1/tests/test_preprocessing.py
```

### Comparing `mosaic-library-0.0.10/mosaicking/mosaic.py` & `mosaic-library-1.0.1/mosaicking/mosaic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import cv2
 from cv2 import fisheye
-import argparse
 from pathlib import Path
 import sys
 import numpy as np
 from scipy.interpolate import interp1d
 from scipy.spatial.transform import Rotation
+
+import mosaicking.transformations
 from mosaicking import preprocessing, utils, transformations, registration
 from itertools import chain
 import yaml
 
 
 def main():
     args = utils.parse_args()
@@ -137,19 +138,19 @@
             if args.fisheye:
                 img = fisheye.undistortImage(img, K, distCoeff)
                 image_mask = fisheye.undistortImage(255 * np.ones_like(img), K, distCoeff)[:, :, 0]
             else:
                 img = cv2.undistort(img, K, distCoeff)
                 image_mask = cv2.undistort(255 * np.ones_like(img), K, distCoeff)[:, :, 0]
             # Then apply color correction if specified
-            img = preprocessing.fix_color(img) if args.fix_color else img
+            img = preprocessing.imadjust(img) if args.imadjust else img
             # Then apply contrast balancing if specified
-            img = preprocessing.fix_contrast(img) if args.fix_contrast else img
+            img = preprocessing.equalize_color(img) if args.equalize_color else img
             # Then apply light balancing if specified
-            img = preprocessing.fix_light(img) if args.fix_light else img
+            img = preprocessing.equalize_luminance(img) if args.equalize_luminance else img
             # Enhance detail
             img = preprocessing.enhance_detail(img)
 
             # DEBUGGING: DISPLAY THE PREPROCESSING
             if args.show_preprocessing:
                 fontsize = 3
                 border = np.zeros((og.shape[0], 20, 3), dtype=np.uint8)
@@ -276,16 +277,16 @@
                 #       "Translation:\n\t\tX: {:.2f}\tY: {:.2f}\tZ: {:.2f}".format(*pose_euler, *pose_t.squeeze()))
                 # Get the new affine alignment and bounds
                 # TODO Sometimes homography wraps the image around, apparently because of vanishing point and the horizon.
                 #  I cannot estimate the vanishing point easily, so in this iteration we have to live with this problem.
                 #  A way to address this is to mask out the components of the image that do not intersect with the ground plane.
                 #  We would need to estimate the ground plane, and compute the intersection of camera rays with this plane.
                 #  If they intersect, then the pixel that the ray goes through needs to be preserved, others are discarded.
-                A, xbounds, ybounds = registration.get_alignment(src_pts, img.shape[:2], dst_pts, mosaic_img.shape[:2],
-                                                                 homography=args.homography, gradient=args.gradientclip)
+                A, xbounds, ybounds = mosaicking.transformations.get_alignment(src_pts, img.shape[:2], dst_pts, mosaic_img.shape[:2],
+                                                                               homography=args.homography, gradient=args.gradientclip)
                 # Get the C of the top left corner of the warped image to be inserted
                 t = [-min(xbounds), -min(ybounds)]
 
                 # TODO: Handling the tiles needs an overhaul.
                 #  I would like to track the coordinates of the mosaic, and assign tiles to grid on this coordinate system.
                 #  The warped image should not need to be padded. Instead the warped image pixels should be assigned a
                 #  coordinated within the mosaic coordinate system. Then, the tiles that share coordinates from the warped
@@ -364,30 +365,31 @@
 
                 key = cv2.waitKey(1)
                 counter = counter + 1
                 if args.save_freq > 0 and counter % args.save_freq == 0:
                     counter = 0
                     fpath = output_path.joinpath("current_mosaic.png")
                     cv2.imwrite(str(fpath), mosaic_img)
-                if key == ord("q"):
-                    sys.stdout.write("Quitting.\n")
-                    break
+                if key == ord("q") or key & 0xff == 27:
+                    raise KeyboardInterrupt
     except Exception as err:
         # Some strange error has occurred, write out to stderr, cleanup and rethrow the error
         sys.stderr.write("\nPipeline failed at frame {}\n".format(reader.get(cv2.CAP_PROP_POS_FRAMES) + 1))
         cv2.destroyAllWindows()
         del reader
         if args.demo:
             writer.release()
         fpath = output_path.joinpath("error_frame.png")
         cv2.imwrite(str(fpath), img)
         fpath = output_path.joinpath("error_mosaic.png")
         cv2.imwrite(str(fpath), mosaic_img)
         raise err
         # The video exited properly, so cleanup and exit.
+    except KeyboardInterrupt:
+        sys.stderr.write("\nUser terminated program.\n")
     fpath = output_path.joinpath("tile_{:03d}.png".format(tile_counter))
     cv2.imwrite(str(fpath), mosaic_img)
     cv2.destroyAllWindows()
     del reader
     if args.demo:
         writer.release()
```

### Comparing `mosaic-library-0.0.10/mosaicking/transformations.py` & `mosaic-library-1.0.1/mosaicking/transformations.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import numpy as np
-import cv2
 from scipy.spatial.transform import Rotation
 import sys
-import copy
+from numpy import typing as npt
+from typing import Tuple, Sequence, List
+import cv2
 
 
-def calculate_homography(K: np.ndarray, width: int, height: int, R: np.ndarray, T: np.ndarray, gradient_clip: float=0.0):
+def calculate_homography(K: npt.NDArray[float], width: int, height: int, R: npt.NDArray[float], T: npt.NDArray[float], gradient_clip: float=0.0) -> Tuple[npt.NDArray[float], Tuple[int, int], Tuple[int, int]]:
     if K.shape[1] < 4:
         K = np.concatenate((K, np.zeros((3, 1))), axis=1)
     # Calculate the inverse of K
     Kinv = np.zeros((4, 3))
     Kinv[:3, :3] = np.linalg.inv(K[:3, :3]) * (K[0, 0] * K[1, 1])
     Kinv[-1, :] = [0, 0, 1]
     # Get the extrinsic matrix (Camera to World)
@@ -47,15 +48,15 @@
     T1 = np.array([[1, 0, -xmin],
                    [0, 1, -ymin],
                    [0, 0, 1]])
     H = np.linalg.multi_dot([T1, K, E, Kinv])
     return H, (xmin, xmax), (ymin, ymax)
 
 
-def apply_transform(img: np.ndarray, K: np.ndarray, R: Rotation, T: np.ndarray, keypoints: list, scale: float = None, mask: np.ndarray = None, gradient_clip: float = 0.0):
+def apply_transform(img: npt.NDArray[np.uint8], K: npt.NDArray[float], R: Rotation, T: npt.NDArray[float], keypoints: Sequence[cv2.KeyPoint], scale: float = None, mask: npt.NDArray[np.uint8] = None, gradient_clip: float = 0.0) -> Tuple[npt.NDArray[np.uint8], List[cv2.KeyPoint], npt.NDArray[np.uint8]]:
     """
     img: input image
     K: camera calibration matrix
     R: Rotation matrix from world to camera
     T: Translation vector (m) from world to camera
     keypoints: list of keypoints
     scale: zoom scaling
@@ -79,15 +80,15 @@
     # for k, pt in zip(keypoints, pts):
     #     k.pt = tuple(pt)
     if scale is not None:
         img_warped, keypoints, mask_warped = apply_scale(img_warped, keypoints, scale, mask_warped)
     return img_warped, mask_warped, kp
 
 
-def apply_scale(img: np.ndarray, keypoints: list, scale: float, mask: np.ndarray=None):
+def apply_scale(img: npt.NDArray[np.uint8], keypoints: Sequence[cv2.KeyPoint], scale: float, mask: npt.NDArray[np.uint8] = None) -> Tuple[npt.NDArray[np.uint8], List[cv2.KeyPoint], npt.NDArray[np.uint8]]:
     if scale == 1.0:
         return img, keypoints, mask
     if scale < 1:
         img = cv2.resize(img, (0, 0), fx=scale, fy=scale, interpolation=cv2.INTER_AREA)
         if mask is not None:
             mask = cv2.resize(mask, (0,0), fx=scale, fy=scale, interpolation=cv2.INTER_AREA)
     else:
@@ -104,15 +105,15 @@
     for k, pt in zip(keypoints, pts):
         kp.append(cv2.KeyPoint(pt[0], pt[1], k.size, k.angle, k.response, k.octave, k.class_id))
     # for k, pt in zip(keypoints, pts):
     #     k.pt = tuple(pt)
     return img, kp, mask
 
 
-def get_extrinsic_matrix(Rc: np.ndarray, C: np.ndarray, order: str = "xyz", degrees: bool=False):
+def get_extrinsic_matrix(Rc: npt.NDArray[float], C: npt.NDArray[float], order: str = "xyz", degrees: bool=False) -> npt.NDArray[float]:
     """
     Converts a rotation from world to camera and C from world to camera into the correct extrinsic form (camera to world).
     @param Rc: Rotation from world frame to camera frame, can be a size 3 euler angle vector, quaternion (wxyz) or rotation matrix.
     @param C: Translation from world frame to camera frame, must be a size 3 vector.
     @param order: String specifying order for euler angles, must be a permutation of "xyz".
     @param degrees: Flag to indicate if euler angles are in degrees.
     """
@@ -132,48 +133,48 @@
     R = Rc.T
     t = -R @ C
     return np.concatenate((np.concatenate((R, t), axis=1), [[0,0,0,1]]), axis=0)
 
 
 ## euler rotation methods
 # Matrix for Yaw-rotation about the Z-axis
-def R_z(psi, degrees=False):
+def R_z(psi: float, degrees=False) -> npt.NDArray[float]:
     psi = psi * np.pi / 180 if degrees else psi
     R = np.array([[np.cos(psi), -np.sin(psi), 0, 0],
                    [np.sin(psi), np.cos(psi), 0, 0],
                    [0, 0, 1, 0],
                    [0, 0, 0, 1]])
     return R
 
 
 # Matrix for Pitch-rotation about the Y-axis
-def R_y(theta, degrees=False):
+def R_y(theta: float, degrees=False) -> npt.NDArray[float]:
     theta = theta * np.pi / 180 if degrees else theta
     R = np.array([[np.cos(theta), 0, np.sin(theta), 0],
                    [0, 1, 0, 0],
                    [-np.sin(theta), 0, np.cos(theta), 0],
                    [0, 0, 0, 1]])
     return R
 
 
 # Matrix for Roll-rotation about the X-axis
-def R_x(phi, degrees=False):
+def R_x(phi: float, degrees=False) -> npt.NDArray[float]:
     phi = phi*np.pi/180 if degrees else phi
     R = np.array([[1, 0, 0, 0],
                    [0, np.cos(phi), -np.sin(phi), 0],
                    [0, np.sin(phi), np.cos(phi), 0],
                    [0, 0, 0, 1]])
     return R
 
 
-def euler_rotation(phi, theta, psi, degrees=False):
+def euler_rotation(phi: float, theta: float, psi: float, degrees=False) -> npt.NDArray[float]:
     return np.linalg.multi_dot([R_x(phi, degrees), R_y(theta, degrees), R_z(psi, degrees)])
 
 
-def euler_affine_rotate(img: np.ndarray, euler: np.array, degrees: bool=False):
+def euler_affine_rotate(img: npt.NDArray[np.uint8], euler: npt.NDArray[float], degrees: bool=False) -> npt.NDArray[np.uint8]:
     """img: numpy array image
     euler: numpy array euler angles in Yaw, Pitch, Roll order"""
     if degrees:
         euler = np.deg2rad(euler)
     R = Rotation.from_euler("zyx", euler, degrees=False).as_matrix()
     height, width, channels = img.shape
     src = np.array([[0, 0, 0],
@@ -186,15 +187,15 @@
     bx, by, bwidth, bheight = cv2.boundingRect(dst)
     h = cv2.getAffineTransform(src[0:3,0:2], dst[0:3,:])
     h[:,-1] = [-bx, -by]
     img_dst = cv2.warpAffine(img, h, (bwidth, bheight), flags=cv2.INTER_CUBIC, borderMode=cv2.BORDER_CONSTANT)
     return img_dst
 
 
-def euler_perspective_rotate(img: np.ndarray, euler: np.array, degrees: bool=False):
+def euler_perspective_rotate(img: npt.NDArray[np.uint8], euler: npt.NDArray[float], degrees: bool=False) -> npt.NDArray[np.uint8]:
     """img: numpy array image
     euler: numpy array euler angles in Yaw, Pitch, Roll order"""
     if degrees:
         euler = np.deg2rad(euler)
     R = Rotation.from_euler("zyx", euler, degrees=False).as_matrix()
     height, width, channels = img.shape
     src = np.array([[0, 0, 0],
@@ -215,15 +216,15 @@
     src = src[:,0:2]
     pers_tform = cv2.getPerspectiveTransform(src.astype("float32"), dst_projection.astype("float32"))
     bx, by, bwidth, bheight = cv2.boundingRect(dst_projection)
     img_dst = cv2.warpPerspective(img, pers_tform, (bwidth, bheight))
     return img_dst
 
 ## Bird View method- get a top down view of the frames
-def bird_view(image, pitch=45):
+def bird_view(image: npt.NDArray[np.uint8], pitch: float = 45) -> npt.NDArray[np.uint8]:
     ## Crop image
 
     IMAGE_H = image.shape[0]
     IMAGE_W = image.shape[1]
 
     # Assume that focus length is equal half image width
     FOCUS = IMAGE_W / 2  ## Focus needs to stay the same height of the seabed-camera
@@ -253,127 +254,92 @@
     #    Minv = cv2.getPerspectiveTransform(dst, src) # Inverse transformation
     warped_img = cv2.warpPerspective(image, fullTransformation, (2 * IMAGE_W, 2 * IMAGE_H),
                                      flags=cv2.INTER_NEAREST + cv2.WARP_FILL_OUTLIERS)  # Image warping
 
     return warped_img
 
 
-import numpy as np
-import cv2
+def get_origin_direction(E: npt.NDArray[float]) -> Tuple[npt.NDArray[float], ...]:
+    """
+    This function accepts a 4x4 camera extrinsic matrix, E, and returns the camera's origin and
+    direction vector (which points towards the scene from the camera origin).
+    """
 
+    # Extract the rotation matrix and translation vector
+    R = E[:3, :3]
+    t = E[:3, 3]
+
+    # The camera's position in world coordinates is the negative translation vector
+    origin = -R.T @ t
+
+    # The camera's direction is the third column of the rotation matrix
+    direction = R[:, 2]
+
+    return origin, direction
+
+
+def get_alignment(src_pts: npt.NDArray[float], src_shape: Tuple[int, int], dst_pts: npt.NDArray[float], dst_shape: Tuple[int, int], homography: str = "similar", gradient: float = 0.0) -> Tuple[npt.NDArray[float], Tuple[int, int], Tuple[int, int]]:
+    assert homography in ["rigid", "similar", "affine", "perspective"], "Homography can be of type similar, affine, or perspective"
+    # Update the homography from current image to mosaic
+    if homography == "rigid":
+        A, mask = cv2.estimateAffinePartial2D(src_pts, dst_pts, method=cv2.RANSAC, ransacReprojThreshold=1)
+        # Remove rotation components
+        theta = np.arctan2(A[1,0], A[0, 0])
+        s = A[0, 0] / np.cos(theta) if np.cos(theta) != 0 else A[1, 0] / np.sin(theta)
+        A[:, :2] = s * np.eye(2)
+    elif homography == "similar":
+        A, mask = cv2.estimateAffinePartial2D(src_pts, dst_pts)#, method=cv2.RANSAC, ransacReprojThreshold=1)
+        # # Remove shear effect from affine transform (according to: https://math.stackexchange.com/a/3521141)
+        # sx = np.sqrt(A[0, 0]**2+A[1,0]**2)
+        # theta = np.arctan2(A[1,0],A[0,0])
+        # msy = A[0,1]*np.cos(theta) + A[1,1]*np.sin(theta)
+        # if np.abs(np.sin(theta)) > 0:
+        #     sy = (msy*np.cos(theta)-A[0,1]) / np.sin(theta)
+        # else:
+        #     sy = (A[1,1] - msy*np.sin(theta)) / np.cos(theta)
+        # m = msy / sy
+        # rot = np.array([[np.cos(theta), -np.sin(theta)],
+        #                      [np.sin(theta), np.cos(theta)]])
+        # shear = np.eye(2)
+        # scale = np.array([[sx, 0],
+        #                   [0, sy]])
+        # A[:2,:2] = rot@shear@scale
+    elif homography == "affine":
+        A, mask = cv2.estimateAffine2D(src_pts, dst_pts, method=cv2.RANSAC, ransacReprojThreshold=1)
+    elif homography == "perspective":
+        A, mask = cv2.findHomography(src_pts, dst_pts, method=cv2.RANSAC, ransacReprojThreshold=1)
+    else:
+        raise ValueError(f'homography argument not supported, choose from {["rigid", "similar", "affine", "perspective"]}')
+    A = np.concatenate((A, np.array([[0, 0, 1]])), axis=0) if A.size < 9 else A  # convert to a homogeneous form
 
-# Usage:
-#     Change main function with ideal arguments
-#     Then
-#     from image_tranformer import ImageTransformer
-#
-# Parameters:
-#     image_path: the path of image that you want rotated
-#     shape     : the ideal shape of input image, None for original size.
-#     theta     : rotation around the x axis
-#     phi       : rotation around the y axis
-#     gamma     : rotation around the z axis (basically a 2D rotation)
-#     dx        : C along the x axis
-#     dy        : C along the y axis
-#     dz        : C along the z axis (distance to the image)
-#
-# Output:
-#     image     : the rotated image
-#
-# Reference:
-#     1.        : http://stackoverflow.com/questions/17087446/how-to-calculate-perspective-transform-for-opencv-from-rotation-angles
-#     2.        : http://jepsonsblog.blogspot.tw/2012/11/rotation-in-3d-using-opencvs.html
-
-class ImageTransformer(object):
-    """ Perspective transformation class for image
-        with shape (height, width, #channels) """
-
-    def __init__(self, image: np.ndarray):
-        self.image = image
-        self.height = self.image.shape[0]
-        self.width = self.image.shape[1]
-        self.num_channels = self.image.shape[2]
-
-    """ Wrapper of Rotating a Image """
-
-    def rotate_along_axis(self, theta: float=0, phi: float=0, gamma: float=0, dx: float=0, dy: float=0, dz: float=0, degrees: bool=False):
-        # Get radius of rotation along 3 axes
-        if degrees:
-            rtheta = np.deg2rad(theta)
-            rphi = np.deg2rad(phi)
-            rgamma = np.deg2rad(gamma)
+    # Warp the image coordinates
+    u_idx, v_idx = np.indices(tuple(s - 1 for s in src_shape[1::-1]), float)
+    grid_dst = np.stack((u_idx, v_idx, np.ones_like(u_idx)), axis=2).reshape((-1, 1, 3))
+    warp_grid_dst = A @ grid_dst.squeeze().T
+    warp_grid_dst = warp_grid_dst[:2, :] / warp_grid_dst[-1, :]
+
+    if gradient > 0:
+        # Compute the gradient of the transformed coordinates
+        grad_x = cv2.Sobel(warp_grid_dst.T[..., 0], cv2.CV_64F, 1, 0, ksize=5)
+        grad_y = cv2.Sobel(warp_grid_dst.T[..., 1], cv2.CV_64F, 0, 1, ksize=5)
+        # Compute the norm of the gradient
+        grad_norm = np.sqrt(grad_x ** 2 + grad_y ** 2)
+        idx = (grad_norm < gradient).squeeze()
+        if not idx.any():
+            sys.stderr.write("WARNING: Gradient Explosion. Is the Image Rapidly Zooming In/Out? Gradient clipping is suppressed to allow continuity, consider increasing gradient clip argument.\n")
         else:
-            rtheta = theta
-            rphi = phi
-            rgamma = gamma
-
-        # Get ideal focal length on z axis
-        # NOTE: Change this section to other axis if needed
-        d = np.sqrt(self.height ** 2 + self.width ** 2)
-        self.focal = d / (2 * np.sin(rgamma) if np.sin(rgamma) != 0 else 1)
-        dz = self.focal
-
-        # Get projection matrix
-        mat = self.get_M(rtheta, rphi, rgamma, dx, dy, dz)
-
-        corners = np.array([[[0, 0],
-                             [self.width, 0],
-                             [self.width, self.height],
-                             [0, self.height]]], dtype="float32")
-
-        dst_corners = cv2.perspectiveTransform(corners, mat)
-        bx, by, bwidth, bheight = cv2.boundingRect(dst_corners)
-        t = np.array([[1, 0, -bx],
-                      [0, 1, -by],
-                      [0, 0, 1]])
-
-        mat = t.dot(mat)
-        img = cv2.warpPerspective(self.image.copy(), mat, (bwidth, bheight))
-        return img
-        return cv2.warpPerspective(self.image.copy(), mat, (self.width, self.height))
-
-    """ Get Perspective Projection Matrix """
-
-    def get_M(self, theta, phi, gamma, dx, dy, dz):
-        w = self.width
-        h = self.height
-        f = self.focal
-
-        # Projection 2D -> 3D matrix
-        A1 = np.array([[1, 0, -w / 2],
-                       [0, 1, -h / 2],
-                       [0, 0, 1],
-                       [0, 0, 1]])
-
-        # Rotation matrices around the X, Y, and Z axis
-        RX = np.array([[1, 0, 0, 0],
-                       [0, np.cos(theta), -np.sin(theta), 0],
-                       [0, np.sin(theta), np.cos(theta), 0],
-                       [0, 0, 0, 1]])
-
-        RY = np.array([[np.cos(phi), 0, -np.sin(phi), 0],
-                       [0, 1, 0, 0],
-                       [np.sin(phi), 0, np.cos(phi), 0],
-                       [0, 0, 0, 1]])
-
-        RZ = np.array([[np.cos(gamma), -np.sin(gamma), 0, 0],
-                       [np.sin(gamma), np.cos(gamma), 0, 0],
-                       [0, 0, 1, 0],
-                       [0, 0, 0, 1]])
-
-        # Composed rotation matrix with (RX, RY, RZ)
-        R = np.dot(np.dot(RX, RY), RZ)
-
-        # Translation matrix
-        T = np.array([[1, 0, 0, dx],
-                      [0, 1, 0, dy],
-                      [0, 0, 1, dz],
-                      [0, 0, 0, 1]])
-
-        # Projection 3D -> 2D matrix
-        A2 = np.array([[f, 0, w / 2, 0],
-                       [0, f, h / 2, 0],
-                       [0, 0, 1, 0]])
+            warp_grid_dst = warp_grid_dst[:, idx]
+
+    # Get the corners of the mosaic image in homogeneous coords (x,y,w=1)
+    dst_crn = np.array([[0, dst_shape[1], dst_shape[1], 0],
+                        [0, 0, dst_shape[0], dst_shape[0]]], float)
 
-        # Final transformation matrix
-        return np.dot(A2, np.dot(T, np.dot(R, A1)))
+    # Concatenate the mosaic and warped corner coordinates
+    pts = np.concatenate([dst_crn, warp_grid_dst], axis=1)
+
+    # Round to pixel centers
+    xmin, ymin = np.int32(pts.min(axis=1) + 0.5)
+    xmax, ymax = np.int32(pts.max(axis=1) + 0.5)
 
+    t = [-xmin, -ymin]  # C of the upper left corner of the transformed image
+    A[:2, -1] = A[:2, -1] + t  # C homography
+    return A, (xmin, xmax), (ymin, ymax)
```

### Comparing `mosaic-library-0.0.10/mosaicking/utils.py` & `mosaic-library-1.0.1/mosaicking/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import argparse
 
 import cv2
 import os
 import pandas as pd
 import numpy as np
+import numpy.typing as npt
 from pathlib import Path
+from matplotlib import pyplot as plt
 
 
 def parse_args():
     parser = argparse.ArgumentParser()
     parser.add_argument("video", type=str, help="Path to video file.")
     parser.add_argument("--output_directory", type=str,
                         help="Path to directory where output mosaics are to be saved. Default is invokation path.",
@@ -42,18 +44,18 @@
                         help="Scale the input image with constant aspect ratio.")
     parser.add_argument("--alpha", type=float, default=0.5,
                         help="Alpha blending scalar for merging new frames into mosaic.")
     parser.add_argument("--show_rotation", action="store_true",
                         help="Flag to display the rotation compensation using rotation data.")
     parser.add_argument("--show_mosaic", action="store_true", help="Flag to display the mosaic output.")
     parser.add_argument("--show_preprocessing", action="store_true", help="Flag to display the preprocessed image")
-    parser.add_argument("--fix_color", action="store_true", help="Flag to preprocess image for color balance.")
-    parser.add_argument("--fix_contrast", action="store_true",
+    parser.add_argument("--imadjust", action="store_true", help="Flag to preprocess image for color balance.")
+    parser.add_argument("--equalize_color", action="store_true",
                         help="Flag to preprocess image for contrast equalization.")
-    parser.add_argument("--fix_light", action="store_true", help="Flag to preprocess image for lighting equalization.")
+    parser.add_argument("--equalize_luminance", action="store_true", help="Flag to preprocess image for lighting equalization.")
     parser.add_argument("-c", "--calibration", type=str, default=None,
                         help="Path to calibration file, overrides --intrinsic and --distortion.")
     parser.add_argument("-k", "--intrinsic", nargs=9, type=float, default=None,
                         help="Space delimited list of intrinsic matrix terms, Read as K[0,0],K[0,1],K[0,2],K[1,0],K[1,1],K[1,2],K[2,0],K[2,1],K[2,2]. Overriden by calibration file if intrinsic present.")
     parser.add_argument("-d", "--distortion", nargs="+", type=float, default=None,
                         help="Space delimited list of distortion coefficients, Read as K1, K2, p1, p2. Overriden by calibration file if distortion present.")
     parser.add_argument("-x", "--xrotation", type=float, default=0,
@@ -130,15 +132,14 @@
             self.set(cv2.CAP_PROP_POS_FRAMES, self._args.start_frame - 1)
         else:
             self.set(cv2.CAP_PROP_POS_FRAMES, 0)
         self._start_frame = int(self.get(cv2.CAP_PROP_POS_FRAMES))
         if self._finish_frame < self._start_frame:
             raise ValueError("Finishing frame is less than starting time.")
 
-
     def evaluate_stopping(self):
         """Return true if stopping conditions met."""
         return self._finish_frame <= self.get(cv2.CAP_PROP_POS_FRAMES)
 
     def __del__(self):
         print(f"Closing video {self._args.video}")
         self.release()
@@ -164,37 +165,45 @@
                 self._index = self._videoplayer.get(cv2.CAP_PROP_POS_FRAMES)
                 return img
         # End of Iteration
         raise StopIteration
 
 
 def check_keypress(key: str):
-    press = cv2.waitKey(1)
-    if key == ord(press):
-        return True
-    return False
+    return key == cv2.waitKey(1)
 
 
 def get_starting_pos(cap: cv2.VideoCapture, args):
     """Set a VideoCapture object to a position (either in seconds or the frame #)"""
     if args.start_time:
         cap.set(cv2.CAP_PROP_POS_MSEC, args.start_time * 1000.0)
     elif args.start_frame:
         cap.set(cv2.CAP_PROP_POS_FRAMES, args.start_frame - 1)
     return cap
 
 
-def evaluate_stopping(cap: cv2.VideoCapture, args):
+def evaluate_stopping(cap: cv2.VideoCapture, args: argparse.Namespace) -> bool:
     """Return true if stopping conditions met."""
     if args.finish_time:
         return cap.get(cv2.CAP_PROP_POS_MSEC) > args.finish_time*1000.0
     elif args.finish_frame:
         return cap.get(cv2.CAP_PROP_POS_FRAMES) > args.finish_frame-1
     return cap.get(cv2.CAP_PROP_FRAME_COUNT)-1 <= cap.get(cv2.CAP_PROP_POS_FRAMES)
 
 
-def load_orientations(path: os.PathLike, args):
+def load_orientations(path: os.PathLike, args: argparse.Namespace) -> pd.DataFrame:
     """Given a path containing orientations, retrieve the orientations corresponding to a time offset between video and orientation data."""
     time_offset = args.time_offset if args.time_offset else args.sync_points[1] - args.sync_points[0]
     df = pd.read_csv(str(path), index_col="timestamp")
     df.index = df.index - time_offset
-    return df[~df.duplicated()]
+    return df[~df.duplicated()]
+
+
+def plot_image_histogram(img: npt.NDArray[np.uint8], ax: plt.Axes = None) -> None:
+    if ax is None:
+        fig, ax = plt.subplots()
+    if img.ndim < 3:
+        img = img[..., None]
+    colors = ('b','g','r') if img.shape[-1] == 3 else ('k',)
+    for channel in range(img.shape[-1]):
+        hist = cv2.calcHist([img], [channel], None, [256], [0, 256])
+        ax.plot(hist, colors[channel])
```

