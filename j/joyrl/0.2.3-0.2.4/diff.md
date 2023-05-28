# Comparing `tmp/joyrl-0.2.3.tar.gz` & `tmp/joyrl-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joyrl-0.2.3.tar", last modified: Sun May 28 10:53:17 2023, max compression
+gzip compressed data, was "joyrl-0.2.4.tar", last modified: Sun May 28 10:55:21 2023, max compression
```

## Comparing `joyrl-0.2.3.tar` & `joyrl-0.2.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 10:53:17.771233 joyrl-0.2.3/
--rw-rw-rw-   0        0        0     1097 2023-01-01 08:20:49.000000 joyrl-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     4412 2023-05-28 10:53:17.771233 joyrl-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     3951 2023-01-01 08:20:49.000000 joyrl-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 10:53:17.739332 joyrl-0.2.3/joyrl/
--rw-rw-rw-   0        0        0      404 2023-05-28 10:53:14.000000 joyrl-0.2.3/joyrl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:53:17.749856 joyrl-0.2.3/joyrl/algos/
-drwxrwxrwx   0        0        0        0 2023-05-28 10:53:17.751897 joyrl-0.2.3/joyrl/algos/DQN/
--rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.3/joyrl/algos/DQN/__init__.py
--rw-rw-rw-   0        0        0     1109 2023-05-27 12:54:10.000000 joyrl-0.2.3/joyrl/algos/DQN/config.py
--rw-rw-rw-   0        0        0      356 2023-05-27 12:54:42.000000 joyrl-0.2.3/joyrl/algos/DQN/data_handler.py
--rw-rw-rw-   0        0        0     4101 2023-05-27 12:54:25.000000 joyrl-0.2.3/joyrl/algos/DQN/policy.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:53:17.755146 joyrl-0.2.3/joyrl/algos/DoubleDQN/
--rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.3/joyrl/algos/DoubleDQN/__init__.py
--rw-rw-rw-   0        0        0     5273 2023-03-15 14:04:30.000000 joyrl-0.2.3/joyrl/algos/DoubleDQN/agent.py
--rw-rw-rw-   0        0        0      962 2023-03-15 14:04:45.000000 joyrl-0.2.3/joyrl/algos/DoubleDQN/config.py
--rw-rw-rw-   0        0        0     1507 2023-03-15 14:05:03.000000 joyrl-0.2.3/joyrl/algos/DoubleDQN/trainer.py
--rw-rw-rw-   0        0        0      269 2023-03-15 14:05:31.000000 joyrl-0.2.3/joyrl/algos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:53:17.756142 joyrl-0.2.3/joyrl/config/
--rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.3/joyrl/config/__init__.py
--rw-rw-rw-   0        0        0     1834 2023-05-27 12:20:08.000000 joyrl-0.2.3/joyrl/config/config.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:53:17.765737 joyrl-0.2.3/joyrl/envs/
--rw-rw-rw-   0        0        0       54 2023-05-28 10:53:02.000000 joyrl-0.2.3/joyrl/envs/__init__.py
--rw-rw-rw-   0        0        0     4380 2023-01-01 08:20:49.000000 joyrl-0.2.3/joyrl/envs/blackjack.py
--rw-rw-rw-   0        0        0     2790 2023-01-01 08:20:49.000000 joyrl-0.2.3/joyrl/envs/cliff_walking.py
--rw-rw-rw-   0        0        0     3996 2023-01-01 08:20:49.000000 joyrl-0.2.3/joyrl/envs/gridworld.py
--rw-rw-rw-   0        0        0     3584 2023-01-01 08:20:49.000000 joyrl-0.2.3/joyrl/envs/gridworld_env.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:53:17.766735 joyrl-0.2.3/joyrl/envs/gym/
--rw-rw-rw-   0        0        0      194 2023-05-28 10:49:52.000000 joyrl-0.2.3/joyrl/envs/gym/__init__.py
--rw-rw-rw-   0        0        0      485 2023-05-27 12:55:35.000000 joyrl-0.2.3/joyrl/envs/gym/config.py
--rw-rw-rw-   0        0        0    10132 2023-01-01 08:20:49.000000 joyrl-0.2.3/joyrl/envs/racetrack.py
--rw-rw-rw-   0        0        0     1080 2023-01-01 08:20:49.000000 joyrl-0.2.3/joyrl/envs/register.py
--rw-rw-rw-   0        0        0     1364 2023-01-01 08:20:49.000000 joyrl-0.2.3/joyrl/envs/stochastic_mdp.py
--rw-rw-rw-   0        0        0     2697 2023-01-01 08:20:49.000000 joyrl-0.2.3/joyrl/envs/windy_gridworld.py
--rw-rw-rw-   0        0        0     2652 2023-01-01 08:20:49.000000 joyrl-0.2.3/joyrl/envs/wrappers.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:53:17.769727 joyrl-0.2.3/joyrl/framework/
--rw-rw-rw-   0        0        0      194 2023-05-28 10:49:40.000000 joyrl-0.2.3/joyrl/framework/__init__.py
--rw-rw-rw-   0        0        0     1332 2023-05-27 12:46:42.000000 joyrl-0.2.3/joyrl/framework/dataserver.py
--rw-rw-rw-   0        0        0     2894 2023-05-27 12:46:27.000000 joyrl-0.2.3/joyrl/framework/learners.py
--rw-rw-rw-   0        0        0     5249 2023-05-27 12:48:22.000000 joyrl-0.2.3/joyrl/framework/stats.py
--rw-rw-rw-   0        0        0     5923 2023-05-27 12:44:48.000000 joyrl-0.2.3/joyrl/framework/workers.py
--rw-rw-rw-   0        0        0     6967 2023-05-27 12:58:24.000000 joyrl-0.2.3/joyrl/run.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:53:17.771233 joyrl-0.2.3/joyrl/utils/
--rw-rw-rw-   0        0        0        2 2023-05-28 10:53:04.000000 joyrl-0.2.3/joyrl/utils/__init__.py
--rw-rw-rw-   0        0        0    36574 2023-05-27 12:50:57.000000 joyrl-0.2.3/joyrl/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:53:17.748859 joyrl-0.2.3/joyrl.egg-info/
--rw-rw-rw-   0        0        0     4412 2023-05-28 10:53:17.000000 joyrl-0.2.3/joyrl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1016 2023-05-28 10:53:17.000000 joyrl-0.2.3/joyrl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 10:53:17.000000 joyrl-0.2.3/joyrl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      350 2023-05-28 10:53:17.000000 joyrl-0.2.3/joyrl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-28 10:53:17.000000 joyrl-0.2.3/joyrl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      995 2023-05-28 10:53:17.773664 joyrl-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1820 2023-05-28 10:45:17.000000 joyrl-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:55:21.439285 joyrl-0.2.4/
+-rw-rw-rw-   0        0        0     1097 2023-01-01 08:20:49.000000 joyrl-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0     4412 2023-05-28 10:55:21.440357 joyrl-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3951 2023-01-01 08:20:49.000000 joyrl-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 10:55:21.414408 joyrl-0.2.4/joyrl/
+-rw-rw-rw-   0        0        0      404 2023-05-28 10:55:13.000000 joyrl-0.2.4/joyrl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:55:21.420642 joyrl-0.2.4/joyrl/algos/
+drwxrwxrwx   0        0        0        0 2023-05-28 10:55:21.422636 joyrl-0.2.4/joyrl/algos/DQN/
+-rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.4/joyrl/algos/DQN/__init__.py
+-rw-rw-rw-   0        0        0     1109 2023-05-27 12:54:10.000000 joyrl-0.2.4/joyrl/algos/DQN/config.py
+-rw-rw-rw-   0        0        0      356 2023-05-27 12:54:42.000000 joyrl-0.2.4/joyrl/algos/DQN/data_handler.py
+-rw-rw-rw-   0        0        0     4101 2023-05-27 12:54:25.000000 joyrl-0.2.4/joyrl/algos/DQN/policy.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:55:21.424631 joyrl-0.2.4/joyrl/algos/DoubleDQN/
+-rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.4/joyrl/algos/DoubleDQN/__init__.py
+-rw-rw-rw-   0        0        0     5273 2023-03-15 14:04:30.000000 joyrl-0.2.4/joyrl/algos/DoubleDQN/agent.py
+-rw-rw-rw-   0        0        0      962 2023-03-15 14:04:45.000000 joyrl-0.2.4/joyrl/algos/DoubleDQN/config.py
+-rw-rw-rw-   0        0        0     1507 2023-03-15 14:05:03.000000 joyrl-0.2.4/joyrl/algos/DoubleDQN/trainer.py
+-rw-rw-rw-   0        0        0      269 2023-03-15 14:05:31.000000 joyrl-0.2.4/joyrl/algos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:55:21.425629 joyrl-0.2.4/joyrl/config/
+-rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.4/joyrl/config/__init__.py
+-rw-rw-rw-   0        0        0     1834 2023-05-27 12:20:08.000000 joyrl-0.2.4/joyrl/config/config.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:55:21.432780 joyrl-0.2.4/joyrl/envs/
+-rw-rw-rw-   0        0        0       54 2023-05-28 10:53:02.000000 joyrl-0.2.4/joyrl/envs/__init__.py
+-rw-rw-rw-   0        0        0     4380 2023-01-01 08:20:49.000000 joyrl-0.2.4/joyrl/envs/blackjack.py
+-rw-rw-rw-   0        0        0     2790 2023-01-01 08:20:49.000000 joyrl-0.2.4/joyrl/envs/cliff_walking.py
+-rw-rw-rw-   0        0        0     3996 2023-01-01 08:20:49.000000 joyrl-0.2.4/joyrl/envs/gridworld.py
+-rw-rw-rw-   0        0        0     3584 2023-01-01 08:20:49.000000 joyrl-0.2.4/joyrl/envs/gridworld_env.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:55:21.433778 joyrl-0.2.4/joyrl/envs/gym/
+-rw-rw-rw-   0        0        0      194 2023-05-28 10:49:52.000000 joyrl-0.2.4/joyrl/envs/gym/__init__.py
+-rw-rw-rw-   0        0        0      485 2023-05-27 12:55:35.000000 joyrl-0.2.4/joyrl/envs/gym/config.py
+-rw-rw-rw-   0        0        0    10132 2023-01-01 08:20:49.000000 joyrl-0.2.4/joyrl/envs/racetrack.py
+-rw-rw-rw-   0        0        0     1080 2023-01-01 08:20:49.000000 joyrl-0.2.4/joyrl/envs/register.py
+-rw-rw-rw-   0        0        0     1364 2023-01-01 08:20:49.000000 joyrl-0.2.4/joyrl/envs/stochastic_mdp.py
+-rw-rw-rw-   0        0        0     2697 2023-01-01 08:20:49.000000 joyrl-0.2.4/joyrl/envs/windy_gridworld.py
+-rw-rw-rw-   0        0        0     2652 2023-01-01 08:20:49.000000 joyrl-0.2.4/joyrl/envs/wrappers.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:55:21.438277 joyrl-0.2.4/joyrl/framework/
+-rw-rw-rw-   0        0        0      194 2023-05-28 10:49:40.000000 joyrl-0.2.4/joyrl/framework/__init__.py
+-rw-rw-rw-   0        0        0     1332 2023-05-27 12:46:42.000000 joyrl-0.2.4/joyrl/framework/dataserver.py
+-rw-rw-rw-   0        0        0     2894 2023-05-27 12:46:27.000000 joyrl-0.2.4/joyrl/framework/learners.py
+-rw-rw-rw-   0        0        0     5249 2023-05-27 12:48:22.000000 joyrl-0.2.4/joyrl/framework/stats.py
+-rw-rw-rw-   0        0        0     5923 2023-05-27 12:44:48.000000 joyrl-0.2.4/joyrl/framework/workers.py
+-rw-rw-rw-   0        0        0     6967 2023-05-27 12:58:24.000000 joyrl-0.2.4/joyrl/run.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:55:21.439285 joyrl-0.2.4/joyrl/utils/
+-rw-rw-rw-   0        0        0        2 2023-05-28 10:53:04.000000 joyrl-0.2.4/joyrl/utils/__init__.py
+-rw-rw-rw-   0        0        0    36574 2023-05-27 12:50:57.000000 joyrl-0.2.4/joyrl/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:55:21.419645 joyrl-0.2.4/joyrl.egg-info/
+-rw-rw-rw-   0        0        0     4412 2023-05-28 10:55:21.000000 joyrl-0.2.4/joyrl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1016 2023-05-28 10:55:21.000000 joyrl-0.2.4/joyrl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 10:55:21.000000 joyrl-0.2.4/joyrl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      350 2023-05-28 10:55:21.000000 joyrl-0.2.4/joyrl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-28 10:55:21.000000 joyrl-0.2.4/joyrl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      995 2023-05-28 10:55:21.441354 joyrl-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1820 2023-05-28 10:45:17.000000 joyrl-0.2.4/setup.py
```

### Comparing `joyrl-0.2.3/LICENSE` & `joyrl-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.3/PKG-INFO` & `joyrl-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joyrl
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Library for Deep Reinforcement Learning
 Home-page: https://github.com/datawhalechina/joyrl
 Author: johnjim0816
 Author-email: johnjim0816@gmail.com
 License: MIT
 Keywords: reinforcement learning platform pytorch
 Platform: any
```

### Comparing `joyrl-0.2.3/README.md` & `joyrl-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.3/joyrl/algos/DQN/config.py` & `joyrl-0.2.4/joyrl/algos/DQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.3/joyrl/algos/DQN/policy.py` & `joyrl-0.2.4/joyrl/algos/DQN/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.3/joyrl/algos/DoubleDQN/agent.py` & `joyrl-0.2.4/joyrl/algos/DoubleDQN/agent.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.3/joyrl/algos/DoubleDQN/config.py` & `joyrl-0.2.4/joyrl/algos/DoubleDQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.3/joyrl/algos/DoubleDQN/trainer.py` & `joyrl-0.2.4/joyrl/algos/DoubleDQN/trainer.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.3/joyrl/config/config.py` & `joyrl-0.2.4/joyrl/config/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.3/joyrl/envs/blackjack.py` & `joyrl-0.2.4/joyrl/envs/blackjack.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.3/joyrl/envs/cliff_walking.py` & `joyrl-0.2.4/joyrl/envs/cliff_walking.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.3/joyrl/envs/gridworld.py` & `joyrl-0.2.4/joyrl/envs/gridworld.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.3/joyrl/envs/gridworld_env.py` & `joyrl-0.2.4/joyrl/envs/gridworld_env.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.3/joyrl/envs/racetrack.py` & `joyrl-0.2.4/joyrl/envs/racetrack.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.3/joyrl/envs/register.py` & `joyrl-0.2.4/joyrl/envs/register.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.3/joyrl/envs/stochastic_mdp.py` & `joyrl-0.2.4/joyrl/envs/stochastic_mdp.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.3/joyrl/envs/windy_gridworld.py` & `joyrl-0.2.4/joyrl/envs/windy_gridworld.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.3/joyrl/envs/wrappers.py` & `joyrl-0.2.4/joyrl/envs/wrappers.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.3/joyrl/framework/dataserver.py` & `joyrl-0.2.4/joyrl/framework/dataserver.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.3/joyrl/framework/learners.py` & `joyrl-0.2.4/joyrl/framework/learners.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.3/joyrl/framework/stats.py` & `joyrl-0.2.4/joyrl/framework/stats.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.3/joyrl/framework/workers.py` & `joyrl-0.2.4/joyrl/framework/workers.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.3/joyrl/run.py` & `joyrl-0.2.4/joyrl/run.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.3/joyrl/utils/utils.py` & `joyrl-0.2.4/joyrl/utils/utils.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.3/joyrl.egg-info/PKG-INFO` & `joyrl-0.2.4/joyrl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joyrl
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Library for Deep Reinforcement Learning
 Home-page: https://github.com/datawhalechina/joyrl
 Author: johnjim0816
 Author-email: johnjim0816@gmail.com
 License: MIT
 Keywords: reinforcement learning platform pytorch
 Platform: any
```

### Comparing `joyrl-0.2.3/joyrl.egg-info/SOURCES.txt` & `joyrl-0.2.4/joyrl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.3/setup.cfg` & `joyrl-0.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.3/setup.py` & `joyrl-0.2.4/setup.py`

 * *Files identical despite different names*

