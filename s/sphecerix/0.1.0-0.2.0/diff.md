# Comparing `tmp/sphecerix-0.1.0-py3-none-any.whl.zip` & `tmp/sphecerix-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,11 @@
-Zip file size: 5776 bytes, number of entries: 10
--rw-r--r--  2.0 unx      333 b- defN 23-May-26 19:31 sphecerix/__init__.py
--rw-r--r--  2.0 unx       21 b- defN 23-May-26 19:31 sphecerix/_version.py
--rw-r--r--  2.0 unx     3394 b- defN 23-May-26 19:31 sphecerix/atomic_wave_functions.py
--rw-r--r--  2.0 unx      688 b- defN 23-May-26 19:31 sphecerix/rotations.py
--rw-r--r--  2.0 unx     1220 b- defN 23-May-26 19:31 sphecerix/tesseral.py
--rw-r--r--  2.0 unx     2189 b- defN 23-May-26 19:31 sphecerix/wignerd.py
--rw-r--r--  2.0 unx     2328 b- defN 23-May-26 19:31 sphecerix-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-26 19:31 sphecerix-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-May-26 19:31 sphecerix-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      783 b- defN 23-May-26 19:31 sphecerix-0.1.0.dist-info/RECORD
-10 files, 11058 bytes uncompressed, 4444 bytes compressed:  59.8%
+Zip file size: 5536 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      219 b- defN 23-May-28 19:49 sphecerix/__init__.py
+-rw-r--r--  2.0 unx       21 b- defN 23-May-28 19:49 sphecerix/_version.py
+-rw-r--r--  2.0 unx     3394 b- defN 23-May-28 19:49 sphecerix/atomic_wave_functions.py
+-rw-r--r--  2.0 unx     1220 b- defN 23-May-28 19:49 sphecerix/tesseral.py
+-rw-r--r--  2.0 unx     2314 b- defN 23-May-28 19:49 sphecerix/wignerd.py
+-rw-r--r--  2.0 unx     2873 b- defN 23-May-28 19:49 sphecerix-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-28 19:49 sphecerix-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-May-28 19:49 sphecerix-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      705 b- defN 23-May-28 19:49 sphecerix-0.2.0.dist-info/RECORD
+9 files, 10848 bytes uncompressed, 4324 bytes compressed:  60.1%
```

## zipnote {}

```diff
@@ -3,29 +3,26 @@
 
 Filename: sphecerix/_version.py
 Comment: 
 
 Filename: sphecerix/atomic_wave_functions.py
 Comment: 
 
-Filename: sphecerix/rotations.py
-Comment: 
-
 Filename: sphecerix/tesseral.py
 Comment: 
 
 Filename: sphecerix/wignerd.py
 Comment: 
 
-Filename: sphecerix-0.1.0.dist-info/METADATA
+Filename: sphecerix-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: sphecerix-0.1.0.dist-info/WHEEL
+Filename: sphecerix-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: sphecerix-0.1.0.dist-info/top_level.txt
+Filename: sphecerix-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: sphecerix-0.1.0.dist-info/RECORD
+Filename: sphecerix-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sphecerix/__init__.py

```diff
@@ -1,9 +1,5 @@
-from .rotations import axis_angle_to_euler, axis_angle_to_rotmat
-
-from .wignerd import wigner_D, wigner_d, wigner_D_axis_angle, tesseral_wigner_D_axis_angle
-
+from .wignerd import tesseral_wigner_D, wigner_D
 from .tesseral import tesseral_transformation, permutation_sh_car
-
 from .atomic_wave_functions import wfcart, wf, wffield, wffield_l
 
 from ._version import __version__
```

## sphecerix/_version.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.0"
+__version__ = "0.2.0"
```

## sphecerix/wignerd.py

```diff
@@ -1,37 +1,38 @@
 # -*- coding: utf-8 -*-
 
 import numpy as np
 from scipy.special import factorial
-from .rotations import axis_angle_to_euler
+from scipy.spatial.transform import Rotation as R
 from .tesseral import tesseral_transformation
 
-def tesseral_wigner_D_axis_angle(l, axis, angle):
+def tesseral_wigner_D(l, Robj):
     """
     Produce the Wigner D-matrix for tesseral spherical harmonics
     """
+    # verify that Robj is a rotation object
+    if not isinstance(Robj, R):
+        raise TypeError('Second argument Robj should be of type scipy.spatial.transform.R')
+    
     T = tesseral_transformation(l)
-    alpha, beta, gamma = axis_angle_to_euler(axis, angle)
-    D = wigner_D(l, alpha, beta, gamma)
+    alpha, beta, gamma = Robj.as_euler('zyz', degrees=False)
+    D = wigner_D(l, Robj)
     
     return np.real(T @ D @ T.conjugate().transpose())
 
-def wigner_D_axis_angle(l, axis, angle):
+def wigner_D(l, Robj):
     """
     Produce Wigner D-matrix for order l of spherical harmonics and
     given axis angle rotation
     """
-    alpha, beta, gamma = axis_angle_to_euler(axis, angle)
-    return wigner_D(l, alpha, beta, gamma)
+    # verify that Robj is a rotation object
+    if not isinstance(Robj, R):
+        raise TypeError('Second argument Robj should be of type scipy.spatial.transform.R')
 
-def wigner_D(l, alpha, beta, gamma):
-    """
-    Produce Wigner D-matrix for order l of spherical harmonics and
-    euler angles
-    """
+    alpha, beta, gamma = Robj.as_euler('zyz', degrees=False)
     d = wigner_d(l, beta)
     m = np.arange(-l, l+1)
     diag_alpha = np.diag(np.exp(1j * m * alpha))
     diag_gamma = np.diag(np.exp(1j * m * gamma))
     
     return diag_gamma @ d @ diag_alpha
```

## Comparing `sphecerix-0.1.0.dist-info/METADATA` & `sphecerix-0.2.0.dist-info/METADATA`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: sphecerix
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python package for constructing Wigner-D matrices
 Home-page: https://github.com/ifilot/sphecerix
 Author: Ivo Filot
 Author-email: ivo@ivofilot.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: scipy
 
 # Sphecerix
 
+![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/ifilot/sphecerix?label=version)
+[![Build](https://github.com/ifilot/sphecerix/actions/workflows/build.yml/badge.svg)](https://github.com/ifilot/sphecerix/actions/workflows/build.yml)
+[![Documentation](https://github.com/ifilot/sphecerix/actions/workflows/docs.yml/badge.svg)](https://sphecerix.imc-tue.nl)
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+
 ![rotation of spherical harmonics](img/rotation_spherical_harmonics.jpg)
 
 **Figure**: Demonstration of rotating a spherical harmonic by means of the
 Wigner D-matrix. In the above image, a 3dz2 and a 4fz3 atomic orbital are rotated
 by an angle $`\pi`$ over an axis with coordinates $`(1,1,1)`$. Note that the image has
 **not** been constructed by rotating the isosurfaces but by calculating the
 scalar field after the rotation.
@@ -45,24 +50,26 @@
 ## Usage
 
 In the script below, a dz2 spherical harmonic is rotated over an axis with
 coordinates $`(1,1,1)`$ by an angle $`\pi`$. The result of this rotation is
 a linear combination of spherical harmonics all with $`l=2`$.
 
 ```python
-from sphecerix import tesseral_wigner_D_axis_angle
+from sphecerix import tesseral_wigner_D
+from scipy.spatial.transform import Rotation as R
 import numpy as np
 
 def main():
     # build rotation axis and set angle
     axis = np.ones(3) / np.sqrt(3)
     angle = np.pi
+    Robj = R.from_rotvec(axis * angle)
     
     # construct tesseral Wigner D matrix
-    D = tesseral_wigner_D_axis_angle(2, axis, angle)
+    D = tesseral_wigner_D(2, Robj)
     Y = np.zeros(5)
     Y[2] = 1
     
     # calculate linear combination of the spherical harmonics after rotation
     Yp = D @ Y
     print(Yp)
```

## Comparing `sphecerix-0.1.0.dist-info/RECORD` & `sphecerix-0.2.0.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-sphecerix/__init__.py,sha256=kkA9fXe9Sj8nVXfbU9txV6aq_9YycRAeZvReIZ2GrI0,333
-sphecerix/_version.py,sha256=Pru0BlFBASFCFo7McHdohtKkUtgMPDwbGfyUZlE2_Vw,21
+sphecerix/__init__.py,sha256=Qq3BOzEm_wsbEA4Shsh5qz7nDqIl82OxlUtcVCMU078,219
+sphecerix/_version.py,sha256=1KhrBItVjTCR-Sumh0o09b_aKrjTTcJrpTBh5GBw6Lk,21
 sphecerix/atomic_wave_functions.py,sha256=VO9_8spYmPvTbRncdG9aPMzjkA3qFTj6jUTJIsOyER0,3394
-sphecerix/rotations.py,sha256=zoazJah-PKHskqIW1mspe0I6VCK6USXt_Hm4qnsS_3g,688
 sphecerix/tesseral.py,sha256=7ak1E_tsT5IMavEVyNqaNtY64jUdfuecl8IZr2M9Rfc,1220
-sphecerix/wignerd.py,sha256=XRYVpslKAHu3M8KReosF3lE-K1KNgAZYv2VQJH6wccg,2189
-sphecerix-0.1.0.dist-info/METADATA,sha256=Z8bLBDCe9TRC1dGGHabad5eC6qf7_nZfFPnFrbGMEss,2328
-sphecerix-0.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-sphecerix-0.1.0.dist-info/top_level.txt,sha256=wx-xiducfOhrGJk9tdcB7P1x6P0oMB-LilN7vRs4-rs,10
-sphecerix-0.1.0.dist-info/RECORD,,
+sphecerix/wignerd.py,sha256=EqU1rwTH93AwEqBHH4f03VplOVqY1F6Q_XccVsd8DyY,2314
+sphecerix-0.2.0.dist-info/METADATA,sha256=Ew6Q7mwcz0VEg2TW9UDXsQlwXP1ZK0uGXkd6jr9WVVc,2873
+sphecerix-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+sphecerix-0.2.0.dist-info/top_level.txt,sha256=wx-xiducfOhrGJk9tdcB7P1x6P0oMB-LilN7vRs4-rs,10
+sphecerix-0.2.0.dist-info/RECORD,,
```

