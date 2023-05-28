# Comparing `tmp/battle-cats-save-editor-2.7.2.tar.gz` & `tmp/battle-cats-save-editor-2.7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "battle-cats-save-editor-2.7.2.tar", last modified: Sun May 28 10:11:11 2023, max compression
+gzip compressed data, was "battle-cats-save-editor-2.7.2.1.tar", last modified: Sun May 28 10:25:50 2023, max compression
```

## Comparing `battle-cats-save-editor-2.7.2.tar` & `battle-cats-save-editor-2.7.2.1.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.554332 battle-cats-save-editor-2.7.2/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1071 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/LICENSE
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       95 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/MANIFEST.in
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    10938 2023-05-28 10:11:11.554332 battle-cats-save-editor-2.7.2/PKG-INFO
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    10502 2023-05-21 14:21:38.000000 battle-cats-save-editor-2.7.2/README.md
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      206 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/pyproject.toml
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       38 2023-05-28 10:11:11.554332 battle-cats-save-editor-2.7.2/setup.cfg
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1177 2023-03-11 10:01:29.000000 battle-cats-save-editor-2.7.2/setup.py
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.531000 battle-cats-save-editor-2.7.2/src/
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.534333 battle-cats-save-editor-2.7.2/src/BCSFE_Python/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      283 2023-04-14 10:31:17.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/__init__.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     9841 2023-04-14 13:40:17.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/__main__.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    10151 2023-03-13 20:26:00.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/adb_handler.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    13745 2023-03-11 10:30:59.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/config_manager.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1501 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/csv_handler.py
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.534333 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       67 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/__init__.py
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.537666 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/basic/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      122 2023-03-14 20:12:33.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/basic/__init__.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     8876 2023-04-14 10:37:56.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/basic/basic_items.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1490 2023-03-11 15:02:56.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/basic/catfruit.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1931 2023-03-11 15:03:21.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/basic/catseyes.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1647 2023-03-14 20:18:26.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/basic/ototo_base_mats.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3984 2023-03-15 16:45:12.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/basic/talent_orbs.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    16533 2023-03-15 16:44:54.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/basic/talent_orbs_new.py
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.541000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      179 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/__init__.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     8978 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/cat_helper.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    11121 2023-02-27 19:14:37.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/cat_id_selector.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3249 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/chara_drop.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1068 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/clear_cat_guide.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2844 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/evolve_cats.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1260 2023-02-25 10:47:53.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/get_remove_cats.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     7933 2023-05-23 19:07:27.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/talents.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1900 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/upgrade_blue.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4428 2023-03-15 16:45:17.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/upgrade_cats.py
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.541000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/gamototo/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       66 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/gamototo/__init__.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      309 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/gamototo/fix_gamatoto.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2794 2023-03-11 15:04:37.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/gamototo/gamatoto_xp.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3393 2023-03-11 15:04:50.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/gamototo/helpers.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     7377 2023-05-28 10:08:58.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/gamototo/ototo_cat_cannon.py
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.544333 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      313 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/__init__.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1035 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/aku.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      491 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/allow_filibuster_clearing.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      790 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/behemoth_culling.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      646 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/clear_tutorial.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1121 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/enigma_stages.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     6307 2023-03-15 16:45:22.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/event_stages.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1873 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/gauntlet.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1027 2023-03-11 15:09:01.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/itf_timed_scores.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1469 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/legend_quest.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4408 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/main_story.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2323 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/outbreaks.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3031 2023-03-15 16:41:58.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/story_level_id_selector.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1175 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/towers.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     8458 2023-03-11 15:10:07.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/treasures.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1043 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/uncanny.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      784 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/unlock_aku_realm.py
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.547666 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      276 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/__init__.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3878 2023-03-11 15:30:39.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/cat_shrine.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1093 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/claim_user_rank_rewards.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1054 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/create_new_account.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2073 2023-04-14 10:35:42.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/fix_elsewhere.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      659 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/fix_time_issues.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3498 2023-04-06 13:00:50.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/get_gold_pass.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     7067 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/meow_medals.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4354 2023-02-17 15:14:36.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/missions.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      975 2023-03-15 16:45:35.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/play_time.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4568 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/scheme_item.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1612 2023-03-11 15:30:52.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/trade_progress.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1284 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/unlock_enemy_guide.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      326 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/unlock_equip_menu.py
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.547666 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/save_management/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       56 2023-03-15 19:40:58.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/save_management/__init__.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1273 2023-03-22 09:51:45.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/save_management/convert.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2578 2023-03-15 19:41:06.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/save_management/load.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      644 2023-03-15 19:41:09.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/save_management/other.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2073 2023-04-14 10:42:44.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/save_management/save.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2149 2023-04-14 13:34:53.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/save_management/server_upload.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    12640 2023-03-22 09:49:57.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/feature_handler.py
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.550999 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-03-11 10:29:48.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/config_path.txt
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      767 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/enigma_names_en.txt
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1521 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/enigma_names_jp.txt
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       89 2023-04-13 17:31:43.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/item_tracker.json
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.531000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/locales/
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.550999 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/locales/en/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      620 2023-03-11 10:18:02.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/locales/en/config.properties
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      511 2023-03-15 16:33:15.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/locales/en/item.properties
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2911 2023-03-11 10:31:05.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/locales/en/main.properties
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1279 2023-03-15 16:32:48.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/locales/en/user_input.properties
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.550999 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/locales/th/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4776 2023-03-11 09:36:19.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/locales/th/main.properties
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      629 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/order.json
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)        5 2023-05-28 10:10:18.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/version.txt
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4822 2023-05-28 10:08:53.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/game_data_getter.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    23804 2023-05-21 13:49:54.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/helper.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     7470 2023-05-23 18:54:33.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/item.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3505 2023-03-11 09:41:17.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/locale_handler.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1269 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/managed_item.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    72134 2023-05-23 19:18:05.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/parse_save.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1301 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/patcher.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/py.typed
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2415 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/root_handler.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    55862 2023-05-28 09:55:28.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/serialise_save.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    26433 2023-04-14 13:46:46.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/server_handler.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3544 2023-03-11 10:58:50.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/updater.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4474 2023-04-14 13:48:10.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/user_info.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     8297 2023-03-15 16:35:35.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/user_input_handler.py
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.554332 battle-cats-save-editor-2.7.2/src/battle_cats_save_editor.egg-info/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    10938 2023-05-28 10:11:11.000000 battle-cats-save-editor-2.7.2/src/battle_cats_save_editor.egg-info/PKG-INFO
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4240 2023-05-28 10:11:11.000000 battle-cats-save-editor-2.7.2/src/battle_cats_save_editor.egg-info/SOURCES.txt
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)        1 2023-05-28 10:11:11.000000 battle-cats-save-editor-2.7.2/src/battle_cats_save_editor.egg-info/dependency_links.txt
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       72 2023-05-28 10:11:11.000000 battle-cats-save-editor-2.7.2/src/battle_cats_save_editor.egg-info/requires.txt
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       13 2023-05-28 10:11:11.000000 battle-cats-save-editor-2.7.2/src/battle_cats_save_editor.egg-info/top_level.txt
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.554332 battle-cats-save-editor-2.7.2/tests/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      648 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/tests/test_helper.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     6784 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/tests/test_item.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1103 2023-05-28 09:58:47.000000 battle-cats-save-editor-2.7.2/tests/test_parse.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:25:50.174747 battle-cats-save-editor-2.7.2.1/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1071 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/LICENSE
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       95 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/MANIFEST.in
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    10940 2023-05-28 10:25:50.174747 battle-cats-save-editor-2.7.2.1/PKG-INFO
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    10502 2023-05-21 14:21:38.000000 battle-cats-save-editor-2.7.2.1/README.md
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      206 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/pyproject.toml
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       38 2023-05-28 10:25:50.174747 battle-cats-save-editor-2.7.2.1/setup.cfg
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1177 2023-03-11 10:01:29.000000 battle-cats-save-editor-2.7.2.1/setup.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:25:50.154748 battle-cats-save-editor-2.7.2.1/src/
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:25:50.161414 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      283 2023-04-14 10:31:17.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/__init__.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     9841 2023-04-14 13:40:17.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/__main__.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    10151 2023-03-13 20:26:00.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/adb_handler.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    13745 2023-03-11 10:30:59.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/config_manager.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1501 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/csv_handler.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:25:50.161414 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       67 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/__init__.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:25:50.161414 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/basic/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      122 2023-03-14 20:12:33.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/basic/__init__.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     8876 2023-04-14 10:37:56.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/basic/basic_items.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1490 2023-03-11 15:02:56.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/basic/catfruit.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1931 2023-03-11 15:03:21.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/basic/catseyes.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1647 2023-03-14 20:18:26.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/basic/ototo_base_mats.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3984 2023-03-15 16:45:12.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/basic/talent_orbs.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    16533 2023-03-15 16:44:54.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/basic/talent_orbs_new.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:25:50.164748 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/cats/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      179 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/cats/__init__.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     8978 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/cats/cat_helper.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    11121 2023-02-27 19:14:37.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/cats/cat_id_selector.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3249 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/cats/chara_drop.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1068 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/cats/clear_cat_guide.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2844 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/cats/evolve_cats.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1260 2023-02-25 10:47:53.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/cats/get_remove_cats.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     7933 2023-05-23 19:07:27.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/cats/talents.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1900 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/cats/upgrade_blue.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4428 2023-03-15 16:45:17.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/cats/upgrade_cats.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:25:50.164748 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/gamototo/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       66 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/gamototo/__init__.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      309 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/gamototo/fix_gamatoto.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2794 2023-03-11 15:04:37.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/gamototo/gamatoto_xp.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3393 2023-03-11 15:04:50.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/gamototo/helpers.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     7377 2023-05-28 10:08:58.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/gamototo/ototo_cat_cannon.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:25:50.168081 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      313 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/__init__.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1035 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/aku.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      491 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/allow_filibuster_clearing.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      790 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/behemoth_culling.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      646 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/clear_tutorial.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1121 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/enigma_stages.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     6307 2023-03-15 16:45:22.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/event_stages.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1873 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/gauntlet.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1027 2023-03-11 15:09:01.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/itf_timed_scores.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1469 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/legend_quest.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4408 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/main_story.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2323 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/outbreaks.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3031 2023-03-15 16:41:58.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/story_level_id_selector.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1175 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/towers.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     8458 2023-03-11 15:10:07.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/treasures.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1043 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/uncanny.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      784 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/unlock_aku_realm.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:25:50.171414 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/other/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      276 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/other/__init__.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3878 2023-03-11 15:30:39.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/other/cat_shrine.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1093 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/other/claim_user_rank_rewards.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1054 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/other/create_new_account.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2073 2023-04-14 10:35:42.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/other/fix_elsewhere.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      659 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/other/fix_time_issues.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3498 2023-04-06 13:00:50.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/other/get_gold_pass.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     7067 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/other/meow_medals.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4354 2023-02-17 15:14:36.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/other/missions.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      975 2023-03-15 16:45:35.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/other/play_time.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4568 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/other/scheme_item.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1612 2023-03-11 15:30:52.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/other/trade_progress.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1284 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/other/unlock_enemy_guide.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      326 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/other/unlock_equip_menu.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:25:50.171414 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/save_management/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       56 2023-03-15 19:40:58.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/save_management/__init__.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1273 2023-03-22 09:51:45.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/save_management/convert.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2578 2023-03-15 19:41:06.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/save_management/load.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      644 2023-03-15 19:41:09.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/save_management/other.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2073 2023-04-14 10:42:44.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/save_management/save.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2149 2023-04-14 13:34:53.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/save_management/server_upload.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    12640 2023-03-22 09:49:57.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/feature_handler.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:25:50.171414 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/files/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-03-11 10:29:48.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/files/config_path.txt
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      767 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/files/enigma_names_en.txt
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1521 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/files/enigma_names_jp.txt
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       89 2023-04-13 17:31:43.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/files/item_tracker.json
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:25:50.154748 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/files/locales/
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:25:50.174747 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/files/locales/en/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      620 2023-03-11 10:18:02.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/files/locales/en/config.properties
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      511 2023-03-15 16:33:15.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/files/locales/en/item.properties
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2911 2023-03-11 10:31:05.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/files/locales/en/main.properties
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1279 2023-03-15 16:32:48.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/files/locales/en/user_input.properties
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:25:50.174747 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/files/locales/th/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4776 2023-03-11 09:36:19.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/files/locales/th/main.properties
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      629 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/files/order.json
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)        7 2023-05-28 10:24:49.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/files/version.txt
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4822 2023-05-28 10:08:53.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/game_data_getter.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    23804 2023-05-21 13:49:54.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/helper.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     7470 2023-05-23 18:54:33.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/item.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3505 2023-03-11 09:41:17.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/locale_handler.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1269 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/managed_item.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    72134 2023-05-23 19:18:05.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/parse_save.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1301 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/patcher.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/py.typed
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2415 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/root_handler.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    55862 2023-05-28 09:55:28.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/serialise_save.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    26433 2023-04-14 13:46:46.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/server_handler.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3544 2023-03-11 10:58:50.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/updater.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4515 2023-05-28 10:23:57.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/user_info.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     8297 2023-03-15 16:35:35.000000 battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/user_input_handler.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:25:50.174747 battle-cats-save-editor-2.7.2.1/src/battle_cats_save_editor.egg-info/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    10940 2023-05-28 10:25:50.000000 battle-cats-save-editor-2.7.2.1/src/battle_cats_save_editor.egg-info/PKG-INFO
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4240 2023-05-28 10:25:50.000000 battle-cats-save-editor-2.7.2.1/src/battle_cats_save_editor.egg-info/SOURCES.txt
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)        1 2023-05-28 10:25:50.000000 battle-cats-save-editor-2.7.2.1/src/battle_cats_save_editor.egg-info/dependency_links.txt
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       72 2023-05-28 10:25:50.000000 battle-cats-save-editor-2.7.2.1/src/battle_cats_save_editor.egg-info/requires.txt
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       13 2023-05-28 10:25:50.000000 battle-cats-save-editor-2.7.2.1/src/battle_cats_save_editor.egg-info/top_level.txt
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:25:50.174747 battle-cats-save-editor-2.7.2.1/tests/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      648 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/tests/test_helper.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     6784 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2.1/tests/test_item.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1103 2023-05-28 09:58:47.000000 battle-cats-save-editor-2.7.2.1/tests/test_parse.py
```

### Comparing `battle-cats-save-editor-2.7.2/LICENSE` & `battle-cats-save-editor-2.7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/PKG-INFO` & `battle-cats-save-editor-2.7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: battle-cats-save-editor
-Version: 2.7.2
+Version: 2.7.2.1
 Summary: A battle cats save file editor
 Home-page: https://github.com/fieryhenry/BCSFE-Python
 Author: fieryhenry
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `battle-cats-save-editor-2.7.2/README.md` & `battle-cats-save-editor-2.7.2.1/README.md`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/setup.py` & `battle-cats-save-editor-2.7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/__main__.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/__main__.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/adb_handler.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/adb_handler.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/config_manager.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/config_manager.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/csv_handler.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/csv_handler.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/basic/basic_items.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/basic/basic_items.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/basic/catfruit.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/basic/catfruit.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/basic/catseyes.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/basic/catseyes.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/basic/ototo_base_mats.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/basic/ototo_base_mats.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/basic/talent_orbs.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/basic/talent_orbs.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/basic/talent_orbs_new.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/basic/talent_orbs_new.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/cat_helper.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/cats/cat_helper.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/cat_id_selector.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/cats/cat_id_selector.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/chara_drop.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/cats/chara_drop.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/clear_cat_guide.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/cats/clear_cat_guide.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/evolve_cats.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/cats/evolve_cats.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/get_remove_cats.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/cats/get_remove_cats.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/talents.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/cats/talents.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/upgrade_blue.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/cats/upgrade_blue.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/upgrade_cats.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/cats/upgrade_cats.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/gamototo/gamatoto_xp.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/gamototo/gamatoto_xp.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/gamototo/helpers.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/gamototo/helpers.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/gamototo/ototo_cat_cannon.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/gamototo/ototo_cat_cannon.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/aku.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/aku.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/behemoth_culling.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/behemoth_culling.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/clear_tutorial.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/clear_tutorial.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/enigma_stages.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/enigma_stages.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/event_stages.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/event_stages.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/gauntlet.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/gauntlet.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/itf_timed_scores.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/itf_timed_scores.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/legend_quest.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/legend_quest.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/main_story.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/main_story.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/outbreaks.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/outbreaks.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/story_level_id_selector.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/story_level_id_selector.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/towers.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/towers.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/treasures.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/treasures.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/uncanny.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/uncanny.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/unlock_aku_realm.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/levels/unlock_aku_realm.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/cat_shrine.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/other/cat_shrine.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/claim_user_rank_rewards.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/other/claim_user_rank_rewards.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/create_new_account.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/other/create_new_account.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/fix_elsewhere.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/other/fix_elsewhere.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/fix_time_issues.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/other/fix_time_issues.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/get_gold_pass.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/other/get_gold_pass.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/meow_medals.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/other/meow_medals.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/missions.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/other/missions.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/play_time.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/other/play_time.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/scheme_item.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/other/scheme_item.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/trade_progress.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/other/trade_progress.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/unlock_enemy_guide.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/other/unlock_enemy_guide.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/save_management/convert.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/save_management/convert.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/save_management/load.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/save_management/load.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/save_management/other.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/save_management/other.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/save_management/save.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/save_management/save.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/save_management/server_upload.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/edits/save_management/server_upload.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/feature_handler.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/feature_handler.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/enigma_names_en.txt` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/files/enigma_names_en.txt`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/enigma_names_jp.txt` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/files/enigma_names_jp.txt`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/locales/en/config.properties` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/files/locales/en/config.properties`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/locales/en/main.properties` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/files/locales/en/main.properties`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/locales/en/user_input.properties` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/files/locales/en/user_input.properties`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/locales/th/main.properties` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/files/locales/th/main.properties`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/order.json` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/files/order.json`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/game_data_getter.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/game_data_getter.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/helper.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/helper.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/item.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/item.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/locale_handler.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/locale_handler.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/managed_item.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/managed_item.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/parse_save.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/parse_save.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/patcher.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/patcher.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/root_handler.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/root_handler.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/serialise_save.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/serialise_save.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/server_handler.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/server_handler.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/updater.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/updater.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/user_info.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/user_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,12 +126,13 @@
         self.managed_items.managed_items[item_type] += amount
         self.save()
 
     @staticmethod
     def clear_all_items():
         app_data_folder = config_manager.get_app_data_folder()
         path = os.path.join(app_data_folder, "user_info")
+        os.makedirs(path, exist_ok=True)
         files = helper.get_files_in_dir(path)
         for file in files:
             if file.endswith(".json"):
                 info = UserInfo(file.replace(".json", ""))
                 info.clear_managed_items()
```

### Comparing `battle-cats-save-editor-2.7.2/src/BCSFE_Python/user_input_handler.py` & `battle-cats-save-editor-2.7.2.1/src/BCSFE_Python/user_input_handler.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/src/battle_cats_save_editor.egg-info/PKG-INFO` & `battle-cats-save-editor-2.7.2.1/src/battle_cats_save_editor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: battle-cats-save-editor
-Version: 2.7.2
+Version: 2.7.2.1
 Summary: A battle cats save file editor
 Home-page: https://github.com/fieryhenry/BCSFE-Python
 Author: fieryhenry
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `battle-cats-save-editor-2.7.2/src/battle_cats_save_editor.egg-info/SOURCES.txt` & `battle-cats-save-editor-2.7.2.1/src/battle_cats_save_editor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/tests/test_helper.py` & `battle-cats-save-editor-2.7.2.1/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/tests/test_item.py` & `battle-cats-save-editor-2.7.2.1/tests/test_item.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.2/tests/test_parse.py` & `battle-cats-save-editor-2.7.2.1/tests/test_parse.py`

 * *Files identical despite different names*

