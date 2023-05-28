# Comparing `tmp/joyrl-0.2.0.tar.gz` & `tmp/joyrl-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joyrl-0.2.0.tar", last modified: Sun May 28 10:35:26 2023, max compression
+gzip compressed data, was "joyrl-0.2.1.tar", last modified: Sun May 28 10:45:47 2023, max compression
```

## Comparing `joyrl-0.2.0.tar` & `joyrl-0.2.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 10:35:26.590222 joyrl-0.2.0/
--rw-rw-rw-   0        0        0     1097 2023-01-01 08:20:49.000000 joyrl-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     4412 2023-05-28 10:35:26.590222 joyrl-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3951 2023-01-01 08:20:49.000000 joyrl-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 10:35:26.557903 joyrl-0.2.0/joyrl/
--rw-rw-rw-   0        0        0      404 2023-05-27 12:56:56.000000 joyrl-0.2.0/joyrl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:35:26.572968 joyrl-0.2.0/joyrl/algos/
-drwxrwxrwx   0        0        0        0 2023-05-28 10:35:26.576070 joyrl-0.2.0/joyrl/algos/DQN/
--rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.0/joyrl/algos/DQN/__init__.py
--rw-rw-rw-   0        0        0     1109 2023-05-27 12:54:10.000000 joyrl-0.2.0/joyrl/algos/DQN/config.py
--rw-rw-rw-   0        0        0      356 2023-05-27 12:54:42.000000 joyrl-0.2.0/joyrl/algos/DQN/data_handler.py
--rw-rw-rw-   0        0        0     4101 2023-05-27 12:54:25.000000 joyrl-0.2.0/joyrl/algos/DQN/policy.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:35:26.579064 joyrl-0.2.0/joyrl/algos/DoubleDQN/
--rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.0/joyrl/algos/DoubleDQN/__init__.py
--rw-rw-rw-   0        0        0     5273 2023-03-15 14:04:30.000000 joyrl-0.2.0/joyrl/algos/DoubleDQN/agent.py
--rw-rw-rw-   0        0        0      962 2023-03-15 14:04:45.000000 joyrl-0.2.0/joyrl/algos/DoubleDQN/config.py
--rw-rw-rw-   0        0        0     1507 2023-03-15 14:05:03.000000 joyrl-0.2.0/joyrl/algos/DoubleDQN/trainer.py
--rw-rw-rw-   0        0        0      269 2023-03-15 14:05:31.000000 joyrl-0.2.0/joyrl/algos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:35:26.580060 joyrl-0.2.0/joyrl/config/
--rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.0/joyrl/config/__init__.py
--rw-rw-rw-   0        0        0     1834 2023-05-27 12:20:08.000000 joyrl-0.2.0/joyrl/config/config.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:35:26.589225 joyrl-0.2.0/joyrl/envs/
--rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.0/joyrl/envs/__init__.py
--rw-rw-rw-   0        0        0     4380 2023-01-01 08:20:49.000000 joyrl-0.2.0/joyrl/envs/blackjack.py
--rw-rw-rw-   0        0        0     2790 2023-01-01 08:20:49.000000 joyrl-0.2.0/joyrl/envs/cliff_walking.py
--rw-rw-rw-   0        0        0     3996 2023-01-01 08:20:49.000000 joyrl-0.2.0/joyrl/envs/gridworld.py
--rw-rw-rw-   0        0        0     3584 2023-01-01 08:20:49.000000 joyrl-0.2.0/joyrl/envs/gridworld_env.py
--rw-rw-rw-   0        0        0    10132 2023-01-01 08:20:49.000000 joyrl-0.2.0/joyrl/envs/racetrack.py
--rw-rw-rw-   0        0        0     1080 2023-01-01 08:20:49.000000 joyrl-0.2.0/joyrl/envs/register.py
--rw-rw-rw-   0        0        0     1364 2023-01-01 08:20:49.000000 joyrl-0.2.0/joyrl/envs/stochastic_mdp.py
--rw-rw-rw-   0        0        0     2697 2023-01-01 08:20:49.000000 joyrl-0.2.0/joyrl/envs/windy_gridworld.py
--rw-rw-rw-   0        0        0     2652 2023-01-01 08:20:49.000000 joyrl-0.2.0/joyrl/envs/wrappers.py
--rw-rw-rw-   0        0        0     6967 2023-05-27 12:58:24.000000 joyrl-0.2.0/joyrl/run.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:35:26.572968 joyrl-0.2.0/joyrl.egg-info/
--rw-rw-rw-   0        0        0     4412 2023-05-28 10:35:26.000000 joyrl-0.2.0/joyrl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      781 2023-05-28 10:35:26.000000 joyrl-0.2.0/joyrl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 10:35:26.000000 joyrl-0.2.0/joyrl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      232 2023-05-28 10:35:26.000000 joyrl-0.2.0/joyrl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-28 10:35:26.000000 joyrl-0.2.0/joyrl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      995 2023-05-28 10:35:26.597300 joyrl-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1605 2023-03-15 14:05:51.000000 joyrl-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:45:47.062680 joyrl-0.2.1/
+-rw-rw-rw-   0        0        0     1097 2023-01-01 08:20:49.000000 joyrl-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     4410 2023-05-28 10:45:47.062680 joyrl-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3951 2023-01-01 08:20:49.000000 joyrl-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 10:45:47.040545 joyrl-0.2.1/joyrl/
+-rw-rw-rw-   0        0        0      404 2023-05-28 10:44:45.000000 joyrl-0.2.1/joyrl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:45:47.047701 joyrl-0.2.1/joyrl/algos/
+drwxrwxrwx   0        0        0        0 2023-05-28 10:45:47.050720 joyrl-0.2.1/joyrl/algos/DQN/
+-rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.1/joyrl/algos/DQN/__init__.py
+-rw-rw-rw-   0        0        0     1109 2023-05-27 12:54:10.000000 joyrl-0.2.1/joyrl/algos/DQN/config.py
+-rw-rw-rw-   0        0        0      356 2023-05-27 12:54:42.000000 joyrl-0.2.1/joyrl/algos/DQN/data_handler.py
+-rw-rw-rw-   0        0        0     4101 2023-05-27 12:54:25.000000 joyrl-0.2.1/joyrl/algos/DQN/policy.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:45:47.053181 joyrl-0.2.1/joyrl/algos/DoubleDQN/
+-rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.1/joyrl/algos/DoubleDQN/__init__.py
+-rw-rw-rw-   0        0        0     5273 2023-03-15 14:04:30.000000 joyrl-0.2.1/joyrl/algos/DoubleDQN/agent.py
+-rw-rw-rw-   0        0        0      962 2023-03-15 14:04:45.000000 joyrl-0.2.1/joyrl/algos/DoubleDQN/config.py
+-rw-rw-rw-   0        0        0     1507 2023-03-15 14:05:03.000000 joyrl-0.2.1/joyrl/algos/DoubleDQN/trainer.py
+-rw-rw-rw-   0        0        0      269 2023-03-15 14:05:31.000000 joyrl-0.2.1/joyrl/algos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:45:47.054178 joyrl-0.2.1/joyrl/config/
+-rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.1/joyrl/config/__init__.py
+-rw-rw-rw-   0        0        0     1834 2023-05-27 12:20:08.000000 joyrl-0.2.1/joyrl/config/config.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:45:47.061681 joyrl-0.2.1/joyrl/envs/
+-rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.1/joyrl/envs/__init__.py
+-rw-rw-rw-   0        0        0     4380 2023-01-01 08:20:49.000000 joyrl-0.2.1/joyrl/envs/blackjack.py
+-rw-rw-rw-   0        0        0     2790 2023-01-01 08:20:49.000000 joyrl-0.2.1/joyrl/envs/cliff_walking.py
+-rw-rw-rw-   0        0        0     3996 2023-01-01 08:20:49.000000 joyrl-0.2.1/joyrl/envs/gridworld.py
+-rw-rw-rw-   0        0        0     3584 2023-01-01 08:20:49.000000 joyrl-0.2.1/joyrl/envs/gridworld_env.py
+-rw-rw-rw-   0        0        0    10132 2023-01-01 08:20:49.000000 joyrl-0.2.1/joyrl/envs/racetrack.py
+-rw-rw-rw-   0        0        0     1080 2023-01-01 08:20:49.000000 joyrl-0.2.1/joyrl/envs/register.py
+-rw-rw-rw-   0        0        0     1364 2023-01-01 08:20:49.000000 joyrl-0.2.1/joyrl/envs/stochastic_mdp.py
+-rw-rw-rw-   0        0        0     2697 2023-01-01 08:20:49.000000 joyrl-0.2.1/joyrl/envs/windy_gridworld.py
+-rw-rw-rw-   0        0        0     2652 2023-01-01 08:20:49.000000 joyrl-0.2.1/joyrl/envs/wrappers.py
+-rw-rw-rw-   0        0        0     6967 2023-05-27 12:58:24.000000 joyrl-0.2.1/joyrl/run.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:45:47.046704 joyrl-0.2.1/joyrl.egg-info/
+-rw-rw-rw-   0        0        0     4410 2023-05-28 10:45:46.000000 joyrl-0.2.1/joyrl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      781 2023-05-28 10:45:46.000000 joyrl-0.2.1/joyrl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 10:45:46.000000 joyrl-0.2.1/joyrl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      350 2023-05-28 10:45:46.000000 joyrl-0.2.1/joyrl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-28 10:45:46.000000 joyrl-0.2.1/joyrl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      995 2023-05-28 10:45:47.064674 joyrl-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1820 2023-05-28 10:45:17.000000 joyrl-0.2.1/setup.py
```

### Comparing `joyrl-0.2.0/LICENSE` & `joyrl-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.0/PKG-INFO` & `joyrl-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joyrl
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Library for Deep Reinforcement Learning
 Home-page: https://github.com/datawhalechina/joyrl
 Author: johnjim0816
 Author-email: johnjim0816@gmail.com
 License: MIT
 Keywords: reinforcement learning platform pytorch
 Platform: any
@@ -86,8 +86,7 @@
 
 More tutorials and API documentation are hosted on [https://datawhalechina.github.io/joyrl/](https://datawhalechina.github.io/joyrl/)
 ## Algorithms
 
 |       Name       |                          Reference                           |                    Author                     | Notes |
 | :--------------: | :----------------------------------------------------------: | :-------------------------------------------: | :---: |
 | DQN | [DQN Paper](https://www.cs.toronto.edu/~vmnih/docs/dqn.pdf) | [johnjim0816](https://github.com/johnjim0816) |       |
-
```

### Comparing `joyrl-0.2.0/README.md` & `joyrl-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.0/joyrl/algos/DQN/config.py` & `joyrl-0.2.1/joyrl/algos/DQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.0/joyrl/algos/DQN/policy.py` & `joyrl-0.2.1/joyrl/algos/DQN/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.0/joyrl/algos/DoubleDQN/agent.py` & `joyrl-0.2.1/joyrl/algos/DoubleDQN/agent.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.0/joyrl/algos/DoubleDQN/config.py` & `joyrl-0.2.1/joyrl/algos/DoubleDQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.0/joyrl/algos/DoubleDQN/trainer.py` & `joyrl-0.2.1/joyrl/algos/DoubleDQN/trainer.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.0/joyrl/config/config.py` & `joyrl-0.2.1/joyrl/config/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.0/joyrl/envs/blackjack.py` & `joyrl-0.2.1/joyrl/envs/blackjack.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.0/joyrl/envs/cliff_walking.py` & `joyrl-0.2.1/joyrl/envs/cliff_walking.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.0/joyrl/envs/gridworld.py` & `joyrl-0.2.1/joyrl/envs/gridworld.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.0/joyrl/envs/gridworld_env.py` & `joyrl-0.2.1/joyrl/envs/gridworld_env.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.0/joyrl/envs/racetrack.py` & `joyrl-0.2.1/joyrl/envs/racetrack.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.0/joyrl/envs/register.py` & `joyrl-0.2.1/joyrl/envs/register.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.0/joyrl/envs/stochastic_mdp.py` & `joyrl-0.2.1/joyrl/envs/stochastic_mdp.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.0/joyrl/envs/windy_gridworld.py` & `joyrl-0.2.1/joyrl/envs/windy_gridworld.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.0/joyrl/envs/wrappers.py` & `joyrl-0.2.1/joyrl/envs/wrappers.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.0/joyrl/run.py` & `joyrl-0.2.1/joyrl/run.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.0/joyrl.egg-info/PKG-INFO` & `joyrl-0.2.1/joyrl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joyrl
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Library for Deep Reinforcement Learning
 Home-page: https://github.com/datawhalechina/joyrl
 Author: johnjim0816
 Author-email: johnjim0816@gmail.com
 License: MIT
 Keywords: reinforcement learning platform pytorch
 Platform: any
@@ -86,8 +86,7 @@
 
 More tutorials and API documentation are hosted on [https://datawhalechina.github.io/joyrl/](https://datawhalechina.github.io/joyrl/)
 ## Algorithms
 
 |       Name       |                          Reference                           |                    Author                     | Notes |
 | :--------------: | :----------------------------------------------------------: | :-------------------------------------------: | :---: |
 | DQN | [DQN Paper](https://www.cs.toronto.edu/~vmnih/docs/dqn.pdf) | [johnjim0816](https://github.com/johnjim0816) |       |
-
```

### Comparing `joyrl-0.2.0/joyrl.egg-info/SOURCES.txt` & `joyrl-0.2.1/joyrl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.0/setup.cfg` & `joyrl-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.0/setup.py` & `joyrl-0.2.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,24 +6,32 @@
     # https://packaging.python.org/guides/single-sourcing-package-version/
     init = open(os.path.join("joyrl", "__init__.py"), "r").read().split()
     return init[init.index("__version__") + 2][1:-1]
 
 
 def get_install_requires() -> str:
     return [
-        "gym==0.25.2",
-        "pyyaml==6.0",
-        "matplotlib==3.5.3",
-        "seaborn==0.12.1",
-        "dill==0.3.5.1",
         "argparse==1.4.0",
-        "pandas==1.3.5",
-        "pyglet==1.5.26",
+        "dill==0.3.5.1",
+        "glfw==2.5.5",
+        "gymnasium==0.28.1",
+        "imageio==2.22.4",
         "importlib-metadata<5.0",
-        "setuptools==65.2.0"
+        "matplotlib==3.5.3",
+        "numpy==1.24.3",
+        "pandas==1.3.5",
+        "Pillow==9.4.0",
+        "pygame==2.1.2",
+        "pyglet==2.0.0",
+        "pyyaml==6.0",
+        "ray==2.3.0",
+        "six==1.16.0",
+        "seaborn==0.12.1",
+        "setuptools==59.5.0",
+        "tensorboard==2.11.2",
     ]
 
 
 def get_extras_require() -> str:
     req = {
         "atari": ["atari_py", "opencv-python"],
         "mujoco": ["mujoco_py"],
```

