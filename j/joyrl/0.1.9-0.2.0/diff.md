# Comparing `tmp/joyrl-0.1.9.tar.gz` & `tmp/joyrl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/joyrl-0.1.9.tar", last modified: Sat Nov 19 17:24:46 2022, max compression
+gzip compressed data, was "joyrl-0.2.0.tar", last modified: Sun May 28 10:35:26 2023, max compression
```

## Comparing `joyrl-0.1.9.tar` & `joyrl-0.2.0.tar`

### file list

```diff
@@ -1,43 +1,41 @@
-drwxr-xr-x   0 jj         (501) staff       (20)        0 2022-11-19 17:24:46.000000 joyrl-0.1.9/
--rw-r--r--   0 jj         (501) staff       (20)     1077 2022-11-19 16:17:31.000000 joyrl-0.1.9/LICENSE
--rw-r--r--   0 jj         (501) staff       (20)     1923 2022-11-19 17:24:46.000000 joyrl-0.1.9/PKG-INFO
--rw-r--r--   0 jj         (501) staff       (20)     1482 2022-11-19 09:44:07.000000 joyrl-0.1.9/README.md
-drwxr-xr-x   0 jj         (501) staff       (20)        0 2022-11-19 17:24:46.000000 joyrl-0.1.9/joyrl/
--rw-r--r--   0 jj         (501) staff       (20)      163 2022-11-19 17:24:43.000000 joyrl-0.1.9/joyrl/__init__.py
-drwxr-xr-x   0 jj         (501) staff       (20)        0 2022-11-19 17:24:46.000000 joyrl-0.1.9/joyrl/algos/
--rw-r--r--   0 jj         (501) staff       (20)        0 2022-11-19 17:24:17.000000 joyrl-0.1.9/joyrl/algos/__init__.py
-drwxr-xr-x   0 jj         (501) staff       (20)        0 2022-11-19 17:24:46.000000 joyrl-0.1.9/joyrl/common/
--rw-r--r--   0 jj         (501) staff       (20)        0 2022-11-19 17:24:26.000000 joyrl-0.1.9/joyrl/common/__init__.py
--rw-r--r--   0 jj         (501) staff       (20)     9679 2022-10-24 08:36:05.000000 joyrl-0.1.9/joyrl/common/atari_wrappers.py
--rw-r--r--   0 jj         (501) staff       (20)     1859 2022-10-24 08:36:05.000000 joyrl-0.1.9/joyrl/common/launcher.py
--rw-r--r--   0 jj         (501) staff       (20)     1595 2022-11-19 08:50:15.000000 joyrl-0.1.9/joyrl/common/layers.py
--rw-r--r--   0 jj         (501) staff       (20)     2498 2022-10-24 08:36:05.000000 joyrl-0.1.9/joyrl/common/memories.py
--rw-r--r--   0 jj         (501) staff       (20)     3190 2022-10-24 08:36:05.000000 joyrl-0.1.9/joyrl/common/models.py
--rw-r--r--   0 jj         (501) staff       (20)     4918 2022-10-24 08:36:05.000000 joyrl-0.1.9/joyrl/common/multiprocessing_env.py
--rw-r--r--   0 jj         (501) staff       (20)     5337 2022-11-19 08:32:20.000000 joyrl-0.1.9/joyrl/common/utils.py
--rw-r--r--   0 jj         (501) staff       (20)      945 2022-10-24 08:36:05.000000 joyrl-0.1.9/joyrl/common/wrappers.py
-drwxr-xr-x   0 jj         (501) staff       (20)        0 2022-11-19 17:24:46.000000 joyrl-0.1.9/joyrl/config/
--rw-r--r--   0 jj         (501) staff       (20)        0 2022-11-19 17:24:29.000000 joyrl-0.1.9/joyrl/config/__init__.py
--rw-r--r--   0 jj         (501) staff       (20)        0 2022-11-19 15:46:20.000000 joyrl-0.1.9/joyrl/config/config.py
-drwxr-xr-x   0 jj         (501) staff       (20)        0 2022-11-19 17:24:46.000000 joyrl-0.1.9/joyrl/envs/
--rw-r--r--   0 jj         (501) staff       (20)        0 2022-11-19 17:24:32.000000 joyrl-0.1.9/joyrl/envs/__init__.py
--rw-r--r--   0 jj         (501) staff       (20)     4258 2022-10-24 08:36:05.000000 joyrl-0.1.9/joyrl/envs/blackjack.py
--rw-r--r--   0 jj         (501) staff       (20)     2706 2022-10-24 08:36:05.000000 joyrl-0.1.9/joyrl/envs/cliff_walking.py
--rw-r--r--   0 jj         (501) staff       (20)     3871 2022-10-24 08:36:05.000000 joyrl-0.1.9/joyrl/envs/gridworld.py
--rw-r--r--   0 jj         (501) staff       (20)     3485 2022-10-24 08:36:05.000000 joyrl-0.1.9/joyrl/envs/gridworld_env.py
--rw-r--r--   0 jj         (501) staff       (20)     9890 2022-10-24 08:36:05.000000 joyrl-0.1.9/joyrl/envs/racetrack.py
--rw-r--r--   0 jj         (501) staff       (20)     1047 2022-10-24 08:36:05.000000 joyrl-0.1.9/joyrl/envs/register.py
--rw-r--r--   0 jj         (501) staff       (20)     1311 2022-10-24 08:36:05.000000 joyrl-0.1.9/joyrl/envs/stochastic_mdp.py
--rw-r--r--   0 jj         (501) staff       (20)     2615 2022-10-24 08:36:05.000000 joyrl-0.1.9/joyrl/envs/windy_gridworld.py
--rw-r--r--   0 jj         (501) staff       (20)     2575 2022-10-24 08:36:05.000000 joyrl-0.1.9/joyrl/envs/wrappers.py
-drwxr-xr-x   0 jj         (501) staff       (20)        0 2022-11-19 17:24:46.000000 joyrl-0.1.9/joyrl/launcher/
--rw-r--r--   0 jj         (501) staff       (20)        0 2022-11-19 17:24:34.000000 joyrl-0.1.9/joyrl/launcher/__init__.py
--rw-r--r--   0 jj         (501) staff       (20)     4622 2022-11-19 17:07:23.000000 joyrl-0.1.9/joyrl/launcher/launcher.py
-drwxr-xr-x   0 jj         (501) staff       (20)        0 2022-11-19 17:24:46.000000 joyrl-0.1.9/joyrl.egg-info/
--rw-r--r--   0 jj         (501) staff       (20)     1923 2022-11-19 17:24:46.000000 joyrl-0.1.9/joyrl.egg-info/PKG-INFO
--rw-r--r--   0 jj         (501) staff       (20)      815 2022-11-19 17:24:46.000000 joyrl-0.1.9/joyrl.egg-info/SOURCES.txt
--rw-r--r--   0 jj         (501) staff       (20)        1 2022-11-19 17:24:46.000000 joyrl-0.1.9/joyrl.egg-info/dependency_links.txt
--rw-r--r--   0 jj         (501) staff       (20)      232 2022-11-19 17:24:46.000000 joyrl-0.1.9/joyrl.egg-info/requires.txt
--rw-r--r--   0 jj         (501) staff       (20)        6 2022-11-19 17:24:46.000000 joyrl-0.1.9/joyrl.egg-info/top_level.txt
--rw-r--r--   0 jj         (501) staff       (20)      940 2022-11-19 17:24:46.000000 joyrl-0.1.9/setup.cfg
--rw-r--r--   0 jj         (501) staff       (20)     1554 2022-11-19 17:15:43.000000 joyrl-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:35:26.590222 joyrl-0.2.0/
+-rw-rw-rw-   0        0        0     1097 2023-01-01 08:20:49.000000 joyrl-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     4412 2023-05-28 10:35:26.590222 joyrl-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3951 2023-01-01 08:20:49.000000 joyrl-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 10:35:26.557903 joyrl-0.2.0/joyrl/
+-rw-rw-rw-   0        0        0      404 2023-05-27 12:56:56.000000 joyrl-0.2.0/joyrl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:35:26.572968 joyrl-0.2.0/joyrl/algos/
+drwxrwxrwx   0        0        0        0 2023-05-28 10:35:26.576070 joyrl-0.2.0/joyrl/algos/DQN/
+-rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.0/joyrl/algos/DQN/__init__.py
+-rw-rw-rw-   0        0        0     1109 2023-05-27 12:54:10.000000 joyrl-0.2.0/joyrl/algos/DQN/config.py
+-rw-rw-rw-   0        0        0      356 2023-05-27 12:54:42.000000 joyrl-0.2.0/joyrl/algos/DQN/data_handler.py
+-rw-rw-rw-   0        0        0     4101 2023-05-27 12:54:25.000000 joyrl-0.2.0/joyrl/algos/DQN/policy.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:35:26.579064 joyrl-0.2.0/joyrl/algos/DoubleDQN/
+-rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.0/joyrl/algos/DoubleDQN/__init__.py
+-rw-rw-rw-   0        0        0     5273 2023-03-15 14:04:30.000000 joyrl-0.2.0/joyrl/algos/DoubleDQN/agent.py
+-rw-rw-rw-   0        0        0      962 2023-03-15 14:04:45.000000 joyrl-0.2.0/joyrl/algos/DoubleDQN/config.py
+-rw-rw-rw-   0        0        0     1507 2023-03-15 14:05:03.000000 joyrl-0.2.0/joyrl/algos/DoubleDQN/trainer.py
+-rw-rw-rw-   0        0        0      269 2023-03-15 14:05:31.000000 joyrl-0.2.0/joyrl/algos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:35:26.580060 joyrl-0.2.0/joyrl/config/
+-rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.0/joyrl/config/__init__.py
+-rw-rw-rw-   0        0        0     1834 2023-05-27 12:20:08.000000 joyrl-0.2.0/joyrl/config/config.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:35:26.589225 joyrl-0.2.0/joyrl/envs/
+-rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.0/joyrl/envs/__init__.py
+-rw-rw-rw-   0        0        0     4380 2023-01-01 08:20:49.000000 joyrl-0.2.0/joyrl/envs/blackjack.py
+-rw-rw-rw-   0        0        0     2790 2023-01-01 08:20:49.000000 joyrl-0.2.0/joyrl/envs/cliff_walking.py
+-rw-rw-rw-   0        0        0     3996 2023-01-01 08:20:49.000000 joyrl-0.2.0/joyrl/envs/gridworld.py
+-rw-rw-rw-   0        0        0     3584 2023-01-01 08:20:49.000000 joyrl-0.2.0/joyrl/envs/gridworld_env.py
+-rw-rw-rw-   0        0        0    10132 2023-01-01 08:20:49.000000 joyrl-0.2.0/joyrl/envs/racetrack.py
+-rw-rw-rw-   0        0        0     1080 2023-01-01 08:20:49.000000 joyrl-0.2.0/joyrl/envs/register.py
+-rw-rw-rw-   0        0        0     1364 2023-01-01 08:20:49.000000 joyrl-0.2.0/joyrl/envs/stochastic_mdp.py
+-rw-rw-rw-   0        0        0     2697 2023-01-01 08:20:49.000000 joyrl-0.2.0/joyrl/envs/windy_gridworld.py
+-rw-rw-rw-   0        0        0     2652 2023-01-01 08:20:49.000000 joyrl-0.2.0/joyrl/envs/wrappers.py
+-rw-rw-rw-   0        0        0     6967 2023-05-27 12:58:24.000000 joyrl-0.2.0/joyrl/run.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:35:26.572968 joyrl-0.2.0/joyrl.egg-info/
+-rw-rw-rw-   0        0        0     4412 2023-05-28 10:35:26.000000 joyrl-0.2.0/joyrl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      781 2023-05-28 10:35:26.000000 joyrl-0.2.0/joyrl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 10:35:26.000000 joyrl-0.2.0/joyrl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      232 2023-05-28 10:35:26.000000 joyrl-0.2.0/joyrl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-28 10:35:26.000000 joyrl-0.2.0/joyrl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      995 2023-05-28 10:35:26.597300 joyrl-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1605 2023-03-15 14:05:51.000000 joyrl-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `joyrl-0.1.9/LICENSE` & `joyrl-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Tianshou contributors
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2022 Tianshou contributors
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `joyrl-0.1.9/joyrl/envs/blackjack.py` & `joyrl-0.2.0/joyrl/envs/blackjack.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-import gym
-from gym import spaces
-from gym.utils import seeding
-
-def cmp(a, b):
-    return int((a > b)) - int((a < b))
-
-# 1 = Ace, 2-10 = Number cards, Jack/Queen/King = 10
-deck = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 10, 10, 10]
-
-
-def draw_card(np_random):
-    return np_random.choice(deck)
-
-
-def draw_hand(np_random):
-    return [draw_card(np_random), draw_card(np_random)]
-
-
-def usable_ace(hand):  # Does this hand have a usable ace?
-    return 1 in hand and sum(hand) + 10 <= 21
-
-
-def sum_hand(hand):  # Return current hand total
-    if usable_ace(hand):
-            return sum(hand) + 10
-    return sum(hand)
-
-
-def is_bust(hand):  # Is this hand a bust?
-    return sum_hand(hand) > 21
-
-
-def score(hand):  # What is the score of this hand (0 if bust)
-    return 0 if is_bust(hand) else sum_hand(hand)
-
-
-def is_natural(hand):  # Is this hand a natural blackjack?
-    return sorted(hand) == [1, 10]
-
-
-class BlackjackEnv(gym.Env):
-    """Simple blackjack environment
-    Blackjack is a card game where the goal is to obtain cards that sum to as
-    near as possible to 21 without going over.  They're playing against a fixed
-    dealer.
-    Face cards (Jack, Queen, King) have point value 10.
-    Aces can either count as 11 or 1, and it's called 'usable' at 11.
-    This game is placed with an infinite deck (or with replacement).
-    The game starts with each (player and dealer) having one face up and one
-    face down card.
-    The player can request additional cards (hit=1) until they decide to stop
-    (stick=0) or exceed 21 (bust).
-    After the player sticks, the dealer reveals their facedown card, and draws
-    until their sum is 17 or greater.  If the dealer goes bust the player wins.
-    If neither player nor dealer busts, the outcome (win, lose, draw) is
-    decided by whose sum is closer to 21.  The reward for winning is +1,
-    drawing is 0, and losing is -1.
-    The observation of a 3-tuple of: the players current sum,
-    the dealer's one showing card (1-10 where 1 is ace),
-    and whether or not the player holds a usable ace (0 or 1).
-    This environment corresponds to the version of the blackjack problem
-    described in Example 5.1 in Reinforcement Learning: An Introduction
-    by Sutton and Barto (1998).
-    https://webdocs.cs.ualberta.ca/~sutton/book/the-book.html
-    """
-    def __init__(self, natural=False):
-        self.action_space = spaces.Discrete(2)
-        self.observation_space = spaces.Tuple((
-            spaces.Discrete(32),
-            spaces.Discrete(11),
-            spaces.Discrete(2)))
-        self._seed()
-
-        # Flag to payout 1.5 on a "natural" blackjack win, like casino rules
-        # Ref: http://www.bicyclecards.com/how-to-play/blackjack/
-        self.natural = natural
-        # Start the first game
-        self._reset()        # Number of 
-        self.n_actions = 2
-
-    def reset(self):
-        return self._reset()
-
-    def step(self, action):
-        return self._step(action)
-
-    def _seed(self, seed=None):
-        self.np_random, seed = seeding.np_random(seed)
-        return [seed]
-
-    def _step(self, action):
-        assert self.action_space.contains(action)
-        if action:  # hit: add a card to players hand and return
-            self.player.append(draw_card(self.np_random))
-            if is_bust(self.player):
-                done = True
-                reward = -1
-            else:
-                done = False
-                reward = 0
-        else:  # stick: play out the dealers hand, and score
-            done = True
-            while sum_hand(self.dealer) < 17:
-                self.dealer.append(draw_card(self.np_random))
-            reward = cmp(score(self.player), score(self.dealer))
-            if self.natural and is_natural(self.player) and reward == 1:
-                reward = 1.5
-        return self._get_obs(), reward, done, {}
-
-    def _get_obs(self):
-        return (sum_hand(self.player), self.dealer[0], usable_ace(self.player))
-
-    def _reset(self):
-        self.dealer = draw_hand(self.np_random)
-        self.player = draw_hand(self.np_random)
-
-        # Auto-draw another card if the score is less than 12
-        while sum_hand(self.player) < 12:
-            self.player.append(draw_card(self.np_random))
-
-        return self._get_obs()
+import gym
+from gym import spaces
+from gym.utils import seeding
+
+def cmp(a, b):
+    return int((a > b)) - int((a < b))
+
+# 1 = Ace, 2-10 = Number cards, Jack/Queen/King = 10
+deck = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 10, 10, 10]
+
+
+def draw_card(np_random):
+    return np_random.choice(deck)
+
+
+def draw_hand(np_random):
+    return [draw_card(np_random), draw_card(np_random)]
+
+
+def usable_ace(hand):  # Does this hand have a usable ace?
+    return 1 in hand and sum(hand) + 10 <= 21
+
+
+def sum_hand(hand):  # Return current hand total
+    if usable_ace(hand):
+            return sum(hand) + 10
+    return sum(hand)
+
+
+def is_bust(hand):  # Is this hand a bust?
+    return sum_hand(hand) > 21
+
+
+def score(hand):  # What is the score of this hand (0 if bust)
+    return 0 if is_bust(hand) else sum_hand(hand)
+
+
+def is_natural(hand):  # Is this hand a natural blackjack?
+    return sorted(hand) == [1, 10]
+
+
+class BlackjackEnv(gym.Env):
+    """Simple blackjack environment
+    Blackjack is a card game where the goal is to obtain cards that sum to as
+    near as possible to 21 without going over.  They're playing against a fixed
+    dealer.
+    Face cards (Jack, Queen, King) have point value 10.
+    Aces can either count as 11 or 1, and it's called 'usable' at 11.
+    This game is placed with an infinite deck (or with replacement).
+    The game starts with each (player and dealer) having one face up and one
+    face down card.
+    The player can request additional cards (hit=1) until they decide to stop
+    (stick=0) or exceed 21 (bust).
+    After the player sticks, the dealer reveals their facedown card, and draws
+    until their sum is 17 or greater.  If the dealer goes bust the player wins.
+    If neither player nor dealer busts, the outcome (win, lose, draw) is
+    decided by whose sum is closer to 21.  The reward for winning is +1,
+    drawing is 0, and losing is -1.
+    The observation of a 3-tuple of: the players current sum,
+    the dealer's one showing card (1-10 where 1 is ace),
+    and whether or not the player holds a usable ace (0 or 1).
+    This environment corresponds to the version of the blackjack problem
+    described in Example 5.1 in Reinforcement Learning: An Introduction
+    by Sutton and Barto (1998).
+    https://webdocs.cs.ualberta.ca/~sutton/book/the-book.html
+    """
+    def __init__(self, natural=False):
+        self.action_space = spaces.Discrete(2)
+        self.observation_space = spaces.Tuple((
+            spaces.Discrete(32),
+            spaces.Discrete(11),
+            spaces.Discrete(2)))
+        self._seed()
+
+        # Flag to payout 1.5 on a "natural" blackjack win, like casino rules
+        # Ref: http://www.bicyclecards.com/how-to-play/blackjack/
+        self.natural = natural
+        # Start the first game
+        self._reset()        # Number of 
+        self.n_actions = 2
+
+    def reset(self):
+        return self._reset()
+
+    def step(self, action):
+        return self._step(action)
+
+    def _seed(self, seed=None):
+        self.np_random, seed = seeding.np_random(seed)
+        return [seed]
+
+    def _step(self, action):
+        assert self.action_space.contains(action)
+        if action:  # hit: add a card to players hand and return
+            self.player.append(draw_card(self.np_random))
+            if is_bust(self.player):
+                done = True
+                reward = -1
+            else:
+                done = False
+                reward = 0
+        else:  # stick: play out the dealers hand, and score
+            done = True
+            while sum_hand(self.dealer) < 17:
+                self.dealer.append(draw_card(self.np_random))
+            reward = cmp(score(self.player), score(self.dealer))
+            if self.natural and is_natural(self.player) and reward == 1:
+                reward = 1.5
+        return self._get_obs(), reward, done, {}
+
+    def _get_obs(self):
+        return (sum_hand(self.player), self.dealer[0], usable_ace(self.player))
+
+    def _reset(self):
+        self.dealer = draw_hand(self.np_random)
+        self.player = draw_hand(self.np_random)
+
+        # Auto-draw another card if the score is less than 12
+        while sum_hand(self.player) < 12:
+            self.player.append(draw_card(self.np_random))
+
+        return self._get_obs()
```

### Comparing `joyrl-0.1.9/joyrl/envs/cliff_walking.py` & `joyrl-0.2.0/joyrl/envs/windy_gridworld.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,84 +1,82 @@
-import numpy as np
-import sys
-from gym.envs.toy_text import discrete
-
-
-UP = 0
-RIGHT = 1
-DOWN = 2
-LEFT = 3
-
-class CliffWalkingEnv(discrete.DiscreteEnv):
-
-    metadata = {'render.modes': ['human', 'ansi']}
-
-    def _limit_coordinates(self, coord):
-        coord[0] = min(coord[0], self.shape[0] - 1)
-        coord[0] = max(coord[0], 0)
-        coord[1] = min(coord[1], self.shape[1] - 1)
-        coord[1] = max(coord[1], 0)
-        return coord
-
-    def _calculate_transition_prob(self, current, delta):
-        new_position = np.array(current) + np.array(delta)
-        new_position = self._limit_coordinates(new_position).astype(int)
-        new_state = np.ravel_multi_index(tuple(new_position), self.shape)
-        reward = -100.0 if self._cliff[tuple(new_position)] else -1.0
-        is_done = self._cliff[tuple(new_position)] or (tuple(new_position) == (3,11))
-        return [(1.0, new_state, reward, is_done)]
-
-    def __init__(self):
-        self.shape = (4, 12)
-
-        nS = np.prod(self.shape)
-        n_actions = 4
-
-        # Cliff Location
-        self._cliff = np.zeros(self.shape, dtype=np.bool)
-        self._cliff[3, 1:-1] = True
-
-        # Calculate transition probabilities
-        P = {}
-        for s in range(nS):
-            position = np.unravel_index(s, self.shape)
-            P[s] = { a : [] for a in range(n_actions) }
-            P[s][UP] = self._calculate_transition_prob(position, [-1, 0])
-            P[s][RIGHT] = self._calculate_transition_prob(position, [0, 1])
-            P[s][DOWN] = self._calculate_transition_prob(position, [1, 0])
-            P[s][LEFT] = self._calculate_transition_prob(position, [0, -1])
-
-        # We always start in state (3, 0)
-        isd = np.zeros(nS)
-        isd[np.ravel_multi_index((3,0), self.shape)] = 1.0
-
-        super(CliffWalkingEnv, self).__init__(nS, n_actions, P, isd)
-
-    def render(self, mode='human', close=False):
-        self._render(mode, close)
-
-    def _render(self, mode='human', close=False):
-        if close:
-            return
-
-        outfile = StringIO() if mode == 'ansi' else sys.stdout
-
-        for s in range(self.nS):
-            position = np.unravel_index(s, self.shape)
-            # print(self.s)
-            if self.s == s:
-                output = " x "
-            elif position == (3,11):
-                output = " T "
-            elif self._cliff[position]:
-                output = " C "
-            else:
-                output = " o "
-
-            if position[1] == 0:
-                output = output.lstrip() 
-            if position[1] == self.shape[1] - 1:
-                output = output.rstrip() 
-                output += "\n"
-
-            outfile.write(output)
-        outfile.write("\n")
+import gym
+import numpy as np
+import sys
+from gym.envs.toy_text import discrete
+
+UP = 0
+RIGHT = 1
+DOWN = 2
+LEFT = 3
+
+class WindyGridworldEnv(discrete.DiscreteEnv):
+
+    metadata = {'render.modes': ['human', 'ansi']}
+
+    def _limit_coordinates(self, coord):
+        coord[0] = min(coord[0], self.shape[0] - 1)
+        coord[0] = max(coord[0], 0)
+        coord[1] = min(coord[1], self.shape[1] - 1)
+        coord[1] = max(coord[1], 0)
+        return coord
+
+    def _calculate_transition_prob(self, current, delta, winds):
+        new_position = np.array(current) + np.array(delta) + np.array([-1, 0]) * winds[tuple(current)]
+        new_position = self._limit_coordinates(new_position).astype(int)
+        new_state = np.ravel_multi_index(tuple(new_position), self.shape)
+        is_done = tuple(new_position) == (3, 7)
+        return [(1.0, new_state, -1.0, is_done)]
+
+    def __init__(self):
+        self.shape = (7, 10)
+
+        nS = np.prod(self.shape)
+        n_actions = 4
+
+        # Wind strength
+        winds = np.zeros(self.shape)
+        winds[:,[3,4,5,8]] = 1
+        winds[:,[6,7]] = 2
+
+        # Calculate transition probabilities
+        P = {}
+        for s in range(nS):
+            position = np.unravel_index(s, self.shape)
+            P[s] = { a : [] for a in range(n_actions) }
+            P[s][UP] = self._calculate_transition_prob(position, [-1, 0], winds)
+            P[s][RIGHT] = self._calculate_transition_prob(position, [0, 1], winds)
+            P[s][DOWN] = self._calculate_transition_prob(position, [1, 0], winds)
+            P[s][LEFT] = self._calculate_transition_prob(position, [0, -1], winds)
+
+        # We always start in state (3, 0)
+        isd = np.zeros(nS)
+        isd[np.ravel_multi_index((3,0), self.shape)] = 1.0
+
+        super(WindyGridworldEnv, self).__init__(nS, n_actions, P, isd)
+
+    def render(self, mode='human', close=False):
+        self._render(mode, close)
+
+    def _render(self, mode='human', close=False):
+        if close:
+            return
+
+        outfile = StringIO() if mode == 'ansi' else sys.stdout
+
+        for s in range(self.nS):
+            position = np.unravel_index(s, self.shape)
+            # print(self.s)
+            if self.s == s:
+                output = " x "
+            elif position == (3,7):
+                output = " T "
+            else:
+                output = " o "
+
+            if position[1] == 0:
+                output = output.lstrip()
+            if position[1] == self.shape[1] - 1:
+                output = output.rstrip()
+                output += "\n"
+
+            outfile.write(output)
+        outfile.write("\n")
```

### Comparing `joyrl-0.1.9/joyrl/envs/gridworld.py` & `joyrl-0.2.0/joyrl/envs/gridworld.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-import io
-import numpy as np
-import sys
-from gym.envs.toy_text import discrete
-
-UP = 0
-RIGHT = 1
-DOWN = 2
-LEFT = 3
-
-class GridworldEnv(discrete.DiscreteEnv):
-    """
-    Grid World environment from Sutton's Reinforcement Learning book chapter 4.
-    You are an agent on an MxN grid and your goal is to reach the terminal
-    state at the top left or the bottom right corner.
-
-    For example, a 4x4 grid looks as follows:
-
-    T  o  o  o
-    o  x  o  o
-    o  o  o  o
-    o  o  o  T
-
-    x is your position and T are the two terminal states.
-
-    You can take actions in each direction (UP=0, RIGHT=1, DOWN=2, LEFT=3).
-    Actions going off the edge leave you in your current state.
-    You receive a reward of -1 at each step until you reach a terminal state.
-    """
-
-    metadata = {'render.modes': ['human', 'ansi']}
-
-    def __init__(self, shape=[4,4]):
-        if not isinstance(shape, (list, tuple)) or not len(shape) == 2:
-            raise ValueError('shape argument must be a list/tuple of length 2')
-
-        self.shape = shape
-
-        nS = np.prod(shape)
-        n_actions = 4
-
-        MAX_Y = shape[0]
-        MAX_X = shape[1]
-
-        P = {}
-        grid = np.arange(nS).reshape(shape)
-        it = np.nditer(grid, flags=['multi_index'])
-
-        while not it.finished:
-            s = it.iterindex
-            y, x = it.multi_index
-
-            # P[s][a] = (prob, next_state, reward, is_done)
-            P[s] = {a : [] for a in range(n_actions)}
-
-            is_done = lambda s: s == 0 or s == (nS - 1)
-            reward = 0.0 if is_done(s) else -1.0
-
-            # We're stuck in a terminal state
-            if is_done(s):
-                P[s][UP] = [(1.0, s, reward, True)]
-                P[s][RIGHT] = [(1.0, s, reward, True)]
-                P[s][DOWN] = [(1.0, s, reward, True)]
-                P[s][LEFT] = [(1.0, s, reward, True)]
-            # Not a terminal state
-            else:
-                ns_up = s if y == 0 else s - MAX_X
-                ns_right = s if x == (MAX_X - 1) else s + 1
-                ns_down = s if y == (MAX_Y - 1) else s + MAX_X
-                ns_left = s if x == 0 else s - 1
-                P[s][UP] = [(1.0, ns_up, reward, is_done(ns_up))]
-                P[s][RIGHT] = [(1.0, ns_right, reward, is_done(ns_right))]
-                P[s][DOWN] = [(1.0, ns_down, reward, is_done(ns_down))]
-                P[s][LEFT] = [(1.0, ns_left, reward, is_done(ns_left))]
-
-            it.iternext()
-
-        # Initial state distribution is uniform
-        isd = np.ones(nS) / nS
-
-        # We expose the model of the environment for educational purposes
-        # This should not be used in any model-free learning algorithm
-        self.P = P
-
-        super(GridworldEnv, self).__init__(nS, n_actions, P, isd)
-
-    def _render(self, mode='human', close=False):
-        """ Renders the current gridworld layout
-
-         For example, a 4x4 grid with the mode="human" looks like:
-            T  o  o  o
-            o  x  o  o
-            o  o  o  o
-            o  o  o  T
-        where x is your position and T are the two terminal states.
-        """
-        if close:
-            return
-
-        outfile = io.StringIO() if mode == 'ansi' else sys.stdout
-
-        grid = np.arange(self.nS).reshape(self.shape)
-        it = np.nditer(grid, flags=['multi_index'])
-        while not it.finished:
-            s = it.iterindex
-            y, x = it.multi_index
-
-            if self.s == s:
-                output = " x "
-            elif s == 0 or s == self.nS - 1:
-                output = " T "
-            else:
-                output = " o "
-
-            if x == 0:
-                output = output.lstrip()
-            if x == self.shape[1] - 1:
-                output = output.rstrip()
-
-            outfile.write(output)
-
-            if x == self.shape[1] - 1:
-                outfile.write("\n")
-
-            it.iternext()
+import io
+import numpy as np
+import sys
+from gym.envs.toy_text import discrete
+
+UP = 0
+RIGHT = 1
+DOWN = 2
+LEFT = 3
+
+class GridworldEnv(discrete.DiscreteEnv):
+    """
+    Grid World environment from Sutton's Reinforcement Learning book chapter 4.
+    You are an agent on an MxN grid and your goal is to reach the terminal
+    state at the top left or the bottom right corner.
+
+    For example, a 4x4 grid looks as follows:
+
+    T  o  o  o
+    o  x  o  o
+    o  o  o  o
+    o  o  o  T
+
+    x is your position and T are the two terminal states.
+
+    You can take actions in each direction (UP=0, RIGHT=1, DOWN=2, LEFT=3).
+    Actions going off the edge leave you in your current state.
+    You receive a reward of -1 at each step until you reach a terminal state.
+    """
+
+    metadata = {'render.modes': ['human', 'ansi']}
+
+    def __init__(self, shape=[4,4]):
+        if not isinstance(shape, (list, tuple)) or not len(shape) == 2:
+            raise ValueError('shape argument must be a list/tuple of length 2')
+
+        self.shape = shape
+
+        nS = np.prod(shape)
+        n_actions = 4
+
+        MAX_Y = shape[0]
+        MAX_X = shape[1]
+
+        P = {}
+        grid = np.arange(nS).reshape(shape)
+        it = np.nditer(grid, flags=['multi_index'])
+
+        while not it.finished:
+            s = it.iterindex
+            y, x = it.multi_index
+
+            # P[s][a] = (prob, next_state, reward, is_done)
+            P[s] = {a : [] for a in range(n_actions)}
+
+            is_done = lambda s: s == 0 or s == (nS - 1)
+            reward = 0.0 if is_done(s) else -1.0
+
+            # We're stuck in a terminal state
+            if is_done(s):
+                P[s][UP] = [(1.0, s, reward, True)]
+                P[s][RIGHT] = [(1.0, s, reward, True)]
+                P[s][DOWN] = [(1.0, s, reward, True)]
+                P[s][LEFT] = [(1.0, s, reward, True)]
+            # Not a terminal state
+            else:
+                ns_up = s if y == 0 else s - MAX_X
+                ns_right = s if x == (MAX_X - 1) else s + 1
+                ns_down = s if y == (MAX_Y - 1) else s + MAX_X
+                ns_left = s if x == 0 else s - 1
+                P[s][UP] = [(1.0, ns_up, reward, is_done(ns_up))]
+                P[s][RIGHT] = [(1.0, ns_right, reward, is_done(ns_right))]
+                P[s][DOWN] = [(1.0, ns_down, reward, is_done(ns_down))]
+                P[s][LEFT] = [(1.0, ns_left, reward, is_done(ns_left))]
+
+            it.iternext()
+
+        # Initial state distribution is uniform
+        isd = np.ones(nS) / nS
+
+        # We expose the model of the environment for educational purposes
+        # This should not be used in any model-free learning algorithm
+        self.P = P
+
+        super(GridworldEnv, self).__init__(nS, n_actions, P, isd)
+
+    def _render(self, mode='human', close=False):
+        """ Renders the current gridworld layout
+
+         For example, a 4x4 grid with the mode="human" looks like:
+            T  o  o  o
+            o  x  o  o
+            o  o  o  o
+            o  o  o  T
+        where x is your position and T are the two terminal states.
+        """
+        if close:
+            return
+
+        outfile = io.StringIO() if mode == 'ansi' else sys.stdout
+
+        grid = np.arange(self.nS).reshape(self.shape)
+        it = np.nditer(grid, flags=['multi_index'])
+        while not it.finished:
+            s = it.iterindex
+            y, x = it.multi_index
+
+            if self.s == s:
+                output = " x "
+            elif s == 0 or s == self.nS - 1:
+                output = " T "
+            else:
+                output = " o "
+
+            if x == 0:
+                output = output.lstrip()
+            if x == self.shape[1] - 1:
+                output = output.rstrip()
+
+            outfile.write(output)
+
+            if x == self.shape[1] - 1:
+                outfile.write("\n")
+
+            it.iternext()
```

### Comparing `joyrl-0.1.9/joyrl/envs/gridworld_env.py` & `joyrl-0.2.0/joyrl/envs/gridworld_env.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-import gym
-import turtle
-import numpy as np
-
-# turtle tutorial : https://docs.python.org/3.3/library/turtle.html
-
-def GridWorld(gridmap=None, is_slippery=False):
-    if gridmap is None:
-        gridmap = ['SFFF', 'FHFH', 'FFFH', 'HFFG']
-    env = gym.make("FrozenLake-v0", desc=gridmap, is_slippery=False)
-    env = FrozenLakeWapper(env)
-    return env
-
-
-class FrozenLakeWapper(gym.Wrapper):
-    def __init__(self, env):
-        gym.Wrapper.__init__(self, env)
-        self.max_y = env.desc.shape[0]
-        self.max_x = env.desc.shape[1]
-        self.t = None
-        self.unit = 50
-
-    def draw_box(self, x, y, fillcolor='', line_color='gray'):
-        self.t.up()
-        self.t.goto(x * self.unit, y * self.unit)
-        self.t.color(line_color)
-        self.t.fillcolor(fillcolor)
-        self.t.setheading(90)
-        self.t.down()
-        self.t.begin_fill()
-        for _ in range(4):
-            self.t.forward(self.unit)
-            self.t.right(90)
-        self.t.end_fill()
-
-    def move_player(self, x, y):
-        self.t.up()
-        self.t.setheading(90)
-        self.t.fillcolor('red')
-        self.t.goto((x + 0.5) * self.unit, (y + 0.5) * self.unit)
-
-    def render(self):
-        if self.t == None:
-            self.t = turtle.Turtle()
-            self.wn = turtle.Screen()
-            self.wn.setup(self.unit * self.max_x + 100,
-                          self.unit * self.max_y + 100)
-            self.wn.setworldcoordinates(0, 0, self.unit * self.max_x,
-                                        self.unit * self.max_y)
-            self.t.shape('circle')
-            self.t.width(2)
-            self.t.speed(0)
-            self.t.color('gray')
-            for i in range(self.desc.shape[0]):
-                for j in range(self.desc.shape[1]):
-                    x = j
-                    y = self.max_y - 1 - i
-                    if self.desc[i][j] == b'S':  # Start
-                        self.draw_box(x, y, 'white')
-                    elif self.desc[i][j] == b'F':  # Frozen ice
-                        self.draw_box(x, y, 'white')
-                    elif self.desc[i][j] == b'G':  # Goal
-                        self.draw_box(x, y, 'yellow')
-                    elif self.desc[i][j] == b'H':  # Hole
-                        self.draw_box(x, y, 'black')
-                    else:
-                        self.draw_box(x, y, 'white')
-            self.t.shape('turtle')
-
-        x_pos = self.s % self.max_x
-        y_pos = self.max_y - 1 - int(self.s / self.max_x)
-        self.move_player(x_pos, y_pos)
-
-
-
-if __name__ == '__main__':
-    # 环境1：FrozenLake, 可以配置冰面是否是滑的
-    # 0 left, 1 down, 2 right, 3 up
-    env = gym.make("FrozenLake-v0", is_slippery=False)
-    env = FrozenLakeWapper(env)
-
-    # 环境2：CliffWalking, 悬崖环境
-    # env = gym.make("CliffWalking-v0")  # 0 up, 1 right, 2 down, 3 left
-    # env = CliffWalkingWapper(env)
-
-    # 环境3：自定义格子世界，可以配置地图, S为出发点Start, F为平地Floor, H为洞Hole, G为出口目标Goal
-    # gridmap = [
-    #         'SFFF',
-    #         'FHFF',
-    #         'FFFF',
-    #         'HFGF' ]
-    # env = GridWorld(gridmap)
-
-    env.reset()
-    for step in range(10):
-        action = np.random.randint(0, 4)
-        obs, reward, done, info = env.step(action)
-        print('step {}: action {}, obs {}, reward {}, done {}, info {}'.format(\
-                step, action, obs, reward, done, info))
+import gym
+import turtle
+import numpy as np
+
+# turtle tutorial : https://docs.python.org/3.3/library/turtle.html
+
+def GridWorld(gridmap=None, is_slippery=False):
+    if gridmap is None:
+        gridmap = ['SFFF', 'FHFH', 'FFFH', 'HFFG']
+    env = gym.make("FrozenLake-v0", desc=gridmap, is_slippery=False)
+    env = FrozenLakeWapper(env)
+    return env
+
+
+class FrozenLakeWapper(gym.Wrapper):
+    def __init__(self, env):
+        gym.Wrapper.__init__(self, env)
+        self.max_y = env.desc.shape[0]
+        self.max_x = env.desc.shape[1]
+        self.t = None
+        self.unit = 50
+
+    def draw_box(self, x, y, fillcolor='', line_color='gray'):
+        self.t.up()
+        self.t.goto(x * self.unit, y * self.unit)
+        self.t.color(line_color)
+        self.t.fillcolor(fillcolor)
+        self.t.setheading(90)
+        self.t.down()
+        self.t.begin_fill()
+        for _ in range(4):
+            self.t.forward(self.unit)
+            self.t.right(90)
+        self.t.end_fill()
+
+    def move_player(self, x, y):
+        self.t.up()
+        self.t.setheading(90)
+        self.t.fillcolor('red')
+        self.t.goto((x + 0.5) * self.unit, (y + 0.5) * self.unit)
+
+    def render(self):
+        if self.t == None:
+            self.t = turtle.Turtle()
+            self.wn = turtle.Screen()
+            self.wn.setup(self.unit * self.max_x + 100,
+                          self.unit * self.max_y + 100)
+            self.wn.setworldcoordinates(0, 0, self.unit * self.max_x,
+                                        self.unit * self.max_y)
+            self.t.shape('circle')
+            self.t.width(2)
+            self.t.speed(0)
+            self.t.color('gray')
+            for i in range(self.desc.shape[0]):
+                for j in range(self.desc.shape[1]):
+                    x = j
+                    y = self.max_y - 1 - i
+                    if self.desc[i][j] == b'S':  # Start
+                        self.draw_box(x, y, 'white')
+                    elif self.desc[i][j] == b'F':  # Frozen ice
+                        self.draw_box(x, y, 'white')
+                    elif self.desc[i][j] == b'G':  # Goal
+                        self.draw_box(x, y, 'yellow')
+                    elif self.desc[i][j] == b'H':  # Hole
+                        self.draw_box(x, y, 'black')
+                    else:
+                        self.draw_box(x, y, 'white')
+            self.t.shape('turtle')
+
+        x_pos = self.s % self.max_x
+        y_pos = self.max_y - 1 - int(self.s / self.max_x)
+        self.move_player(x_pos, y_pos)
+
+
+
+if __name__ == '__main__':
+    # 环境1：FrozenLake, 可以配置冰面是否是滑的
+    # 0 left, 1 down, 2 right, 3 up
+    env = gym.make("FrozenLake-v0", is_slippery=False)
+    env = FrozenLakeWapper(env)
+
+    # 环境2：CliffWalking, 悬崖环境
+    # env = gym.make("CliffWalking-v0")  # 0 up, 1 right, 2 down, 3 left
+    # env = CliffWalkingWapper(env)
+
+    # 环境3：自定义格子世界，可以配置地图, S为出发点Start, F为平地Floor, H为洞Hole, G为出口目标Goal
+    # gridmap = [
+    #         'SFFF',
+    #         'FHFF',
+    #         'FFFF',
+    #         'HFGF' ]
+    # env = GridWorld(gridmap)
+
+    env.reset()
+    for step in range(10):
+        action = np.random.randint(0, 4)
+        obs, reward, done, info = env.step(action)
+        print('step {}: action {}, obs {}, reward {}, done {}, info {}'.format(\
+                step, action, obs, reward, done, info))
         # env.render() # 渲染一帧图像
```

### Comparing `joyrl-0.1.9/joyrl/envs/racetrack.py` & `joyrl-0.2.0/joyrl/envs/racetrack.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,242 +1,242 @@
-import time
-import random
-import numpy as np
-import os
-import matplotlib.pyplot as plt
-import matplotlib.patheffects as pe
-from IPython.display import clear_output
-from gym.spaces import Discrete,Box
-from matplotlib import colors
-import gym
-
-class RacetrackEnv(gym.Env) :
-    """
-    Class representing a race-track environment inspired by exercise 5.12 in Sutton & Barto 2018 (p.111).
-    Please do not make changes to this class - it will be overwritten with a clean version when it comes to marking.
-
-    The dynamics of this environment are detailed in this coursework exercise's jupyter notebook, although I have
-    included rather verbose comments here  for those of you who are interested in how the environment has been
-    implemented (though this should not impact your solution code).ss
-    """
-
-    ACTIONS_DICT = {
-        0 : (1, -1),  # Acc Vert., Brake Horiz.
-        1 : (1, 0),   # Acc Vert., Hold Horiz.
-        2 : (1, 1),   # Acc Vert., Acc Horiz.
-        3 : (0, -1),  # Hold Vert., Brake Horiz.
-        4 : (0, 0),   # Hold Vert., Hold Horiz.
-        5 : (0, 1),   # Hold Vert., Acc Horiz.
-        6 : (-1, -1), # Brake Vert., Brake Horiz.
-        7 : (-1, 0),  # Brake Vert., Hold Horiz.
-        8 : (-1, 1)   # Brake Vert., Acc Horiz.
-    }
-
-
-    CELL_TYPES_DICT = {
-        0 : "track",
-        1 : "wall",
-        2 : "start",
-        3 : "goal"
-    }
-
-
-    def __init__(self) :
-        # Load racetrack map from file.
-        self.track = np.flip(np.loadtxt(os.path.dirname(__file__)+"/track.txt", dtype = int), axis = 0)
-
-
-        # Discover start grid squares.
-        self.initial_states = []
-        for y in range(self.track.shape[0]) :
-            for x in range(self.track.shape[1]) :
-                if (self.CELL_TYPES_DICT[self.track[y, x]] == "start") :
-                    self.initial_states.append((y, x))
-        high= np.array([np.finfo(np.float32).max, np.finfo(np.float32).max, np.finfo(np.float32).max, np.finfo(np.float32).max])
-        self.observation_space = Box(low=-high, high=high, shape=(4,), dtype=np.float32)
-        self.action_space = Discrete(9)
-        self.is_reset = False
-
-    def step(self, action : int) :
-        """
-        Takes a given action in the environment's current state, and returns a next state,
-        reward, and whether the next state is done or not.
-
-        Arguments:
-            action {int} -- The action to take in the environment's current state. Should be an integer in the range [0-8].
-
-        Raises:
-            RuntimeError: Raised when the environment needs resetting.\n
-            TypeError: Raised when an action of an invalid type is given.\n
-            ValueError: Raised when an action outside the range [0-8] is given.\n
-
-        Returns:
-            A tuple of:\n
-                {(int, int, int, int)} -- The next state, a tuple of (y_pos, x_pos, y_velocity, x_velocity).\n
-                {int} -- The reward earned by taking the given action in the current environment state.\n
-                {bool} -- Whether the environment's next state is done or not.\n
-
-        """
-
-        # Check whether a reset is needed.
-        if (not self.is_reset) :
-            raise RuntimeError(".step() has been called when .reset() is needed.\n" +
-                               "You need to call .reset() before using .step() for the first time, and after an episode ends.\n" +
-                               ".reset() initialises the environment at the start of an episode, then returns an initial state.")
-
-        # Check that action is the correct type (either a python integer or a numpy integer).
-        if (not (isinstance(action, int) or isinstance(action, np.integer))) :
-            raise TypeError("action should be an integer.\n" +
-                            "action value {} of type {} was supplied.".format(action, type(action)))
-
-        # Check that action is an allowed value.
-        if (action < 0 or action > 8) :
-            raise ValueError("action must be an integer in the range [0-8] corresponding to one of the legal actions.\n" +
-                             "action value {} was supplied.".format(action))
-
-
-        # Update Velocity.
-        # With probability, 0.85 update velocity components as intended.
-        if (np.random.uniform() < 0.8) :
-            (d_y, d_x) = self.ACTIONS_DICT[action]
-        # With probability, 0.15 Do not change velocity components.
-        else :
-            (d_y, d_x) = (0, 0)
-
-        self.velocity = (self.velocity[0] + d_y, self.velocity[1] + d_x)
-
-		# Keep velocity within bounds (-10, 10).
-        if (self.velocity[0] > 10) :
-            self.velocity[0] = 10
-        elif (self.velocity[0] < -10) :
-            self.velocity[0] = -10
-        if (self.velocity[1] > 10) :
-            self.velocity[1] = 10
-        elif (self.velocity[1] < -10) :
-            self.velocity[1] = -10
-
-        # Update Position.
-        new_position = (self.position[0] + self.velocity[0], self.position[1] + self.velocity[1])
-
-        reward = 0
-        done = False
-
-        # If position is out-of-bounds, return to start and set velocity components to zero.
-        if (new_position[0] < 0 or new_position[1] < 0 or new_position[0] >= self.track.shape[0] or new_position[1] >= self.track.shape[1]) :
-            self.position = random.choice(self.initial_states)
-            self.velocity = (0, 0)
-            reward -= 10
-        # If position is in a wall grid-square, return to start and set velocity components to zero.
-        elif (self.CELL_TYPES_DICT[self.track[new_position]] == "wall") :
-            self.position = random.choice(self.initial_states)
-            self.velocity = (0, 0)
-            reward -= 10
-        # If position is in a track grid-squre or a start-square, update position.
-        elif (self.CELL_TYPES_DICT[self.track[new_position]] in ["track", "start"]) :
-            self.position = new_position
-        # If position is in a goal grid-square, end episode.
-        elif (self.CELL_TYPES_DICT[self.track[new_position]] == "goal") :
-            self.position = new_position
-            reward += 10
-            done = True
-        # If this gets reached, then the student has touched something they shouldn't have. Naughty!
-        else :
-            raise RuntimeError("You've met with a terrible fate, haven't you?\nDon't modify things you shouldn't!")
-
-        # Penalise every timestep.
-        reward -= 1
-
-        # Require a reset if the current state is done.
-        if (done) :
-            self.is_reset = False
-
-        # Return next state, reward, and whether the episode has ended.
-        return np.array([self.position[0], self.position[1], self.velocity[0], self.velocity[1]]), reward, done,{}
-
-
-    def reset(self) :
-        """
-        Resets the environment, ready for a new episode to begin, then returns an initial state.
-        The initial state will be a starting grid square randomly chosen using a uniform distribution,
-        with both components of the velocity being zero.
-
-        Returns:
-            {(int, int, int, int)} -- an initial state, a tuple of (y_pos, x_pos, y_velocity, x_velocity).
-        """
-
-        # Pick random starting grid-square.
-        self.position = random.choice(self.initial_states)
-
-        # Set both velocity components to zero.
-        self.velocity = (0, 0)
-
-        self.is_reset = True
-
-        return np.array([self.position[0], self.position[1], self.velocity[0], self.velocity[1]])
-
-
-    def render(self, mode = 'human') :
-        """
-        Renders a pretty matplotlib plot representing the current state of the environment.
-        Calling this method on subsequent timesteps will update the plot.
-        This is VERY VERY SLOW and wil slow down training a lot. Only use for debugging/testing.
-
-        Arguments:
-            sleep_time {float} -- How many seconds (or partial seconds) you want to wait on this rendered frame.
-
-        """
-        # Turn interactive mode on.
-        plt.ion()
-        fig = plt.figure(num = "env_render")
-        ax = plt.gca()
-        ax.clear()
-        clear_output(wait = True)
-
-        # Prepare the environment plot and mark the car's position.
-        env_plot = np.copy(self.track)
-        env_plot[self.position] = 4
-        env_plot = np.flip(env_plot, axis = 0)
-
-        # Plot the gridworld.
-        cmap = colors.ListedColormap(["white", "black", "green", "red", "yellow"])
-        bounds = list(range(6))
-        norm = colors.BoundaryNorm(bounds, cmap.N)
-        ax.imshow(env_plot, cmap = cmap, norm = norm, zorder = 0)
-
-        # Plot the velocity.
-        if (not self.velocity == (0, 0)) :
-            ax.arrow(self.position[1], self.track.shape[0] - 1 - self.position[0], self.velocity[1], -self.velocity[0],
-                     path_effects=[pe.Stroke(linewidth=1, foreground='black')], color = "yellow", width = 0.1, length_includes_head = True, zorder = 2)
-
-        # Set up axes.
-        ax.grid(which = 'major', axis = 'both', linestyle = '-', color = 'k', linewidth = 2, zorder = 1)
-        ax.set_xticks(np.arange(-0.5, self.track.shape[1] , 1));
-        ax.set_xticklabels([])
-        ax.set_yticks(np.arange(-0.5, self.track.shape[0], 1));
-        ax.set_yticklabels([])
-
-        # Draw everything.
-        #fig.canvas.draw()
-        #fig.canvas.flush_events()
-        plt.show()
-        # time sleep
-        time.sleep(0.1)
-
-    def get_actions(self) :
-        """
-        Returns the available actions in the current state - will always be a list
-        of integers in the range [0-8].
-        """
-        return [*self.ACTIONS_DICT]
-if __name__ == "__main__":
-    num_steps = 1000000
-    env = RacetrackEnv()
-    state = env.reset()
-    print(state)
-    for _ in range(num_steps) :
-
-        next_state, reward, done,_ = env.step(random.choice(env.get_actions()))
-        print(next_state)
-        env.render()
-
-        if (done) :
-            _ = env.reset()
+import time
+import random
+import numpy as np
+import os
+import matplotlib.pyplot as plt
+import matplotlib.patheffects as pe
+from IPython.display import clear_output
+from gym.spaces import Discrete,Box
+from matplotlib import colors
+import gym
+
+class RacetrackEnv(gym.Env) :
+    """
+    Class representing a race-track environment inspired by exercise 5.12 in Sutton & Barto 2018 (p.111).
+    Please do not make changes to this class - it will be overwritten with a clean version when it comes to marking.
+
+    The dynamics of this environment are detailed in this coursework exercise's jupyter notebook, although I have
+    included rather verbose comments here  for those of you who are interested in how the environment has been
+    implemented (though this should not impact your solution code).ss
+    """
+
+    ACTIONS_DICT = {
+        0 : (1, -1),  # Acc Vert., Brake Horiz.
+        1 : (1, 0),   # Acc Vert., Hold Horiz.
+        2 : (1, 1),   # Acc Vert., Acc Horiz.
+        3 : (0, -1),  # Hold Vert., Brake Horiz.
+        4 : (0, 0),   # Hold Vert., Hold Horiz.
+        5 : (0, 1),   # Hold Vert., Acc Horiz.
+        6 : (-1, -1), # Brake Vert., Brake Horiz.
+        7 : (-1, 0),  # Brake Vert., Hold Horiz.
+        8 : (-1, 1)   # Brake Vert., Acc Horiz.
+    }
+
+
+    CELL_TYPES_DICT = {
+        0 : "track",
+        1 : "wall",
+        2 : "start",
+        3 : "goal"
+    }
+
+
+    def __init__(self) :
+        # Load racetrack map from file.
+        self.track = np.flip(np.loadtxt(os.path.dirname(__file__)+"/track.txt", dtype = int), axis = 0)
+
+
+        # Discover start grid squares.
+        self.initial_states = []
+        for y in range(self.track.shape[0]) :
+            for x in range(self.track.shape[1]) :
+                if (self.CELL_TYPES_DICT[self.track[y, x]] == "start") :
+                    self.initial_states.append((y, x))
+        high= np.array([np.finfo(np.float32).max, np.finfo(np.float32).max, np.finfo(np.float32).max, np.finfo(np.float32).max])
+        self.observation_space = Box(low=-high, high=high, shape=(4,), dtype=np.float32)
+        self.action_space = Discrete(9)
+        self.is_reset = False
+
+    def step(self, action : int) :
+        """
+        Takes a given action in the environment's current state, and returns a next state,
+        reward, and whether the next state is done or not.
+
+        Arguments:
+            action {int} -- The action to take in the environment's current state. Should be an integer in the range [0-8].
+
+        Raises:
+            RuntimeError: Raised when the environment needs resetting.\n
+            TypeError: Raised when an action of an invalid type is given.\n
+            ValueError: Raised when an action outside the range [0-8] is given.\n
+
+        Returns:
+            A tuple of:\n
+                {(int, int, int, int)} -- The next state, a tuple of (y_pos, x_pos, y_velocity, x_velocity).\n
+                {int} -- The reward earned by taking the given action in the current environment state.\n
+                {bool} -- Whether the environment's next state is done or not.\n
+
+        """
+
+        # Check whether a reset is needed.
+        if (not self.is_reset) :
+            raise RuntimeError(".step() has been called when .reset() is needed.\n" +
+                               "You need to call .reset() before using .step() for the first time, and after an episode ends.\n" +
+                               ".reset() initialises the environment at the start of an episode, then returns an initial state.")
+
+        # Check that action is the correct type (either a python integer or a numpy integer).
+        if (not (isinstance(action, int) or isinstance(action, np.integer))) :
+            raise TypeError("action should be an integer.\n" +
+                            "action value {} of type {} was supplied.".format(action, type(action)))
+
+        # Check that action is an allowed value.
+        if (action < 0 or action > 8) :
+            raise ValueError("action must be an integer in the range [0-8] corresponding to one of the legal actions.\n" +
+                             "action value {} was supplied.".format(action))
+
+
+        # Update Velocity.
+        # With probability, 0.85 update velocity components as intended.
+        if (np.random.uniform() < 0.8) :
+            (d_y, d_x) = self.ACTIONS_DICT[action]
+        # With probability, 0.15 Do not change velocity components.
+        else :
+            (d_y, d_x) = (0, 0)
+
+        self.velocity = (self.velocity[0] + d_y, self.velocity[1] + d_x)
+
+		# Keep velocity within bounds (-10, 10).
+        if (self.velocity[0] > 10) :
+            self.velocity[0] = 10
+        elif (self.velocity[0] < -10) :
+            self.velocity[0] = -10
+        if (self.velocity[1] > 10) :
+            self.velocity[1] = 10
+        elif (self.velocity[1] < -10) :
+            self.velocity[1] = -10
+
+        # Update Position.
+        new_position = (self.position[0] + self.velocity[0], self.position[1] + self.velocity[1])
+
+        reward = 0
+        done = False
+
+        # If position is out-of-bounds, return to start and set velocity components to zero.
+        if (new_position[0] < 0 or new_position[1] < 0 or new_position[0] >= self.track.shape[0] or new_position[1] >= self.track.shape[1]) :
+            self.position = random.choice(self.initial_states)
+            self.velocity = (0, 0)
+            reward -= 10
+        # If position is in a wall grid-square, return to start and set velocity components to zero.
+        elif (self.CELL_TYPES_DICT[self.track[new_position]] == "wall") :
+            self.position = random.choice(self.initial_states)
+            self.velocity = (0, 0)
+            reward -= 10
+        # If position is in a track grid-squre or a start-square, update position.
+        elif (self.CELL_TYPES_DICT[self.track[new_position]] in ["track", "start"]) :
+            self.position = new_position
+        # If position is in a goal grid-square, end episode.
+        elif (self.CELL_TYPES_DICT[self.track[new_position]] == "goal") :
+            self.position = new_position
+            reward += 10
+            done = True
+        # If this gets reached, then the student has touched something they shouldn't have. Naughty!
+        else :
+            raise RuntimeError("You've met with a terrible fate, haven't you?\nDon't modify things you shouldn't!")
+
+        # Penalise every timestep.
+        reward -= 1
+
+        # Require a reset if the current state is done.
+        if (done) :
+            self.is_reset = False
+
+        # Return next state, reward, and whether the episode has ended.
+        return np.array([self.position[0], self.position[1], self.velocity[0], self.velocity[1]]), reward, done,{}
+
+
+    def reset(self) :
+        """
+        Resets the environment, ready for a new episode to begin, then returns an initial state.
+        The initial state will be a starting grid square randomly chosen using a uniform distribution,
+        with both components of the velocity being zero.
+
+        Returns:
+            {(int, int, int, int)} -- an initial state, a tuple of (y_pos, x_pos, y_velocity, x_velocity).
+        """
+
+        # Pick random starting grid-square.
+        self.position = random.choice(self.initial_states)
+
+        # Set both velocity components to zero.
+        self.velocity = (0, 0)
+
+        self.is_reset = True
+
+        return np.array([self.position[0], self.position[1], self.velocity[0], self.velocity[1]])
+
+
+    def render(self, mode = 'human') :
+        """
+        Renders a pretty matplotlib plot representing the current state of the environment.
+        Calling this method on subsequent timesteps will update the plot.
+        This is VERY VERY SLOW and wil slow down training a lot. Only use for debugging/testing.
+
+        Arguments:
+            sleep_time {float} -- How many seconds (or partial seconds) you want to wait on this rendered frame.
+
+        """
+        # Turn interactive mode on.
+        plt.ion()
+        fig = plt.figure(num = "env_render")
+        ax = plt.gca()
+        ax.clear()
+        clear_output(wait = True)
+
+        # Prepare the environment plot and mark the car's position.
+        env_plot = np.copy(self.track)
+        env_plot[self.position] = 4
+        env_plot = np.flip(env_plot, axis = 0)
+
+        # Plot the gridworld.
+        cmap = colors.ListedColormap(["white", "black", "green", "red", "yellow"])
+        bounds = list(range(6))
+        norm = colors.BoundaryNorm(bounds, cmap.N)
+        ax.imshow(env_plot, cmap = cmap, norm = norm, zorder = 0)
+
+        # Plot the velocity.
+        if (not self.velocity == (0, 0)) :
+            ax.arrow(self.position[1], self.track.shape[0] - 1 - self.position[0], self.velocity[1], -self.velocity[0],
+                     path_effects=[pe.Stroke(linewidth=1, foreground='black')], color = "yellow", width = 0.1, length_includes_head = True, zorder = 2)
+
+        # Set up axes.
+        ax.grid(which = 'major', axis = 'both', linestyle = '-', color = 'k', linewidth = 2, zorder = 1)
+        ax.set_xticks(np.arange(-0.5, self.track.shape[1] , 1));
+        ax.set_xticklabels([])
+        ax.set_yticks(np.arange(-0.5, self.track.shape[0], 1));
+        ax.set_yticklabels([])
+
+        # Draw everything.
+        #fig.canvas.draw()
+        #fig.canvas.flush_events()
+        plt.show()
+        # time sleep
+        time.sleep(0.1)
+
+    def get_actions(self) :
+        """
+        Returns the available actions in the current state - will always be a list
+        of integers in the range [0-8].
+        """
+        return [*self.ACTIONS_DICT]
+if __name__ == "__main__":
+    num_steps = 1000000
+    env = RacetrackEnv()
+    state = env.reset()
+    print(state)
+    for _ in range(num_steps) :
+
+        next_state, reward, done,_ = env.step(random.choice(env.get_actions()))
+        print(next_state)
+        env.render()
+
+        if (done) :
+            _ = env.reset()
```

### Comparing `joyrl-0.1.9/joyrl/envs/register.py` & `joyrl-0.2.0/joyrl/envs/register.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-
-from gym.envs.registration import register
-
-def register_env(env_name):
-    if env_name == 'Racetrack-v0':
-        register(
-            id='Racetrack-v0',
-            entry_point='envs.racetrack:RacetrackEnv',
-            max_episode_steps=1000,
-            kwargs={}
-        )
-    elif env_name == 'FrozenLakeNoSlippery-v1':
-        register(
-            id='FrozenLakeNoSlippery-v1',
-            entry_point='gym.envs.toy_text.frozen_lake:FrozenLakeEnv',
-            kwargs={'map_name':"4x4",'is_slippery':False},
-        )
-    else:
-        print("The env name must be wrong or the environment donot need to register!")
-
-# if __name__ == "__main__":
-#     import random
-#     import gym
-#     env = gym.make('FrozenLakeNoSlippery-v1')
-#     num_steps = 1000000
-#     state = env.reset()
-#     n_actions = env.action_space.n
-#     print(state)
-#     for _ in range(num_steps) :
-#         next_state, reward, done,_ = env.step(random.choice(range(n_actions)))
-#         print(next_state)
-#         if (done) :
-#             _ = env.reset()
+
+from gym.envs.registration import register
+
+def register_env(env_name):
+    if env_name == 'Racetrack-v0':
+        register(
+            id='Racetrack-v0',
+            entry_point='envs.racetrack:RacetrackEnv',
+            max_episode_steps=1000,
+            kwargs={}
+        )
+    elif env_name == 'FrozenLakeNoSlippery-v1':
+        register(
+            id='FrozenLakeNoSlippery-v1',
+            entry_point='gym.envs.toy_text.frozen_lake:FrozenLakeEnv',
+            kwargs={'map_name':"4x4",'is_slippery':False},
+        )
+    else:
+        print("The env name must be wrong or the environment donot need to register!")
+
+# if __name__ == "__main__":
+#     import random
+#     import gym
+#     env = gym.make('FrozenLakeNoSlippery-v1')
+#     num_steps = 1000000
+#     state = env.reset()
+#     n_actions = env.action_space.n
+#     print(state)
+#     for _ in range(num_steps) :
+#         next_state, reward, done,_ = env.step(random.choice(range(n_actions)))
+#         print(next_state)
+#         if (done) :
+#             _ = env.reset()
```

### Comparing `joyrl-0.1.9/joyrl/envs/stochastic_mdp.py` & `joyrl-0.2.0/joyrl/envs/stochastic_mdp.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-#!/usr/bin/env python
-# coding=utf-8
-'''
-Author: John
-Email: johnjim0816@gmail.com
-Date: 2021-03-24 22:12:19
-LastEditor: John
-LastEditTime: 2021-03-26 17:12:43
-Discription: 
-Environment: 
-'''
-import numpy as np
-import random
-
-
-class StochasticMDP:
-    def __init__(self):
-        self.end = False
-        self.curr_state = 2
-        self.n_actions = 2
-        self.n_states = 6
-        self.p_right = 0.5
-
-    def reset(self):
-        self.end = False
-        self.curr_state = 2
-        state = np.zeros(self.n_states)
-        state[self.curr_state - 1] = 1.
-        return state
-
-    def step(self, action):
-        if self.curr_state != 1:
-            if action == 1:
-                if random.random() < self.p_right and self.curr_state < self.n_states:
-                    self.curr_state += 1
-                else:
-                    self.curr_state -= 1
-
-            if action == 0:
-                self.curr_state -= 1
-        if self.curr_state == self.n_states:
-            self.end = True
-
-        state = np.zeros(self.n_states)
-        state[self.curr_state - 1] = 1.
-
-        if self.curr_state == 1:
-            if self.end:
-                return state, 1.00, True, {}
-            else:
-                return state, 1.00/100.00, True, {}
-        else:
-            return state, 0.0, False, {}
+#!/usr/bin/env python
+# coding=utf-8
+'''
+Author: John
+Email: johnjim0816@gmail.com
+Date: 2021-03-24 22:12:19
+LastEditor: John
+LastEditTime: 2021-03-26 17:12:43
+Discription: 
+Environment: 
+'''
+import numpy as np
+import random
+
+
+class StochasticMDP:
+    def __init__(self):
+        self.end = False
+        self.curr_state = 2
+        self.n_actions = 2
+        self.n_states = 6
+        self.p_right = 0.5
+
+    def reset(self):
+        self.end = False
+        self.curr_state = 2
+        state = np.zeros(self.n_states)
+        state[self.curr_state - 1] = 1.
+        return state
+
+    def step(self, action):
+        if self.curr_state != 1:
+            if action == 1:
+                if random.random() < self.p_right and self.curr_state < self.n_states:
+                    self.curr_state += 1
+                else:
+                    self.curr_state -= 1
+
+            if action == 0:
+                self.curr_state -= 1
+        if self.curr_state == self.n_states:
+            self.end = True
+
+        state = np.zeros(self.n_states)
+        state[self.curr_state - 1] = 1.
+
+        if self.curr_state == 1:
+            if self.end:
+                return state, 1.00, True, {}
+            else:
+                return state, 1.00/100.00, True, {}
+        else:
+            return state, 0.0, False, {}
```

### Comparing `joyrl-0.1.9/joyrl/envs/wrappers.py` & `joyrl-0.2.0/joyrl/envs/wrappers.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-import gym
-class CliffWalkingWapper(gym.Wrapper):
-    def __init__(self, env):
-        gym.Wrapper.__init__(self, env)
-        self.t = None
-        self.unit = 50
-        self.max_x = 12
-        self.max_y = 4
-
-    def draw_x_line(self, y, x0, x1, color='gray'):
-        assert x1 > x0
-        self.t.color(color)
-        self.t.setheading(0)
-        self.t.up()
-        self.t.goto(x0, y)
-        self.t.down()
-        self.t.forward(x1 - x0)
-
-    def draw_y_line(self, x, y0, y1, color='gray'):
-        assert y1 > y0
-        self.t.color(color)
-        self.t.setheading(90)
-        self.t.up()
-        self.t.goto(x, y0)
-        self.t.down()
-        self.t.forward(y1 - y0)
-
-    def draw_box(self, x, y, fillcolor='', line_color='gray'):
-        self.t.up()
-        self.t.goto(x * self.unit, y * self.unit)
-        self.t.color(line_color)
-        self.t.fillcolor(fillcolor)
-        self.t.setheading(90)
-        self.t.down()
-        self.t.begin_fill()
-        for i in range(4):
-            self.t.forward(self.unit)
-            self.t.right(90)
-        self.t.end_fill()
-
-    def move_player(self, x, y):
-        self.t.up()
-        self.t.setheading(90)
-        self.t.fillcolor('red')
-        self.t.goto((x + 0.5) * self.unit, (y + 0.5) * self.unit)
-
-    def render(self):
-        if self.t == None:
-            self.t = turtle.Turtle()
-            self.wn = turtle.Screen()
-            self.wn.setup(self.unit * self.max_x + 100,
-                          self.unit * self.max_y + 100)
-            self.wn.setworldcoordinates(0, 0, self.unit * self.max_x,
-                                        self.unit * self.max_y)
-            self.t.shape('circle')
-            self.t.width(2)
-            self.t.speed(0)
-            self.t.color('gray')
-            for _ in range(2):
-                self.t.forward(self.max_x * self.unit)
-                self.t.left(90)
-                self.t.forward(self.max_y * self.unit)
-                self.t.left(90)
-            for i in range(1, self.max_y):
-                self.draw_x_line(
-                    y=i * self.unit, x0=0, x1=self.max_x * self.unit)
-            for i in range(1, self.max_x):
-                self.draw_y_line(
-                    x=i * self.unit, y0=0, y1=self.max_y * self.unit)
-
-            for i in range(1, self.max_x - 1):
-                self.draw_box(i, 0, 'black')
-            self.draw_box(self.max_x - 1, 0, 'yellow')
-            self.t.shape('turtle')
-
-        x_pos = self.s % self.max_x
-        y_pos = self.max_y - 1 - int(self.s / self.max_x)
+import gym
+class CliffWalkingWapper(gym.Wrapper):
+    def __init__(self, env):
+        gym.Wrapper.__init__(self, env)
+        self.t = None
+        self.unit = 50
+        self.max_x = 12
+        self.max_y = 4
+
+    def draw_x_line(self, y, x0, x1, color='gray'):
+        assert x1 > x0
+        self.t.color(color)
+        self.t.setheading(0)
+        self.t.up()
+        self.t.goto(x0, y)
+        self.t.down()
+        self.t.forward(x1 - x0)
+
+    def draw_y_line(self, x, y0, y1, color='gray'):
+        assert y1 > y0
+        self.t.color(color)
+        self.t.setheading(90)
+        self.t.up()
+        self.t.goto(x, y0)
+        self.t.down()
+        self.t.forward(y1 - y0)
+
+    def draw_box(self, x, y, fillcolor='', line_color='gray'):
+        self.t.up()
+        self.t.goto(x * self.unit, y * self.unit)
+        self.t.color(line_color)
+        self.t.fillcolor(fillcolor)
+        self.t.setheading(90)
+        self.t.down()
+        self.t.begin_fill()
+        for i in range(4):
+            self.t.forward(self.unit)
+            self.t.right(90)
+        self.t.end_fill()
+
+    def move_player(self, x, y):
+        self.t.up()
+        self.t.setheading(90)
+        self.t.fillcolor('red')
+        self.t.goto((x + 0.5) * self.unit, (y + 0.5) * self.unit)
+
+    def render(self):
+        if self.t == None:
+            self.t = turtle.Turtle()
+            self.wn = turtle.Screen()
+            self.wn.setup(self.unit * self.max_x + 100,
+                          self.unit * self.max_y + 100)
+            self.wn.setworldcoordinates(0, 0, self.unit * self.max_x,
+                                        self.unit * self.max_y)
+            self.t.shape('circle')
+            self.t.width(2)
+            self.t.speed(0)
+            self.t.color('gray')
+            for _ in range(2):
+                self.t.forward(self.max_x * self.unit)
+                self.t.left(90)
+                self.t.forward(self.max_y * self.unit)
+                self.t.left(90)
+            for i in range(1, self.max_y):
+                self.draw_x_line(
+                    y=i * self.unit, x0=0, x1=self.max_x * self.unit)
+            for i in range(1, self.max_x):
+                self.draw_y_line(
+                    x=i * self.unit, y0=0, y1=self.max_y * self.unit)
+
+            for i in range(1, self.max_x - 1):
+                self.draw_box(i, 0, 'black')
+            self.draw_box(self.max_x - 1, 0, 'yellow')
+            self.t.shape('turtle')
+
+        x_pos = self.s % self.max_x
+        y_pos = self.max_y - 1 - int(self.s / self.max_x)
         self.move_player(x_pos, y_pos)
```

### Comparing `joyrl-0.1.9/setup.py` & `joyrl-0.2.0/setup.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import sys,os
-from setuptools import setup, find_packages
-curr_path = os.path.dirname(os.path.abspath(__file__))  # current path
-
-def get_version() -> str:
-    # https://packaging.python.org/guides/single-sourcing-package-version/
-    init = open(os.path.join("joyrl", "__init__.py"), "r").read().split()
-    return init[init.index("__version__") + 2][1:-1]
-
-
-def get_install_requires() -> str:
-    return [
-        "gym==0.25.2",
-        "pyyaml==6.0",
-        "matplotlib==3.5.3",
-        "seaborn==0.12.1",
-        "dill==0.3.5.1",
-        "argparse==1.4.0",
-        "pandas==1.3.5",
-        "pyglet==1.5.26",
-        "importlib-metadata<5.0",
-        "setuptools==65.2.0"
-    ]
-
-
-def get_extras_require() -> str:
-    req = {
-        "atari": ["atari_py", "opencv-python"],
-        "mujoco": ["mujoco_py"],
-        "pybullet": ["pybullet"],
-    }
-    return req
-
-setup(
-    name="joyrl",
-    version=get_version(),
-    description="A Library for Deep Reinforcement Learning",
-    long_description=open(f"{curr_path}/README.md", encoding="utf8").read(),
-    long_description_content_type="text/markdown",
-    url="https://github.com/datawhalechina/joyrl",
-    author="johnjim0816",
-    author_email="johnjim0816@gmail.com",
-    license="MIT",
-    python_requires=">=3.7",
-    keywords="reinforcement learning platform pytorch",
-    packages=find_packages(
-        exclude=["test", "test.*", "examples", "examples.*", "docs", "docs.*"]
-    ),
-    platforms = "any",
-    install_requires=get_install_requires(),
-    extras_require=get_extras_require(),
+import sys,os
+from setuptools import setup, find_packages
+curr_path = os.path.dirname(os.path.abspath(__file__))  # current path
+
+def get_version() -> str:
+    # https://packaging.python.org/guides/single-sourcing-package-version/
+    init = open(os.path.join("joyrl", "__init__.py"), "r").read().split()
+    return init[init.index("__version__") + 2][1:-1]
+
+
+def get_install_requires() -> str:
+    return [
+        "gym==0.25.2",
+        "pyyaml==6.0",
+        "matplotlib==3.5.3",
+        "seaborn==0.12.1",
+        "dill==0.3.5.1",
+        "argparse==1.4.0",
+        "pandas==1.3.5",
+        "pyglet==1.5.26",
+        "importlib-metadata<5.0",
+        "setuptools==65.2.0"
+    ]
+
+
+def get_extras_require() -> str:
+    req = {
+        "atari": ["atari_py", "opencv-python"],
+        "mujoco": ["mujoco_py"],
+        "pybullet": ["pybullet"],
+    }
+    return req
+
+setup(
+    name="joyrl",
+    version=get_version(),
+    description="A Library for Deep Reinforcement Learning",
+    long_description=open(f"{curr_path}/README.md", encoding="utf8").read(),
+    long_description_content_type="text/markdown",
+    url="https://github.com/datawhalechina/joyrl",
+    author="johnjim0816",
+    author_email="johnjim0816@gmail.com",
+    license="MIT",
+    python_requires=">=3.7",
+    keywords="reinforcement learning platform pytorch",
+    packages=find_packages(
+        exclude=["test", "test.*", "examples", "examples.*", "docs", "docs.*"]
+    ),
+    platforms = "any",
+    install_requires=get_install_requires(),
+    extras_require=get_extras_require(),
 )
```

