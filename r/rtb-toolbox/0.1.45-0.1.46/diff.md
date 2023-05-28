# Comparing `tmp/rtb_toolbox-0.1.45.tar.gz` & `tmp/rtb_toolbox-0.1.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtb_toolbox-0.1.45.tar", max compression
+gzip compressed data, was "rtb_toolbox-0.1.46.tar", max compression
```

## Comparing `rtb_toolbox-0.1.45.tar` & `rtb_toolbox-0.1.46.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     4034 2023-04-14 22:16:46.136319 rtb_toolbox-0.1.45/README.md
--rw-r--r--   0        0        0      323 2023-05-28 00:57:22.501507 rtb_toolbox-0.1.45/pyproject.toml
--rw-r--r--   0        0        0     4034 2023-04-14 22:17:39.372360 rtb_toolbox-0.1.45/src/rtb_toolbox/README.md
--rw-r--r--   0        0        0      297 2023-05-27 00:03:43.689963 rtb_toolbox-0.1.45/src/rtb_toolbox/__init__.py
--rw-r--r--   0        0        0     2298 2023-04-14 22:12:18.847856 rtb_toolbox-0.1.45/src/rtb_toolbox/forward_dynamics/__init__.py
--rw-r--r--   0        0        0     3636 2023-05-28 00:44:55.252589 rtb_toolbox-0.1.45/src/rtb_toolbox/forward_kinematics/__init__.py
--rw-r--r--   0        0        0     3232 2023-05-28 00:45:48.876655 rtb_toolbox-0.1.45/src/rtb_toolbox/frame/__init__.py
--rw-r--r--   0        0        0    33140 2023-04-14 21:54:20.903286 rtb_toolbox-0.1.45/src/rtb_toolbox/images/full_ik.png
--rw-r--r--   0        0        0    33229 2023-04-14 21:54:20.907286 rtb_toolbox-0.1.45/src/rtb_toolbox/images/partial_ik.png
--rw-r--r--   0        0        0     6569 2023-04-14 21:54:20.915286 rtb_toolbox-0.1.45/src/rtb_toolbox/images/tau1.png
--rw-r--r--   0        0        0     5005 2023-04-14 21:54:20.915286 rtb_toolbox-0.1.45/src/rtb_toolbox/images/tau2.png
--rw-r--r--   0        0        0   479230 2023-04-14 21:54:20.923286 rtb_toolbox-0.1.45/src/rtb_toolbox/images/trajectories.png
--rw-r--r--   0        0        0     7449 2023-05-28 00:56:24.869436 rtb_toolbox-0.1.45/src/rtb_toolbox/inverse_kinematics/__init__.py
--rw-r--r--   0        0        0     1681 2023-05-28 00:44:50.244583 rtb_toolbox-0.1.45/src/rtb_toolbox/link/__init__.py
--rw-r--r--   0        0        0      408 2023-05-27 17:37:29.169298 rtb_toolbox-0.1.45/src/rtb_toolbox/robots/SCARA.py
--rw-r--r--   0        0        0      510 2023-05-27 23:57:51.896877 rtb_toolbox-0.1.45/src/rtb_toolbox/robots/puma260.py
--rw-r--r--   0        0        0       55 2023-04-14 21:52:22.347973 rtb_toolbox-0.1.45/src/rtb_toolbox/symbols.py
--rw-r--r--   0        0        0     1150 2023-04-14 21:52:22.231974 rtb_toolbox-0.1.45/src/rtb_toolbox/trajectory/__init__.py
--rw-r--r--   0        0        0     4919 2023-05-27 00:08:26.422563 rtb_toolbox-0.1.45/src/rtb_toolbox/utils/__init__.py
--rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 rtb_toolbox-0.1.45/setup.py
--rw-r--r--   0        0        0     4374 1970-01-01 00:00:00.000000 rtb_toolbox-0.1.45/PKG-INFO
+-rw-r--r--   0        0        0     4034 2023-04-14 22:16:46.136319 rtb_toolbox-0.1.46/README.md
+-rw-r--r--   0        0        0      323 2023-05-28 01:06:51.462215 rtb_toolbox-0.1.46/pyproject.toml
+-rw-r--r--   0        0        0     4034 2023-04-14 22:17:39.372360 rtb_toolbox-0.1.46/src/rtb_toolbox/README.md
+-rw-r--r--   0        0        0      297 2023-05-27 00:03:43.689963 rtb_toolbox-0.1.46/src/rtb_toolbox/__init__.py
+-rw-r--r--   0        0        0     2298 2023-04-14 22:12:18.847856 rtb_toolbox-0.1.46/src/rtb_toolbox/forward_dynamics/__init__.py
+-rw-r--r--   0        0        0     3636 2023-05-28 00:44:55.252589 rtb_toolbox-0.1.46/src/rtb_toolbox/forward_kinematics/__init__.py
+-rw-r--r--   0        0        0     3232 2023-05-28 00:45:48.876655 rtb_toolbox-0.1.46/src/rtb_toolbox/frame/__init__.py
+-rw-r--r--   0        0        0    33140 2023-04-14 21:54:20.903286 rtb_toolbox-0.1.46/src/rtb_toolbox/images/full_ik.png
+-rw-r--r--   0        0        0    33229 2023-04-14 21:54:20.907286 rtb_toolbox-0.1.46/src/rtb_toolbox/images/partial_ik.png
+-rw-r--r--   0        0        0     6569 2023-04-14 21:54:20.915286 rtb_toolbox-0.1.46/src/rtb_toolbox/images/tau1.png
+-rw-r--r--   0        0        0     5005 2023-04-14 21:54:20.915286 rtb_toolbox-0.1.46/src/rtb_toolbox/images/tau2.png
+-rw-r--r--   0        0        0   479230 2023-04-14 21:54:20.923286 rtb_toolbox-0.1.46/src/rtb_toolbox/images/trajectories.png
+-rw-r--r--   0        0        0     7411 2023-05-28 01:06:06.522155 rtb_toolbox-0.1.46/src/rtb_toolbox/inverse_kinematics/__init__.py
+-rw-r--r--   0        0        0     1681 2023-05-28 00:44:50.244583 rtb_toolbox-0.1.46/src/rtb_toolbox/link/__init__.py
+-rw-r--r--   0        0        0      408 2023-05-27 17:37:29.169298 rtb_toolbox-0.1.46/src/rtb_toolbox/robots/SCARA.py
+-rw-r--r--   0        0        0      674 2023-05-28 01:06:43.874203 rtb_toolbox-0.1.46/src/rtb_toolbox/robots/comau.py
+-rw-r--r--   0        0        0      510 2023-05-27 23:57:51.896877 rtb_toolbox-0.1.46/src/rtb_toolbox/robots/puma260.py
+-rw-r--r--   0        0        0       55 2023-04-14 21:52:22.347973 rtb_toolbox-0.1.46/src/rtb_toolbox/symbols.py
+-rw-r--r--   0        0        0     1150 2023-04-14 21:52:22.231974 rtb_toolbox-0.1.46/src/rtb_toolbox/trajectory/__init__.py
+-rw-r--r--   0        0        0     4919 2023-05-27 00:08:26.422563 rtb_toolbox-0.1.46/src/rtb_toolbox/utils/__init__.py
+-rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 rtb_toolbox-0.1.46/setup.py
+-rw-r--r--   0        0        0     4374 1970-01-01 00:00:00.000000 rtb_toolbox-0.1.46/PKG-INFO
```

### Comparing `rtb_toolbox-0.1.45/README.md` & `rtb_toolbox-0.1.46/README.md`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.45/src/rtb_toolbox/README.md` & `rtb_toolbox-0.1.46/src/rtb_toolbox/README.md`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.45/src/rtb_toolbox/forward_dynamics/__init__.py` & `rtb_toolbox-0.1.46/src/rtb_toolbox/forward_dynamics/__init__.py`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.45/src/rtb_toolbox/forward_kinematics/__init__.py` & `rtb_toolbox-0.1.46/src/rtb_toolbox/forward_kinematics/__init__.py`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.45/src/rtb_toolbox/frame/__init__.py` & `rtb_toolbox-0.1.46/src/rtb_toolbox/frame/__init__.py`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.45/src/rtb_toolbox/images/full_ik.png` & `rtb_toolbox-0.1.46/src/rtb_toolbox/images/full_ik.png`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.45/src/rtb_toolbox/images/partial_ik.png` & `rtb_toolbox-0.1.46/src/rtb_toolbox/images/partial_ik.png`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.45/src/rtb_toolbox/images/tau1.png` & `rtb_toolbox-0.1.46/src/rtb_toolbox/images/tau1.png`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.45/src/rtb_toolbox/images/tau2.png` & `rtb_toolbox-0.1.46/src/rtb_toolbox/images/tau2.png`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.45/src/rtb_toolbox/images/trajectories.png` & `rtb_toolbox-0.1.46/src/rtb_toolbox/images/trajectories.png`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.45/src/rtb_toolbox/inverse_kinematics/__init__.py` & `rtb_toolbox-0.1.46/src/rtb_toolbox/inverse_kinematics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,21 +11,19 @@
 
 
 class InverseKinematicProblem(Problem):
     def __init__(
             self,
             desired_pose=None,
             fk: ForwardKinematic = None,
-            n_var=6,
-            n_obj=1,
     ):
         lb = [fk.links[i].limits[0] for i in range(fk.len_links)]
         ub = [fk.links[i].limits[1] for i in range(fk.len_links)]
 
-        super().__init__(n_var=n_var, n_obj=n_obj, n_constr=0, xl=lb, xu=ub)
+        super().__init__(n_var=fk.len_links, n_obj=1, n_constr=0, xl=lb, xu=ub)
 
         self.desired_pose = desired_pose
         self.fk = fk
     
     def _evaluate(self, X, out, *args, **kwargs):
         iters = X.shape[0]
         F = np.zeros((iters, 1))
@@ -81,27 +79,27 @@
         from pymoo.algorithms.soo.nonconvex.cmaes import CMAES
 
         algorithm = CMAES(
             restarts=2,
             bipop=True,
             sigma=1,
             tolfun=1e-8,
-            tolx=1e-8
+            tolx=1e-8,
         )
 
     res = minimize(
         problem,
         algorithm,
         termination,
         verbose=verbose,
         save_history=False,
     )
 
     theta_i = res.X
-    success = res.F.min() < 1e-7
+    success = res.F.min() < 1e-5
 
     return theta_i, desired_pose, success
 
 
 def ik_position(
         desired_position=None,
         fk: ForwardKinematic = None,
```

### Comparing `rtb_toolbox-0.1.45/src/rtb_toolbox/link/__init__.py` & `rtb_toolbox-0.1.46/src/rtb_toolbox/link/__init__.py`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.45/src/rtb_toolbox/trajectory/__init__.py` & `rtb_toolbox-0.1.46/src/rtb_toolbox/trajectory/__init__.py`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.45/src/rtb_toolbox/utils/__init__.py` & `rtb_toolbox-0.1.46/src/rtb_toolbox/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.45/setup.py` & `rtb_toolbox-0.1.46/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'rtb_toolbox.utils']
 
 package_data = \
 {'': ['*'], 'rtb_toolbox': ['images/*']}
 
 setup_kwargs = {
     'name': 'rtb-toolbox',
-    'version': '0.1.45',
+    'version': '0.1.46',
     'description': '',
     'long_description': "# Robotic Tools\n\nRobotic tools is a library made to make some calculations easier, like robots forward\nkinematic's and dynamics. There is also an numerical implementation of inverse velocity kinematic's.\n\nYou can use this lib for any robot, since you have the Denavit Hartenberg parameters.\n\n## Forward Kinematics\n\nin order to use the forward kinematics, you gonna need the robot DH parameters. Then\nu can create a 'Link' object representation for each link, using the parameters.\n\n```python\nimport sympy as sp\nfrom lib.link import Link\n\nq1, q2, q3 = sp.symbols('q_1 q_2 q_3')\n\nj0 = Link([q1, 450, 150, sp.pi / 2])\nj1 = Link([q2, 0, 590, 0])\nj2 = Link([q3, 0, 130, sp.pi / 2])\n```\n\nFinally create an instance of the ForwardKinematic class, and pass a list with\nall links in the constructor. You can also pass an offset with the angles of home position.\n\n```python\nfrom lib.forward_kinematics import ForwardKinematic\n\nfk = ForwardKinematic([j0, j1, j2], offset=np.array([.0, .0, .0]))\n```\n\nThe ForwardKinematic class contains the symbolic matrices of transformations, like transformations\nfrom the reference frame to the i-th frame, the end-effector transformation matrix, the jacobian matrix, and other\nthings.\n\n## Inverse Kinematics\n\nTo use the inverse kinematics u need first to have the ForwardKinematic of the robot\n\n### Inverse Kinematics of Position\n\nThe inverse kinematics of position uses the Gradient Descent method to find an optimal solution\nfor the end-effector position.\n\nTo use it, as said before, u need the ForwardKinematic. Then, just import the ik_position\nmethod from lib.inverse_kinematics package\n\n```python\nimport numpy as np\nfrom lib.inverse_kinematics import ik_position\n\n# PX, Py, Pz\ndesired_position = np.array([.1, .4, .0])\n\nthetas, _, success = ik_position(\n  desired_position=desired_position,\n  fk=fk,\n  initial_guess=np.array([.2, .7, -.1]),\n  f_tolerance=1e-5,\n  max_iterations=1000,\n  lmbd=.1,\n  verbose=True\n)\n```\n\nOutput example of the inverse kinematics of position:\n![position ik](images/partial_ik.png)\n\n### Inverse Kinematics of Position and Orientation\n\nThe inverse kinematics of position and orientation uses the jacobian matrix and end-effector velocities\nnecessary to achive an wanted transformation. This method is also called inverse velocity kinematics. The\nend-effector velocities mentioned before are calculated using the methods explained in\nModern Robotics Book (http://hades.mech.northwestern.edu/index.php/Modern_Robotics).\n\n```python\nimport numpy as np\nfrom lib.inverse_kinematics import ik\n\n# Px, Py, Pz, Rx, Ry, Rz\ndesired_transformation = np.array([.1, .4, .0, 0, np.pi / 4, 0])\n\nthetas, _, success = ik(\n  desired_transformation=desired_transformation,\n  fk=fk,\n  initial_guess=np.array([.2, .7, -.1]),\n  epsilon_wb=1e-5,\n  epsilon_vb=1e-5,\n  max_iterations=1000,\n  lmbd=.1,\n  verbose=True,\n  only_position=False,\n  normalize=False\n)\n```\n\nOutput example for the inverse kinematics of position and orientation\n![position ik](images/full_ik.png)\n\n## Forward Dynamics\n\nIn order to compute the ForwardDynamics u first need the ForwardKinematic of the robot.\nWhen u instantiate the ForwardDynamic class, it will start to calculate the equations of motion (resulting torque's)\nin each link, so it can take a long time if you use the simplify method of sympy library.\n\nThe joint variables (thetas) need to be functions of time.\n\n```python\nfrom lib.symbols import t\nimport sympy as sp\n\nfrom lib.forward_kinematics import ForwardKinematic\nfrom lib.forward_dynamics import ForwardDynamics\nfrom lib.link import Link\n\n# To use the forward dynamics, the q's need to be functions of time\n\nq1 = sp.Function('q_1')(t)\nq2 = sp.Function('q_2')(t)\na1, a2 = sp.symbols('a_1 a_2')\n\nj0 = Link([q1, 0, a1, 0])\nj1 = Link([q2, 0, a2, 0])\n\nrr_fk = ForwardKinematic([j0, j1])\n\nfd = ForwardDynamics(rr_fk)\nfor eq in fd.equations:\n  print(' ')\n  sp.print_latex(sp.simplify(eq))\n  print(' ')\n```\n\nExample of forward dynamic equations of an RR planar robot\n![tau 1](images/tau1.png)\n![tau 2](images/tau2.png)",
     'author': 'Miguel',
     'author_email': 'miguellukas52@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `rtb_toolbox-0.1.45/PKG-INFO` & `rtb_toolbox-0.1.46/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtb-toolbox
-Version: 0.1.45
+Version: 0.1.46
 Summary: 
 Author: Miguel
 Author-email: miguellukas52@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```
