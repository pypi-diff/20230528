# Comparing `tmp/rtb_toolbox-0.1.47.tar.gz` & `tmp/rtb_toolbox-0.1.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtb_toolbox-0.1.47.tar", max compression
+gzip compressed data, was "rtb_toolbox-0.1.48.tar", max compression
```

## Comparing `rtb_toolbox-0.1.47.tar` & `rtb_toolbox-0.1.48.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     4034 2023-04-14 22:16:46.136319 rtb_toolbox-0.1.47/README.md
--rw-r--r--   0        0        0      323 2023-05-28 01:09:47.982492 rtb_toolbox-0.1.47/pyproject.toml
--rw-r--r--   0        0        0     4034 2023-04-14 22:17:39.372360 rtb_toolbox-0.1.47/src/rtb_toolbox/README.md
--rw-r--r--   0        0        0      297 2023-05-27 00:03:43.689963 rtb_toolbox-0.1.47/src/rtb_toolbox/__init__.py
--rw-r--r--   0        0        0     2298 2023-04-14 22:12:18.847856 rtb_toolbox-0.1.47/src/rtb_toolbox/forward_dynamics/__init__.py
--rw-r--r--   0        0        0     3636 2023-05-28 00:44:55.252589 rtb_toolbox-0.1.47/src/rtb_toolbox/forward_kinematics/__init__.py
--rw-r--r--   0        0        0     3232 2023-05-28 00:45:48.876655 rtb_toolbox-0.1.47/src/rtb_toolbox/frame/__init__.py
--rw-r--r--   0        0        0    33140 2023-04-14 21:54:20.903286 rtb_toolbox-0.1.47/src/rtb_toolbox/images/full_ik.png
--rw-r--r--   0        0        0    33229 2023-04-14 21:54:20.907286 rtb_toolbox-0.1.47/src/rtb_toolbox/images/partial_ik.png
--rw-r--r--   0        0        0     6569 2023-04-14 21:54:20.915286 rtb_toolbox-0.1.47/src/rtb_toolbox/images/tau1.png
--rw-r--r--   0        0        0     5005 2023-04-14 21:54:20.915286 rtb_toolbox-0.1.47/src/rtb_toolbox/images/tau2.png
--rw-r--r--   0        0        0   479230 2023-04-14 21:54:20.923286 rtb_toolbox-0.1.47/src/rtb_toolbox/images/trajectories.png
--rw-r--r--   0        0        0     7035 2023-05-28 01:09:40.074479 rtb_toolbox-0.1.47/src/rtb_toolbox/inverse_kinematics/__init__.py
--rw-r--r--   0        0        0     1681 2023-05-28 00:44:50.244583 rtb_toolbox-0.1.47/src/rtb_toolbox/link/__init__.py
--rw-r--r--   0        0        0      408 2023-05-27 17:37:29.169298 rtb_toolbox-0.1.47/src/rtb_toolbox/robots/SCARA.py
--rw-r--r--   0        0        0      674 2023-05-28 01:06:43.874203 rtb_toolbox-0.1.47/src/rtb_toolbox/robots/comau.py
--rw-r--r--   0        0        0      510 2023-05-27 23:57:51.896877 rtb_toolbox-0.1.47/src/rtb_toolbox/robots/puma260.py
--rw-r--r--   0        0        0       55 2023-04-14 21:52:22.347973 rtb_toolbox-0.1.47/src/rtb_toolbox/symbols.py
--rw-r--r--   0        0        0     1150 2023-04-14 21:52:22.231974 rtb_toolbox-0.1.47/src/rtb_toolbox/trajectory/__init__.py
--rw-r--r--   0        0        0     4919 2023-05-27 00:08:26.422563 rtb_toolbox-0.1.47/src/rtb_toolbox/utils/__init__.py
--rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 rtb_toolbox-0.1.47/setup.py
--rw-r--r--   0        0        0     4374 1970-01-01 00:00:00.000000 rtb_toolbox-0.1.47/PKG-INFO
+-rw-r--r--   0        0        0     4034 2023-04-14 22:16:46.136319 rtb_toolbox-0.1.48/README.md
+-rw-r--r--   0        0        0      323 2023-05-28 01:15:08.131047 rtb_toolbox-0.1.48/pyproject.toml
+-rw-r--r--   0        0        0     4034 2023-04-14 22:17:39.372360 rtb_toolbox-0.1.48/src/rtb_toolbox/README.md
+-rw-r--r--   0        0        0      297 2023-05-27 00:03:43.689963 rtb_toolbox-0.1.48/src/rtb_toolbox/__init__.py
+-rw-r--r--   0        0        0     2298 2023-04-14 22:12:18.847856 rtb_toolbox-0.1.48/src/rtb_toolbox/forward_dynamics/__init__.py
+-rw-r--r--   0        0        0     3636 2023-05-28 00:44:55.252589 rtb_toolbox-0.1.48/src/rtb_toolbox/forward_kinematics/__init__.py
+-rw-r--r--   0        0        0     3232 2023-05-28 00:45:48.876655 rtb_toolbox-0.1.48/src/rtb_toolbox/frame/__init__.py
+-rw-r--r--   0        0        0    33140 2023-04-14 21:54:20.903286 rtb_toolbox-0.1.48/src/rtb_toolbox/images/full_ik.png
+-rw-r--r--   0        0        0    33229 2023-04-14 21:54:20.907286 rtb_toolbox-0.1.48/src/rtb_toolbox/images/partial_ik.png
+-rw-r--r--   0        0        0     6569 2023-04-14 21:54:20.915286 rtb_toolbox-0.1.48/src/rtb_toolbox/images/tau1.png
+-rw-r--r--   0        0        0     5005 2023-04-14 21:54:20.915286 rtb_toolbox-0.1.48/src/rtb_toolbox/images/tau2.png
+-rw-r--r--   0        0        0   479230 2023-04-14 21:54:20.923286 rtb_toolbox-0.1.48/src/rtb_toolbox/images/trajectories.png
+-rw-r--r--   0        0        0     5959 2023-05-28 01:15:56.231124 rtb_toolbox-0.1.48/src/rtb_toolbox/inverse_kinematics/__init__.py
+-rw-r--r--   0        0        0     1681 2023-05-28 00:44:50.244583 rtb_toolbox-0.1.48/src/rtb_toolbox/link/__init__.py
+-rw-r--r--   0        0        0      408 2023-05-27 17:37:29.169298 rtb_toolbox-0.1.48/src/rtb_toolbox/robots/SCARA.py
+-rw-r--r--   0        0        0     1054 2023-05-28 01:15:03.271038 rtb_toolbox-0.1.48/src/rtb_toolbox/robots/comau.py
+-rw-r--r--   0        0        0      510 2023-05-27 23:57:51.896877 rtb_toolbox-0.1.48/src/rtb_toolbox/robots/puma260.py
+-rw-r--r--   0        0        0       55 2023-04-14 21:52:22.347973 rtb_toolbox-0.1.48/src/rtb_toolbox/symbols.py
+-rw-r--r--   0        0        0     1150 2023-04-14 21:52:22.231974 rtb_toolbox-0.1.48/src/rtb_toolbox/trajectory/__init__.py
+-rw-r--r--   0        0        0     4919 2023-05-27 00:08:26.422563 rtb_toolbox-0.1.48/src/rtb_toolbox/utils/__init__.py
+-rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 rtb_toolbox-0.1.48/setup.py
+-rw-r--r--   0        0        0     4374 1970-01-01 00:00:00.000000 rtb_toolbox-0.1.48/PKG-INFO
```

### Comparing `rtb_toolbox-0.1.47/README.md` & `rtb_toolbox-0.1.48/README.md`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.47/src/rtb_toolbox/README.md` & `rtb_toolbox-0.1.48/src/rtb_toolbox/README.md`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.47/src/rtb_toolbox/forward_dynamics/__init__.py` & `rtb_toolbox-0.1.48/src/rtb_toolbox/forward_dynamics/__init__.py`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.47/src/rtb_toolbox/forward_kinematics/__init__.py` & `rtb_toolbox-0.1.48/src/rtb_toolbox/forward_kinematics/__init__.py`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.47/src/rtb_toolbox/frame/__init__.py` & `rtb_toolbox-0.1.48/src/rtb_toolbox/frame/__init__.py`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.47/src/rtb_toolbox/images/full_ik.png` & `rtb_toolbox-0.1.48/src/rtb_toolbox/images/full_ik.png`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.47/src/rtb_toolbox/images/partial_ik.png` & `rtb_toolbox-0.1.48/src/rtb_toolbox/images/partial_ik.png`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.47/src/rtb_toolbox/images/tau1.png` & `rtb_toolbox-0.1.48/src/rtb_toolbox/images/tau1.png`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.47/src/rtb_toolbox/images/tau2.png` & `rtb_toolbox-0.1.48/src/rtb_toolbox/images/tau2.png`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.47/src/rtb_toolbox/images/trajectories.png` & `rtb_toolbox-0.1.48/src/rtb_toolbox/images/trajectories.png`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.47/src/rtb_toolbox/inverse_kinematics/__init__.py` & `rtb_toolbox-0.1.48/src/rtb_toolbox/inverse_kinematics/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     f = res.F.min()
     theta_i = res.X
     success = f < 1e-5
 
     return theta_i, desired_pose, success, f
 
 
-def ik_position(
+def position_ik(
         desired_position=None,
         fk: ForwardKinematic = None,
         initial_guess=None,
         f_tolerance=1e-7,
         max_iterations=1500,
         lmbd=.1,
         verbose=False,
@@ -152,28 +152,28 @@
             )
 
             theta_i[i] = theta
 
     return theta_i, desired_position, not error
 
 
-def ik(
+def full_ik(
         desired_transformation=None,
         fk: ForwardKinematic = None,
         initial_guess=None,
         epsilon_wb=1e-5,
         epsilon_vb=1e-5,
         max_iterations=1000,
         lmbd=.1,
         verbose=False,
         only_position=False,
         normalize=True):
-    # finding the thetas only for the position
+
     if only_position:
-        return ik_position(
+        return position_ik(
             desired_position=desired_transformation[:3],
             fk=fk,
             initial_guess=initial_guess,
             f_tolerance=epsilon_vb,
             max_iterations=max_iterations,
             lmbd=lmbd,
             verbose=not verbose)
@@ -217,41 +217,8 @@
         error = wb_err > epsilon_wb or vb_err > epsilon_vb
 
         i += 1
 
         if verbose:
             print(f'Iteration {i}, s = {s}')
 
-    success_de = False
-
-    if error:
-        theta_i, desired_pose, success_de = evolutive_ik(
-            desired_transformation=desired_transformation,
-            fk=fk,
-            initial_guess=initial_guess,
-            max_iterations=max_iterations,
-            verbose=verbose,
-        )
-
-        if not success_de:
-            theta_i, desired_pose, success_pose = ik_position(
-                desired_position=desired_transformation[:3],
-                fk=fk,
-                f_tolerance=epsilon_vb,
-                max_iterations=max_iterations,
-                lmbd=lmbd,
-                verbose=verbose
-            )
-
-    if normalize and not success_de:
-        for i in range(fk.len_links):
-            link_limits = fk.links[i].limits
-
-            theta = normalize_angle_between_limits(
-                theta_i[i],
-                link_limits[0],
-                link_limits[1]
-            )
-
-            theta_i[i] = theta
-
-    return theta_i, desired_pose, 'Full' if not error else 'Full - Evolutive' if success_de else 'Only Position' if success_pose else 'Failed'
+    return theta_i, desired_pose, np.linalg.norm(s)
```

### Comparing `rtb_toolbox-0.1.47/src/rtb_toolbox/link/__init__.py` & `rtb_toolbox-0.1.48/src/rtb_toolbox/link/__init__.py`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.47/src/rtb_toolbox/trajectory/__init__.py` & `rtb_toolbox-0.1.48/src/rtb_toolbox/trajectory/__init__.py`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.47/src/rtb_toolbox/utils/__init__.py` & `rtb_toolbox-0.1.48/src/rtb_toolbox/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.47/setup.py` & `rtb_toolbox-0.1.48/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'rtb_toolbox.utils']
 
 package_data = \
 {'': ['*'], 'rtb_toolbox': ['images/*']}
 
 setup_kwargs = {
     'name': 'rtb-toolbox',
-    'version': '0.1.47',
+    'version': '0.1.48',
     'description': '',
     'long_description': "# Robotic Tools\n\nRobotic tools is a library made to make some calculations easier, like robots forward\nkinematic's and dynamics. There is also an numerical implementation of inverse velocity kinematic's.\n\nYou can use this lib for any robot, since you have the Denavit Hartenberg parameters.\n\n## Forward Kinematics\n\nin order to use the forward kinematics, you gonna need the robot DH parameters. Then\nu can create a 'Link' object representation for each link, using the parameters.\n\n```python\nimport sympy as sp\nfrom lib.link import Link\n\nq1, q2, q3 = sp.symbols('q_1 q_2 q_3')\n\nj0 = Link([q1, 450, 150, sp.pi / 2])\nj1 = Link([q2, 0, 590, 0])\nj2 = Link([q3, 0, 130, sp.pi / 2])\n```\n\nFinally create an instance of the ForwardKinematic class, and pass a list with\nall links in the constructor. You can also pass an offset with the angles of home position.\n\n```python\nfrom lib.forward_kinematics import ForwardKinematic\n\nfk = ForwardKinematic([j0, j1, j2], offset=np.array([.0, .0, .0]))\n```\n\nThe ForwardKinematic class contains the symbolic matrices of transformations, like transformations\nfrom the reference frame to the i-th frame, the end-effector transformation matrix, the jacobian matrix, and other\nthings.\n\n## Inverse Kinematics\n\nTo use the inverse kinematics u need first to have the ForwardKinematic of the robot\n\n### Inverse Kinematics of Position\n\nThe inverse kinematics of position uses the Gradient Descent method to find an optimal solution\nfor the end-effector position.\n\nTo use it, as said before, u need the ForwardKinematic. Then, just import the ik_position\nmethod from lib.inverse_kinematics package\n\n```python\nimport numpy as np\nfrom lib.inverse_kinematics import ik_position\n\n# PX, Py, Pz\ndesired_position = np.array([.1, .4, .0])\n\nthetas, _, success = ik_position(\n  desired_position=desired_position,\n  fk=fk,\n  initial_guess=np.array([.2, .7, -.1]),\n  f_tolerance=1e-5,\n  max_iterations=1000,\n  lmbd=.1,\n  verbose=True\n)\n```\n\nOutput example of the inverse kinematics of position:\n![position ik](images/partial_ik.png)\n\n### Inverse Kinematics of Position and Orientation\n\nThe inverse kinematics of position and orientation uses the jacobian matrix and end-effector velocities\nnecessary to achive an wanted transformation. This method is also called inverse velocity kinematics. The\nend-effector velocities mentioned before are calculated using the methods explained in\nModern Robotics Book (http://hades.mech.northwestern.edu/index.php/Modern_Robotics).\n\n```python\nimport numpy as np\nfrom lib.inverse_kinematics import ik\n\n# Px, Py, Pz, Rx, Ry, Rz\ndesired_transformation = np.array([.1, .4, .0, 0, np.pi / 4, 0])\n\nthetas, _, success = ik(\n  desired_transformation=desired_transformation,\n  fk=fk,\n  initial_guess=np.array([.2, .7, -.1]),\n  epsilon_wb=1e-5,\n  epsilon_vb=1e-5,\n  max_iterations=1000,\n  lmbd=.1,\n  verbose=True,\n  only_position=False,\n  normalize=False\n)\n```\n\nOutput example for the inverse kinematics of position and orientation\n![position ik](images/full_ik.png)\n\n## Forward Dynamics\n\nIn order to compute the ForwardDynamics u first need the ForwardKinematic of the robot.\nWhen u instantiate the ForwardDynamic class, it will start to calculate the equations of motion (resulting torque's)\nin each link, so it can take a long time if you use the simplify method of sympy library.\n\nThe joint variables (thetas) need to be functions of time.\n\n```python\nfrom lib.symbols import t\nimport sympy as sp\n\nfrom lib.forward_kinematics import ForwardKinematic\nfrom lib.forward_dynamics import ForwardDynamics\nfrom lib.link import Link\n\n# To use the forward dynamics, the q's need to be functions of time\n\nq1 = sp.Function('q_1')(t)\nq2 = sp.Function('q_2')(t)\na1, a2 = sp.symbols('a_1 a_2')\n\nj0 = Link([q1, 0, a1, 0])\nj1 = Link([q2, 0, a2, 0])\n\nrr_fk = ForwardKinematic([j0, j1])\n\nfd = ForwardDynamics(rr_fk)\nfor eq in fd.equations:\n  print(' ')\n  sp.print_latex(sp.simplify(eq))\n  print(' ')\n```\n\nExample of forward dynamic equations of an RR planar robot\n![tau 1](images/tau1.png)\n![tau 2](images/tau2.png)",
     'author': 'Miguel',
     'author_email': 'miguellukas52@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `rtb_toolbox-0.1.47/PKG-INFO` & `rtb_toolbox-0.1.48/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtb-toolbox
-Version: 0.1.47
+Version: 0.1.48
 Summary: 
 Author: Miguel
 Author-email: miguellukas52@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

