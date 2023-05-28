# Comparing `tmp/battle-cats-save-editor-2.7.1.tar.gz` & `tmp/battle-cats-save-editor-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "battle-cats-save-editor-2.7.1.tar", last modified: Wed Mar 22 09:57:39 2023, max compression
+gzip compressed data, was "battle-cats-save-editor-2.7.2.tar", last modified: Sun May 28 10:11:11 2023, max compression
```

## Comparing `battle-cats-save-editor-2.7.1.tar` & `battle-cats-save-editor-2.7.2.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-03-22 09:57:39.672621 battle-cats-save-editor-2.7.1/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1071 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/LICENSE
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       95 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/MANIFEST.in
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    10948 2023-03-22 09:57:39.672621 battle-cats-save-editor-2.7.1/PKG-INFO
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    10511 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/README.md
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      206 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/pyproject.toml
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       38 2023-03-22 09:57:39.672621 battle-cats-save-editor-2.7.1/setup.cfg
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1177 2023-03-11 10:01:29.000000 battle-cats-save-editor-2.7.1/setup.py
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-03-22 09:57:39.659288 battle-cats-save-editor-2.7.1/src/
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-03-22 09:57:39.662621 battle-cats-save-editor-2.7.1/src/BCSFE_Python/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      281 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/__init__.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     9869 2023-03-15 19:52:30.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/__main__.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    10151 2023-03-13 20:26:00.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/adb_handler.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    13745 2023-03-11 10:30:59.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/config_manager.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1501 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/csv_handler.py
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-03-22 09:57:39.662621 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       67 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/__init__.py
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-03-22 09:57:39.665954 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/basic/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      122 2023-03-14 20:12:33.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/basic/__init__.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     8690 2023-03-14 20:19:57.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/basic/basic_items.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1490 2023-03-11 15:02:56.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/basic/catfruit.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1931 2023-03-11 15:03:21.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/basic/catseyes.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1647 2023-03-14 20:18:26.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/basic/ototo_base_mats.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3984 2023-03-15 16:45:12.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/basic/talent_orbs.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    16533 2023-03-15 16:44:54.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/basic/talent_orbs_new.py
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-03-22 09:57:39.665954 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/cats/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      179 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/cats/__init__.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     8978 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/cats/cat_helper.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    11121 2023-02-27 19:14:37.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/cats/cat_id_selector.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3249 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/cats/chara_drop.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1068 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/cats/clear_cat_guide.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2844 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/cats/evolve_cats.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1260 2023-02-25 10:47:53.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/cats/get_remove_cats.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     7936 2023-03-11 15:25:34.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/cats/talents.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1900 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/cats/upgrade_blue.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4428 2023-03-15 16:45:17.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/cats/upgrade_cats.py
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-03-22 09:57:39.665954 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/gamototo/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       66 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/gamototo/__init__.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      309 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/gamototo/fix_gamatoto.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2794 2023-03-11 15:04:37.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/gamototo/gamatoto_xp.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3393 2023-03-11 15:04:50.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/gamototo/helpers.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4137 2023-03-11 15:33:10.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/gamototo/ototo_cat_cannon.py
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-03-22 09:57:39.669288 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      313 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/__init__.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1035 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/aku.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      491 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/allow_filibuster_clearing.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      790 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/behemoth_culling.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      646 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/clear_tutorial.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1121 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/enigma_stages.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     6307 2023-03-15 16:45:22.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/event_stages.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1873 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/gauntlet.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1027 2023-03-11 15:09:01.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/itf_timed_scores.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1469 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/legend_quest.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4408 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/main_story.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2323 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/outbreaks.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3031 2023-03-15 16:41:58.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/story_level_id_selector.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1175 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/towers.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     8458 2023-03-11 15:10:07.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/treasures.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1043 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/uncanny.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      784 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/unlock_aku_realm.py
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-03-22 09:57:39.669288 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/other/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      276 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/other/__init__.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3878 2023-03-11 15:30:39.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/other/cat_shrine.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1093 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/other/claim_user_rank_rewards.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1054 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/other/create_new_account.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2187 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/other/fix_elsewhere.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      659 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/other/fix_time_issues.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3445 2023-03-15 16:45:27.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/other/get_gold_pass.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     7067 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/other/meow_medals.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4354 2023-02-17 15:14:36.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/other/missions.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      975 2023-03-15 16:45:35.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/other/play_time.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4568 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/other/scheme_item.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1612 2023-03-11 15:30:52.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/other/trade_progress.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1284 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/other/unlock_enemy_guide.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      326 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/other/unlock_equip_menu.py
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-03-22 09:57:39.669288 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/save_management/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       56 2023-03-15 19:40:58.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/save_management/__init__.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1273 2023-03-22 09:51:45.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/save_management/convert.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2578 2023-03-15 19:41:06.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/save_management/load.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      644 2023-03-15 19:41:09.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/save_management/other.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2049 2023-03-15 20:17:25.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/save_management/save.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1904 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/save_management/server_upload.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    12640 2023-03-22 09:49:57.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/feature_handler.py
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-03-22 09:57:39.669288 battle-cats-save-editor-2.7.1/src/BCSFE_Python/files/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-03-11 10:29:48.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/files/config_path.txt
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      767 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/files/enigma_names_en.txt
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1521 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/files/enigma_names_jp.txt
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       89 2023-03-22 09:51:08.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/files/item_tracker.json
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-03-22 09:57:39.659288 battle-cats-save-editor-2.7.1/src/BCSFE_Python/files/locales/
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-03-22 09:57:39.672621 battle-cats-save-editor-2.7.1/src/BCSFE_Python/files/locales/en/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      620 2023-03-11 10:18:02.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/files/locales/en/config.properties
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      511 2023-03-15 16:33:15.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/files/locales/en/item.properties
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2911 2023-03-11 10:31:05.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/files/locales/en/main.properties
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1279 2023-03-15 16:32:48.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/files/locales/en/user_input.properties
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-03-22 09:57:39.672621 battle-cats-save-editor-2.7.1/src/BCSFE_Python/files/locales/th/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4776 2023-03-11 09:36:19.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/files/locales/th/main.properties
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      629 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/files/order.json
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)        5 2023-03-22 09:56:37.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/files/version.txt
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4822 2023-03-14 20:07:04.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/game_data_getter.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    22888 2023-03-15 16:44:14.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/helper.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     7075 2023-03-15 16:50:29.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/item.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3505 2023-03-11 09:41:17.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/locale_handler.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1269 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/managed_item.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    66964 2023-03-15 20:17:36.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/parse_save.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1301 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/patcher.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/py.typed
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2415 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/root_handler.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    53791 2023-03-15 20:16:59.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/serialise_save.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    25118 2023-03-13 21:13:33.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/server_handler.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3717 2023-02-25 14:42:42.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/tracker.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3544 2023-03-11 10:58:50.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/updater.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     8297 2023-03-15 16:35:35.000000 battle-cats-save-editor-2.7.1/src/BCSFE_Python/user_input_handler.py
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-03-22 09:57:39.672621 battle-cats-save-editor-2.7.1/src/battle_cats_save_editor.egg-info/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    10948 2023-03-22 09:57:39.000000 battle-cats-save-editor-2.7.1/src/battle_cats_save_editor.egg-info/PKG-INFO
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4238 2023-03-22 09:57:39.000000 battle-cats-save-editor-2.7.1/src/battle_cats_save_editor.egg-info/SOURCES.txt
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)        1 2023-03-22 09:57:39.000000 battle-cats-save-editor-2.7.1/src/battle_cats_save_editor.egg-info/dependency_links.txt
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       72 2023-03-22 09:57:39.000000 battle-cats-save-editor-2.7.1/src/battle_cats_save_editor.egg-info/requires.txt
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       13 2023-03-22 09:57:39.000000 battle-cats-save-editor-2.7.1/src/battle_cats_save_editor.egg-info/top_level.txt
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-03-22 09:57:39.672621 battle-cats-save-editor-2.7.1/tests/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      648 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/tests/test_helper.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     6784 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.1/tests/test_item.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1103 2023-03-04 14:35:58.000000 battle-cats-save-editor-2.7.1/tests/test_parse.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.554332 battle-cats-save-editor-2.7.2/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1071 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/LICENSE
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       95 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/MANIFEST.in
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    10938 2023-05-28 10:11:11.554332 battle-cats-save-editor-2.7.2/PKG-INFO
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    10502 2023-05-21 14:21:38.000000 battle-cats-save-editor-2.7.2/README.md
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      206 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/pyproject.toml
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       38 2023-05-28 10:11:11.554332 battle-cats-save-editor-2.7.2/setup.cfg
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1177 2023-03-11 10:01:29.000000 battle-cats-save-editor-2.7.2/setup.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.531000 battle-cats-save-editor-2.7.2/src/
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.534333 battle-cats-save-editor-2.7.2/src/BCSFE_Python/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      283 2023-04-14 10:31:17.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/__init__.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     9841 2023-04-14 13:40:17.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/__main__.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    10151 2023-03-13 20:26:00.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/adb_handler.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    13745 2023-03-11 10:30:59.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/config_manager.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1501 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/csv_handler.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.534333 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       67 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/__init__.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.537666 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/basic/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      122 2023-03-14 20:12:33.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/basic/__init__.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     8876 2023-04-14 10:37:56.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/basic/basic_items.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1490 2023-03-11 15:02:56.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/basic/catfruit.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1931 2023-03-11 15:03:21.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/basic/catseyes.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1647 2023-03-14 20:18:26.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/basic/ototo_base_mats.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3984 2023-03-15 16:45:12.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/basic/talent_orbs.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    16533 2023-03-15 16:44:54.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/basic/talent_orbs_new.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.541000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      179 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/__init__.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     8978 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/cat_helper.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    11121 2023-02-27 19:14:37.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/cat_id_selector.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3249 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/chara_drop.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1068 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/clear_cat_guide.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2844 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/evolve_cats.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1260 2023-02-25 10:47:53.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/get_remove_cats.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     7933 2023-05-23 19:07:27.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/talents.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1900 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/upgrade_blue.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4428 2023-03-15 16:45:17.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/upgrade_cats.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.541000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/gamototo/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       66 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/gamototo/__init__.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      309 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/gamototo/fix_gamatoto.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2794 2023-03-11 15:04:37.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/gamototo/gamatoto_xp.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3393 2023-03-11 15:04:50.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/gamototo/helpers.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     7377 2023-05-28 10:08:58.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/gamototo/ototo_cat_cannon.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.544333 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      313 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/__init__.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1035 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/aku.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      491 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/allow_filibuster_clearing.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      790 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/behemoth_culling.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      646 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/clear_tutorial.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1121 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/enigma_stages.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     6307 2023-03-15 16:45:22.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/event_stages.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1873 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/gauntlet.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1027 2023-03-11 15:09:01.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/itf_timed_scores.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1469 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/legend_quest.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4408 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/main_story.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2323 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/outbreaks.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3031 2023-03-15 16:41:58.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/story_level_id_selector.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1175 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/towers.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     8458 2023-03-11 15:10:07.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/treasures.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1043 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/uncanny.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      784 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/unlock_aku_realm.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.547666 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      276 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/__init__.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3878 2023-03-11 15:30:39.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/cat_shrine.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1093 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/claim_user_rank_rewards.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1054 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/create_new_account.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2073 2023-04-14 10:35:42.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/fix_elsewhere.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      659 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/fix_time_issues.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3498 2023-04-06 13:00:50.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/get_gold_pass.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     7067 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/meow_medals.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4354 2023-02-17 15:14:36.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/missions.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      975 2023-03-15 16:45:35.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/play_time.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4568 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/scheme_item.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1612 2023-03-11 15:30:52.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/trade_progress.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1284 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/unlock_enemy_guide.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      326 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/unlock_equip_menu.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.547666 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/save_management/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       56 2023-03-15 19:40:58.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/save_management/__init__.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1273 2023-03-22 09:51:45.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/save_management/convert.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2578 2023-03-15 19:41:06.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/save_management/load.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      644 2023-03-15 19:41:09.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/save_management/other.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2073 2023-04-14 10:42:44.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/save_management/save.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2149 2023-04-14 13:34:53.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/save_management/server_upload.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    12640 2023-03-22 09:49:57.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/feature_handler.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.550999 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-03-11 10:29:48.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/config_path.txt
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      767 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/enigma_names_en.txt
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1521 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/enigma_names_jp.txt
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       89 2023-04-13 17:31:43.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/item_tracker.json
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.531000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/locales/
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.550999 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/locales/en/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      620 2023-03-11 10:18:02.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/locales/en/config.properties
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      511 2023-03-15 16:33:15.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/locales/en/item.properties
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2911 2023-03-11 10:31:05.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/locales/en/main.properties
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1279 2023-03-15 16:32:48.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/locales/en/user_input.properties
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.550999 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/locales/th/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4776 2023-03-11 09:36:19.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/locales/th/main.properties
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      629 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/order.json
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)        5 2023-05-28 10:10:18.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/version.txt
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4822 2023-05-28 10:08:53.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/game_data_getter.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    23804 2023-05-21 13:49:54.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/helper.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     7470 2023-05-23 18:54:33.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/item.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3505 2023-03-11 09:41:17.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/locale_handler.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1269 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/managed_item.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    72134 2023-05-23 19:18:05.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/parse_save.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1301 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/patcher.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/py.typed
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2415 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/root_handler.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    55862 2023-05-28 09:55:28.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/serialise_save.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    26433 2023-04-14 13:46:46.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/server_handler.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3544 2023-03-11 10:58:50.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/updater.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4474 2023-04-14 13:48:10.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/user_info.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     8297 2023-03-15 16:35:35.000000 battle-cats-save-editor-2.7.2/src/BCSFE_Python/user_input_handler.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.554332 battle-cats-save-editor-2.7.2/src/battle_cats_save_editor.egg-info/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    10938 2023-05-28 10:11:11.000000 battle-cats-save-editor-2.7.2/src/battle_cats_save_editor.egg-info/PKG-INFO
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     4240 2023-05-28 10:11:11.000000 battle-cats-save-editor-2.7.2/src/battle_cats_save_editor.egg-info/SOURCES.txt
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)        1 2023-05-28 10:11:11.000000 battle-cats-save-editor-2.7.2/src/battle_cats_save_editor.egg-info/dependency_links.txt
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       72 2023-05-28 10:11:11.000000 battle-cats-save-editor-2.7.2/src/battle_cats_save_editor.egg-info/requires.txt
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       13 2023-05-28 10:11:11.000000 battle-cats-save-editor-2.7.2/src/battle_cats_save_editor.egg-info/top_level.txt
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-05-28 10:11:11.554332 battle-cats-save-editor-2.7.2/tests/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      648 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/tests/test_helper.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     6784 2023-01-22 17:25:20.000000 battle-cats-save-editor-2.7.2/tests/test_item.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1103 2023-05-28 09:58:47.000000 battle-cats-save-editor-2.7.2/tests/test_parse.py
```

### Comparing `battle-cats-save-editor-2.7.1/LICENSE` & `battle-cats-save-editor-2.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/PKG-INFO` & `battle-cats-save-editor-2.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: battle-cats-save-editor
-Version: 2.7.1
+Version: 2.7.2
 Summary: A battle cats save file editor
 Home-page: https://github.com/fieryhenry/BCSFE-Python
 Author: fieryhenry
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 # Battle Cats Save File Editor
 
+[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/M4M53M4MN)
+
 A python save editor for the mobile game The Battle Cats
 
 Join the [discord server](https://discord.gg/DvmMgvn5ZB) if you want to suggest new features, report bugs or get help on how to use the editor (please read the below tutorials / watch the latest [tutorial video](https://www.youtube.com/watch?v=Kr6VaLTXOSY) first before asking for help).
 
-[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/M4M53M4MN)
-
-## Thanks to:
+## Thanks to
 
-Lethal's editor for giving me inspiration to start the project and it helped me work out how to patch the save data and edit cf/xp: https://www.reddit.com/r/BattleCatsCheats/comments/djehhn/editoren/
+Lethal's editor for giving me inspiration to start the project and it helped me work out how to patch the save data and edit cf/xp: <https://www.reddit.com/r/BattleCatsCheats/comments/djehhn/editoren/>
 
 Beeven and csehydrogen's open source code, which helped me figure out how to patch save data: [beeven/battlecats](https://github.com/beeven/battlecats), [csehydrogen/BattleCatsHacker](https://github.com/csehydrogen/BattleCatsHacker)
 
 Everyone who's given me saves, which helped to test save parsing/serialising and to test/develop new features
 
-## How to use:
+## How to use
 
 If you have a pc: watch a [Tutorial video](https://www.youtube.com/watch?v=Kr6VaLTXOSY), or scroll down for a text tutorial
 
 If you only have an android device: read the [Android text tutorial](https://github.com/fieryhenry/BCSFE-Python#android-tutorial)
 
 If you only have an ios device: watch the [IOS tutorial video](https://www.youtube.com/watch?v=xw-uOqQRYJ8) (Made by Viarules)
 
@@ -40,15 +40,15 @@
 
 You no longer need a rooted device nor a rooted android emulator.
 
 Although if you want to get unbanned / fix the elsewhere error you will still need one. I recommend LDPlayer, Nox, or MEmu if needed. Bluestacks is also an option but is more difficult to root as it doesn't have a built in option.
 
 ---
 
-1. Install python (You'll need version 3.9 and up) https://www.python.org/downloads/
+1. Install python (You'll need version 3.9 and up) <https://www.python.org/downloads/>
 
 2. Enter the command: `py -m pip install -U battle-cats-save-editor` into command prompt or another terminal to install the editor (**NOT the Windows Python app**). If that doesn't work then use `python3` or `python` instead of `py` in the command
 
 3. Enter the command: `py -m BCSFE_Python` to run the editor. If that doesn't work then use `python3` or `python` instead of `py` in the command
 
 4. Look below for the tutorial that you need, or watch [here](https://www.youtube.com/watch?v=Kr6VaLTXOSY) for a video
 
@@ -83,27 +83,27 @@
 #### Using a rooted device
 
 If you can't upload your save data using the in-game system because your are banned or the `This save data is currently active elsewhere` message appears, you will need direct access to the save data:
 
 If you don't have a rooted device:
 
 5. You will need to get one of the emulators listed earlier, I recommend LD Player because I know that it works with this method. If you change the default install location, make sure to keep a note of it for it later
-   
+
    1. Enable `root permission` in the settings and under `ADB Debugging` select `Open local connection`. You will need to restart LD Player for the changes to work
-   
+
    2. Open the editor and select the option named `Use adb to pull the save from a rooted device` and enter your game version
 
 6. If you get the option to add adb to your path, select enter `y`.
 
 7. The editor will look for adb in default install directories of common emulators and add it automatically
 
 8. If it fails, then you will need to either
-   
+
    1. Enter the path to your emulator's install directory, it might look like `C:\LDPlayer\LDPlayer4.0`
-   
+
    2. Download adb with from [here](https://dl.google.com/android/repository/platform-tools-latest-windows.zip). Extract the zip and copy the folder path (not adb.exe itself) into the editor
 
 9. Now rerun the editor and try the option again. If it still doesn't work you'll need to manually do it, using the tutorial below.
 
 10. If you get a parsing issue please join the [discord server](https://discord.gg/DvmMgvn5ZB) and report it in #bug-reports and / or dm me your save file (preferably not transfer codes)
 
 11. Edit what you want
@@ -124,25 +124,25 @@
 
 3. Copy the path to the folder that you are in (not adb.exe itself)
 
 4. Then open the windows start menu and search: `edit the system environment variables` and press enter.
 
 5. Then click on the `Environment Variables` button.
 
-6. Then in the `System variables` box find the variable named `Path`, then 
+6. Then in the `System variables` box find the variable named `Path`, then
    click on the `edit` button.
 
 7. Then click `New` and paste the path into it.
 
 8. Click `Ok` then `Ok` again then `Ok` again.
 
 9. Relaunch powershell and maybe restart your whole pc, and try the command
    again.
 
-If this method is too difficult, just use a root file explorer instead 
+If this method is too difficult, just use a root file explorer instead
     and manually get the files that you want. The path that you will need is: `/data/data/jp.co.ponos.battlecatsen/files/SAVE_DATA`
 
 ### How to fix "This save data is currently active elsewhere" or "The current Save Data is in violation"
 
 1. You will need to get access to save data so you will need a rooted device / emulator, so look at the first part of the `Using a rooted device` tutorial.
 
 2. Select the option in `Inquiry Code / Token` to `Fix elsewhere error / Unban account`
@@ -181,15 +181,15 @@
 
 5. Tap `Termux Terminal emulator with packages`
 
 6. Tap `INSTALL` and then `OPEN` once installed
 
 7. Once opened enter the command `pkg install python`
 
-8. If that doesn't work then read this: https://stackoverflow.com/a/71097459
+8. If that doesn't work then read this: <https://stackoverflow.com/a/71097459>
 
 9. Then run `python -m pip install -U battle-cats-save-editor`
 
 10. If that doesn't work then run `pkg upgrade` and try again
 
 11. Then run `python -m BCSFE_Python`
```

### Comparing `battle-cats-save-editor-2.7.1/README.md` & `battle-cats-save-editor-2.7.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Battle Cats Save File Editor
 
+[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/M4M53M4MN)
+
 A python save editor for the mobile game The Battle Cats
 
 Join the [discord server](https://discord.gg/DvmMgvn5ZB) if you want to suggest new features, report bugs or get help on how to use the editor (please read the below tutorials / watch the latest [tutorial video](https://www.youtube.com/watch?v=Kr6VaLTXOSY) first before asking for help).
 
-[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/M4M53M4MN)
-
-## Thanks to:
+## Thanks to
 
-Lethal's editor for giving me inspiration to start the project and it helped me work out how to patch the save data and edit cf/xp: https://www.reddit.com/r/BattleCatsCheats/comments/djehhn/editoren/
+Lethal's editor for giving me inspiration to start the project and it helped me work out how to patch the save data and edit cf/xp: <https://www.reddit.com/r/BattleCatsCheats/comments/djehhn/editoren/>
 
 Beeven and csehydrogen's open source code, which helped me figure out how to patch save data: [beeven/battlecats](https://github.com/beeven/battlecats), [csehydrogen/BattleCatsHacker](https://github.com/csehydrogen/BattleCatsHacker)
 
 Everyone who's given me saves, which helped to test save parsing/serialising and to test/develop new features
 
-## How to use:
+## How to use
 
 If you have a pc: watch a [Tutorial video](https://www.youtube.com/watch?v=Kr6VaLTXOSY), or scroll down for a text tutorial
 
 If you only have an android device: read the [Android text tutorial](https://github.com/fieryhenry/BCSFE-Python#android-tutorial)
 
 If you only have an ios device: watch the [IOS tutorial video](https://www.youtube.com/watch?v=xw-uOqQRYJ8) (Made by Viarules)
 
@@ -26,15 +26,15 @@
 
 You no longer need a rooted device nor a rooted android emulator.
 
 Although if you want to get unbanned / fix the elsewhere error you will still need one. I recommend LDPlayer, Nox, or MEmu if needed. Bluestacks is also an option but is more difficult to root as it doesn't have a built in option.
 
 ---
 
-1. Install python (You'll need version 3.9 and up) https://www.python.org/downloads/
+1. Install python (You'll need version 3.9 and up) <https://www.python.org/downloads/>
 
 2. Enter the command: `py -m pip install -U battle-cats-save-editor` into command prompt or another terminal to install the editor (**NOT the Windows Python app**). If that doesn't work then use `python3` or `python` instead of `py` in the command
 
 3. Enter the command: `py -m BCSFE_Python` to run the editor. If that doesn't work then use `python3` or `python` instead of `py` in the command
 
 4. Look below for the tutorial that you need, or watch [here](https://www.youtube.com/watch?v=Kr6VaLTXOSY) for a video
 
@@ -69,27 +69,27 @@
 #### Using a rooted device
 
 If you can't upload your save data using the in-game system because your are banned or the `This save data is currently active elsewhere` message appears, you will need direct access to the save data:
 
 If you don't have a rooted device:
 
 5. You will need to get one of the emulators listed earlier, I recommend LD Player because I know that it works with this method. If you change the default install location, make sure to keep a note of it for it later
-   
+
    1. Enable `root permission` in the settings and under `ADB Debugging` select `Open local connection`. You will need to restart LD Player for the changes to work
-   
+
    2. Open the editor and select the option named `Use adb to pull the save from a rooted device` and enter your game version
 
 6. If you get the option to add adb to your path, select enter `y`.
 
 7. The editor will look for adb in default install directories of common emulators and add it automatically
 
 8. If it fails, then you will need to either
-   
+
    1. Enter the path to your emulator's install directory, it might look like `C:\LDPlayer\LDPlayer4.0`
-   
+
    2. Download adb with from [here](https://dl.google.com/android/repository/platform-tools-latest-windows.zip). Extract the zip and copy the folder path (not adb.exe itself) into the editor
 
 9. Now rerun the editor and try the option again. If it still doesn't work you'll need to manually do it, using the tutorial below.
 
 10. If you get a parsing issue please join the [discord server](https://discord.gg/DvmMgvn5ZB) and report it in #bug-reports and / or dm me your save file (preferably not transfer codes)
 
 11. Edit what you want
@@ -110,25 +110,25 @@
 
 3. Copy the path to the folder that you are in (not adb.exe itself)
 
 4. Then open the windows start menu and search: `edit the system environment variables` and press enter.
 
 5. Then click on the `Environment Variables` button.
 
-6. Then in the `System variables` box find the variable named `Path`, then 
+6. Then in the `System variables` box find the variable named `Path`, then
    click on the `edit` button.
 
 7. Then click `New` and paste the path into it.
 
 8. Click `Ok` then `Ok` again then `Ok` again.
 
 9. Relaunch powershell and maybe restart your whole pc, and try the command
    again.
 
-If this method is too difficult, just use a root file explorer instead 
+If this method is too difficult, just use a root file explorer instead
     and manually get the files that you want. The path that you will need is: `/data/data/jp.co.ponos.battlecatsen/files/SAVE_DATA`
 
 ### How to fix "This save data is currently active elsewhere" or "The current Save Data is in violation"
 
 1. You will need to get access to save data so you will need a rooted device / emulator, so look at the first part of the `Using a rooted device` tutorial.
 
 2. Select the option in `Inquiry Code / Token` to `Fix elsewhere error / Unban account`
@@ -167,15 +167,15 @@
 
 5. Tap `Termux Terminal emulator with packages`
 
 6. Tap `INSTALL` and then `OPEN` once installed
 
 7. Once opened enter the command `pkg install python`
 
-8. If that doesn't work then read this: https://stackoverflow.com/a/71097459
+8. If that doesn't work then read this: <https://stackoverflow.com/a/71097459>
 
 9. Then run `python -m pip install -U battle-cats-save-editor`
 
 10. If that doesn't work then run `pkg upgrade` and try again
 
 11. Then run `python -m BCSFE_Python`
 
@@ -193,8 +193,8 @@
 git clone https://github.com/fieryhenry/BCSFE-Python.git
 py -m pip install -e BCSFE-Python/
 py -m BCSFE_Python
 ```
 
 If you want to use the editor again all you need to do is run the `py -m BCSFE_Python` command
 
-Then if you want the latest changes you only need to run `git pull` in the downloaded `BCSFE-Python` folder. (use `cd` to change the folder)
+Then if you want the latest changes you only need to run `git pull` in the downloaded `BCSFE-Python` folder. (use `cd` to change the folder)
```

### Comparing `battle-cats-save-editor-2.7.1/setup.py` & `battle-cats-save-editor-2.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/__main__.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     feature_handler,
     game_data_getter,
     helper,
     parse_save,
     patcher,
     serialise_save,
     server_handler,
-    tracker,
+    user_info,
     updater,
     user_input_handler,
     root_handler,
     locale_handler,
 )
 from .edits.levels import clear_tutorial
 
@@ -100,20 +100,18 @@
             updater.try_update(update_data[1])
             helper.exit_editor()
 
 
 def main():
     """Main function"""
 
-    item_tracker = tracker.Tracker()
-
     if config_manager.get_config_value_category(
         "SERVER", "WIPE_TRACKED_ITEMS_ON_START"
     ):
-        item_tracker.reset_tracker()
+        user_info.UserInfo.clear_all_items()
     game_data_getter.check_remove_handler()
 
     check_updates = config_manager.get_config_value_category(
         "START_UP", "CHECK_FOR_UPDATES"
     )
     show_start = not config_manager.get_config_value_category(
         "START_UP", "HIDE_START_TEXT"
```

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/adb_handler.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/adb_handler.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/config_manager.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/config_manager.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/csv_handler.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/csv_handler.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/basic/basic_items.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/basic/basic_items.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     """Handler for editing cat food"""
 
     cat_food = item.IntItem(
         name="Cat Food",
         value=item.Int(save_stats["cat_food"]["Value"]),
         max_value=45000,
         bannable=item.Bannable(
-            managed_item.ManagedItemType.CATFOOD,
+            managed_item.ManagedItemType.CATFOOD, save_stats["inquiry_code"]
         ),
     )
     cat_food.edit()
     save_stats["cat_food"]["Value"] = cat_food.get_value()
     return save_stats
 
 
@@ -49,14 +49,15 @@
     """Handler for editing rare tickets"""
 
     rare_tickets = item.IntItem(
         name="Rare Tickets",
         value=item.Int(save_stats["rare_tickets"]["Value"]),
         max_value=299,
         bannable=item.Bannable(
+            inquiry_code=save_stats["inquiry_code"],
             work_around='&Instead of editing rare tickets directly, use the "Normal Ticket Max Trade Progress" conversion feature instead! It is much more safe.',
             type=managed_item.ManagedItemType.RARE_TICKET,
         ),
     )
     rare_tickets.edit()
     save_stats["rare_tickets"]["Value"] = rare_tickets.get_value()
     return save_stats
@@ -66,14 +67,15 @@
     """Handler for editing platinum tickets"""
 
     platinum_tickets = item.IntItem(
         name="Platinum Tickets",
         value=item.Int(save_stats["platinum_tickets"]["Value"]),
         max_value=9,
         bannable=item.Bannable(
+            inquiry_code=save_stats["inquiry_code"],
             work_around="&Instead of editing platinum tickets, edit platinum shards instead! They are much more safe. 10 platinum shards = 1 platinum ticket",
             type=managed_item.ManagedItemType.PLATINUM_TICKET,
         ),
     )
     platinum_tickets.edit()
     save_stats["platinum_tickets"]["Value"] = platinum_tickets.get_value()
     return save_stats
@@ -255,14 +257,15 @@
     """Handler for editing legend tickets"""
 
     legend_tickets = item.IntItem(
         name="Legend Tickets",
         value=item.Int(save_stats["legend_tickets"]["Value"]),
         max_value=4,
         bannable=item.Bannable(
+            inquiry_code=save_stats["inquiry_code"],
             type=managed_item.ManagedItemType.LEGEND_TICKET,
         ),
     )
     legend_tickets.edit()
     save_stats["legend_tickets"]["Value"] = legend_tickets.get_value()
     return save_stats
```

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/basic/catfruit.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/basic/catfruit.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/basic/catseyes.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/basic/catseyes.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/basic/ototo_base_mats.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/basic/ototo_base_mats.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/basic/talent_orbs.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/basic/talent_orbs.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/basic/talent_orbs_new.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/basic/talent_orbs_new.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/cats/cat_helper.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/cat_helper.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/cats/cat_id_selector.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/cat_id_selector.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/cats/chara_drop.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/chara_drop.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/cats/clear_cat_guide.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/clear_cat_guide.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/cats/evolve_cats.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/evolve_cats.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/cats/get_remove_cats.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/get_remove_cats.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/cats/talents.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/talents.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,32 +69,27 @@
 
 
 def find_order(
     cat_talents: list[dict[str, Any]], cat_talent_data: dict[str, Any]
 ) -> list[str]:
     """Find what talent slot each letter corresponds to"""
 
-    letters = [
-        "A",
-        "B",
-        "C",
-        "D",
-        "E",
-        "F",
-    ]
+    letters = ["A", "B", "C", "D", "E", "F", "G", "H"]
     letter_order: list[str] = []
 
-    for i, talent in enumerate(cat_talents):
-        if i == 0:
-            continue
+    for talent in cat_talents:
         talent_id = talent["id"]
         for letter in letters:
-            ability_id = int(cat_talent_data[f"abilityID_{letter}"])
+            key = f"abilityID_{letter}"
+            if key not in cat_talent_data:
+                continue
+            ability_id = int(cat_talent_data[key])
             if ability_id == talent_id:
                 letter_order.append(letter)
+                break
     return letter_order
 
 
 def get_cat_talents(
     cat_talents: list[dict[str, Any]], cat_talent_data: dict[str, Any]
 ) -> dict[Any, Any]:
     """Get the name and max value of each talent for a specific cat"""
@@ -150,15 +145,15 @@
     cat_talents_levels: list[int] = []
     for cat_id in ids:
         if cat_id not in talents or cat_id not in talent_data:
             continue
         cat_talents = talents[cat_id]
         cat_talents_levels = get_talent_levels(talent_data, talents, cat_id)
         for i, cat_talent_level in enumerate(cat_talents_levels):
-            cat_talents[i + 1]["level"] = cat_talent_level
+            cat_talents[i]["level"] = cat_talent_level
         save_stats["talents"] = talents
 
     print("Successfully set talents")
     return save_stats
 
 
 def remove_all_talents(save_stats: dict[str, Any]) -> dict[str, Any]:
@@ -181,15 +176,15 @@
     cat_talents_levels: list[int] = []
     for cat_id in ids:
         if cat_id not in talents or cat_id not in talent_data:
             continue
         cat_talents = talents[cat_id]
         cat_talents_levels = get_talent_levels(talent_data, talents, cat_id)
         for i in range(len(cat_talents_levels)):
-            cat_talents[i + 1]["level"] = 0
+            cat_talents[i]["level"] = 0
         save_stats["talents"] = talents
 
     print("Successfully removed talents")
     return save_stats
 
 
 def edit_talents_individual(save_stats: dict[str, Any]) -> dict[str, Any]:
@@ -215,27 +210,27 @@
         cat_talent_data = talent_data[cat_id]
         cat_talents = talents[cat_id]
         cat_talent_data_formatted = get_cat_talents(cat_talents, cat_talent_data)
         names: list[str] = []
         maxes: list[int] = []
         for talent_index, cat_talent_formatted in cat_talent_data_formatted.items():
             names.append(cat_talent_formatted["name"])
-            cat_talents_levels.append(cat_talents[talent_index + 1]["level"])
+            cat_talents_levels.append(cat_talents[talent_index]["level"])
             maxes.append(cat_talent_formatted["max"])
         helper.colored_text(f"Cat &{cat_id}& is selected:")
         cat_talents_levels_g = item.IntItemGroup.from_lists(
             names=names,
             values=cat_talents_levels,
             maxes=maxes,
             group_name="Talents",
         )
         cat_talents_levels_g.edit()
         cat_talents_levels = cat_talents_levels_g.get_values()
         for i, cat_talent_level in enumerate(cat_talents_levels):
-            cat_talents[i + 1]["level"] = cat_talent_level
+            cat_talents[i]["level"] = cat_talent_level
 
         talents[cat_id] = cat_talents
 
         save_stats["talents"] = talents
 
     print("Successfully set talents")
     return save_stats
```

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/cats/upgrade_blue.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/upgrade_blue.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/cats/upgrade_cats.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/cats/upgrade_cats.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/gamototo/gamatoto_xp.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/gamototo/gamatoto_xp.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/gamototo/helpers.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/gamototo/helpers.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/aku.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/aku.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/behemoth_culling.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/behemoth_culling.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/clear_tutorial.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/clear_tutorial.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/enigma_stages.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/enigma_stages.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/event_stages.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/event_stages.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/gauntlet.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/gauntlet.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/itf_timed_scores.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/itf_timed_scores.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/legend_quest.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/legend_quest.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/main_story.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/main_story.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/outbreaks.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/outbreaks.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/story_level_id_selector.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/story_level_id_selector.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/towers.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/towers.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/treasures.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/treasures.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/uncanny.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/uncanny.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/levels/unlock_aku_realm.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/levels/unlock_aku_realm.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/other/cat_shrine.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/cat_shrine.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/other/claim_user_rank_rewards.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/claim_user_rank_rewards.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/other/create_new_account.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/create_new_account.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/other/fix_elsewhere.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/fix_elsewhere.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Fix the elsewhere issue and unban an account"""
 import json
 import os
 from typing import Any
 
 
-from ... import helper, adb_handler, server_handler, tracker
+from ... import helper, adb_handler, server_handler, user_info
 
 
 def edit_cache(password: str, token: str, save_stats: dict[str, Any]) -> bool:
     """Edit the cache file in /data/data/jp.co.ponos.battlecats/files/cache/ to add the token and password"""
 
     data = {"password": password, "token": token}
     data_s = json.dumps(data)
@@ -26,30 +26,30 @@
         )
     except adb_handler.ADBException:
         success = False
     os.remove(local_path)
     return success
 
 
-def fix_elsewhere(save_stats: dict[str, Any], force_mi: bool = False, text: bool = True) -> dict[str, Any]:
+def fix_elsewhere(
+    save_stats: dict[str, Any], force_mi: bool = False, text: bool = True
+) -> dict[str, Any]:
     """Handler for fixing the elsewhere issue and unban an account"""
 
     helper.colored_text("Getting account password...", helper.GREEN)
     original_iq = save_stats["inquiry_code"]
     data = server_handler.check_gen_token(save_stats)
     token = data["token"]
     inquiry_code = data["inquiry_code"]
-    password_refresh_data = data["password_refresh_data"]
     if token is None:
         helper.colored_text("Failed to get auth token", helper.RED)
         return save_stats
-    edit_cache(password_refresh_data["password"], token, save_stats)
     if original_iq != inquiry_code or force_mi:
-        item_tracker = tracker.Tracker()
-        item_tracker.reset_tracker()
+        info = user_info.UserInfo(inquiry_code)
+        info.clear_managed_items()
         server_handler.update_managed_items(
             save_stats["inquiry_code"], token, save_stats
         )
     if text:
         helper.colored_text(
             "Done!\nYou may get a ban message when pressing play. If you do, just press play again and it should go away\nPress enter to continue...(You still need to save your changes)",
             helper.DARK_YELLOW,
```

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/other/fix_time_issues.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/fix_time_issues.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/other/get_gold_pass.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/get_gold_pass.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,14 +97,16 @@
     """Give the gold pass"""
 
     officer_id = user_input_handler.colored_input(
         "Enter the &officer ID& you want (Press &enter& for a &random id&, and enter &-1& to &remove the gold pass&):"
     )
     if officer_id == "":
         officer_id = get_random_officer_id()
+    elif officer_id == "-1":
+        officer_id = -1
     else:
         officer_id = helper.check_int_max(officer_id)
 
     if officer_id is None:
         officer_id = 0
 
     if officer_id == -1:
```

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/other/meow_medals.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/meow_medals.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/other/missions.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/missions.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/other/play_time.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/play_time.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/other/scheme_item.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/scheme_item.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/other/trade_progress.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/trade_progress.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/other/unlock_enemy_guide.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/other/unlock_enemy_guide.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/save_management/convert.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/save_management/convert.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/save_management/load.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/save_management/load.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/save_management/other.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/save_management/other.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/save_management/save.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/save_management/save.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,55 +9,55 @@
     """Serialise the save data and exit"""
 
     save_data = serialise_save.start_serialize(save_stats)
     helper.write_save_data(
         save_data, save_stats["version"], helper.get_save_path(), True
     )
 
-    helper.check_tracker(save_stats, helper.get_save_path())
+    helper.check_managed_items(save_stats, helper.get_save_path())
 
     return save_stats
 
 
 def save_save(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Serialise the save data"""
 
     save_data = serialise_save.start_serialize(save_stats)
     helper.write_save_data(
         save_data, save_stats["version"], helper.get_save_path(), False
     )
 
-    helper.check_tracker(save_stats, helper.get_save_path())
+    helper.check_managed_items(save_stats, helper.get_save_path())
 
     return save_stats
 
 
 def save_and_push(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Serialise the save data and and push it to the game"""
 
     save_data = serialise_save.start_serialize(save_stats)
     save_data = patcher.patch_save_data(save_data, save_stats["version"])
     helper.write_file_bytes(helper.get_save_path(), save_data)
 
-    helper.check_tracker(save_stats, helper.get_save_path())
+    helper.check_managed_items(save_stats, helper.get_save_path())
 
     if not helper.is_android():
         adb_handler.adb_push_save_data(save_stats["version"], helper.get_save_path())
 
     return save_stats
 
 
 def save_and_push_rerun(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Serialise the save data and push it to the game and restart the game"""
 
     save_data = serialise_save.start_serialize(save_stats)
     save_data = patcher.patch_save_data(save_data, save_stats["version"])
     helper.write_file_bytes(helper.get_save_path(), save_data)
 
-    helper.check_tracker(save_stats, helper.get_save_path())
+    helper.check_managed_items(save_stats, helper.get_save_path())
 
     if not helper.is_android():
         adb_handler.adb_push_save_data(save_stats["version"], helper.get_save_path())
         adb_handler.rerun_game(save_stats["version"])
     else:
         root_handler.rerun_game(save_stats["version"])
```

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/edits/save_management/server_upload.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/edits/save_management/server_upload.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Handler for server save management functions"""
 from typing import Any
 
-from ... import helper, serialise_save, server_handler
+from ... import helper, serialise_save, server_handler, user_info
 
 
 def upload_metadata(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Upload the metadata to the game server"""
 
     _, save_stats = server_handler.meta_data_upload_handler(
         save_stats, helper.get_save_path()
@@ -22,33 +22,41 @@
     if token is None:
         helper.colored_text("Error generating token")
         return save_stats
     server_handler.update_managed_items(save_stats["inquiry_code"], token, save_stats)
     return save_stats
 
 
+def handle_upload_error(inquiry_code: str):
+    """Show an error message"""
+    info = user_info.UserInfo(inquiry_code)
+    info.set_auth_token("")
+    info.set_password("")
+    helper.colored_text(
+        "Error uploading save data\nPlease try again. If error persists, please report this in #bug-reports"
+    )
+
+
 def save_and_upload(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Serialise the save data, and upload it to the game server"""
 
     save_data = serialise_save.start_serialize(save_stats)
     save_data = helper.write_save_data(
         save_data, save_stats["version"], helper.get_save_path(), False
     )
     upload_data = server_handler.upload_handler(save_stats, helper.get_save_path())
     if upload_data is None:
-        helper.colored_text(
-            "Error uploading save data\nPlease report this in #bug-reports"
-        )
+        handle_upload_error(save_stats["inquiry_code"])
+        return save_stats
+    upload_data, save_stats = upload_data
+    inquiry_code = save_stats["inquiry_code"]
+    if upload_data is None:
+        handle_upload_error(inquiry_code)
         return save_stats
     if "transferCode" not in upload_data:
-        helper.colored_text(
-            "Error uploading save data\nPlease report this in #bug-reports"
-        )
-    if len(upload_data["transferCode"]) < 5:
-        helper.colored_text(
-            "Error uploading save data\nPlease report this in #bug-reports"
-        )
+        handle_upload_error(inquiry_code)
+        return save_stats
     else:
         helper.colored_text(f"Transfer code : &{upload_data['transferCode']}&")
         helper.colored_text(f"Confirmation Code : &{upload_data['pin']}&")
 
     return save_stats
```

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/feature_handler.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/feature_handler.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/files/enigma_names_en.txt` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/enigma_names_en.txt`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/files/enigma_names_jp.txt` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/enigma_names_jp.txt`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/files/locales/en/config.properties` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/locales/en/config.properties`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/files/locales/en/main.properties` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/locales/en/main.properties`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/files/locales/en/user_input.properties` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/locales/en/user_input.properties`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/files/locales/th/main.properties` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/locales/th/main.properties`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/files/order.json` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/files/order.json`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/game_data_getter.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/game_data_getter.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/helper.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 from . import (
     user_input_handler,
     server_handler,
     patcher,
     serialise_save,
     parse_save,
-    tracker,
     config_manager,
+    user_info,
 )
 
 GREEN = "#008000"
 RED = "#FF0000"
 DARK_YELLOW = "#D7C32A"
 BLACK = "#000000"
 WHITE = "#FFFFFF"
@@ -56,14 +56,17 @@
 
     return [dir for dir in os.listdir(path) if os.path.isdir(os.path.join(path, dir))]
 
 
 def delete_dir(path: str) -> None:
     """Delete a directory and all of its contents"""
 
+    if not os.path.exists(path):
+        return
+
     for root, dirs, files in os.walk(path, topdown=False):
         for name in files:
             os.remove(os.path.join(root, name))
         for name in dirs:
             os.rmdir(os.path.join(root, name))
     os.rmdir(path)
 
@@ -124,21 +127,25 @@
 def get_local_files_path() -> str:
     """Get the local files path"""
 
     dir_path = os.path.join(os.path.dirname(os.path.realpath(__file__)), "files")
     return dir_path
 
 
-def read_file_string(file_path: str) -> str:
+def read_file_string(file_path: str, create: bool = False) -> str:
     """Reads a file and returns its contents as a string"""
 
     try:
         with open(file_path, "r", encoding="utf-8") as file:
             return file.read()
     except FileNotFoundError as err:
+        if create:
+            os.makedirs(os.path.dirname(file_path), exist_ok=True)
+            write_file_string(file_path, "")
+            return ""
         raise Exception("File not found: " + file_path) from err
     except UnicodeDecodeError as err:
         raise Exception("Error reading file: " + file_path + ": " + str(err)) from err
 
 
 def chunks(lst: list[Any], chunk_len: int) -> Generator[Any, Any, Any]:
     """Split list into chunks of n"""
@@ -299,14 +306,25 @@
 def write_file_string(file_path: str, data: str):
     """Write file as string"""
 
     with open(file_path, "w", encoding="utf-8") as file:
         file.write(data)
 
 
+def config_clamp(value: int, min: int, max: int, clamp_max_int: bool = True):
+    """Clamp a value between 0 and a max value"""
+
+    disable = config_manager.get_config_value_category("EDITOR", "DISABLE_MAXES")
+    if disable:
+        if clamp_max_int:
+            return clamp_int(value)
+        return value
+    return clamp(value, min, max)
+
+
 def check_clamp(
     values: Any, max_value: int, min_value: int = 0, offset: int = -1
 ) -> list[int]:
     """turn a list of strings into a list of ints and clamp them between a min and max"""
 
     if isinstance(values, str):
         values = [values]
@@ -402,28 +420,38 @@
     """Check if the save data is a Japanese save, checking the config file"""
 
     if config_manager.get_config_value_category("EDITOR", "ONLY_GET_EN_DATA"):
         return False
     return is_jp(save_stats)
 
 
-def check_tracker(save_stats: dict[str, Any], path: str) -> None:
-    """Check if the tracker is enabled"""
-    item_tracker = tracker.Tracker()
+def check_managed_items(save_stats: dict[str, Any], path: str) -> None:
+    """Check if the user has untracked bannable items"""
+    info = user_info.UserInfo(save_stats["inquiry_code"])
 
-    if item_tracker.has_data():
+    if info.has_managed_items():
         upload = (
             user_input_handler.colored_input(
-                "You have untracked bannable items that need to be uploaded. Do you want to upload them now? (&y&/&n&) (You will be unable to do so after exiting unless you have WIPE_TRACKED_ITEMS_ON_START set to False):"
+                "You have untracked bannable items that need to be uploaded. Do you want to upload them now? (&y&/&n&) (I recommend saying &y& to avoid bans):"
             )
             == "y"
         )
         if upload:
             server_handler.meta_data_upload_handler(save_stats, path)
-            colored_text("Uploaded meta data", new=GREEN)
+            colored_text("&Uploaded meta data", new=GREEN)
+        else:
+            delete = (
+                user_input_handler.colored_input(
+                    "Do you want to remove your item logs? (&y&/&n&):"
+                )
+                == "y"
+            )
+            if delete:
+                info.clear_managed_items()
+                colored_text("&Removed item logs", new=GREEN)
 
 
 def exit_editor():
     """Exit the editor"""
 
     sys.exit(0)
 
@@ -470,15 +498,15 @@
         current_path = get_save_path()
         temp_file_path = os.path.join(
             config_manager.get_app_data_folder(), "SAVE_DATA_temp"
         )
         if os.path.exists(temp_file_path):
             data = read_file_bytes(temp_file_path)
             save_stats = parse_save.start_parse(data, get_country_code(data))
-            check_tracker(save_stats, temp_file_path)
+            check_managed_items(save_stats, temp_file_path)
             write_file_bytes(current_path, read_file_bytes(temp_file_path))
             colored_text(
                 f"Save data saved to &{current_path}&",
                 base=GREEN,
                 new=WHITE,
             )
 
@@ -743,14 +771,15 @@
     except PermissionError:
         print(
             colored_text(
                 "Permission denied. Make sure the file is not in use", base=RED
             )
         )
         exit_editor()
+        return
     return path_d.name
 
 
 def select_file(
     title: str,
     file_types: list[tuple[str, str]],
     default_dir: str = "",
```

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/item.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/item.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,27 @@
 from typing import Optional, Union
-from . import managed_item, user_input_handler, helper, locale_handler, tracker
+from . import (
+    managed_item,
+    user_input_handler,
+    helper,
+    locale_handler,
+    config_manager,
+    user_info,
+)
 
 
 class Bannable:
-    def __init__(self, type: "managed_item.ManagedItemType", work_around: str = ""):
+    def __init__(
+        self,
+        type: "managed_item.ManagedItemType",
+        inquiry_code: str,
+        work_around: str = "",
+    ):
         self.type = type
+        self.inquiry_code = inquiry_code
         self.work_around = work_around
 
 
 class Int:
     def __init__(self, value: Optional[int], byte_size: int = 4, signed: bool = True):
         self.value = value
         self.byte_size = byte_size
@@ -27,15 +40,20 @@
         value: Int,
         max_value: Optional[int],
         bannable: Optional[Bannable] = None,
         offset: int = 0,
     ):
         self.name = name
         self.__value = value
+        disable_maxes = config_manager.get_config_value_category(
+            "EDITOR", "DISABLE_MAXES"
+        )
         self.max_value = max_value
+        if disable_maxes:
+            self.max_value = None
         self.bannable = bannable
         self.offset = offset
         self.locale_manager = locale_handler.LocalManager.from_config()
 
     def get_max_value(self) -> int:
         if self.max_value is not None:
             return self.max_value
@@ -77,18 +95,17 @@
                 self.get_value_off(),
             )
         )
         if self.bannable is not None and self.__value.value != original_value:
             new_value = self.__value.value
             if original_value is None:
                 original_value = 0
-            item_tracker = tracker.Tracker()
-            item_tracker.update_tracker(
-                self.__value.value - original_value, self.bannable.type
-            )
+
+            info = user_info.UserInfo(self.bannable.inquiry_code)
+            info.update_item(self.bannable.type, self.__value.value - original_value)
 
     def get_value_off(self) -> int:
         if self.__value.value is None:
             return 0
         return self.__value.value + self.offset
 
     def get_value(self) -> int:
@@ -147,16 +164,16 @@
                 self.locale_manager.search_key("enter_value_text")
                 % (self.group_name, max_str)
             )
             new_value -= offset
             entered_value = helper.clamp(new_value, 0, max_value)
             for id in ids:
                 max_value = self.items[id].get_max_value()
-                new_value = helper.clamp(new_value, 0, max_value)
-                self.items[id].set_value(new_value)
+                value = helper.clamp(new_value, 0, max_value)
+                self.items[id].set_value(value)
 
             helper.colored_text(
                 self.locale_manager.search_key("success_set")
                 % (self.group_name, entered_value + offset)
             )
 
     def get_max_max_value(self) -> int:
@@ -169,18 +186,22 @@
         maxes: Union[list[int], int, None],
         group_name: str,
         offset: int = 0,
     ) -> "IntItemGroup":
         items: list[IntItem] = []
         for i in range(len(names)):
             max_value = maxes[i] if isinstance(maxes, list) else maxes
+            try:
+                value = values[i] if values is not None else None
+            except IndexError:
+                value = None
             items.append(
                 IntItem(
                     names[i],
-                    Int(values[i]) if values is not None else Int(None),
+                    Int(value),
                     max_value,
                     offset=offset,
                 )
             )
         return IntItemGroup(group_name, items)
```

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/locale_handler.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/locale_handler.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/managed_item.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/managed_item.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/parse_save.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/parse_save.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Handler for parsing the save file"""
 
 import collections
 import datetime
+import enum
 import json
 import struct
 import traceback
 from typing import Any, Optional, Union
 
 
 from . import helper
@@ -122,15 +123,14 @@
     time = datetime.datetime(year, month, day, hour, minute, second)
     return time.isoformat()
 
 
 def get_length_data(
     length_bytes: int = 4, separator: int = 4, length: Union[int, None] = None
 ) -> list[int]:
-
     data: list[int] = []
     if length is None:
         length = next_int(length_bytes)
     if save_data_g is None:
         raise Exception("Invalid save data")
     if length > len(save_data_g):
         raise Exception("Length too large")
@@ -497,33 +497,35 @@
 
         val_2 = next_int_len(1)
         data.append(val_2)
 
     return data
 
 
-def get_cat_cannon_data() -> dict[int, dict[str, int]]:
+def get_cat_cannon_data() -> dict[int, dict[str, Any]]:
     length = next_int(4)
-    cannon_data: dict[int, dict[str, int]] = {}
+    cannon_data: dict[int, dict[str, Any]] = {}
     for _ in range(length):
-        cannon = {"level": 0, "unlock_flag": 0}
+        cannon: dict[str, Any] = {}
         cannon_id = next_int(4)
         len_val = next_int(4)
         unlock_flag = next_int(4)
-        level = next_int(4)
-        extra_1 = 0
-        extra_2 = 0
+        effect_level = next_int(4)
+        foundation_level = 0
+        style_level = 0
         if len_val == 4:
-            extra_1 = next_int(4)
-            extra_2 = next_int(4)
-        cannon["level"] = level
+            foundation_level = next_int(4)
+            style_level = next_int(4)
+        cannon["levels"] = {
+            "effect": effect_level,
+            "foundation": foundation_level,
+            "style": style_level,
+        }
         cannon["unlock_flag"] = unlock_flag
         cannon["len_val"] = len_val
-        cannon["extra_1"] = extra_1
-        cannon["extra_2"] = extra_2
         cannon_data[cannon_id] = cannon
     return cannon_data
 
 
 def get_data_near_ht() -> list[dict[str, int]]:
     data: list[dict[str, int]] = []
 
@@ -1577,14 +1579,15 @@
                 f"\nThis save is from before &11.0.0& (current save version is &{helper.gv_to_str(game_version)}&), so this is likely the cause for the issue. &The save editor is not designed to work with saves from before 11.0.0&"
             )
         else:
             helper.colored_text(
                 "\nPlease report this to &#bug-reports&, and/or &dm me your save& on discord"
             )
         helper.exit_editor()
+        return {}
     return save_stats
 
 
 def get_game_version(save_data: bytes) -> int:
     """Get the game version from the save data."""
 
     return convert_little(save_data[0:3])
@@ -1724,21 +1727,170 @@
         elif value_type == bool:
             data[key] = next_int(1) == 1
         else:
             raise Exception("Invalid value type")
     return data
 
 
+class BackupState(enum.Enum):
+    IDLE = 0
+    GO_TO_CAN_BACKUP = 1
+    IN_CAN_BACKUP = 2
+    GO_TO_CHECK_BAN = 3
+    IN_CHECK_BAN = 4
+    GO_TO_BACKUP = 5
+    IN_BACKUP = 6
+    FINISHED = 7
+
+
+def get_110900_data() -> list[dict[str, int]]:
+    data: list[dict[str, int]] = []
+
+    data.append(next_int_len(4))
+    data.append(next_int_len(2))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+
+    ivar_14 = next_int_len(1)
+    data.append(ivar_14)
+
+    for _ in range(ivar_14["Value"]):
+        data.append(next_int_len(2))
+
+    svar6 = next_int_len(2)
+    data.append(svar6)
+
+    for _ in range(svar6["Value"]):
+        data.append(next_int_len(2))
+
+    svar6 = next_int_len(2)
+    data.append(svar6)
+
+    for _ in range(svar6["Value"]):
+        data.append(next_int_len(2))
+
+    data.append(next_int_len(4))
+    data.append(next_int_len(4))
+    data.append(next_int_len(4))
+    data.append(next_int_len(2))
+    data.append(next_int_len(2))
+    data.append(next_int_len(2))
+    data.append(next_int_len(2))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    svar6 = next_int_len(2)
+    data.append(svar6)
+
+    for _ in range(svar6["Value"]):
+        data.append(next_int_len(2))
+
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+
+    cvar4 = next_int_len(1)
+    data.append(cvar4)
+    if 0 < cvar4["Value"]:
+        data.append(next_int_len(2))
+        if cvar4["Value"] != 1:
+            data.append(next_int_len(2))
+            if cvar4["Value"] != 2:
+                data.append(next_int_len(2))
+                if cvar4["Value"] != 3:
+                    data.append(next_int_len(2))
+                    if cvar4["Value"] != 4:
+                        ivar32 = cvar4["Value"] + 4
+                        for _ in range(ivar32):
+                            data.append(next_int_len(2))
+    return data
+
+
+def get_zero_legends() -> list[Any]:
+    total_chapters = next_int(2)
+    chapters: list[dict[str, Any]] = []
+    for _ in range(total_chapters):
+        unknown_1 = next_int(1)
+        total_stars = next_int(1)
+        stars: list[dict[str, Any]] = []
+        for _ in range(total_stars):
+            selected_stage = next_int(1)
+            stages_cleared = next_int(1)
+            unlock_next = next_int(1)
+            total_stages = next_int(2)
+            stages: list[Any] = []
+            for _ in range(total_stages):
+                clear_amount = next_int(2)
+                stages.append(clear_amount)
+            stars.append(
+                {
+                    "selected_stage": selected_stage,
+                    "stages_cleared": stages_cleared,
+                    "unlock_next": unlock_next,
+                    "stages": stages,
+                }
+            )
+        chapters.append(
+            {
+                "unknown_1": unknown_1,
+                "stars": stars,
+            }
+        )
+    return chapters
+
+
+def get_120100_data() -> list[dict[str, int]]:
+    data: list[dict[str, int]] = []
+    svar19 = next_int_len(2)
+    data.append(svar19)
+    for _ in range(svar19["Value"]):
+        data.append(next_int_len(2))
+
+    return data
+
+
+def get_120200_data() -> list[dict[str, int]]:
+    data: list[dict[str, int]] = []
+    data.append(next_int_len(1))
+    data.append(next_int_len(2))
+    cvar4 = next_int_len(1)
+    data.append(cvar4)
+    for _ in range(cvar4["Value"]):
+        data.append(next_int_len(2))
+        data.append(next_int_len(2))
+
+    return data
+
+
 def parse_save(
     save_data: bytes,
     country_code: Union[str, None],
     dst: Optional[bool] = None,
 ) -> dict[str, Any]:
     """Parse the save data."""
-
+    if country_code == "ja" or country_code == "":
+        country_code = "jp"
     set_address(0)
     global save_data_g
     save_data_g = save_data
     save_stats: dict[str, Any] = {}
     save_stats["editor_version"] = updater.get_local_version()
 
     save_stats["game_version"] = next_int_len(4)
@@ -2319,15 +2471,40 @@
     save_stats["unknown_129"] = get_110800_data()
 
     save_stats["dojo_3x_speed"] = next_int_len(1)
 
     save_stats["unknown_132"] = get_110800_data_2()
 
     save_stats["gv_110800"] = next_int_len(4)  # 110800
-    save_stats = check_gv(save_stats, 110800)
+    save_stats = check_gv(save_stats, 110900)
+    if save_stats["exit"]:
+        return save_stats
+
+    save_stats["unknown_135"] = get_110900_data()
+    save_stats["gv_110900"] = next_int_len(4)  # 110900
+    save_stats = check_gv(save_stats, 120000)
+    if save_stats["exit"]:
+        return save_stats
+
+    save_stats["zero_legends"] = get_zero_legends()
+    save_stats["unknown_136"] = next_int_len(1)
+    save_stats["gv_120000"] = next_int_len(4)  # 120000
+    save_stats = check_gv(save_stats, 120100)
+    if save_stats["exit"]:
+        return save_stats
+
+    save_stats["unknown_137"] = get_120100_data()
+    save_stats["gv_120100"] = next_int_len(4)  # 120100
+    save_stats = check_gv(save_stats, 120200)
+    if save_stats["exit"]:
+        return save_stats
+
+    save_stats["unknown_138"] = get_120200_data()
+    save_stats["gv_120200"] = next_int_len(4)  # 120200
+    save_stats = check_gv(save_stats, 120200)
     if save_stats["exit"]:
         return save_stats
 
     length = len(save_data) - address - 32
     save_stats["extra_data"] = next_int_len(length)
 
     save_stats = exit_parser(save_stats)
```

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/patcher.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/patcher.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/root_handler.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/root_handler.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/serialise_save.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/serialise_save.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,18 +311,19 @@
     save_data = write(save_data, len(ototo_cannon), 4)
     for cannon_id in ototo_cannon:
         cannon = ototo_cannon[cannon_id]
 
         save_data = write(save_data, int(cannon_id), 4)
         save_data = write(save_data, cannon["len_val"], 4)
         save_data = write(save_data, cannon["unlock_flag"], 4)
-        save_data = write(save_data, cannon["level"], 4)
+        levels = cannon["levels"]
+        save_data = write(save_data, levels["effect"], 4)
         if cannon["len_val"] == 4:
-            save_data = write(save_data, cannon["extra_1"], 4)
-            save_data = write(save_data, cannon["extra_2"], 4)
+            save_data = write(save_data, levels["foundation"], 4)
+            save_data = write(save_data, levels["style"], 4)
     return save_data
 
 
 def serialise_uncanny_current(
     save_data: list[int], uncanny_current: dict[str, Any]
 ) -> list[int]:
     total_sub_chapters = uncanny_current["total"]
@@ -873,14 +874,40 @@
             save_data = write(save_data, value, 1)
         else:
             save_data = write(save_data, value, 4)
 
     return save_data
 
 
+def serialise_zero_legends(save_data: list[int], data: list[Any]):
+    """
+    Serialises the zero legends data
+
+    Args:
+        save_data (list[int]): The save data
+        data (list[Any]): The zero legends data
+    """
+    save_data = write(save_data, len(data), 2)
+    for chapter in data:
+        unknown_1 = chapter["unknown_1"]
+        save_data = write(save_data, unknown_1, 1)
+        save_data = write(save_data, len(chapter["stars"]), 1)
+        for star in chapter["stars"]:
+            selected_stage = star["selected_stage"]
+            stages_cleared = star["stages_cleared"]
+            unlock_next = star["unlock_next"]
+            save_data = write(save_data, selected_stage, 1)
+            save_data = write(save_data, stages_cleared, 1)
+            save_data = write(save_data, unlock_next, 1)
+            save_data = write(save_data, len(star["stages"]), 2)
+            for clear_amount in star["stages"]:
+                save_data = write(save_data, clear_amount, 2)
+    return save_data
+
+
 def serialize_save(save_stats: dict[str, Any]) -> bytes:
     """Serialises the save stats"""
 
     save_data: list[int] = []
 
     save_data = write(save_data, save_stats["game_version"])
 
@@ -1498,17 +1525,47 @@
     save_data = serialise_dumped_data(save_data, save_stats["unknown_129"])
 
     save_data = write(save_data, save_stats["dojo_3x_speed"])
 
     save_data = serialise_dumped_data(save_data, save_stats["unknown_132"])
 
     save_data = write(save_data, save_stats["gv_110800"])
-    data = check_gv(save_data, save_stats, 110800)
+    data = check_gv(save_data, save_stats, 110900)
+    save_data = data["save_data"]
+    if data["exit"]:
+        return bytes(save_data)
+
+    save_data = serialise_dumped_data(save_data, save_stats["unknown_135"])
+
+    save_data = write(save_data, save_stats["gv_110900"])
+    data = check_gv(save_data, save_stats, 120000)
     save_data = data["save_data"]
     if data["exit"]:
         return bytes(save_data)
 
+    save_data = serialise_zero_legends(save_data, save_stats["zero_legends"])
+
+    save_data = write(save_data, save_stats["unknown_136"])
+
+    save_data = write(save_data, save_stats["gv_120000"])
+    data = check_gv(save_data, save_stats, 120100)
+    save_data = data["save_data"]
+    if data["exit"]:
+        return bytes(save_data)
+
+    save_data = serialise_dumped_data(save_data, save_stats["unknown_137"])
+
+    save_data = write(save_data, save_stats["gv_120100"])
+    data = check_gv(save_data, save_stats, 120200)
+    save_data = data["save_data"]
+    if data["exit"]:
+        return bytes(save_data)
+
+    save_data = serialise_dumped_data(save_data, save_stats["unknown_138"])
+
+    save_data = write(save_data, save_stats["gv_120200"])
+
     save_data = write(save_data, save_stats["extra_data"])
 
     save_data = exit_serialiser(save_data, save_stats)
 
     return bytes(save_data)
```

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/server_handler.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/server_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,23 @@
 import json
 from random import randint
 import time
 from typing import Any, Optional, Union
 
 import requests
 
-from . import helper, managed_item, serialise_save, patcher, config_manager, tracker
+from . import (
+    helper,
+    managed_item,
+    serialise_save,
+    patcher,
+    config_manager,
+    user_info,
+    parse_save,
+)
 
 
 def get_current_time() -> int:
     """Get current time."""
 
     return int(time.time())
 
@@ -254,15 +262,15 @@
 
 
 def download_save(
     country_code: str,
     transfer_code: str,
     confirmation_code: str,
     game_version: str,
-) -> bytes:
+) -> requests.Response:
     """Downloads the save for the given country_code, transfer_code, confirmation_code
     and game_version"""
 
     country_code = country_code.replace("jp", "ja")
     url = get_nyanko_save_url() + "/v2/transfers/" + transfer_code + "/reception"
     data = get_client_info(country_code, game_version)
     data["pin"] = confirmation_code
@@ -275,15 +283,15 @@
         "connection": "keep-alive",
         "user-agent": "Dalvik/2.1.0 (Linux; U; Android 9; SM-G955F Build/N2G48B)",
     }
     try:
         response = requests.post(url, data=data_s, headers=headers)
     except requests.exceptions.RequestException as err:
         raise Exception("Error getting save: " + str(err)) from err
-    return response.content
+    return response
 
 
 def upload_save_data_body_v2(
     save_data: bytes,
     save_key_data: dict[str, Any],
 ) -> tuple[bytes, bytes]:
     """Returns the body for the upload save data request
@@ -579,113 +587,132 @@
 
 
 def check_gen_token(
     save_stats: dict[str, Any], path: Optional[str] = None
 ) -> dict[str, Any]:
     """Gets the account auth token"""
 
-    save_stats, password_refresh_data = check_gen_password(save_stats)
+    save_stats, password = check_gen_password(save_stats)
     inquiry_code = save_stats["inquiry_code"]
 
     save_data = None
 
     if path is not None:
         save_data = serialise_save.start_serialize(save_stats)
         save_data = patcher.patch_save_data(save_data, save_stats["version"])
         save_data = helper.write_file_bytes(path, save_data)
 
+    # token = get_auth_token_from_file(inquiry_code)
+    # if token is None:
     token = get_token(
         inquiry_code,
-        password_refresh_data["password"],
+        password,
         save_stats["version"],
         save_stats["game_version"]["Value"],
     )
 
+    info = user_info.UserInfo(inquiry_code)
+
+    info.set_auth_token("" if token is None else token)
+
     return {
         "token": token,
         "save_data": save_data,
         "inquiry_code": inquiry_code,
-        "password_refresh_data": password_refresh_data,
         "save_stats": save_stats,
     }
 
 
-def check_gen_password(
-    save_stats: dict[str, Any]
-) -> tuple[dict[str, Any], dict[str, str]]:
+def check_gen_password(save_stats: dict[str, Any]) -> tuple[dict[str, Any], str]:
     """Checks the password for the given save_stats and generates new if stuff is invalid"""
 
     inquiry_code = save_stats["inquiry_code"]
     password_refresh_token = save_stats["token"]
 
+    info = user_info.UserInfo(inquiry_code)
+
+    password = info.get_password()
+    if password:
+        return save_stats, password
+
     password_refresh_data = get_password_refresh(inquiry_code, password_refresh_token)
     if password_refresh_data is not None:
-        return save_stats, password_refresh_data
+        info.set_password(password_refresh_data["password"])
+        save_stats["token"] = password_refresh_data["passwordRefreshToken"]
+        return save_stats, password_refresh_data["password"]
 
     password_refresh_data = get_password(inquiry_code)
     if password_refresh_data is None:
         inquiry_code = get_inquiry_code()
         save_stats["inquiry_code"] = inquiry_code
 
         return check_gen_password(save_stats)
 
     if "accountCode" in password_refresh_data:
         save_stats["inquiry_code"] = password_refresh_data["accountCode"]
+        info = user_info.UserInfo(password_refresh_data["accountCode"])
 
     password_refresh_token = password_refresh_data["passwordRefreshToken"]
     save_stats["token"] = password_refresh_token
-    return save_stats, password_refresh_data
+    info.set_password(password_refresh_data["password"])
+    return save_stats, password_refresh_data["password"]
 
 
 def prepare_upload(
     save_stats: dict[str, Any],
     path: str,
     print_text: bool = True,
     managed_items: Optional[list[managed_item.ManagedItem]] = None,
-) -> Optional[tuple[str, Any, bytes, int, list[managed_item.ManagedItem]]]:
+) -> Optional[
+    tuple[str, Any, bytes, int, list[managed_item.ManagedItem], dict[str, Any]]
+]:
     """Handles the pre-upload of the save data"""
 
     original_iq = save_stats["inquiry_code"]
     if print_text:
         helper.colored_text("Getting account password...", helper.GREEN)
     data = check_gen_token(save_stats, path)
     token = data["token"]
     inquiry_code = data["inquiry_code"]
     save_data = data["save_data"]
+    save_stats = data["save_stats"]
+    info = user_info.UserInfo(inquiry_code)
     if token is None:
-        if print_text:
-            helper.colored_text(
-                "Error getting account auth token",
-                helper.RED,
-            )
-        return None
-    item_tracker = tracker.Tracker()
+        token = info.get_auth_token()
+        if not token:
+            info.set_password("")
+            if print_text:
+                helper.colored_text(
+                    "Error getting account auth token. Please try again. If this error persists, please report it on the discord server.",
+                    helper.RED,
+                )
+            return None
     if original_iq != inquiry_code:
-        item_tracker.reset_tracker()
+        info.clear_managed_items()
         update_managed_items(save_stats["inquiry_code"], token, save_stats)
 
     if print_text:
         helper.colored_text("Adding meta data...", helper.GREEN)
     if managed_items is None:
-        managed_items = item_tracker.parse_tracker_managed()
+        managed_items = info.get_managed_items_lst()
     playtime = helper.time_to_frames(save_stats["play_time"])
-    tracker.Tracker().reset_tracker()
+    info.clear_managed_items()
 
-    return token, inquiry_code, save_data, playtime, managed_items
+    return token, inquiry_code, save_data, playtime, managed_items, save_stats
 
 
 def upload_handler(
     save_stats: dict[str, Any], path: str
-) -> Union[None, dict[str, Any]]:
+) -> Optional[tuple[Union[None, dict[str, Any]], dict[str, Any]]]:
     """Handles the upload of the save data"""
 
     data = prepare_upload(save_stats, path)
     if data is None:
         return None
-    token, inquiry_code, save_data, playtime, managed_items = data
+    token, inquiry_code, save_data, playtime, managed_items, save_stats = data
 
     helper.colored_text("Uploading save data...", helper.GREEN)
     upload_data = upload_save_data_v2(
         token,
         inquiry_code,
         save_data,
         playtime,
@@ -702,26 +729,26 @@
     # )
 
     helper.colored_text(
         "After entering these codes in game, you may get a ban message when pressing play. If you do, just press play again and it should go away.\nPress enter to get your codes...",
         helper.DARK_YELLOW,
     )
     input()
-    return upload_data
+    return upload_data, save_stats
 
 
 def meta_data_upload_handler(
     save_stats: dict[str, Any], path: str
 ) -> tuple[Union[None, dict[str, Any]], dict[str, Any]]:
     """Handles the upload of the meta data"""
 
     data = prepare_upload(save_stats, path)
     if data is None:
         return None, save_stats
-    token, inquiry_code, save_data, playtime, managed_items = data
+    token, inquiry_code, save_data, playtime, managed_items, save_stats = data
 
     helper.colored_text("Uploading meta data...", helper.GREEN)
     upload_data = upload_metadata_v2(
         token,
         inquiry_code,
         save_data,
         playtime,
@@ -765,25 +792,33 @@
         helper.colored_text(
             "Confirmation code must only be made up of numbers 0-9",
             helper.RED,
         )
         return None
     game_version = input("Enter current game version (e.g 11.3, 9.6, 10.4.0):")
     game_version = helper.str_to_gv(game_version)
-    save_data = download_save(
+    response = download_save(
         country_code, transfer_code, confirmation_code, game_version
     )
+    save_data = response.content
     if test_is_save_data(save_data):
         helper.colored_text("Successfully downloaded save data\n", base=helper.GREEN)
     else:
         helper.colored_text(
-            "Incorrect transfer code / confirmation code",
+            "Incorrect transfer code / confirmation code / country code",
             base=helper.RED,
         )
         return None
+    headers = response.headers
+    save_stats = parse_save.start_parse(save_data, country_code)
+    save_stats["token"] = headers["nyanko-password-refresh-token"]
+    info = user_info.UserInfo(save_stats["inquiry_code"])
+    info.set_password(headers["nyanko-password"])
+    save_data = serialise_save.start_serialize(save_stats)
+    save_data = patcher.patch_save_data(save_data, country_code)
     path = helper.save_file(
         "Save save data",
         helper.get_save_file_filetype(),
         helper.get_save_path_home(),
     )
     if path is None:
         return None
```

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/updater.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/updater.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/BCSFE_Python/user_input_handler.py` & `battle-cats-save-editor-2.7.2/src/BCSFE_Python/user_input_handler.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/src/battle_cats_save_editor.egg-info/PKG-INFO` & `battle-cats-save-editor-2.7.2/src/battle_cats_save_editor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: battle-cats-save-editor
-Version: 2.7.1
+Version: 2.7.2
 Summary: A battle cats save file editor
 Home-page: https://github.com/fieryhenry/BCSFE-Python
 Author: fieryhenry
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 # Battle Cats Save File Editor
 
+[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/M4M53M4MN)
+
 A python save editor for the mobile game The Battle Cats
 
 Join the [discord server](https://discord.gg/DvmMgvn5ZB) if you want to suggest new features, report bugs or get help on how to use the editor (please read the below tutorials / watch the latest [tutorial video](https://www.youtube.com/watch?v=Kr6VaLTXOSY) first before asking for help).
 
-[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/M4M53M4MN)
-
-## Thanks to:
+## Thanks to
 
-Lethal's editor for giving me inspiration to start the project and it helped me work out how to patch the save data and edit cf/xp: https://www.reddit.com/r/BattleCatsCheats/comments/djehhn/editoren/
+Lethal's editor for giving me inspiration to start the project and it helped me work out how to patch the save data and edit cf/xp: <https://www.reddit.com/r/BattleCatsCheats/comments/djehhn/editoren/>
 
 Beeven and csehydrogen's open source code, which helped me figure out how to patch save data: [beeven/battlecats](https://github.com/beeven/battlecats), [csehydrogen/BattleCatsHacker](https://github.com/csehydrogen/BattleCatsHacker)
 
 Everyone who's given me saves, which helped to test save parsing/serialising and to test/develop new features
 
-## How to use:
+## How to use
 
 If you have a pc: watch a [Tutorial video](https://www.youtube.com/watch?v=Kr6VaLTXOSY), or scroll down for a text tutorial
 
 If you only have an android device: read the [Android text tutorial](https://github.com/fieryhenry/BCSFE-Python#android-tutorial)
 
 If you only have an ios device: watch the [IOS tutorial video](https://www.youtube.com/watch?v=xw-uOqQRYJ8) (Made by Viarules)
 
@@ -40,15 +40,15 @@
 
 You no longer need a rooted device nor a rooted android emulator.
 
 Although if you want to get unbanned / fix the elsewhere error you will still need one. I recommend LDPlayer, Nox, or MEmu if needed. Bluestacks is also an option but is more difficult to root as it doesn't have a built in option.
 
 ---
 
-1. Install python (You'll need version 3.9 and up) https://www.python.org/downloads/
+1. Install python (You'll need version 3.9 and up) <https://www.python.org/downloads/>
 
 2. Enter the command: `py -m pip install -U battle-cats-save-editor` into command prompt or another terminal to install the editor (**NOT the Windows Python app**). If that doesn't work then use `python3` or `python` instead of `py` in the command
 
 3. Enter the command: `py -m BCSFE_Python` to run the editor. If that doesn't work then use `python3` or `python` instead of `py` in the command
 
 4. Look below for the tutorial that you need, or watch [here](https://www.youtube.com/watch?v=Kr6VaLTXOSY) for a video
 
@@ -83,27 +83,27 @@
 #### Using a rooted device
 
 If you can't upload your save data using the in-game system because your are banned or the `This save data is currently active elsewhere` message appears, you will need direct access to the save data:
 
 If you don't have a rooted device:
 
 5. You will need to get one of the emulators listed earlier, I recommend LD Player because I know that it works with this method. If you change the default install location, make sure to keep a note of it for it later
-   
+
    1. Enable `root permission` in the settings and under `ADB Debugging` select `Open local connection`. You will need to restart LD Player for the changes to work
-   
+
    2. Open the editor and select the option named `Use adb to pull the save from a rooted device` and enter your game version
 
 6. If you get the option to add adb to your path, select enter `y`.
 
 7. The editor will look for adb in default install directories of common emulators and add it automatically
 
 8. If it fails, then you will need to either
-   
+
    1. Enter the path to your emulator's install directory, it might look like `C:\LDPlayer\LDPlayer4.0`
-   
+
    2. Download adb with from [here](https://dl.google.com/android/repository/platform-tools-latest-windows.zip). Extract the zip and copy the folder path (not adb.exe itself) into the editor
 
 9. Now rerun the editor and try the option again. If it still doesn't work you'll need to manually do it, using the tutorial below.
 
 10. If you get a parsing issue please join the [discord server](https://discord.gg/DvmMgvn5ZB) and report it in #bug-reports and / or dm me your save file (preferably not transfer codes)
 
 11. Edit what you want
@@ -124,25 +124,25 @@
 
 3. Copy the path to the folder that you are in (not adb.exe itself)
 
 4. Then open the windows start menu and search: `edit the system environment variables` and press enter.
 
 5. Then click on the `Environment Variables` button.
 
-6. Then in the `System variables` box find the variable named `Path`, then 
+6. Then in the `System variables` box find the variable named `Path`, then
    click on the `edit` button.
 
 7. Then click `New` and paste the path into it.
 
 8. Click `Ok` then `Ok` again then `Ok` again.
 
 9. Relaunch powershell and maybe restart your whole pc, and try the command
    again.
 
-If this method is too difficult, just use a root file explorer instead 
+If this method is too difficult, just use a root file explorer instead
     and manually get the files that you want. The path that you will need is: `/data/data/jp.co.ponos.battlecatsen/files/SAVE_DATA`
 
 ### How to fix "This save data is currently active elsewhere" or "The current Save Data is in violation"
 
 1. You will need to get access to save data so you will need a rooted device / emulator, so look at the first part of the `Using a rooted device` tutorial.
 
 2. Select the option in `Inquiry Code / Token` to `Fix elsewhere error / Unban account`
@@ -181,15 +181,15 @@
 
 5. Tap `Termux Terminal emulator with packages`
 
 6. Tap `INSTALL` and then `OPEN` once installed
 
 7. Once opened enter the command `pkg install python`
 
-8. If that doesn't work then read this: https://stackoverflow.com/a/71097459
+8. If that doesn't work then read this: <https://stackoverflow.com/a/71097459>
 
 9. Then run `python -m pip install -U battle-cats-save-editor`
 
 10. If that doesn't work then run `pkg upgrade` and try again
 
 11. Then run `python -m BCSFE_Python`
```

### Comparing `battle-cats-save-editor-2.7.1/src/battle_cats_save_editor.egg-info/SOURCES.txt` & `battle-cats-save-editor-2.7.2/src/battle_cats_save_editor.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 src/BCSFE_Python/managed_item.py
 src/BCSFE_Python/parse_save.py
 src/BCSFE_Python/patcher.py
 src/BCSFE_Python/py.typed
 src/BCSFE_Python/root_handler.py
 src/BCSFE_Python/serialise_save.py
 src/BCSFE_Python/server_handler.py
-src/BCSFE_Python/tracker.py
 src/BCSFE_Python/updater.py
+src/BCSFE_Python/user_info.py
 src/BCSFE_Python/user_input_handler.py
 src/BCSFE_Python/edits/__init__.py
 src/BCSFE_Python/edits/basic/__init__.py
 src/BCSFE_Python/edits/basic/basic_items.py
 src/BCSFE_Python/edits/basic/catfruit.py
 src/BCSFE_Python/edits/basic/catseyes.py
 src/BCSFE_Python/edits/basic/ototo_base_mats.py
```

### Comparing `battle-cats-save-editor-2.7.1/tests/test_helper.py` & `battle-cats-save-editor-2.7.2/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/tests/test_item.py` & `battle-cats-save-editor-2.7.2/tests/test_item.py`

 * *Files identical despite different names*

### Comparing `battle-cats-save-editor-2.7.1/tests/test_parse.py` & `battle-cats-save-editor-2.7.2/tests/test_parse.py`

 * *Files identical despite different names*

