# Comparing `tmp/joyrl-0.2.6.tar.gz` & `tmp/joyrl-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joyrl-0.2.6.tar", last modified: Sun May 28 10:59:07 2023, max compression
+gzip compressed data, was "joyrl-0.2.7.tar", last modified: Sun May 28 11:00:15 2023, max compression
```

## Comparing `joyrl-0.2.6.tar` & `joyrl-0.2.7.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 10:59:07.658668 joyrl-0.2.6/
--rw-rw-rw-   0        0        0     1097 2023-01-01 08:20:49.000000 joyrl-0.2.6/LICENSE
--rw-rw-rw-   0        0        0     4412 2023-05-28 10:59:07.658668 joyrl-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     3951 2023-01-01 08:20:49.000000 joyrl-0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 10:59:07.629556 joyrl-0.2.6/joyrl/
--rw-rw-rw-   0        0        0      404 2023-05-28 10:59:05.000000 joyrl-0.2.6/joyrl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:59:07.639052 joyrl-0.2.6/joyrl/algos/
-drwxrwxrwx   0        0        0        0 2023-05-28 10:59:07.642047 joyrl-0.2.6/joyrl/algos/DQN/
--rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.6/joyrl/algos/DQN/__init__.py
--rw-rw-rw-   0        0        0     1109 2023-05-27 12:54:10.000000 joyrl-0.2.6/joyrl/algos/DQN/config.py
--rw-rw-rw-   0        0        0      356 2023-05-27 12:54:42.000000 joyrl-0.2.6/joyrl/algos/DQN/data_handler.py
--rw-rw-rw-   0        0        0     4101 2023-05-27 12:54:25.000000 joyrl-0.2.6/joyrl/algos/DQN/policy.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:59:07.644635 joyrl-0.2.6/joyrl/algos/DoubleDQN/
--rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.6/joyrl/algos/DoubleDQN/__init__.py
--rw-rw-rw-   0        0        0     5273 2023-03-15 14:04:30.000000 joyrl-0.2.6/joyrl/algos/DoubleDQN/agent.py
--rw-rw-rw-   0        0        0      962 2023-03-15 14:04:45.000000 joyrl-0.2.6/joyrl/algos/DoubleDQN/config.py
--rw-rw-rw-   0        0        0     1507 2023-03-15 14:05:03.000000 joyrl-0.2.6/joyrl/algos/DoubleDQN/trainer.py
--rw-rw-rw-   0        0        0      269 2023-03-15 14:05:31.000000 joyrl-0.2.6/joyrl/algos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:59:07.645625 joyrl-0.2.6/joyrl/config/
--rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.6/joyrl/config/__init__.py
--rw-rw-rw-   0        0        0     1834 2023-05-27 12:20:08.000000 joyrl-0.2.6/joyrl/config/config.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:59:07.652609 joyrl-0.2.6/joyrl/envs/
--rw-rw-rw-   0        0        0       54 2023-05-28 10:53:02.000000 joyrl-0.2.6/joyrl/envs/__init__.py
--rw-rw-rw-   0        0        0     4380 2023-01-01 08:20:49.000000 joyrl-0.2.6/joyrl/envs/blackjack.py
--rw-rw-rw-   0        0        0     2790 2023-01-01 08:20:49.000000 joyrl-0.2.6/joyrl/envs/cliff_walking.py
--rw-rw-rw-   0        0        0     3996 2023-01-01 08:20:49.000000 joyrl-0.2.6/joyrl/envs/gridworld.py
--rw-rw-rw-   0        0        0     3584 2023-01-01 08:20:49.000000 joyrl-0.2.6/joyrl/envs/gridworld_env.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:59:07.653603 joyrl-0.2.6/joyrl/envs/gym/
--rw-rw-rw-   0        0        0      194 2023-05-28 10:49:52.000000 joyrl-0.2.6/joyrl/envs/gym/__init__.py
--rw-rw-rw-   0        0        0      485 2023-05-27 12:55:35.000000 joyrl-0.2.6/joyrl/envs/gym/config.py
--rw-rw-rw-   0        0        0    10132 2023-01-01 08:20:49.000000 joyrl-0.2.6/joyrl/envs/racetrack.py
--rw-rw-rw-   0        0        0     1080 2023-01-01 08:20:49.000000 joyrl-0.2.6/joyrl/envs/register.py
--rw-rw-rw-   0        0        0     1364 2023-01-01 08:20:49.000000 joyrl-0.2.6/joyrl/envs/stochastic_mdp.py
--rw-rw-rw-   0        0        0     2697 2023-01-01 08:20:49.000000 joyrl-0.2.6/joyrl/envs/windy_gridworld.py
--rw-rw-rw-   0        0        0     2652 2023-01-01 08:20:49.000000 joyrl-0.2.6/joyrl/envs/wrappers.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:59:07.656672 joyrl-0.2.6/joyrl/framework/
--rw-rw-rw-   0        0        0      194 2023-05-28 10:49:40.000000 joyrl-0.2.6/joyrl/framework/__init__.py
--rw-rw-rw-   0        0        0     1332 2023-05-27 12:46:42.000000 joyrl-0.2.6/joyrl/framework/dataserver.py
--rw-rw-rw-   0        0        0     2894 2023-05-27 12:46:27.000000 joyrl-0.2.6/joyrl/framework/learners.py
--rw-rw-rw-   0        0        0     5249 2023-05-27 12:48:22.000000 joyrl-0.2.6/joyrl/framework/stats.py
--rw-rw-rw-   0        0        0     5923 2023-05-27 12:44:48.000000 joyrl-0.2.6/joyrl/framework/workers.py
--rw-rw-rw-   0        0        0     6979 2023-05-28 10:56:12.000000 joyrl-0.2.6/joyrl/run.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:59:07.657671 joyrl-0.2.6/joyrl/utils/
--rw-rw-rw-   0        0        0        2 2023-05-28 10:53:04.000000 joyrl-0.2.6/joyrl/utils/__init__.py
--rw-rw-rw-   0        0        0    36574 2023-05-27 12:50:57.000000 joyrl-0.2.6/joyrl/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:59:07.639052 joyrl-0.2.6/joyrl.egg-info/
--rw-rw-rw-   0        0        0     4412 2023-05-28 10:59:07.000000 joyrl-0.2.6/joyrl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1016 2023-05-28 10:59:07.000000 joyrl-0.2.6/joyrl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 10:59:07.000000 joyrl-0.2.6/joyrl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      350 2023-05-28 10:59:07.000000 joyrl-0.2.6/joyrl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-28 10:59:07.000000 joyrl-0.2.6/joyrl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      995 2023-05-28 10:59:07.659669 joyrl-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1820 2023-05-28 10:45:17.000000 joyrl-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:00:15.073170 joyrl-0.2.7/
+-rw-rw-rw-   0        0        0     1097 2023-01-01 08:20:49.000000 joyrl-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0     4412 2023-05-28 11:00:15.073170 joyrl-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3951 2023-01-01 08:20:49.000000 joyrl-0.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 11:00:15.043450 joyrl-0.2.7/joyrl/
+-rw-rw-rw-   0        0        0      404 2023-05-28 11:00:13.000000 joyrl-0.2.7/joyrl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:00:15.054790 joyrl-0.2.7/joyrl/algos/
+drwxrwxrwx   0        0        0        0 2023-05-28 11:00:15.056784 joyrl-0.2.7/joyrl/algos/DQN/
+-rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.7/joyrl/algos/DQN/__init__.py
+-rw-rw-rw-   0        0        0     1109 2023-05-27 12:54:10.000000 joyrl-0.2.7/joyrl/algos/DQN/config.py
+-rw-rw-rw-   0        0        0      356 2023-05-27 12:54:42.000000 joyrl-0.2.7/joyrl/algos/DQN/data_handler.py
+-rw-rw-rw-   0        0        0     4101 2023-05-27 12:54:25.000000 joyrl-0.2.7/joyrl/algos/DQN/policy.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:00:15.059777 joyrl-0.2.7/joyrl/algos/DoubleDQN/
+-rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.7/joyrl/algos/DoubleDQN/__init__.py
+-rw-rw-rw-   0        0        0     5273 2023-03-15 14:04:30.000000 joyrl-0.2.7/joyrl/algos/DoubleDQN/agent.py
+-rw-rw-rw-   0        0        0      962 2023-03-15 14:04:45.000000 joyrl-0.2.7/joyrl/algos/DoubleDQN/config.py
+-rw-rw-rw-   0        0        0     1507 2023-03-15 14:05:03.000000 joyrl-0.2.7/joyrl/algos/DoubleDQN/trainer.py
+-rw-rw-rw-   0        0        0      269 2023-03-15 14:05:31.000000 joyrl-0.2.7/joyrl/algos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:00:15.059777 joyrl-0.2.7/joyrl/config/
+-rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.7/joyrl/config/__init__.py
+-rw-rw-rw-   0        0        0     1834 2023-05-27 12:20:08.000000 joyrl-0.2.7/joyrl/config/config.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:00:15.066780 joyrl-0.2.7/joyrl/envs/
+-rw-rw-rw-   0        0        0       54 2023-05-28 10:53:02.000000 joyrl-0.2.7/joyrl/envs/__init__.py
+-rw-rw-rw-   0        0        0     4380 2023-01-01 08:20:49.000000 joyrl-0.2.7/joyrl/envs/blackjack.py
+-rw-rw-rw-   0        0        0     2790 2023-01-01 08:20:49.000000 joyrl-0.2.7/joyrl/envs/cliff_walking.py
+-rw-rw-rw-   0        0        0     3996 2023-01-01 08:20:49.000000 joyrl-0.2.7/joyrl/envs/gridworld.py
+-rw-rw-rw-   0        0        0     3584 2023-01-01 08:20:49.000000 joyrl-0.2.7/joyrl/envs/gridworld_env.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:00:15.067777 joyrl-0.2.7/joyrl/envs/gym/
+-rw-rw-rw-   0        0        0      194 2023-05-28 10:49:52.000000 joyrl-0.2.7/joyrl/envs/gym/__init__.py
+-rw-rw-rw-   0        0        0      485 2023-05-27 12:55:35.000000 joyrl-0.2.7/joyrl/envs/gym/config.py
+-rw-rw-rw-   0        0        0    10132 2023-01-01 08:20:49.000000 joyrl-0.2.7/joyrl/envs/racetrack.py
+-rw-rw-rw-   0        0        0     1080 2023-01-01 08:20:49.000000 joyrl-0.2.7/joyrl/envs/register.py
+-rw-rw-rw-   0        0        0     1364 2023-01-01 08:20:49.000000 joyrl-0.2.7/joyrl/envs/stochastic_mdp.py
+-rw-rw-rw-   0        0        0     2697 2023-01-01 08:20:49.000000 joyrl-0.2.7/joyrl/envs/windy_gridworld.py
+-rw-rw-rw-   0        0        0     2652 2023-01-01 08:20:49.000000 joyrl-0.2.7/joyrl/envs/wrappers.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:00:15.070769 joyrl-0.2.7/joyrl/framework/
+-rw-rw-rw-   0        0        0      194 2023-05-28 10:49:40.000000 joyrl-0.2.7/joyrl/framework/__init__.py
+-rw-rw-rw-   0        0        0     1332 2023-05-27 12:46:42.000000 joyrl-0.2.7/joyrl/framework/dataserver.py
+-rw-rw-rw-   0        0        0     2894 2023-05-27 12:46:27.000000 joyrl-0.2.7/joyrl/framework/learners.py
+-rw-rw-rw-   0        0        0     5249 2023-05-27 12:48:22.000000 joyrl-0.2.7/joyrl/framework/stats.py
+-rw-rw-rw-   0        0        0     5923 2023-05-27 12:44:48.000000 joyrl-0.2.7/joyrl/framework/workers.py
+-rw-rw-rw-   0        0        0     7028 2023-05-28 11:00:00.000000 joyrl-0.2.7/joyrl/run.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:00:15.073170 joyrl-0.2.7/joyrl/utils/
+-rw-rw-rw-   0        0        0        2 2023-05-28 10:53:04.000000 joyrl-0.2.7/joyrl/utils/__init__.py
+-rw-rw-rw-   0        0        0    36574 2023-05-27 12:50:57.000000 joyrl-0.2.7/joyrl/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:00:15.053793 joyrl-0.2.7/joyrl.egg-info/
+-rw-rw-rw-   0        0        0     4412 2023-05-28 11:00:14.000000 joyrl-0.2.7/joyrl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1016 2023-05-28 11:00:14.000000 joyrl-0.2.7/joyrl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 11:00:14.000000 joyrl-0.2.7/joyrl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      350 2023-05-28 11:00:14.000000 joyrl-0.2.7/joyrl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-28 11:00:14.000000 joyrl-0.2.7/joyrl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      995 2023-05-28 11:00:15.075170 joyrl-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1820 2023-05-28 10:45:17.000000 joyrl-0.2.7/setup.py
```

### Comparing `joyrl-0.2.6/LICENSE` & `joyrl-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.6/PKG-INFO` & `joyrl-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joyrl
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Library for Deep Reinforcement Learning
 Home-page: https://github.com/datawhalechina/joyrl
 Author: johnjim0816
 Author-email: johnjim0816@gmail.com
 License: MIT
 Keywords: reinforcement learning platform pytorch
 Platform: any
```

### Comparing `joyrl-0.2.6/README.md` & `joyrl-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.6/joyrl/algos/DQN/config.py` & `joyrl-0.2.7/joyrl/algos/DQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.6/joyrl/algos/DQN/policy.py` & `joyrl-0.2.7/joyrl/algos/DQN/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.6/joyrl/algos/DoubleDQN/agent.py` & `joyrl-0.2.7/joyrl/algos/DoubleDQN/agent.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.6/joyrl/algos/DoubleDQN/config.py` & `joyrl-0.2.7/joyrl/algos/DoubleDQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.6/joyrl/algos/DoubleDQN/trainer.py` & `joyrl-0.2.7/joyrl/algos/DoubleDQN/trainer.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.6/joyrl/config/config.py` & `joyrl-0.2.7/joyrl/config/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.6/joyrl/envs/blackjack.py` & `joyrl-0.2.7/joyrl/envs/blackjack.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.6/joyrl/envs/cliff_walking.py` & `joyrl-0.2.7/joyrl/envs/cliff_walking.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.6/joyrl/envs/gridworld.py` & `joyrl-0.2.7/joyrl/envs/gridworld.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.6/joyrl/envs/gridworld_env.py` & `joyrl-0.2.7/joyrl/envs/gridworld_env.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.6/joyrl/envs/racetrack.py` & `joyrl-0.2.7/joyrl/envs/racetrack.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.6/joyrl/envs/register.py` & `joyrl-0.2.7/joyrl/envs/register.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.6/joyrl/envs/stochastic_mdp.py` & `joyrl-0.2.7/joyrl/envs/stochastic_mdp.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.6/joyrl/envs/windy_gridworld.py` & `joyrl-0.2.7/joyrl/envs/windy_gridworld.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.6/joyrl/envs/wrappers.py` & `joyrl-0.2.7/joyrl/envs/wrappers.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.6/joyrl/framework/dataserver.py` & `joyrl-0.2.7/joyrl/framework/dataserver.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.6/joyrl/framework/learners.py` & `joyrl-0.2.7/joyrl/framework/learners.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.6/joyrl/framework/stats.py` & `joyrl-0.2.7/joyrl/framework/stats.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.6/joyrl/framework/workers.py` & `joyrl-0.2.7/joyrl/framework/workers.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.6/joyrl/run.py` & `joyrl-0.2.7/joyrl/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,29 +51,29 @@
     for k,v in dirs_dic.items():
         config_dir(v,name=k)
     return cfg
 
 def print_cfgs(cfg, logger):
     def print_cfg(cfg, name = ''):
         cfg_dict = vars(cfg)
-        logger.info(f"{name}:")
-        logger.info(''.join(['='] * 80))
+        logger.info.remote(f"{name}:")
+        logger.info.remote(''.join(['='] * 80))
         tplt = "{:^20}\t{:^20}\t{:^20}"
-        logger.info(tplt.format("Name", "Value", "Type"))
+        logger.info.remote(tplt.format("Name", "Value", "Type"))
         for k, v in cfg_dict.items():
             if v.__class__.__name__ == 'list': # convert list to str
                 v = str(v)
             if k in ['model_dir','tb_writter']:
                 continue
             if v is None: # avoid NoneType
                 v = 'None'
             if "support" in k: # avoid ndarray
                 v = str(v[0])
-            logger.info(tplt.format(k, v, str(type(v))))
-        logger.info(''.join(['='] * 80))
+            logger.info.remote(tplt.format(k, v, str(type(v))))
+        logger.info.remote(''.join(['='] * 80))
     print_cfg(cfg.general_cfg,name = 'General Configs')
     print_cfg(cfg.algo_cfg,name = 'Algo Configs')
     print_cfg(cfg.env_cfg,name = 'Env Configs')
 def check_n_workers(cfg):
     ''' check n_workers
     '''
     if cfg.__dict__.get('n_workers',None) is None: # set n_workers to 1 if not set
@@ -101,15 +101,15 @@
     # register_env(env_cfg.id)
     envs = [] # numbers of envs, equal to cfg.n_workers
     for _ in range(cfg.n_workers):
         env = create_single_env()
         envs.append(env)
     setattr(cfg, 'obs_space', envs[0].observation_space)
     setattr(cfg, 'action_space', envs[0].action_space)
-    logger.info(f"obs_space: {envs[0].observation_space}, n_actions: {envs[0].action_space}")  # print info
+    logger.info.remote(f"obs_space: {envs[0].observation_space}, n_actions: {envs[0].action_space}")  # print info
 
 def policy_config(cfg):
     ''' configure policy and data_handler
     '''
     policy_mod = importlib.import_module(f"algos.{cfg.algo_name}.policy")
         # create agent
     data_handler_mod = importlib.import_module(f"algos.{cfg.algo_name}.data_handler")
@@ -144,9 +144,9 @@
         worker.set_learner_id.remote(i%cfg.n_learners)
         workers.append(worker)
     s_t = time.time()
     worker_tasks = [worker.run.remote(data_server = data_server,learners = learners,stats_recorder = stats_recorder) for worker in workers]
     ray.get(worker_tasks) # wait for all workers finish
     ray.shutdown() # shutdown ray
     e_t = time.time()
-    logger.info(f"Finish {cfg.mode}ing! total time consumed: {e_t-s_t:.2f}s")
+    logger.info.remote(f"Finish {cfg.mode}ing! total time consumed: {e_t-s_t:.2f}s")
     save_cfgs( {'general_cfg': general_cfg, 'algo_cfg': algo_cfg, 'env_cfg': env_cfg}, cfg.task_dir)  # save config
```

### Comparing `joyrl-0.2.6/joyrl/utils/utils.py` & `joyrl-0.2.7/joyrl/utils/utils.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.6/joyrl.egg-info/PKG-INFO` & `joyrl-0.2.7/joyrl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joyrl
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Library for Deep Reinforcement Learning
 Home-page: https://github.com/datawhalechina/joyrl
 Author: johnjim0816
 Author-email: johnjim0816@gmail.com
 License: MIT
 Keywords: reinforcement learning platform pytorch
 Platform: any
```

### Comparing `joyrl-0.2.6/joyrl.egg-info/SOURCES.txt` & `joyrl-0.2.7/joyrl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.6/setup.cfg` & `joyrl-0.2.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.6/setup.py` & `joyrl-0.2.7/setup.py`

 * *Files identical despite different names*

