# Comparing `tmp/auraxium-0.2.3.tar.gz` & `tmp/auraxium-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auraxium-0.2.3.tar", last modified: Sun Mar  5 10:25:51 2023, max compression
+gzip compressed data, was "auraxium-0.2.4.tar", last modified: Sun May 28 21:42:46 2023, max compression
```

## Comparing `auraxium-0.2.3.tar` & `auraxium-0.2.4.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 10:25:51.196756 auraxium-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-05 10:25:39.000000 auraxium-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16385 2023-03-05 10:25:51.192756 auraxium-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-03-05 10:25:39.000000 auraxium-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 10:25:51.184756 auraxium-0.2.3/auraxium/
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    22023 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/_rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/_support.py
--rw-r--r--   0 runner    (1001) docker     (123)    15774 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 10:25:51.188756 auraxium-0.2.3/auraxium/census/
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/census/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34751 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/census/_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/census/_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/census/_urlgen.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 10:25:51.188756 auraxium-0.2.3/auraxium/event/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21405 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/event/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/event/_trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 10:25:51.192756 auraxium-0.2.3/auraxium/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/models/_ability.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/models/_achievement.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/models/_armour.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/models/_character.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/models/_currency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/models/_depot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/models/_directive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/models/_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)    19710 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/models/_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/models/_experience.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/models/_faction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/models/_fire.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/models/_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/models/_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/models/_metagame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/models/_objective.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/models/_outfit.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/models/_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/models/_projectile.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/models/_resist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/models/_reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/models/_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/models/_states.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/models/_vehicle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/models/_weapon.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/models/_world.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/models/_zone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 10:25:51.192756 auraxium-0.2.3/auraxium/ps2/
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/ps2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/ps2/_ability.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/ps2/_achievement.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/ps2/_armour.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/ps2/_character.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/ps2/_currency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/ps2/_depot.py
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/ps2/_directive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10551 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/ps2/_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/ps2/_experience.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/ps2/_faction.py
--rw-r--r--   0 runner    (1001) docker     (123)    30132 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/ps2/_fire.py
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/ps2/_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     9577 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/ps2/_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/ps2/_metagame.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/ps2/_objective.py
--rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/ps2/_outfit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/ps2/_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/ps2/_projectile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/ps2/_resist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/ps2/_reward.py
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/ps2/_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/ps2/_states.py
--rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/ps2/_vehicle.py
--rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/ps2/_weapon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/ps2/_world.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/ps2/_zone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/ps2/leaderboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-03-05 10:25:39.000000 auraxium-0.2.3/auraxium/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 10:25:51.188756 auraxium-0.2.3/auraxium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16385 2023-03-05 10:25:51.000000 auraxium-0.2.3/auraxium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-03-05 10:25:51.000000 auraxium-0.2.3/auraxium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 10:25:51.000000 auraxium-0.2.3/auraxium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 10:25:51.000000 auraxium-0.2.3/auraxium.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-05 10:25:51.000000 auraxium-0.2.3/auraxium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-05 10:25:51.000000 auraxium-0.2.3/auraxium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-05 10:25:51.196756 auraxium-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-03-05 10:25:39.000000 auraxium-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:42:46.781984 auraxium-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-28 21:42:25.000000 auraxium-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-05-28 21:42:46.781984 auraxium-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15709 2023-05-28 21:42:25.000000 auraxium-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:42:46.773984 auraxium-0.2.4/auraxium/
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22023 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:42:46.773984 auraxium-0.2.4/auraxium/census/
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/census/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34687 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/census/_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/census/_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/census/_urlgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:42:46.773984 auraxium-0.2.4/auraxium/event/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21405 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/event/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/event/_trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:42:46.777984 auraxium-0.2.4/auraxium/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_ability.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_achievement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_armour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_character.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_currency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_depot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18276 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_experience.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_faction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_fire.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_metagame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_outfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_projectile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_resist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_weapon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:42:46.781984 auraxium-0.2.4/auraxium/ps2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_ability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_achievement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_armour.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_character.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_currency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_depot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10551 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_experience.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_faction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30132 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_fire.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_metagame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_outfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_projectile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_resist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_weapon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/leaderboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:42:46.773984 auraxium-0.2.4/auraxium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-05-28 21:42:46.000000 auraxium-0.2.4/auraxium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-28 21:42:46.000000 auraxium-0.2.4/auraxium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 21:42:46.000000 auraxium-0.2.4/auraxium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 21:42:46.000000 auraxium-0.2.4/auraxium.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-28 21:42:46.000000 auraxium-0.2.4/auraxium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-28 21:42:46.000000 auraxium-0.2.4/auraxium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 21:42:46.781984 auraxium-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-28 21:42:25.000000 auraxium-0.2.4/setup.py
```

### Comparing `auraxium-0.2.3/LICENSE` & `auraxium-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/PKG-INFO` & `auraxium-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: auraxium
-Version: 0.2.3
+Version: 0.2.4
 Summary: A python wrapper for the PlanetSide 2 Census API.
 Home-page: https://github.com/leonhard-s/auraxium
 Author: Leonhard S.
 Author-email: leonhard-sei@outlook.com
 License: MIT
 Keywords: auraxium python daybreak census planetside ps2
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # <img src="https://raw.githubusercontent.com/leonhard-s/auraxium/master/assets/icon_256.png" align="left" height="140"/>Auraxium
 
@@ -162,16 +163,14 @@
 - Any number of **conditions** that decide whether to run or not
 - An **action** that will be run if the conditions are met
 
 #### Events
 
 The event type definitions are available in the [`auraxium.event`](https://auraxium.readthedocs.io/en/latest/api/event.html#event-types) namespace.
 
-> **Note:** The `ContinentUnlock` event is currently broken on Daybreak's side.
-
 #### Conditions
 
 Trigger conditions can be attached to a trigger to limit what events it will respond to, in addition to the event type.
 
 This is useful if you have a commonly encountered event (like [`event.DEATH`](https://auraxium.readthedocs.io/en/latest/api/event.html#auraxium.event.DEATH)) and would like your action to only run if the event data matches some other requirement (for example "the killing player must be part of my outfit").
 
 #### Actions
```

### Comparing `auraxium-0.2.3/README.md` & `auraxium-0.2.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -145,16 +145,14 @@
 - Any number of **conditions** that decide whether to run or not
 - An **action** that will be run if the conditions are met
 
 #### Events
 
 The event type definitions are available in the [`auraxium.event`](https://auraxium.readthedocs.io/en/latest/api/event.html#event-types) namespace.
 
-> **Note:** The `ContinentUnlock` event is currently broken on Daybreak's side.
-
 #### Conditions
 
 Trigger conditions can be attached to a trigger to limit what events it will respond to, in addition to the event type.
 
 This is useful if you have a commonly encountered event (like [`event.DEATH`](https://auraxium.readthedocs.io/en/latest/api/event.html#auraxium.event.DEATH)) and would like your action to only run if the event data matches some other requirement (for example "the killing player must be part of my outfit").
 
 #### Actions
```

### Comparing `auraxium-0.2.3/auraxium/__init__.py` & `auraxium-0.2.4/auraxium/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,8 +30,8 @@
     'ps2',
     'Ps2Object',
     'SequenceProxy',
     'Trigger'
 ]
 
 __author__ = 'Leonhard S.'
-__version__ = '0.2.3'
+__version__ = '0.2.4'
```

### Comparing `auraxium-0.2.3/auraxium/_cache.py` & `auraxium-0.2.4/auraxium/_cache.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/_client.py` & `auraxium-0.2.4/auraxium/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,15 @@
            not found.
         """
         key = f'{locale}_{name.lower()}'
         _log.debug('%s "%s"[%s] requested', type_.__name__, name, locale)
         # pylint: disable=protected-access
         if (instance := type_._cache.get(key)) is not None:  # type: ignore
             _log.debug('%r restored from cache', instance)
-            return instance  # type: ignore
+            return instance
         _log.debug('%s "%s"[%s] not cached, generating API query...',
                    type_.__name__, name, locale)
         query = Query(type_.collection, service_id=self.service_id)
         if issubclass(type_, Character):
             query.add_term(field='name.first_lower', value=name.lower())
         else:
             query.case(False).add_term(field=f'name.{locale}', value=name)
```

### Comparing `auraxium-0.2.3/auraxium/_log.py` & `auraxium-0.2.4/auraxium/_log.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/_proxy.py` & `auraxium-0.2.4/auraxium/_proxy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Define the proxy object system."""
 
 import asyncio
 import copy
 import datetime
 import warnings
-from typing import (Any, Dict, Generator, Generic, Iterator, List, Optional,
+from typing import (Any, Awaitable, Dict, Generator, Generic, List, Optional,
                     Type, TypeVar)
 
 from .base import Ps2Object
 from .census import JoinedQuery, Query
 from ._rest import RequestClient, extract_payload
 from .types import CensusData
 
@@ -65,20 +65,15 @@
 
         This method uses a lock to ensure it does not try to query the
         same object multiple times.
         """
         async with self._lock:
             payload = await self._client.request(self.query)
             list_ = self._resolve_nested_payload(payload)
-            # NOTE: There does not appear to be an easy way to type something
-            # as "subclass of an abstract class and all abstract methods have
-            # been overwritten", which is why this is typed as being a
-            # Ps2Object subclass and then promptly ignored here.
-            self._data = [self._type(  # type: ignore
-                data, client=self._client) for data in list_]
+            self._data = [self._type(d, client=self._client) for d in list_]
             self._last_fetched = datetime.datetime.utcnow()
 
     def _resolve_nested_payload(self, payload: CensusData) -> List[CensusData]:
         """Resolve the object payload.
 
         This introspects the given query to determine the sub-key for
         the actual object to return.
@@ -128,15 +123,15 @@
             # their outputs before returning
             data.clear()
             for join in self.query.joins:
                 data.extend(resolve_join(join, parent))
         return data
 
 
-class SequenceProxy(Proxy[_Ps2ObjectT]):
+class SequenceProxy(Proxy[_Ps2ObjectT], Awaitable[List[_Ps2ObjectT]]):
     """Proxy for lists of results.
 
     This object supports asynchronous iteration (in which case all
     elements are returned in a single request prior to iteration).
 
     Alternatively, you can await it to receive a list of elements.
 
@@ -155,15 +150,15 @@
             await self._poll()
         self._index += 1
         try:
             return self._data[self._index]
         except IndexError as err:
             raise StopAsyncIteration from err
 
-    def __await__(self) -> Iterator[List[_Ps2ObjectT]]:
+    def __await__(self) -> Generator[Any, None, List[_Ps2ObjectT]]:
         return self.flatten().__await__()
 
     async def flatten(self) -> List[_Ps2ObjectT]:
         """Retrieve all elements in the response as a list.
 
         :return: A list of instantiated objects.
         """
```

### Comparing `auraxium-0.2.3/auraxium/_rest.py` & `auraxium-0.2.4/auraxium/_rest.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/_support.py` & `auraxium-0.2.4/auraxium/_support.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/base.py` & `auraxium-0.2.4/auraxium/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 These classes define shared functionality required by all object
 representations of API data, and defines the basic class hierarchy used
 throughout the PlanetSide 2 object model.
 """
 
 import abc
 import logging
-from typing import Any, ClassVar, List, Optional, Type, TypeVar, Union
+from typing import Any, ClassVar, List, Optional, Type, TypeVar, Union, cast
 
 import pydantic
 
 from .models.base import RESTPayload
 from ._cache import TLRUCache
 from .census import Query
 from .endpoints import DBG_FILES
@@ -288,15 +288,15 @@
         cls._cache.clear()
         cls._cache.size = size
         if ttu is not None:
             cls._cache.ttu = ttu
 
     @classmethod
     @deprecated('0.2', '0.3', replacement=':meth:`auraxium.Client.get`')  # pragma: no cover
-    async def get_by_id(cls: Type[CachedT], id_: int, *,  # type: ignore
+    async def get_by_id(cls: Type[CachedT], id_: int, *,
                         client: RequestClient) -> Optional[CachedT]:
         """Retrieve an object by by ID.
 
         This query uses caches and might return an existing instance if
         the object has been recently retrieved.
 
         :param int id\\_: The unique id of the object.
@@ -304,18 +304,18 @@
            perform the request.
         :return: The object matching the given ID or :obj:`None` if no
            match was found.
         """
         _log.debug('<%s:%d> requested', cls.__name__, id_)
         if (instance := cls._cache.get(id_)) is not None:
             _log.debug('%r restored from cache', instance)
-            return instance  # type: ignore
+            return instance
         _log.debug('<%s:%d> not cached, generating API query...',
                    cls.__name__, id_)
-        return await super().get_by_id(id_, client=client)  # type: ignore
+        return await super().get_by_id(id_, client=client)
 
 
 class Named(Cached, cache_size=0, cache_ttu=0.0, metaclass=abc.ABCMeta):
     """Mix-in class for named objects.
 
     This extends the functionality provided by
     :class:`~auraxium.base.Cached` to also cache objects retrieved via
@@ -385,14 +385,14 @@
 
 
 class ImageMixin(Ps2Object, metaclass=abc.ABCMeta):
     """A mixin class for types supporting image access."""
 
     def image(self) -> str:
         """Return the default image for this type."""
-        image_id: int = self.data.image_id  # type: ignore
+        image_id = cast(int, getattr(self.data, 'image_id', 0))
         return self._image_url(image_id)
 
     @staticmethod
     def _image_url(image_id: int) -> str:
         """Return the URL for a given image ID."""
         return str(DBG_FILES / f'{image_id}.png')
```

### Comparing `auraxium-0.2.3/auraxium/census/__init__.py` & `auraxium-0.2.4/auraxium/census/__init__.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/census/_query.py` & `auraxium-0.2.4/auraxium/census/_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,15 +272,15 @@
         :param str service_id: The service ID identifying this app.
         :param endpoint: The endpoint to use for the API. Allows for
            targeting community endpoints.
         :type endpoint: yarl.URL or None
         """
         super().__init__(collection, **kwargs)
         self.endpoint = endpoint or default_endpoints()[0]
-        data: QueryBaseData = self.data  # type: ignore
+        data: QueryBaseData = self.data
         self.data: QueryData = QueryData.from_base(data)
         self.data.namespace = namespace
         self.data.service_id = service_id
 
     def __str__(self) -> str:
         """Generate and return the URL defined by this query.
 
@@ -301,15 +301,15 @@
         :param bool value: Whether to ignore case for this query.
         :return: The current query instance.
         """
         self.data.case = value
         return self
 
     @classmethod
-    def copy(cls, template: QueryBase,  # type: ignore
+    def copy(cls, template: QueryBase,
              copy_joins: bool = False, deep_copy: bool = False,
              **kwargs: Any) -> 'Query':
         """Create a new query, copying most data from the template.
 
         The new query will share the collection, terms and show/hide
         markers of the template. If `copy_joins` is enabled, it will
         also copy its list of joins.
@@ -669,19 +669,19 @@
         :param str: The API collection to join.
         :param kwargs: Key-value pairs to add to the query. Any search
            modifier literals will first be parsed by
            :meth:`SearchTerm.infer`.
         :type kwargs: float | int | str
         """
         super().__init__(collection, **kwargs)
-        data: QueryBaseData = self.data  # type: ignore
+        data: QueryBaseData = self.data
         self.data: JoinedQueryData = JoinedQueryData.from_base(data)
 
     @classmethod
-    def copy(cls, template: QueryBase,  # type: ignore
+    def copy(cls, template: QueryBase,
              copy_joins: bool = False,   deep_copy: bool = False,
              **kwargs: Any) -> 'JoinedQuery':
         """Create a new query, copying most data from the template.
 
         The new query will share the collection, terms and show/hide
         markers of the template. If `copy_joins` is enabled, it will
         also copy its list of joins.
```

### Comparing `auraxium-0.2.3/auraxium/census/_support.py` & `auraxium-0.2.4/auraxium/census/_support.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/census/_urlgen.py` & `auraxium-0.2.4/auraxium/census/_urlgen.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/endpoints.py` & `auraxium-0.2.4/auraxium/endpoints.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/errors.py` & `auraxium-0.2.4/auraxium/errors.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/event/__init__.py` & `auraxium-0.2.4/auraxium/event/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,27 +7,25 @@
 
 from ._client import EventClient
 from ._trigger import Trigger
 from ..models import (AchievementAdded, BattleRankUp, Death, Event,
                       FacilityControl, GainExperience, ItemAdded,
                       MetagameEvent, PlayerFacilityCapture,
                       PlayerFacilityDefend, PlayerLogin, PlayerLogout,
-                      SkillAdded, VehicleDestroy, ContinentLock,
-                      ContinentUnlock)
+                      SkillAdded, VehicleDestroy, ContinentLock)
 
 __all__ = [
     'Event',
     'EventClient',
     'Trigger',
 
     # Event subclasses
     'AchievementAdded',
     'BattleRankUp',
     'ContinentLock',
-    'ContinentUnlock',
     'Death',
     'FacilityControl',
     'GainExperience',
     'ItemAdded',
     'MetagameEvent',
     'PlayerFacilityCapture',
     'PlayerFacilityDefend',
```

### Comparing `auraxium-0.2.3/auraxium/event/_client.py` & `auraxium-0.2.4/auraxium/event/_client.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/event/_trigger.py` & `auraxium-0.2.4/auraxium/event/_trigger.py`

 * *Files 3% similar despite different names*

```diff
@@ -208,18 +208,21 @@
             json_data['worlds'] = ['all']
         if logical_and is not None:
             json_data['logicalAndCharactersWithWorlds'] = (
                 'true' if logical_and else 'false')
         # When subscribing to character-centric events using only a world ID,
         # set the "logicalAnd*" flag to avoid subscribing to all characters on
         # all continents (characters would default to "all" if not specified).
-        elif (self.worlds and not self.characters
-                and any((issubclass(e, CharacterEvent))  # type: ignore
-                        for e in self.events)):
-            json_data['logicalAndCharactersWithWorlds'] = 'true'
+        elif (self.worlds and not self.characters):
+            char_events = [s.__name__ for s in CharacterEvent.__subclasses__()]
+            event_names = [e if isinstance(e, str) else e.__name__
+                           for e in self.events]
+            if any((e.startswith('GainExperience_experience_id_')
+                   or e in char_events) for e in event_names):
+                json_data['logicalAndCharactersWithWorlds'] = 'true'
         return json.dumps(json_data)
 
     async def run(self, event: Event) -> None:
         """Perform the action associated with this trigger.
 
         :param Event event: The event to pass to the trigger action.
         """
```

### Comparing `auraxium-0.2.3/auraxium/models/__init__.py` & `auraxium-0.2.4/auraxium/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 from ._directive import (DirectiveData, DirectiveTierData,
                          DirectiveTreeCategoryData, DirectiveTreeData)
 from ._effect import (EffectData, EffectTypeData, ZoneEffectData,
                       ZoneEffectTypeData)
 from ._events import (AchievementAdded, BattleRankUp, Death, FacilityControl,
                       GainExperience, ItemAdded, MetagameEvent,
                       PlayerFacilityCapture, PlayerFacilityDefend, PlayerLogin,
-                      PlayerLogout, SkillAdded, VehicleDestroy, ContinentLock,
-                      ContinentUnlock)
+                      PlayerLogout, SkillAdded, VehicleDestroy, ContinentLock)
 from ._experience import ExperienceData, ExperienceRankData
 from ._faction import FactionData
 from ._fire import FireGroupData, FireModeData
 from ._item import ItemCategoryData, ItemData, ItemTypeData
 from ._map import FacilityTypeData, MapHexData, MapRegionData, RegionData
 from ._metagame import MetagameEventData
 from ._objective import ObjectiveData, ObjectiveTypeData
@@ -49,15 +48,14 @@
     'CharacterData',
     'CharacterDirective',
     'CharacterDirectiveObjective',
     'CharacterDirectiveTier',
     'CharacterDirectiveTree',
     'CharacterEvent',
     'ContinentLock',
-    'ContinentUnlock',
     'CurrencyData',
     'Death',
     'DirectiveData',
     'DirectiveTierData',
     'DirectiveTreeCategoryData',
     'DirectiveTreeData',
     'EffectData',
```

### Comparing `auraxium-0.2.3/auraxium/models/_ability.py` & `auraxium-0.2.4/auraxium/models/_ability.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/models/_achievement.py` & `auraxium-0.2.4/auraxium/models/_achievement.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/models/_armour.py` & `auraxium-0.2.4/auraxium/models/_armour.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/models/_character.py` & `auraxium-0.2.4/auraxium/models/_character.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
 
         .. attribute:: date
             type: str
 
             Human-readable version of :attr:`time`.
         """
 
-        count: int  # type: ignore
+        count: int
         time: Optional[int] = None
         date: Optional[str] = None
 
     class Name(RESTPayload):
         """Object representation of the "name" sub-key.
 
         .. note::
```

### Comparing `auraxium-0.2.3/auraxium/models/_depot.py` & `auraxium-0.2.4/auraxium/models/_depot.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/models/_directive.py` & `auraxium-0.2.4/auraxium/models/_directive.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/models/_effect.py` & `auraxium-0.2.4/auraxium/models/_effect.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/models/_events.py` & `auraxium-0.2.4/auraxium/models/_events.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from .base import Event, CharacterEvent, WorldEvent
 
 __all__ = [
     'AchievementAdded',
     'BattleRankUp',
     'ContinentLock',
-    'ContinentUnlock',
     'Death',
     'FacilityControl',
     'GainExperience',
     'ItemAdded',
     'MetagameEvent',
     'PlayerFacilityCapture',
     'PlayerFacilityDefend',
@@ -753,79 +752,14 @@
 
     .. attribute:: timestamp
        :type: int
 
        The UTC timestamp of the event. May be used to infer latency to
        the event streaming endpoint.
 
-    .. attribute:: world_id
-       :type: int
-
-       ID of the :class:`~auraxium.ps2.World` whose event streaming
-       endpoint broadcast the event.
-    """
-
-    zone_id: int
-    triggering_faction: int
-    previous_faction: int
-    vs_population: float
-    nc_population: float
-    tr_population: float
-    metagame_event_id: int
-
-
-class ContinentUnlock(Event, WorldEvent):
-    """A continent has been unlocked.
-
-    .. note::
-
-       As of March 2021, this event is broken and never actually gets
-       broadcast via the event streaming service.
-
-    .. attribute:: zone_id
-       :type: int
-
-       ID of the :class:`~auraxium.ps2.Zone` that unlocked.
-
-    .. attribute:: triggering_faction
-       :type: int
-
-       (Unknown due to event being broken)
-
-    .. attribute:: previous_faction
-       :type: int
-
-       (Unknown due to event being broken)
-
-    .. attribute:: vs_population
-       :type: float
-
-       (Unknown due to event being broken)
-
-    .. attribute:: nc_population
-       :type: float
-
-       (Unknown due to event being broken)
-
-    .. attribute:: tr_population
-       :type: float
-
-       (Unknown due to event being broken)
-
-    .. attribute:: metagame_event_id
-       :type: int
-
-       (Unknown due to event being broken)
-
-    .. attribute:: timestamp
-       :type: int
-
-       The UTC timestamp of the event. May be used to infer latency to
-       the event streaming endpoint.
-
     .. attribute:: world_id
        :type: int
 
        ID of the :class:`~auraxium.ps2.World` whose event streaming
        endpoint broadcast the event.
     """
```

### Comparing `auraxium-0.2.3/auraxium/models/_experience.py` & `auraxium-0.2.4/auraxium/models/_experience.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/models/_faction.py` & `auraxium-0.2.4/auraxium/models/_faction.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/models/_fire.py` & `auraxium-0.2.4/auraxium/models/_fire.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/models/_item.py` & `auraxium-0.2.4/auraxium/models/_item.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/models/_map.py` & `auraxium-0.2.4/auraxium/models/_map.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/models/_metagame.py` & `auraxium-0.2.4/auraxium/models/_metagame.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/models/_objective.py` & `auraxium-0.2.4/auraxium/models/_objective.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/models/_outfit.py` & `auraxium-0.2.4/auraxium/models/_outfit.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/models/_profile.py` & `auraxium-0.2.4/auraxium/models/_profile.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/models/_projectile.py` & `auraxium-0.2.4/auraxium/models/_projectile.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/models/_resist.py` & `auraxium-0.2.4/auraxium/models/_resist.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/models/_reward.py` & `auraxium-0.2.4/auraxium/models/_reward.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/models/_skill.py` & `auraxium-0.2.4/auraxium/models/_skill.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/models/_states.py` & `auraxium-0.2.4/auraxium/models/_states.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/models/_vehicle.py` & `auraxium-0.2.4/auraxium/models/_vehicle.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/models/_weapon.py` & `auraxium-0.2.4/auraxium/models/_weapon.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/models/_world.py` & `auraxium-0.2.4/auraxium/models/_world.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/models/base.py` & `auraxium-0.2.4/auraxium/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 class RESTPayload(Payload):
     """A JSON payload received through the REST interface.
 
     This :class:`Payload` subclass implicitly converts NULL strings to
     :obj:`None`.
     """
 
-    @pydantic.validator('*', pre=True)
+    @pydantic.validator('*', pre=True)  # type: ignore
     @classmethod
     def _convert_null(cls, value: _T) -> Optional[_T]:
         """Replace any "NULL" string inputs with :obj:`None`.
 
         This is a pre-validator; it is run before any other validation
         or conversion takes place.
 
@@ -146,15 +146,15 @@
        endpoint broadcast the event.
     """
 
     event_name: str
     timestamp: datetime.datetime
     world_id: int
 
-    @pydantic.validator('timestamp', pre=True)
+    @pydantic.validator('timestamp', pre=True)  # type: ignore
     @classmethod
     def _utc_from_timestamp(cls, value: str) -> datetime.datetime:
         """Convert timestamps to UTC datetimes."""
         return datetime.datetime.utcfromtimestamp(int(value))
 
     @property
     def age(self) -> float:
```

### Comparing `auraxium-0.2.3/auraxium/ps2/__init__.py` & `auraxium-0.2.4/auraxium/ps2/__init__.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/ps2/_ability.py` & `auraxium-0.2.4/auraxium/ps2/_ability.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/ps2/_achievement.py` & `auraxium-0.2.4/auraxium/ps2/_achievement.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/ps2/_armour.py` & `auraxium-0.2.4/auraxium/ps2/_armour.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/ps2/_character.py` & `auraxium-0.2.4/auraxium/ps2/_character.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/ps2/_currency.py` & `auraxium-0.2.4/auraxium/ps2/_currency.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/ps2/_depot.py` & `auraxium-0.2.4/auraxium/ps2/_depot.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/ps2/_directive.py` & `auraxium-0.2.4/auraxium/ps2/_directive.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/ps2/_effect.py` & `auraxium-0.2.4/auraxium/ps2/_effect.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/ps2/_experience.py` & `auraxium-0.2.4/auraxium/ps2/_experience.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/ps2/_faction.py` & `auraxium-0.2.4/auraxium/ps2/_faction.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/ps2/_fire.py` & `auraxium-0.2.4/auraxium/ps2/_fire.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/ps2/_item.py` & `auraxium-0.2.4/auraxium/ps2/_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Item and item attachment class definitions."""
 
 from typing import Any, Final, Optional, TYPE_CHECKING, cast
 
 from ..base import Cached, ImageMixin, Named
 from ..census import Query
+from ..errors import NotFoundError
 from ..models import ItemCategoryData, ItemData, ItemTypeData
 from .._rest import extract_single
 from .._proxy import InstanceProxy, SequenceProxy
 from ..types import LocaleData
 
 from ._faction import Faction
 from ._profile import Profile
@@ -240,23 +241,26 @@
         This returns an :class:`auraxium.InstanceProxy`.
         """
         value = self.data.faction_id or -1
         query = Query(Faction.collection, service_id=self._client.service_id)
         query.add_term(field=Faction.id_field, value=value)
         return InstanceProxy(Faction, query, client=self._client)
 
-    async def datasheet(self) -> 'WeaponDatasheet':
+    async def datasheet(self) -> Optional['WeaponDatasheet']:
         """Return the datasheet for the weapon."""
         # pylint: disable=import-outside-toplevel
         from ._weapon import WeaponDatasheet
         collection: Final[str] = 'weapon_datasheet'
         query = Query(collection, service_id=self._client.service_id)
         query.add_term(field=self.id_field, value=self.id)
         payload = await self._client.request(query)
-        data = extract_single(payload, collection)
+        try:
+            data = extract_single(payload, collection)
+        except NotFoundError:
+            return None
         return WeaponDatasheet(**cast(Any, data))
 
     def profiles(self) -> SequenceProxy[Profile]:
         """Return the profiles the item is available to.
 
         This returns a :class:`auraxium.SequenceProxy`.
         """
```

### Comparing `auraxium-0.2.3/auraxium/ps2/_map.py` & `auraxium-0.2.4/auraxium/ps2/_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,15 +235,15 @@
     async def get_connected(self) -> Set['MapRegion']:
         """Return the facilities connected to this region."""
         if self.data.facility_id is None:
             return set()
         # NOTE: This operation cannot be done in a single query as there is no
         # "or" operator.
         collection: Final[str] = 'facility_link'
-        connected: Set['MapRegion'] = set()  # type: ignore
+        connected: Set['MapRegion'] = set()
         # Set up the base query
         query = Query(collection, service_id=self._client.service_id)
         query.limit(10)
         join = query.create_join(self.collection)
         join.set_fields('facility_id_a', 'facility_id')
         join = query.create_join(self.collection)
         join.set_fields('facility_id_b', 'facility_id')
```

### Comparing `auraxium-0.2.3/auraxium/ps2/_metagame.py` & `auraxium-0.2.4/auraxium/ps2/_metagame.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/ps2/_objective.py` & `auraxium-0.2.4/auraxium/ps2/_objective.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/ps2/_outfit.py` & `auraxium-0.2.4/auraxium/ps2/_outfit.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/ps2/_profile.py` & `auraxium-0.2.4/auraxium/ps2/_profile.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/ps2/_projectile.py` & `auraxium-0.2.4/auraxium/ps2/_projectile.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/ps2/_resist.py` & `auraxium-0.2.4/auraxium/ps2/_resist.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/ps2/_reward.py` & `auraxium-0.2.4/auraxium/ps2/_reward.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/ps2/_skill.py` & `auraxium-0.2.4/auraxium/ps2/_skill.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/ps2/_states.py` & `auraxium-0.2.4/auraxium/ps2/_states.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/ps2/_vehicle.py` & `auraxium-0.2.4/auraxium/ps2/_vehicle.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/ps2/_weapon.py` & `auraxium-0.2.4/auraxium/ps2/_weapon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Weapon class definition."""
 
 import logging
 from typing import Any, Final, List, Optional, cast
 
 from ..base import Cached
 from ..census import Query
+from ..errors import NotFoundError
 from ..models import WeaponAmmoSlot, WeaponData, WeaponDatasheet
 from .._proxy import InstanceProxy, SequenceProxy
 from .._rest import RequestClient, extract_payload, extract_single
 from .._support import deprecated
 
 from ._fire import FireGroup
 from ._item import Item
@@ -161,23 +162,26 @@
         query.add_term(field='weapon_group_id', value=group_id)
         query.limit(100)
         join = query.create_join(Item.collection)
         join.set_fields(Item.id_field)
         join.set_outer(False)
         return SequenceProxy(Item, query, client=self._client)
 
-    async def datasheet(self) -> WeaponDatasheet:
+    async def datasheet(self) -> Optional[WeaponDatasheet]:
         """Return the datasheet for the weapon."""
         collection: Final[str] = 'weapon_datasheet'
         if (item := await self.item()) is None:  # pragma: no cover
             raise RuntimeError(f'Invalid item for weapon ID: {self.id}')
         query = Query(collection, service_id=self._client.service_id)
         query.add_term(field=Item.id_field, value=item.id)
         payload = await self._client.request(query)
-        data = extract_single(payload, collection)
+        try:
+            data = extract_single(payload, collection)
+        except NotFoundError:
+            return None
         return WeaponDatasheet(**cast(Any, data))
 
     def fire_groups(self) -> SequenceProxy[FireGroup]:
         """Return the fire groups for this weapon.
 
         This returns a :class:`auraxium.SequenceProxy`.
         """
```

### Comparing `auraxium-0.2.3/auraxium/ps2/_world.py` & `auraxium-0.2.4/auraxium/ps2/_world.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/ps2/_zone.py` & `auraxium-0.2.4/auraxium/ps2/_zone.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/ps2/leaderboard.py` & `auraxium-0.2.4/auraxium/ps2/leaderboard.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium/types.py` & `auraxium-0.2.4/auraxium/types.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/auraxium.egg-info/PKG-INFO` & `auraxium-0.2.4/auraxium.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: auraxium
-Version: 0.2.3
+Version: 0.2.4
 Summary: A python wrapper for the PlanetSide 2 Census API.
 Home-page: https://github.com/leonhard-s/auraxium
 Author: Leonhard S.
 Author-email: leonhard-sei@outlook.com
 License: MIT
 Keywords: auraxium python daybreak census planetside ps2
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # <img src="https://raw.githubusercontent.com/leonhard-s/auraxium/master/assets/icon_256.png" align="left" height="140"/>Auraxium
 
@@ -162,16 +163,14 @@
 - Any number of **conditions** that decide whether to run or not
 - An **action** that will be run if the conditions are met
 
 #### Events
 
 The event type definitions are available in the [`auraxium.event`](https://auraxium.readthedocs.io/en/latest/api/event.html#event-types) namespace.
 
-> **Note:** The `ContinentUnlock` event is currently broken on Daybreak's side.
-
 #### Conditions
 
 Trigger conditions can be attached to a trigger to limit what events it will respond to, in addition to the event type.
 
 This is useful if you have a commonly encountered event (like [`event.DEATH`](https://auraxium.readthedocs.io/en/latest/api/event.html#auraxium.event.DEATH)) and would like your action to only run if the event data matches some other requirement (for example "the killing player must be part of my outfit").
 
 #### Actions
```

### Comparing `auraxium-0.2.3/auraxium.egg-info/SOURCES.txt` & `auraxium-0.2.4/auraxium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.3/setup.py` & `auraxium-0.2.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,16 +17,17 @@
                  description='A python wrapper for the PlanetSide 2 Census API.',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  keywords='auraxium python daybreak census planetside ps2',
                  url='https://github.com/leonhard-s/auraxium',
                  packages=setuptools.find_packages(),
                  package_data={'auraxium': ['py.typed']},
-                 classifiers=['Development Status :: 4 - Beta',
+                 classifiers=['Development Status :: 5 - Production/Stable',
                               'Programming Language :: Python :: 3.9',
                               'Programming Language :: Python :: 3.10',
+                              'Programming Language :: Python :: 3.11',
                               'License :: OSI Approved :: MIT License',
                               'Operating System :: OS Independent'],
                  install_requires=install_requires,
                  license='MIT',
                  include_package_data=True,
                  zip_safe=False)
```

