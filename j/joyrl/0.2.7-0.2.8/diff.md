# Comparing `tmp/joyrl-0.2.7.tar.gz` & `tmp/joyrl-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joyrl-0.2.7.tar", last modified: Sun May 28 11:00:15 2023, max compression
+gzip compressed data, was "joyrl-0.2.8.tar", last modified: Sun May 28 12:09:41 2023, max compression
```

## Comparing `joyrl-0.2.7.tar` & `joyrl-0.2.8.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 11:00:15.073170 joyrl-0.2.7/
--rw-rw-rw-   0        0        0     1097 2023-01-01 08:20:49.000000 joyrl-0.2.7/LICENSE
--rw-rw-rw-   0        0        0     4412 2023-05-28 11:00:15.073170 joyrl-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     3951 2023-01-01 08:20:49.000000 joyrl-0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 11:00:15.043450 joyrl-0.2.7/joyrl/
--rw-rw-rw-   0        0        0      404 2023-05-28 11:00:13.000000 joyrl-0.2.7/joyrl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 11:00:15.054790 joyrl-0.2.7/joyrl/algos/
-drwxrwxrwx   0        0        0        0 2023-05-28 11:00:15.056784 joyrl-0.2.7/joyrl/algos/DQN/
--rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.7/joyrl/algos/DQN/__init__.py
--rw-rw-rw-   0        0        0     1109 2023-05-27 12:54:10.000000 joyrl-0.2.7/joyrl/algos/DQN/config.py
--rw-rw-rw-   0        0        0      356 2023-05-27 12:54:42.000000 joyrl-0.2.7/joyrl/algos/DQN/data_handler.py
--rw-rw-rw-   0        0        0     4101 2023-05-27 12:54:25.000000 joyrl-0.2.7/joyrl/algos/DQN/policy.py
-drwxrwxrwx   0        0        0        0 2023-05-28 11:00:15.059777 joyrl-0.2.7/joyrl/algos/DoubleDQN/
--rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.7/joyrl/algos/DoubleDQN/__init__.py
--rw-rw-rw-   0        0        0     5273 2023-03-15 14:04:30.000000 joyrl-0.2.7/joyrl/algos/DoubleDQN/agent.py
--rw-rw-rw-   0        0        0      962 2023-03-15 14:04:45.000000 joyrl-0.2.7/joyrl/algos/DoubleDQN/config.py
--rw-rw-rw-   0        0        0     1507 2023-03-15 14:05:03.000000 joyrl-0.2.7/joyrl/algos/DoubleDQN/trainer.py
--rw-rw-rw-   0        0        0      269 2023-03-15 14:05:31.000000 joyrl-0.2.7/joyrl/algos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 11:00:15.059777 joyrl-0.2.7/joyrl/config/
--rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.7/joyrl/config/__init__.py
--rw-rw-rw-   0        0        0     1834 2023-05-27 12:20:08.000000 joyrl-0.2.7/joyrl/config/config.py
-drwxrwxrwx   0        0        0        0 2023-05-28 11:00:15.066780 joyrl-0.2.7/joyrl/envs/
--rw-rw-rw-   0        0        0       54 2023-05-28 10:53:02.000000 joyrl-0.2.7/joyrl/envs/__init__.py
--rw-rw-rw-   0        0        0     4380 2023-01-01 08:20:49.000000 joyrl-0.2.7/joyrl/envs/blackjack.py
--rw-rw-rw-   0        0        0     2790 2023-01-01 08:20:49.000000 joyrl-0.2.7/joyrl/envs/cliff_walking.py
--rw-rw-rw-   0        0        0     3996 2023-01-01 08:20:49.000000 joyrl-0.2.7/joyrl/envs/gridworld.py
--rw-rw-rw-   0        0        0     3584 2023-01-01 08:20:49.000000 joyrl-0.2.7/joyrl/envs/gridworld_env.py
-drwxrwxrwx   0        0        0        0 2023-05-28 11:00:15.067777 joyrl-0.2.7/joyrl/envs/gym/
--rw-rw-rw-   0        0        0      194 2023-05-28 10:49:52.000000 joyrl-0.2.7/joyrl/envs/gym/__init__.py
--rw-rw-rw-   0        0        0      485 2023-05-27 12:55:35.000000 joyrl-0.2.7/joyrl/envs/gym/config.py
--rw-rw-rw-   0        0        0    10132 2023-01-01 08:20:49.000000 joyrl-0.2.7/joyrl/envs/racetrack.py
--rw-rw-rw-   0        0        0     1080 2023-01-01 08:20:49.000000 joyrl-0.2.7/joyrl/envs/register.py
--rw-rw-rw-   0        0        0     1364 2023-01-01 08:20:49.000000 joyrl-0.2.7/joyrl/envs/stochastic_mdp.py
--rw-rw-rw-   0        0        0     2697 2023-01-01 08:20:49.000000 joyrl-0.2.7/joyrl/envs/windy_gridworld.py
--rw-rw-rw-   0        0        0     2652 2023-01-01 08:20:49.000000 joyrl-0.2.7/joyrl/envs/wrappers.py
-drwxrwxrwx   0        0        0        0 2023-05-28 11:00:15.070769 joyrl-0.2.7/joyrl/framework/
--rw-rw-rw-   0        0        0      194 2023-05-28 10:49:40.000000 joyrl-0.2.7/joyrl/framework/__init__.py
--rw-rw-rw-   0        0        0     1332 2023-05-27 12:46:42.000000 joyrl-0.2.7/joyrl/framework/dataserver.py
--rw-rw-rw-   0        0        0     2894 2023-05-27 12:46:27.000000 joyrl-0.2.7/joyrl/framework/learners.py
--rw-rw-rw-   0        0        0     5249 2023-05-27 12:48:22.000000 joyrl-0.2.7/joyrl/framework/stats.py
--rw-rw-rw-   0        0        0     5923 2023-05-27 12:44:48.000000 joyrl-0.2.7/joyrl/framework/workers.py
--rw-rw-rw-   0        0        0     7028 2023-05-28 11:00:00.000000 joyrl-0.2.7/joyrl/run.py
-drwxrwxrwx   0        0        0        0 2023-05-28 11:00:15.073170 joyrl-0.2.7/joyrl/utils/
--rw-rw-rw-   0        0        0        2 2023-05-28 10:53:04.000000 joyrl-0.2.7/joyrl/utils/__init__.py
--rw-rw-rw-   0        0        0    36574 2023-05-27 12:50:57.000000 joyrl-0.2.7/joyrl/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-28 11:00:15.053793 joyrl-0.2.7/joyrl.egg-info/
--rw-rw-rw-   0        0        0     4412 2023-05-28 11:00:14.000000 joyrl-0.2.7/joyrl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1016 2023-05-28 11:00:14.000000 joyrl-0.2.7/joyrl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 11:00:14.000000 joyrl-0.2.7/joyrl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      350 2023-05-28 11:00:14.000000 joyrl-0.2.7/joyrl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-28 11:00:14.000000 joyrl-0.2.7/joyrl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      995 2023-05-28 11:00:15.075170 joyrl-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1820 2023-05-28 10:45:17.000000 joyrl-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:09:41.417931 joyrl-0.2.8/
+-rw-rw-rw-   0        0        0     1097 2023-01-01 08:20:49.000000 joyrl-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0     4412 2023-05-28 12:09:41.417931 joyrl-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3951 2023-01-01 08:20:49.000000 joyrl-0.2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 12:09:41.387927 joyrl-0.2.8/joyrl/
+-rw-rw-rw-   0        0        0      404 2023-05-28 12:09:27.000000 joyrl-0.2.8/joyrl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:09:41.398695 joyrl-0.2.8/joyrl/algos/
+drwxrwxrwx   0        0        0        0 2023-05-28 12:09:41.400689 joyrl-0.2.8/joyrl/algos/DQN/
+-rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.8/joyrl/algos/DQN/__init__.py
+-rw-rw-rw-   0        0        0     1109 2023-05-27 12:54:10.000000 joyrl-0.2.8/joyrl/algos/DQN/config.py
+-rw-rw-rw-   0        0        0      356 2023-05-27 12:54:42.000000 joyrl-0.2.8/joyrl/algos/DQN/data_handler.py
+-rw-rw-rw-   0        0        0     4101 2023-05-27 12:54:25.000000 joyrl-0.2.8/joyrl/algos/DQN/policy.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:09:41.403193 joyrl-0.2.8/joyrl/algos/DoubleDQN/
+-rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.8/joyrl/algos/DoubleDQN/__init__.py
+-rw-rw-rw-   0        0        0     5273 2023-03-15 14:04:30.000000 joyrl-0.2.8/joyrl/algos/DoubleDQN/agent.py
+-rw-rw-rw-   0        0        0      962 2023-03-15 14:04:45.000000 joyrl-0.2.8/joyrl/algos/DoubleDQN/config.py
+-rw-rw-rw-   0        0        0     1507 2023-03-15 14:05:03.000000 joyrl-0.2.8/joyrl/algos/DoubleDQN/trainer.py
+-rw-rw-rw-   0        0        0      269 2023-03-15 14:05:31.000000 joyrl-0.2.8/joyrl/algos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:09:41.405190 joyrl-0.2.8/joyrl/config/
+-rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.8/joyrl/config/__init__.py
+-rw-rw-rw-   0        0        0     1711 2023-05-28 11:04:19.000000 joyrl-0.2.8/joyrl/config/config.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:09:41.411687 joyrl-0.2.8/joyrl/envs/
+-rw-rw-rw-   0        0        0       54 2023-05-28 10:53:02.000000 joyrl-0.2.8/joyrl/envs/__init__.py
+-rw-rw-rw-   0        0        0     4380 2023-01-01 08:20:49.000000 joyrl-0.2.8/joyrl/envs/blackjack.py
+-rw-rw-rw-   0        0        0     2790 2023-01-01 08:20:49.000000 joyrl-0.2.8/joyrl/envs/cliff_walking.py
+-rw-rw-rw-   0        0        0     3996 2023-01-01 08:20:49.000000 joyrl-0.2.8/joyrl/envs/gridworld.py
+-rw-rw-rw-   0        0        0     3584 2023-01-01 08:20:49.000000 joyrl-0.2.8/joyrl/envs/gridworld_env.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:09:41.412703 joyrl-0.2.8/joyrl/envs/gym/
+-rw-rw-rw-   0        0        0      194 2023-05-28 10:49:52.000000 joyrl-0.2.8/joyrl/envs/gym/__init__.py
+-rw-rw-rw-   0        0        0      485 2023-05-27 12:55:35.000000 joyrl-0.2.8/joyrl/envs/gym/config.py
+-rw-rw-rw-   0        0        0    10132 2023-01-01 08:20:49.000000 joyrl-0.2.8/joyrl/envs/racetrack.py
+-rw-rw-rw-   0        0        0     1080 2023-01-01 08:20:49.000000 joyrl-0.2.8/joyrl/envs/register.py
+-rw-rw-rw-   0        0        0     1364 2023-01-01 08:20:49.000000 joyrl-0.2.8/joyrl/envs/stochastic_mdp.py
+-rw-rw-rw-   0        0        0     2697 2023-01-01 08:20:49.000000 joyrl-0.2.8/joyrl/envs/windy_gridworld.py
+-rw-rw-rw-   0        0        0     2652 2023-01-01 08:20:49.000000 joyrl-0.2.8/joyrl/envs/wrappers.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:09:41.415938 joyrl-0.2.8/joyrl/framework/
+-rw-rw-rw-   0        0        0      194 2023-05-28 10:49:40.000000 joyrl-0.2.8/joyrl/framework/__init__.py
+-rw-rw-rw-   0        0        0     1332 2023-05-27 12:46:42.000000 joyrl-0.2.8/joyrl/framework/dataserver.py
+-rw-rw-rw-   0        0        0     2894 2023-05-27 12:46:27.000000 joyrl-0.2.8/joyrl/framework/learners.py
+-rw-rw-rw-   0        0        0     5249 2023-05-27 12:48:22.000000 joyrl-0.2.8/joyrl/framework/stats.py
+-rw-rw-rw-   0        0        0     5923 2023-05-27 12:44:48.000000 joyrl-0.2.8/joyrl/framework/workers.py
+-rw-rw-rw-   0        0        0     7036 2023-05-28 11:09:11.000000 joyrl-0.2.8/joyrl/run.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:09:41.417931 joyrl-0.2.8/joyrl/utils/
+-rw-rw-rw-   0        0        0        2 2023-05-28 10:53:04.000000 joyrl-0.2.8/joyrl/utils/__init__.py
+-rw-rw-rw-   0        0        0    36574 2023-05-27 12:50:57.000000 joyrl-0.2.8/joyrl/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:09:41.397697 joyrl-0.2.8/joyrl.egg-info/
+-rw-rw-rw-   0        0        0     4412 2023-05-28 12:09:41.000000 joyrl-0.2.8/joyrl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1016 2023-05-28 12:09:41.000000 joyrl-0.2.8/joyrl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 12:09:41.000000 joyrl-0.2.8/joyrl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      350 2023-05-28 12:09:41.000000 joyrl-0.2.8/joyrl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-28 12:09:41.000000 joyrl-0.2.8/joyrl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      995 2023-05-28 12:09:41.418930 joyrl-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     1820 2023-05-28 10:45:17.000000 joyrl-0.2.8/setup.py
```

### Comparing `joyrl-0.2.7/LICENSE` & `joyrl-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.7/PKG-INFO` & `joyrl-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joyrl
-Version: 0.2.7
+Version: 0.2.8
 Summary: A Library for Deep Reinforcement Learning
 Home-page: https://github.com/datawhalechina/joyrl
 Author: johnjim0816
 Author-email: johnjim0816@gmail.com
 License: MIT
 Keywords: reinforcement learning platform pytorch
 Platform: any
```

### Comparing `joyrl-0.2.7/README.md` & `joyrl-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.7/joyrl/algos/DQN/config.py` & `joyrl-0.2.8/joyrl/algos/DQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.7/joyrl/algos/DQN/policy.py` & `joyrl-0.2.8/joyrl/algos/DQN/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.7/joyrl/algos/DoubleDQN/agent.py` & `joyrl-0.2.8/joyrl/algos/DoubleDQN/agent.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.7/joyrl/algos/DoubleDQN/config.py` & `joyrl-0.2.8/joyrl/algos/DoubleDQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.7/joyrl/algos/DoubleDQN/trainer.py` & `joyrl-0.2.8/joyrl/algos/DoubleDQN/trainer.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.7/joyrl/config/config.py` & `joyrl-0.2.8/joyrl/config/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2023-01-01 16:20:49
 LastEditor: JiangJi
-LastEditTime: 2023-05-27 20:20:02
+LastEditTime: 2023-05-28 19:04:17
 Discription: 
 '''
 
 class MergedConfig:
     ''' Merge general, algorithm and environment config
     '''
     def __init__(self) -> None:
@@ -26,16 +26,14 @@
         self.algo_name = "DQN" # name of algorithm
         self.mode = "train" # train, test
         self.device = "cpu" # device to use
         self.seed = 0 # random seed
         self.max_episode = 100 # number of episodes for training, set -1 to keep running
         self.max_step = 200 # number of episodes for testing, set -1 means unlimited steps
         self.collect_traj = False # if collect trajectory or not
-        # multiprocessing settings
-        self.mp_backend = "single" # multiprocessing backend: "ray", default "single"
         self.n_workers = 1 # number of workers
         self.n_learners = 1 # number of learners if using multi-processing, default 1
         self.share_buffer = True # if all learners share the same buffer
         # online evaluation settings
         self.online_eval = False # online evaluation or not
         self.online_eval_episode = 10 # online eval episodes
         self.model_save_fre = 500 # model save frequency per update step
```

### Comparing `joyrl-0.2.7/joyrl/envs/blackjack.py` & `joyrl-0.2.8/joyrl/envs/blackjack.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.7/joyrl/envs/cliff_walking.py` & `joyrl-0.2.8/joyrl/envs/cliff_walking.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.7/joyrl/envs/gridworld.py` & `joyrl-0.2.8/joyrl/envs/gridworld.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.7/joyrl/envs/gridworld_env.py` & `joyrl-0.2.8/joyrl/envs/gridworld_env.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.7/joyrl/envs/racetrack.py` & `joyrl-0.2.8/joyrl/envs/racetrack.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.7/joyrl/envs/register.py` & `joyrl-0.2.8/joyrl/envs/register.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.7/joyrl/envs/stochastic_mdp.py` & `joyrl-0.2.8/joyrl/envs/stochastic_mdp.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.7/joyrl/envs/windy_gridworld.py` & `joyrl-0.2.8/joyrl/envs/windy_gridworld.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.7/joyrl/envs/wrappers.py` & `joyrl-0.2.8/joyrl/envs/wrappers.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.7/joyrl/framework/dataserver.py` & `joyrl-0.2.8/joyrl/framework/dataserver.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.7/joyrl/framework/learners.py` & `joyrl-0.2.8/joyrl/framework/learners.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.7/joyrl/framework/stats.py` & `joyrl-0.2.8/joyrl/framework/stats.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.7/joyrl/framework/workers.py` & `joyrl-0.2.8/joyrl/framework/workers.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.7/joyrl/run.py` & `joyrl-0.2.8/joyrl/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     general_cfg = cfg.general_cfg
     env_cfg = cfg.env_cfg
     def config_dir(dir,name = None):
             Path(dir).mkdir(parents=True, exist_ok=True)
             setattr(cfg, name, dir)
     curr_time = datetime.datetime.now().strftime("%Y%m%d-%H%M%S")  # obtain current time
     env_name = env_cfg.id if env_cfg.id is not None else general_cfg.env_name
-    task_dir = f"{os.getcwd()}/tasks/{general_cfg.mode.capitalize()}_{general_cfg.mp_backend}_{env_name}_{general_cfg.algo_name}_{curr_time}"
+    task_dir = f"{os.getcwd()}/tasks/{general_cfg.mode.capitalize()}_{env_name}_{general_cfg.algo_name}_{curr_time}"
     dirs_dic = {
         'task_dir':task_dir,
         'model_dir':f"{task_dir}/models",
         'res_dir':f"{task_dir}/results",
         'log_dir':f"{task_dir}/logs",
         'traj_dir':f"{task_dir}/traj",
         'video_dir':f"{task_dir}/videos",
@@ -97,26 +97,27 @@
     return env
 def envs_config(cfg,logger):
     ''' configure environment
     '''
     # register_env(env_cfg.id)
     envs = [] # numbers of envs, equal to cfg.n_workers
     for _ in range(cfg.n_workers):
-        env = create_single_env()
+        env = create_single_env(cfg)
         envs.append(env)
     setattr(cfg, 'obs_space', envs[0].observation_space)
     setattr(cfg, 'action_space', envs[0].action_space)
     logger.info.remote(f"obs_space: {envs[0].observation_space}, n_actions: {envs[0].action_space}")  # print info
+    return envs
 
 def policy_config(cfg):
     ''' configure policy and data_handler
     '''
-    policy_mod = importlib.import_module(f"algos.{cfg.algo_name}.policy")
+    policy_mod = importlib.import_module(f"joyrl.algos.{cfg.algo_name}.policy")
         # create agent
-    data_handler_mod = importlib.import_module(f"algos.{cfg.algo_name}.data_handler")
+    data_handler_mod = importlib.import_module(f"joyrl.algos.{cfg.algo_name}.data_handler")
     policy = policy_mod.Policy(cfg) 
     if cfg.load_checkpoint:
         policy.load_model(f"tasks/{cfg.load_path}/models/{cfg.load_model_step}")
     data_handler = data_handler_mod.DataHandler(cfg)
     return policy, data_handler
 
 def run(**kwargs):
@@ -125,15 +126,15 @@
     cfg = create_dirs(cfg)
     ray.shutdown()
     ray.init(include_dashboard=True)
     logger = RayLogger.remote(cfg.log_dir) # create ray logger 
     print_cfgs(cfg,logger)
     all_seed(cfg.seed) # set seed
     envs = envs_config(cfg,logger) # configure environment
-    test_env = create_single_env() # create test environment
+    test_env = create_single_env(cfg) # create test environment
     online_tester = RayTester.remote(cfg,test_env) # create online tester
     policy, data_handler = policy_config(cfg) # create policy and data_handler
     stats_recorder = StatsRecorder.remote(cfg) # create stats recorder
     data_server = DataServer.remote(cfg) # create data server
     learners = []
     for i in range(cfg.n_learners):
         learner = Learner.remote(cfg, learner_id = i, policy = policy,data_handler = data_handler, online_tester = online_tester)
@@ -142,11 +143,11 @@
     for i in range(cfg.n_workers):
         worker = Worker.remote(cfg, worker_id = i,env = envs[i], logger = logger)
         worker.set_learner_id.remote(i%cfg.n_learners)
         workers.append(worker)
     s_t = time.time()
     worker_tasks = [worker.run.remote(data_server = data_server,learners = learners,stats_recorder = stats_recorder) for worker in workers]
     ray.get(worker_tasks) # wait for all workers finish
-    ray.shutdown() # shutdown ray
     e_t = time.time()
     logger.info.remote(f"Finish {cfg.mode}ing! total time consumed: {e_t-s_t:.2f}s")
     save_cfgs( {'general_cfg': general_cfg, 'algo_cfg': algo_cfg, 'env_cfg': env_cfg}, cfg.task_dir)  # save config
+    ray.shutdown() # shutdown ray
```

### Comparing `joyrl-0.2.7/joyrl/utils/utils.py` & `joyrl-0.2.8/joyrl/utils/utils.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.7/joyrl.egg-info/PKG-INFO` & `joyrl-0.2.8/joyrl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joyrl
-Version: 0.2.7
+Version: 0.2.8
 Summary: A Library for Deep Reinforcement Learning
 Home-page: https://github.com/datawhalechina/joyrl
 Author: johnjim0816
 Author-email: johnjim0816@gmail.com
 License: MIT
 Keywords: reinforcement learning platform pytorch
 Platform: any
```

### Comparing `joyrl-0.2.7/joyrl.egg-info/SOURCES.txt` & `joyrl-0.2.8/joyrl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.7/setup.cfg` & `joyrl-0.2.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.7/setup.py` & `joyrl-0.2.8/setup.py`

 * *Files identical despite different names*

