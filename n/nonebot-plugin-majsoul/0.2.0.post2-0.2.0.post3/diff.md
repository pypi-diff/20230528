# Comparing `tmp/nonebot_plugin_majsoul-0.2.0.post2.tar.gz` & `tmp/nonebot_plugin_majsoul-0.2.0.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_majsoul-0.2.0.post2.tar", max compression
+gzip compressed data, was "nonebot_plugin_majsoul-0.2.0.post3.tar", max compression
```

## Comparing `nonebot_plugin_majsoul-0.2.0.post2.tar` & `nonebot_plugin_majsoul-0.2.0.post3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448957 nonebot_plugin_majsoul-0.2.0.post2/LICENSE
--rw-r--r--   0        0        0      745 2023-05-28 01:29:10.206173 nonebot_plugin_majsoul-0.2.0.post2/pyproject.toml
--rw-r--r--   0        0        0     3619 2023-05-25 09:15:00.279006 nonebot_plugin_majsoul-0.2.0.post2/README.md
--rw-r--r--   0        0        0     1206 2023-05-28 01:28:19.075384 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/__init__.py
--rw-r--r--   0        0        0      366 2023-05-25 08:45:02.584548 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/config.py
--rw-r--r--   0        0        0      189 2022-12-04 13:51:12.479077 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/errors.py
--rw-r--r--   0        0        0        0 2022-12-04 13:51:12.480120 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/interceptors/__init__.py
--rw-r--r--   0        0        0     1463 2022-12-05 01:32:49.512537 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/interceptors/handle_error.py
--rw-r--r--   0        0        0        0 2022-12-04 15:13:35.630196 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/network/__init__.py
--rw-r--r--   0        0        0      730 2022-12-09 13:59:04.659310 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/network/auto_retry.py
--rw-r--r--   0        0        0     3623 2022-12-09 13:59:04.628312 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/network/host_prober.py
--rw-r--r--   0        0        0      108 2022-12-05 07:11:39.022841 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/__init__.py
--rw-r--r--   0        0        0        0 2022-12-04 13:51:12.475435 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/data/__init__.py
--rw-r--r--   0        0        0     5024 2022-12-05 14:11:58.665190 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/data/api.py
--rw-r--r--   0        0        0        0 2022-12-04 13:51:12.475949 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/data/models/__init__.py
--rw-r--r--   0        0        0     1194 2022-12-05 03:49:36.925512 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/data/models/game_record.py
--rw-r--r--   0        0        0     1967 2022-12-13 10:02:54.142968 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/data/models/player_extended_stats.py
--rw-r--r--   0        0        0      608 2022-12-05 14:13:38.468214 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/data/models/player_info.py
--rw-r--r--   0        0        0       85 2022-12-04 13:51:12.476988 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/data/models/player_num.py
--rw-r--r--   0        0        0     1538 2023-05-10 04:19:02.870093 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/data/models/player_rank.py
--rw-r--r--   0        0        0      490 2022-12-13 10:02:53.723372 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/data/models/player_stats.py
--rw-r--r--   0        0        0     2153 2022-12-04 13:51:12.478551 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/data/models/room_rank.py
--rw-r--r--   0        0        0        0 2022-12-04 13:51:12.481159 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/mappers/__init__.py
--rw-r--r--   0        0        0     2377 2022-12-05 07:11:39.023842 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/mappers/game_record.py
--rw-r--r--   0        0        0      262 2022-12-04 13:51:12.481677 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/mappers/general.py
--rw-r--r--   0        0        0     1634 2022-12-04 14:39:58.711032 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/mappers/player_extended_stats.py
--rw-r--r--   0        0        0      232 2022-12-04 13:58:13.904298 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/mappers/player_num.py
--rw-r--r--   0        0        0      480 2023-05-10 04:19:26.060573 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/mappers/player_rank.py
--rw-r--r--   0        0        0     2536 2022-12-05 14:13:31.596221 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/mappers/player_stats.py
--rw-r--r--   0        0        0     4126 2022-12-04 13:58:13.909299 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/mappers/room_rank.py
--rw-r--r--   0        0        0        0 2022-12-04 13:51:12.483754 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/parsers/__init__.py
--rw-r--r--   0        0        0      568 2023-01-25 14:19:08.842106 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/parsers/limit_of_games.py
--rw-r--r--   0        0        0     2544 2022-12-04 15:26:45.927547 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/parsers/room_rank.py
--rw-r--r--   0        0        0     1189 2023-01-25 14:19:08.832105 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/parsers/time_span.py
--rw-r--r--   0        0        0     7318 2023-05-10 04:08:59.781216 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/query_majsoul_info.py
--rw-r--r--   0        0        0     9731 2023-05-25 08:57:58.318285 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/query_majsoul_pt_plot.py
--rw-r--r--   0        0        0     6945 2023-05-10 04:08:59.775198 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/query_majsoul_records.py
--rw-r--r--   0        0        0       67 2023-05-25 08:11:04.925321 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paipu/__init__.py
--rw-r--r--   0        0        0      887 2023-05-25 08:12:40.329877 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paipu/downloader.py
--rw-r--r--   0        0        0     2631 2023-05-25 09:15:00.280009 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paipu/query_paipu.py
--rw-r--r--   0        0        0        0 2023-05-25 08:00:39.014941 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/utils/__init__.py
--rw-r--r--   0        0        0     1148 2022-12-04 13:51:12.509611 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/utils/decode_integer.py
--rw-r--r--   0        0        0      354 2022-12-11 14:52:31.955889 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/utils/my_executor.py
--rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247572 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/utils/nonebot.py
--rw-r--r--   0        0        0       98 2022-12-04 14:29:52.531881 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/utils/percentile.py
--rw-r--r--   0        0        0      482 2022-12-05 03:18:06.269891 nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/utils/rank.py
--rw-r--r--   0        0        0     4589 1970-01-01 00:00:00.000000 nonebot_plugin_majsoul-0.2.0.post2/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448957 nonebot_plugin_majsoul-0.2.0.post3/LICENSE
+-rw-r--r--   0        0        0      745 2023-05-28 02:02:06.426699 nonebot_plugin_majsoul-0.2.0.post3/pyproject.toml
+-rw-r--r--   0        0        0     3619 2023-05-25 09:15:00.279006 nonebot_plugin_majsoul-0.2.0.post3/README.md
+-rw-r--r--   0        0        0     1144 2023-05-28 02:01:05.003855 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/__init__.py
+-rw-r--r--   0        0        0      366 2023-05-25 08:45:02.584548 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/config.py
+-rw-r--r--   0        0        0      189 2022-12-04 13:51:12.479077 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/errors.py
+-rw-r--r--   0        0        0        0 2022-12-04 13:51:12.480120 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/interceptors/__init__.py
+-rw-r--r--   0        0        0     1463 2022-12-05 01:32:49.512537 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/interceptors/handle_error.py
+-rw-r--r--   0        0        0        0 2022-12-04 15:13:35.630196 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/network/__init__.py
+-rw-r--r--   0        0        0      730 2022-12-09 13:59:04.659310 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/network/auto_retry.py
+-rw-r--r--   0        0        0     3623 2022-12-09 13:59:04.628312 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/network/host_prober.py
+-rw-r--r--   0        0        0      108 2022-12-05 07:11:39.022841 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-04 13:51:12.475435 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/data/__init__.py
+-rw-r--r--   0        0        0     5024 2022-12-05 14:11:58.665190 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/data/api.py
+-rw-r--r--   0        0        0        0 2022-12-04 13:51:12.475949 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/data/models/__init__.py
+-rw-r--r--   0        0        0     1194 2022-12-05 03:49:36.925512 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/data/models/game_record.py
+-rw-r--r--   0        0        0     1967 2022-12-13 10:02:54.142968 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/data/models/player_extended_stats.py
+-rw-r--r--   0        0        0      608 2022-12-05 14:13:38.468214 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/data/models/player_info.py
+-rw-r--r--   0        0        0       85 2022-12-04 13:51:12.476988 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/data/models/player_num.py
+-rw-r--r--   0        0        0     1538 2023-05-10 04:19:02.870093 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/data/models/player_rank.py
+-rw-r--r--   0        0        0      490 2022-12-13 10:02:53.723372 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/data/models/player_stats.py
+-rw-r--r--   0        0        0     2153 2022-12-04 13:51:12.478551 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/data/models/room_rank.py
+-rw-r--r--   0        0        0        0 2022-12-04 13:51:12.481159 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/mappers/__init__.py
+-rw-r--r--   0        0        0     2377 2022-12-05 07:11:39.023842 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/mappers/game_record.py
+-rw-r--r--   0        0        0      262 2022-12-04 13:51:12.481677 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/mappers/general.py
+-rw-r--r--   0        0        0     1634 2022-12-04 14:39:58.711032 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/mappers/player_extended_stats.py
+-rw-r--r--   0        0        0      232 2022-12-04 13:58:13.904298 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/mappers/player_num.py
+-rw-r--r--   0        0        0      480 2023-05-10 04:19:26.060573 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/mappers/player_rank.py
+-rw-r--r--   0        0        0     2536 2022-12-05 14:13:31.596221 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/mappers/player_stats.py
+-rw-r--r--   0        0        0     4126 2022-12-04 13:58:13.909299 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/mappers/room_rank.py
+-rw-r--r--   0        0        0        0 2022-12-04 13:51:12.483754 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/parsers/__init__.py
+-rw-r--r--   0        0        0      568 2023-01-25 14:19:08.842106 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/parsers/limit_of_games.py
+-rw-r--r--   0        0        0     2544 2022-12-04 15:26:45.927547 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/parsers/room_rank.py
+-rw-r--r--   0        0        0     1189 2023-01-25 14:19:08.832105 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/parsers/time_span.py
+-rw-r--r--   0        0        0     7318 2023-05-10 04:08:59.781216 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/query_majsoul_info.py
+-rw-r--r--   0        0        0     9731 2023-05-25 08:57:58.318285 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/query_majsoul_pt_plot.py
+-rw-r--r--   0        0        0     6945 2023-05-10 04:08:59.775198 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/query_majsoul_records.py
+-rw-r--r--   0        0        0       67 2023-05-25 08:11:04.925321 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paipu/__init__.py
+-rw-r--r--   0        0        0      887 2023-05-25 08:12:40.329877 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paipu/downloader.py
+-rw-r--r--   0        0        0     2857 2023-05-28 02:00:53.524174 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paipu/query_paipu.py
+-rw-r--r--   0        0        0        0 2023-05-25 08:00:39.014941 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/utils/__init__.py
+-rw-r--r--   0        0        0     1148 2022-12-04 13:51:12.509611 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/utils/decode_integer.py
+-rw-r--r--   0        0        0      354 2022-12-11 14:52:31.955889 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/utils/my_executor.py
+-rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247572 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/utils/nonebot.py
+-rw-r--r--   0        0        0       98 2022-12-04 14:29:52.531881 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/utils/percentile.py
+-rw-r--r--   0        0        0      482 2022-12-05 03:18:06.269891 nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/utils/rank.py
+-rw-r--r--   0        0        0     4589 1970-01-01 00:00:00.000000 nonebot_plugin_majsoul-0.2.0.post3/PKG-INFO
```

### Comparing `nonebot_plugin_majsoul-0.2.0.post2/LICENSE` & `nonebot_plugin_majsoul-0.2.0.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.0.post2/pyproject.toml` & `nonebot_plugin_majsoul-0.2.0.post3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-majsoul"
-version = "0.2.0.post2"
+version = "0.2.0.post3"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 license = "AGPL-3.0"
 readme = "README.md"
 packages = [
     { include = "nonebot_plugin_majsoul", from = "src" },
 ]
```

### Comparing `nonebot_plugin_majsoul-0.2.0.post2/README.md` & `nonebot_plugin_majsoul-0.2.0.post3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/__init__.py` & `nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 @Author         : ssttkkl
 @License        : AGPLv3
 @GitHub         : https://github.com/ssttkkl/nonebot-plugin-majsoul
 """
 from nonebot import require
 
 require("nonebot_plugin_saa")
-require("nonebot_plugin_gocqhttp_cross_machine_upload_file")
 
 from .utils.nonebot import default_cmd_start
 
 help_text = f"""
 牌谱屋：
 - {default_cmd_start}雀魂(三麻)信息 <雀魂账号> [<房间类型>] [最近<数量>场] [最近<数量>{{天|周|个月|年}}]
 - {default_cmd_start}雀魂(三麻)对局 <雀魂账号> [<房间类型>]
```

### Comparing `nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/interceptors/handle_error.py` & `nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/interceptors/handle_error.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/network/auto_retry.py` & `nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/network/auto_retry.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/network/host_prober.py` & `nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/network/host_prober.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/data/api.py` & `nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/data/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/data/models/game_record.py` & `nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/data/models/game_record.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/data/models/player_extended_stats.py` & `nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/data/models/player_extended_stats.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/data/models/player_info.py` & `nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/data/models/player_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/data/models/player_rank.py` & `nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/data/models/player_rank.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/data/models/room_rank.py` & `nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/data/models/room_rank.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/mappers/game_record.py` & `nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/mappers/game_record.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/mappers/player_extended_stats.py` & `nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/mappers/player_extended_stats.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/mappers/player_stats.py` & `nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/mappers/player_stats.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/mappers/room_rank.py` & `nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/mappers/room_rank.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/parsers/limit_of_games.py` & `nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/parsers/limit_of_games.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/parsers/room_rank.py` & `nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/parsers/room_rank.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/parsers/time_span.py` & `nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/parsers/time_span.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/query_majsoul_info.py` & `nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/query_majsoul_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/query_majsoul_pt_plot.py` & `nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/query_majsoul_pt_plot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paifuya/query_majsoul_records.py` & `nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paifuya/query_majsoul_records.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paipu/downloader.py` & `nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paipu/downloader.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/paipu/query_paipu.py` & `nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/paipu/query_paipu.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,36 @@
-import json
-import re
-from asyncio import wait_for
-
-from nonebot import on_command, logger, require
-from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent, MessageEvent
-from nonebot.params import CommandArg
-from tensoul.downloader import MajsoulDownloadError
+from nonebot import logger, get_driver
 
 from ..config import conf
 
-require("nonebot_plugin_gocqhttp_cross_machine_upload_file")
+if not conf.majsoul_username:
+    logger.warning("majsoul_paipu is disabled because majsoul_username is not configured")
+elif get_driver().type != "fastapi":
+    logger.warning("majsoul_paipu is disabled because only FastAPI Driver is supported")
+else:
+    import json
+    import re
+    from asyncio import wait_for
 
-from nonebot_plugin_gocqhttp_cross_machine_upload_file import upload_group_file, upload_private_file
+    from nonebot import on_command, logger, require
+    from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent, MessageEvent
+    from nonebot.params import CommandArg
+    from tensoul.downloader import MajsoulDownloadError
 
-from .downloader import get_downloader
-from ..errors import BadRequestError
-from ..interceptors.handle_error import handle_error
-from ..utils.nonebot import default_cmd_start
+    from .downloader import get_downloader
+    from ..errors import BadRequestError
+    from ..interceptors.handle_error import handle_error
+    from ..utils.nonebot import default_cmd_start
 
-uuid_reg = re.compile(r"\d{6}-[\da-fA-F]{8}-[\da-fA-F]{4}-[\da-fA-F]{4}-[\da-fA-F]{4}-[\da-fA-F]{12}")
+    uuid_reg = re.compile(r"\d{6}-[\da-fA-F]{8}-[\da-fA-F]{4}-[\da-fA-F]{4}-[\da-fA-F]{4}-[\da-fA-F]{12}")
+
+    require("nonebot_plugin_gocqhttp_cross_machine_upload_file")
+
+    from nonebot_plugin_gocqhttp_cross_machine_upload_file import upload_group_file, upload_private_file
 
-if not conf.majsoul_username:
-    logger.warning("majsoul_paipu is disabled because majsoul_username is not configured")
-else:
     query_majsoul_paipu_matcher = on_command("下载雀魂牌谱")
 
 
     @query_majsoul_paipu_matcher.handle()
     @handle_error(query_majsoul_paipu_matcher)
     async def majsoul_paipu(bot: Bot, event: MessageEvent, args=CommandArg()):
         plain_args = args.extract_plain_text()
```

### Comparing `nonebot_plugin_majsoul-0.2.0.post2/src/nonebot_plugin_majsoul/utils/decode_integer.py` & `nonebot_plugin_majsoul-0.2.0.post3/src/nonebot_plugin_majsoul/utils/decode_integer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.0.post2/PKG-INFO` & `nonebot_plugin_majsoul-0.2.0.post3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-majsoul
-Version: 0.2.0.post2
+Version: 0.2.0.post3
 Summary: 
 License: AGPL-3.0
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-majsoul Version: 0.2.0.post2
+Metadata-Version: 2.1 Name: nonebot-plugin-majsoul Version: 0.2.0.post3
 Summary: License: AGPL-3.0 Author: ssttkkl Author-email:
 huang.wen.long@hotmail.com Requires-Python: >=3.9,<4.0 Classifier: License ::
 OSI Approved :: GNU Affero General Public License v3 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: httpx (>=0.23.0,<0.24.0) Requires-
 Dist: icmplib (>=3.0.3,<4.0.0) Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
```

