# Comparing `tmp/nonebot_plugin_l4d2_server-0.5.4.2.tar.gz` & `tmp/nonebot_plugin_l4d2_server-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.4.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.5.tar", max compression
```

## Comparing `nonebot_plugin_l4d2_server-0.5.4.2.tar` & `nonebot_plugin_l4d2_server-0.5.5.tar`

### file list

```diff
@@ -1,60 +1,63 @@
--rw-r--r--   0        0        0    35149 2023-05-16 06:29:03.169550 nonebot_plugin_l4d2_server-0.5.4.2/LICENSE
--rw-r--r--   0        0        0    11703 2023-05-16 06:29:03.169550 nonebot_plugin_l4d2_server-0.5.4.2/README.md
--rw-r--r--   0        0        0    17493 2023-05-16 06:29:03.173550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/__init__.py
--rw-r--r--   0        0        0   158357 2023-05-16 06:29:03.173550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
--rw-r--r--   0        0        0   631630 2023-05-16 06:29:03.177550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
--rw-r--r--   0        0        0   405369 2023-05-16 06:29:03.177550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
--rw-r--r--   0        0        0     1590 2023-05-16 06:29:03.177550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
--rw-r--r--   0        0        0   242997 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
--rw-r--r--   0        0        0     2135 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
--rw-r--r--   0        0        0     6135 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
--rw-r--r--   0        0        0     6170 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
--rw-r--r--   0        0        0     1523 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
--rw-r--r--   0        0        0     5506 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
--rw-r--r--   0        0        0     2408 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
--rw-r--r--   0        0        0     7874 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
--rw-r--r--   0        0        0      486 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
--rw-r--r--   0        0        0     8734 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
--rw-r--r--   0        0        0     1610 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
--rw-r--r--   0        0        0     3010 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
--rw-r--r--   0        0        0     1694 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_anne/server.py
--rw-r--r--   0        0        0      359 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
--rw-r--r--   0        0        0     3252 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
--rw-r--r--   0        0        0      468 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_data/config.py
--rw-r--r--   0        0        0        0 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_data/database.py
--rw-r--r--   0        0        0     3232 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_data/players.py
--rw-r--r--   0        0        0     1295 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
--rw-r--r--   0        0        0     4097 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
--rw-r--r--   0        0        0     1906 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
--rw-r--r--   0        0        0     2688 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_file/remote.py
--rw-r--r--   0        0        0     4148 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
--rw-r--r--   0        0        0     4007 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_image/download.py
--rw-r--r--   0        0        0     1038 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
--rw-r--r--   0        0        0     9524 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_image/image.py
--rw-r--r--   0        0        0      936 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
--rw-r--r--   0        0        0     3799 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_image/steam.py
--rw-r--r--   0        0        0     1387 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
--rw-r--r--   0        0        0     5429 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
--rw-r--r--   0        0        0     3791 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
--rw-r--r--   0        0        0     1157 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_queries/api.py
--rw-r--r--   0        0        0     1191 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
--rw-r--r--   0        0        0    10855 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
--rw-r--r--   0        0        0     1615 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 06:29:03.181550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_server/index.py
--rw-r--r--   0        0        0     1248 2023-05-16 06:29:03.185550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
--rw-r--r--   0        0        0     1359 2023-05-16 06:29:03.185550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
--rw-r--r--   0        0        0     4113 2023-05-16 06:29:03.185550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
--rw-r--r--   0        0        0     1179 2023-05-16 06:29:03.185550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
--rw-r--r--   0        0        0     2024 2023-05-16 06:29:03.185550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_update/restart.py
--rw-r--r--   0        0        0     1417 2023-05-16 06:29:03.185550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_update/update.py
--rw-r--r--   0        0        0     8892 2023-05-16 06:29:03.185550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_utils/command.py
--rw-r--r--   0        0        0     6212 2023-05-16 06:29:03.185550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_utils/config.py
--rw-r--r--   0        0        0     1620 2023-05-16 06:29:03.185550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_utils/message.py
--rw-r--r--   0        0        0      337 2023-05-16 06:29:03.185550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
--rw-r--r--   0        0        0      992 2023-05-16 06:29:03.185550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
--rw-r--r--   0        0        0     2133 2023-05-16 06:29:03.185550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
--rw-r--r--   0        0        0     8907 2023-05-16 06:29:03.185550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
--rw-r--r--   0        0        0     8575 2023-05-16 06:29:03.185550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_web/web.py
--rw-r--r--   0        0        0    14159 2023-05-16 06:29:03.185550 nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
--rw-r--r--   0        0        0     1434 2023-05-16 06:29:03.185550 nonebot_plugin_l4d2_server-0.5.4.2/pyproject.toml
--rw-r--r--   0        0        0    13540 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.4.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-28 14:15:57.285629 nonebot_plugin_l4d2_server-0.5.5/LICENSE
+-rw-r--r--   0        0        0    11703 2023-05-28 14:15:57.285629 nonebot_plugin_l4d2_server-0.5.5/README.md
+-rw-r--r--   0        0        0    17493 2023-05-28 14:15:57.289629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/__init__.py
+-rw-r--r--   0        0        0   158357 2023-05-28 14:15:57.289629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
+-rw-r--r--   0        0        0   631630 2023-05-28 14:15:57.289629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
+-rw-r--r--   0        0        0   405369 2023-05-28 14:15:57.293629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
+-rw-r--r--   0        0        0     1590 2023-05-28 14:15:57.293629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
+-rw-r--r--   0        0        0   242997 2023-05-28 14:15:57.293629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
+-rw-r--r--   0        0        0     2135 2023-05-28 14:15:57.293629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
+-rw-r--r--   0        0        0     6135 2023-05-28 14:15:57.293629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
+-rw-r--r--   0        0        0     6170 2023-05-28 14:15:57.293629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
+-rw-r--r--   0        0        0     1523 2023-05-28 14:15:57.293629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
+-rw-r--r--   0        0        0     5506 2023-05-28 14:15:57.293629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
+-rw-r--r--   0        0        0     2408 2023-05-28 14:15:57.293629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
+-rw-r--r--   0        0        0     7874 2023-05-28 14:15:57.293629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
+-rw-r--r--   0        0        0      486 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
+-rw-r--r--   0        0        0     1350 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/data/img/white.png
+-rw-r--r--   0        0        0     8734 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
+-rw-r--r--   0        0        0     1610 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
+-rw-r--r--   0        0        0     3010 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
+-rw-r--r--   0        0        0     1694 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_anne/server.py
+-rw-r--r--   0        0        0      359 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
+-rw-r--r--   0        0        0     3252 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
+-rw-r--r--   0        0        0      468 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_data/config.py
+-rw-r--r--   0        0        0        0 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_data/database.py
+-rw-r--r--   0        0        0     3232 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_data/players.py
+-rw-r--r--   0        0        0     1295 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
+-rw-r--r--   0        0        0     4097 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
+-rw-r--r--   0        0        0     1906 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
+-rw-r--r--   0        0        0     1148 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
+-rw-r--r--   0        0        0     2688 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_file/remote.py
+-rw-r--r--   0        0        0     4148 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
+-rw-r--r--   0        0        0     4007 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_image/download.py
+-rw-r--r--   0        0        0     1038 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
+-rw-r--r--   0        0        0     9524 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_image/image.py
+-rw-r--r--   0        0        0     1073 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_image/one.py
+-rw-r--r--   0        0        0      936 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
+-rw-r--r--   0        0        0     3799 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_image/steam.py
+-rw-r--r--   0        0        0     1387 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
+-rw-r--r--   0        0        0     7415 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
+-rw-r--r--   0        0        0     3735 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
+-rw-r--r--   0        0        0     1157 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_queries/api.py
+-rw-r--r--   0        0        0     1191 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
+-rw-r--r--   0        0        0    10855 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
+-rw-r--r--   0        0        0     1615 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_server/index.py
+-rw-r--r--   0        0        0     1248 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
+-rw-r--r--   0        0        0     1359 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
+-rw-r--r--   0        0        0     4113 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
+-rw-r--r--   0        0        0     1175 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
+-rw-r--r--   0        0        0     2024 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_update/restart.py
+-rw-r--r--   0        0        0     1417 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_update/update.py
+-rw-r--r--   0        0        0     9768 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_utils/command.py
+-rw-r--r--   0        0        0     6275 2023-05-28 14:15:57.297629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_utils/config.py
+-rw-r--r--   0        0        0     1620 2023-05-28 14:15:57.301629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_utils/message.py
+-rw-r--r--   0        0        0      337 2023-05-28 14:15:57.301629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
+-rw-r--r--   0        0        0      992 2023-05-28 14:15:57.301629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
+-rw-r--r--   0        0        0     2133 2023-05-28 14:15:57.301629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
+-rw-r--r--   0        0        0     8928 2023-05-28 14:15:57.301629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
+-rw-r--r--   0        0        0     8575 2023-05-28 14:15:57.301629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_web/web.py
+-rw-r--r--   0        0        0    14159 2023-05-28 14:15:57.301629 nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
+-rw-r--r--   0        0        0     1450 2023-05-28 14:15:57.301629 nonebot_plugin_l4d2_server-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0    13578 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.5/PKG-INFO
```

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/LICENSE` & `nonebot_plugin_l4d2_server-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/README.md` & `nonebot_plugin_l4d2_server-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 from .l4d2_utils.txt_to_img import mode_txt_to_img
 # from .l4d2_server import RCONClient
 scheduler = require("nonebot_plugin_apscheduler").scheduler
 
 driver = get_driver()
 
 
-__version__ = "0.5.3"
+__version__ = "0.5.5"
 __plugin_meta__ = PluginMetadata(
     name="求生之路小助手",
     description='群内对有关求生之路的查询和操作',
     usage='求生服务器操作指令',
     extra={
         "version": __version__,
         "author": "Agnes4m <Z735803792@163.com>",
```

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_anne/server.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_anne/server.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_data/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_data/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_data/players.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_data/players.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_data/serverip.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_data/serverip.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_file/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_file/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_file/remote.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_file/remote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_image/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_image/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_image/download.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_image/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_image/image.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_image/image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_image/steam.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_image/steam.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_push/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_push/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pathlib import Path
 import re
+import a2s
 from typing import Dict,List,Union
 try:
     import ujson as json
 except:
     import json
 
 from nonebot.log import logger
@@ -17,16 +18,17 @@
     GROUP_ADMIN,
     GROUP_OWNER,
 )
 require("nonebot_plugin_apscheduler")
 from nonebot_plugin_apscheduler import scheduler
 
 from ..l4d2_utils.command import get_ip_to_mes
-from ..l4d2_utils.utils import extract_last_digit
+from ..l4d2_utils.utils import extract_last_digit,json_server_to_tag_dict,split_maohao
 from ..l4d2_utils.config import l4_config
+from ..l4d2_queries import queries_dict
 
 driver = get_driver()
 sch_json = Path('data/L4D2/scheduler.json')
 if not sch_json.exists():
     with sch_json.open('w') as f:
         json.dump({}, f ,ensure_ascii=False)
         
@@ -39,23 +41,22 @@
     msg = args.extract_plain_text()
     command,message = await extract_last_digit(msg)
     push_msg =  await get_ip_to_mes(msg= message,  command= command)
     if push_msg in ["服务器无响应" ,None] :
         await matcher.finish('无响应的服务器，请检查')
     else:
         return_msg = await add_or_update_data(group_id,msg)
-        print(return_msg)
         if isinstance(push_msg , bytes):
             await matcher.send(MessageSegment.image(push_msg))
         else:
             await matcher.send(push_msg)
         if return_msg == 'add':
-            await matcher.send(f'已添加群定时任务【{msg}】10次')
+            await matcher.send(f'已添加群定时任务【{msg}】{l4_config.l4_push_times}次')
         elif return_msg in ['update','change']:
-            await matcher.send(f'已更新群定时任务【{msg}】10次')
+            await matcher.send(f'已更新群定时任务【{msg}】{l4_config.l4_push_times}次')
 
 @del_rss.handle()
 async def _(event:GroupMessageEvent , matcher:Matcher):
     group_id = event.group_id
     await add_or_update_data(group_id, '' , ad_mode= 'del')
     await matcher.finish('已删除群定时任务')
 
@@ -68,77 +69,128 @@
     group_id = str(group_id)
     sch_json = Path('data/L4D2/scheduler.json')
     if ad_mode == 'add':
         if sch_json.exists():
             with sch_json.open(encoding='utf-8') as f:
                 scheduler_data = json.load(f)
             try:
-                times , old_msg = scheduler_data[group_id]
-                scheduler_data[group_id] = [l4_config.l4_push_times, some_str]
+                msg_dict = scheduler_data[group_id]
+                times = msg_dict['times'] 
+                old_msg = msg_dict['msg']
+                scheduler_data[group_id] = {
+                    'times' :l4_config.l4_push_times, 
+                    'msg' :some_str
+                    }
                 if old_msg == some_str:
                     mode = 'update' 
                 else:
                     mode = 'change'
             except:
-                scheduler_data[group_id] = [l4_config.l4_push_times, some_str]
+                scheduler_data[group_id] = {
+                    'times' :l4_config.l4_push_times, 
+                    'msg' :some_str
+                    }
                 mode = 'new'
 
         else:
-            scheduler_data = {group_id: [l4_config.l4_push_times, some_str]}
+            scheduler_data = {group_id: {
+                    'times' :l4_config.l4_push_times, 
+                    'msg' :some_str
+                    }}
             mode = 'new'
             
         with sch_json.open('w',encoding='utf-8') as f:
             json.dump(scheduler_data, f ,ensure_ascii=False)
     
     else:
         if sch_json.exists():
             with sch_json.open() as f:
-                scheduler_data = json.load(f)
+                scheduler_data:Dict[str,Dict[str,Union[str,int]]] = json.load(f)
             try:
-                times , old_msg = scheduler_data[group_id]  
-                scheduler_data[group_id] = [0, old_msg]
+                msg_dict = scheduler_data[group_id]
+                times = msg_dict['times'] 
+                old_msg = msg_dict['msg'] 
+                scheduler_data[group_id] = {
+                    'times' :0, 
+                    'msg' :old_msg
+                    }
             except:      
-                scheduler_data[group_id] = [0, some_str]
+                scheduler_data[group_id] = {
+                    'times' :0, 
+                    'msg' :some_str
+                    }
         else:
-            scheduler_data = {group_id: [0, some_str]}
+            scheduler_data = {group_id: {
+                    'times' :0, 
+                    'msg' :some_str
+                    }}
         mode = 'del'
             
         with sch_json.open('w',encoding='utf-8') as f:
             json.dump(scheduler_data, f ,ensure_ascii=False)  
             
     return mode
 
 async def rss_ip():
+    """推送一次"""
     sch_json = Path('data/L4D2/scheduler.json')
     
     if sch_json.exists():
         with sch_json.open(encoding='utf-8') as f:
-            scheduler_data:Dict[str,List[Union[int,str]]] = json.load(f)
+            scheduler_data:Dict[str,Dict[str,Union[int,str]]] = json.load(f)
             
             for key, value in scheduler_data.items():
-                recipient_id = int(key)
-                count = value[0]
-                msg = value[-1]
-                
-                if count > 0:
-                    await send_message(recipient_id, msg)
-                    count -= 1
-                
-                scheduler_data[key][0] = count  # 更新次数
+                try:
+                    recipient_id = int(key)
+                    count = value['times']
+                    msg = value['msg']
+        
+                    if count > 0:
+                        msg_read = await send_message(recipient_id, msg ,value)
+                        print(msg_read)
+                        if msg_read:
+                            scheduler_data[key]['ip_detail']  = msg_read
+                        count -= 1
+                    
+                    scheduler_data[key]['times'] = count
+                except TypeError:
+                    continue
                 
         with sch_json.open(mode='w',encoding='utf-8') as f:
             json.dump(scheduler_data, f ,ensure_ascii=False)
         
-async def send_message(recipient_id :int, msg :str):
+async def send_message(recipient_id :int, msg :str ,value :Dict[str,Union[int,str]] = None):
     # 执行发送消息的操作，参数可以根据需要进行传递和使用
     command,message = await extract_last_digit(msg)
     push_msg =  await get_ip_to_mes(msg= message,  command= command)
     if isinstance(push_msg ,bytes):
         await get_bot().send_group_msg(group_id=recipient_id, message=MessageSegment.image(push_msg))
     elif msg and isinstance(push_msg ,str):
-        await get_bot().send_group_msg(group_id=recipient_id, message=push_msg)
+        # 单服务器
+        message = await json_server_to_tag_dict(msg,command)
+        if len(message) == 0:
+            # 关键词不匹配，忽略
+            return
+        try:
+            old_msg = value.get('ip_detail',{})
+            ip = str(message['ip'])
+            host,port = split_maohao(ip)
+            msg:a2s.SourceInfo = await a2s.ainfo((host,port))
+            value['map_'] = msg.map_name
+            value['rank_players'] = f'{msg.player_count}/{msg.max_players}'
+            if old_msg['map_'] == value['map_'] and old_msg['rank_players'] == value['rank_players']:
+                logger.info(f'{msg}{command}人数和地图未发生变化')
+            else:
+                await get_bot().send_group_msg(group_id=recipient_id, message=push_msg)
+        except Exception as e:
+            logger.warning(e)
+            
+        return value
+    
+async def server_is_change():
+    """检测服务器是否发生变化""" 
     
 @driver.on_bot_connect
 async def _():    
     logger.success('已成功启动求生定时推送')
     scheduler.add_job(rss_ip, "interval", minutes=l4_config.l4_push_interval, id="rss_ip")
```

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 async def queries_dict(ip:str,port:int) -> dict:
     port = int(port)
     ip = str(ip)
     msg_dict = {}
     # message_dict = await l4d(ip,port)
     msg:a2s.SourceInfo = await a2s.ainfo((ip,port))
-    # message_dict = await l4d2.server(ip,port,times=5)
     msg_dict['folder'] =  msg.folder
     msg_dict['name'] =  msg.server_name
     msg_dict['map_'] =  msg.map_name
     msg_dict['players'] =  msg.player_count
     msg_dict['max_players'] =  msg.max_players
     msg_dict['rank_players'] =  f'{msg.player_count}/{msg.max_players}'
     msg_dict['ip'] = str(ip) + ':' +str(port)
```

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_queries/api.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_queries/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_server/rcon.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_server/rcon.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_server/workshop.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_server/workshop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_update/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_update/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,10 +32,10 @@
         return '更新失败!更多错误信息请查看控制台...\n' \
                '>> 可以尝试使用\n' \
                '>> [l4强制更新](危险)\n' \
                '>> [l4强行强制更新](超级危险)!'
 
     result = 'L4D2Bot 更新记录\n\n'
     for log in log_list:
-        result += f'- {log[2:]}\n'
+        result += f'- {log}\n'
 
     return result
```

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_update/restart.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_update/restart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_update/update.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_update/update.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_utils/command.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_utils/command.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,17 @@
     )
 
 from ..l4d2_anne.server import server_key,ANNE_IP
 from .config import *
 from ..l4d2_queries.qqgroup import split_maohao
 # from .utils import qq_ip_queries_pic,json_server_to_tag_dict,get_anne_server_ip,get_tan_jian
 from .utils import *
+from .txt_to_img import mode_txt_to_img
+from ..l4d2_image.one import one_server_img
+
 help_ = on_command('l4_help',aliases={'求生帮助'},priority=20,block=True)
 
 # 服务器
 # last_operation_time = nonebot.Config.parse_obj(nonebot.get_driver().config.dict()).SUPERUSERS
 
 
 
@@ -184,17 +187,27 @@
             command = command.replace(start,'')
         if command == 'anne':
             command = '云'
         msg:str = args.extract_plain_text()
         push_msg = await get_ip_to_mes(msg, command)
         if isinstance(push_msg ,bytes):
             await matcher.finish(MessageSegment.image(push_msg))
+        elif msg and isinstance(push_msg ,list):
+            await matcher.finish(MessageSegment.image(push_msg[0]) + Message(push_msg[-1]))
         elif msg and isinstance(push_msg ,str):
-            await matcher.finish(push_msg)
+            try:
+                await matcher.finish(push_msg)
+            except nonebot.adapters.onebot.v11.exception.ActionFailed:
+                lines = push_msg.splitlines()
+                first_str = lines[0]
+                last_str = lines[-1]
+                push_msg = '\n'.join(lines[1:-1])
+                await matcher.finish(mode_txt_to_img(first_str,push_msg)+Message(last_str))
                 
+
 async def get_ip_to_mes(msg:str ,command: str = ''):   
     if not msg:
         # 以图片输出全部当前
         igr = False
         if command in gamemode_list:
             this_ips = [d for l in ALL_HOST.values() for d in l if d.get('version') == command]
             igr = True
@@ -209,28 +222,36 @@
             ip_list.append((one_ip['id'],host,port))
         img = await qq_ip_queries_pic(ip_list,igr)
         if img:
             return img
         else:
             return "服务器无响应"
     else:
+
         if not msg[0].isdigit():
             if any(mode in msg for mode in gamemode_list):
                 pass
             else:
                 return
         message = await json_server_to_tag_dict(command,msg)
         if len(message) == 0:
             # 关键词不匹配，忽略
             return
         ip = str(message['ip'])
         logger.info(ip)
+        
         try:
-            msg= await get_anne_server_ip(ip)
-            return  msg
+            if l4_config.l4_image:
+                host,port = split_maohao(ip)
+                msgs = await queries_dict(host,port)
+                msgs['Players'] += await player_queries_anne_dict(host,port)
+                imgs = await one_server_img()
+            else:
+                msgs = await get_anne_server_ip(ip)
+                return  msgs
         except (OSError,asyncio.exceptions.TimeoutError):
             return '服务器无响应'
```

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_utils/config.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_utils/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 
 class L4d2Config(BaseModel):
     total_enable: bool = Field(True, alias='是否全局启用求生功能')
     map_path: List[str] = Field([], alias='求生地图路径')
     web_username: str = Field('l4d2', alias='后台管理用户名')
     web_password: str = Field('admin', alias='后台管理密码')
     l4_style: str = Field("standard", alias='图片风格')
+    l4_image: bool = Field(False , alias='是否启用图片')
     # l4_file: List[str] = Field(	["/home/ubuntu/l4d2/coop"], alias='本地求生服务器地址')
     # l4_host: List[str] = Field(['127.0.0.1'], alias='求生服务器地址')
     # l4_port: List[str] = Field(['20715'], alias='求生服务器端口')
     # l4_rcon: List[str] = Field(['114514'], alias='求生服务器rcon密码')
     
     l4_ipall: List[Dict[str,Union[str,int,bool]]] = Field(
         [{
```

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_utils/message.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_utils/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_utils/seach.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_utils/seach.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_utils/utils.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,15 +187,15 @@
         return None
     
 async def save_file(file:bytes,path_name):
     """保存文件"""
     with open(path_name,'w') as files:
         files.write(file)
         
-async def get_anne_server_ip(ip):
+async def get_anne_server_ip(ip ,ismsg :bool = False):
     """输出查询ip和ping"""
     host,port = split_maohao(ip)
     data = await queries_server([host,port])
     lines = data.splitlines()
     msg = '\n'.join(lines[1:])
     msg += '\nconnect ' + ip
     return msg
```

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_web/web.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_web/web.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/nonebot_plugin_l4d2_server/l4d2_web/webUI.py` & `nonebot_plugin_l4d2_server-0.5.5/nonebot_plugin_l4d2_server/l4d2_web/webUI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/pyproject.toml` & `nonebot_plugin_l4d2_server-0.5.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-l4d2-server"
-version = "0.5.4.2"
+version = "0.5.5"
 description = "L4D2 server related operations plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 keywords = ["steam", "game", "l4d2", "nonebot2", "plugin"]
@@ -41,11 +41,12 @@
 patool = "^1.12"
 python-a2s = "^1.3.0"
 amis-python = "^1.0.6"
 jieba = "^0.42.1"
 pandas = ">=1.5.2"
 python-jose = "^3.3.0"
 gitpython = ">=3.1.27"
+attrs = "^23.1.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_l4d2_server-0.5.4.2/PKG-INFO` & `nonebot_plugin_l4d2_server-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-l4d2-server
-Version: 0.5.4.2
+Version: 0.5.5
 Summary: L4D2 server related operations plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 License: GPLv3
 Keywords: steam,game,l4d2,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: amis-python (>=1.0.6,<2.0.0)
 Requires-Dist: asyncio (>=3.4.3)
+Requires-Dist: attrs (>=23.1.0,<24.0.0)
 Requires-Dist: beautifulsoup4 (>=4.8.0)
 Requires-Dist: gitpython (>=3.1.27)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: jieba (>=0.42.1,<0.43.0)
 Requires-Dist: jinja2 (>=3.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1.5)
 Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0)
```

#### html2text {}

```diff
@@ -1,32 +1,33 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.4.2
-Summary: L4D2 server related operations plugin for NoneBot2 Home-page: https://
+Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.5 Summary:
+L4D2 server related operations plugin for NoneBot2 Home-page: https://
 github.com/Agnes4m/nonebot_plugin_l4d2_server License: GPLv3 Keywords:
 steam,game,l4d2,nonebot2,plugin Author: Agnes_Digital Author-email:
 Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0) Requires-Dist: amis-python
-(>=1.0.6,<2.0.0) Requires-Dist: asyncio (>=3.4.3) Requires-Dist: beautifulsoup4
-(>=4.8.0) Requires-Dist: gitpython (>=3.1.27) Requires-Dist: httpx
-(>=0.23.3,<0.24.0) Requires-Dist: jieba (>=0.42.1,<0.43.0) Requires-Dist:
-jinja2 (>=3.0.0) Requires-Dist: nonebot-adapter-onebot (>=2.1.5) Requires-Dist:
-nonebot2 (>=2.0.0rc4,<3.0.0) Requires-Dist: nonebot_plugin_apscheduler
-(>=0.2.0,<0.3.0) Requires-Dist: nonebot_plugin_htmlrender (>=0.2.0.1,<0.3.0.0)
-Requires-Dist: nonebot_plugin_txt2img (>=0.3.0) Requires-Dist: pandas (>=1.5.2)
-Requires-Dist: patool (>=1.12,<2.0) Requires-Dist: pillow (>=9.3.0,<10.0.0)
-Requires-Dist: python-a2s (>=1.3.0,<2.0.0) Requires-Dist: python-jose
-(>=3.3.0,<4.0.0) Requires-Dist: pyunpack (>=0.3.0,<0.4.0) Requires-Dist:
-rarfile (>=4.0,<5.0) Requires-Dist: rcon (>=2.1.0,<3.0.0) Requires-Dist:
-ruamel.yaml (>=0.17.21,<0.18.0) Requires-Dist: srctools (>=2.3.9,<3.0.0)
-Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_l4d2_server
-Description-Content-Type: text/markdown
+(>=1.0.6,<2.0.0) Requires-Dist: asyncio (>=3.4.3) Requires-Dist: attrs
+(>=23.1.0,<24.0.0) Requires-Dist: beautifulsoup4 (>=4.8.0) Requires-Dist:
+gitpython (>=3.1.27) Requires-Dist: httpx (>=0.23.3,<0.24.0) Requires-Dist:
+jieba (>=0.42.1,<0.43.0) Requires-Dist: jinja2 (>=3.0.0) Requires-Dist:
+nonebot-adapter-onebot (>=2.1.5) Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0)
+Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0) Requires-Dist:
+nonebot_plugin_htmlrender (>=0.2.0.1,<0.3.0.0) Requires-Dist:
+nonebot_plugin_txt2img (>=0.3.0) Requires-Dist: pandas (>=1.5.2) Requires-Dist:
+patool (>=1.12,<2.0) Requires-Dist: pillow (>=9.3.0,<10.0.0) Requires-Dist:
+python-a2s (>=1.3.0,<2.0.0) Requires-Dist: python-jose (>=3.3.0,<4.0.0)
+Requires-Dist: pyunpack (>=0.3.0,<0.4.0) Requires-Dist: rarfile (>=4.0,<5.0)
+Requires-Dist: rcon (>=2.1.0,<3.0.0) Requires-Dist: ruamel.yaml
+(>=0.17.21,<0.18.0) Requires-Dist: srctools (>=2.3.9,<3.0.0) Project-URL:
+Repository, https://github.com/Agnes4m/nonebot_plugin_l4d2_server Description-
+Content-Type: text/markdown
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
  # nonebot_plugin_l4d2_server 0.5 _â¨Nonebot & Left 4 Dead 2 serveræä½â¨_
                 ææ¡£   Â·   æä»¤åè¡¨   Â·   å¸¸è§é®é¢
 
 [GitHub_stars] [GitHub_issues] [QQ_Chat_Group] [pypi] [pypi_download] [python]
                                    [NoneBot]
```

