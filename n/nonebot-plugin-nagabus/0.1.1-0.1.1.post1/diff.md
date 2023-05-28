# Comparing `tmp/nonebot_plugin_nagabus-0.1.1.tar.gz` & `tmp/nonebot_plugin_nagabus-0.1.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nagabus-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_nagabus-0.1.1.post1.tar", max compression
```

## Comparing `nonebot_plugin_nagabus-0.1.1.tar` & `nonebot_plugin_nagabus-0.1.1.post1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448000 nonebot_plugin_nagabus-0.1.1/LICENSE
--rw-r--r--   0        0        0     1031 2023-05-27 04:29:09.853194 nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/__init__.py
--rw-r--r--   0        0        0      129 2023-05-27 04:29:09.849196 nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/ac.py
--rw-r--r--   0        0        0     1163 2023-05-28 03:25:19.174130 nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/config.py
--rw-r--r--   0        0        0        4 2023-05-26 13:11:24.775555 nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/data/__init__.py
--rw-r--r--   0        0        0      116 2023-05-26 11:41:42.946553 nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/data/base.py
--rw-r--r--   0        0        0      317 2023-05-26 11:41:42.956553 nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/data/mjs.py
--rw-r--r--   0        0        0     1697 2023-05-27 07:16:52.720509 nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/data/naga.py
--rw-r--r--   0        0        0      775 2023-05-26 11:41:42.960551 nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/data/session.py
--rw-r--r--   0        0        0      713 2023-05-26 15:21:27.421204 nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/data/utils/__init__.py
--rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843000 nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/data/utils/utc_datetime.py
--rw-r--r--   0        0        0       95 2023-05-28 01:19:53.575323 nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/matchers/__init__.py
--rw-r--r--   0        0        0     2130 2023-05-28 01:19:53.557320 nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/matchers/errors.py
--rw-r--r--   0        0        0     5435 2023-05-28 01:19:53.569323 nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/matchers/naga_analyze.py
--rw-r--r--   0        0        0     2462 2023-05-28 01:19:53.563321 nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/matchers/naga_statistic.py
--rw-r--r--   0        0        0     2278 2023-05-27 02:48:33.707764 nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/migrations/24aec3c56623_.py
--rw-r--r--   0        0        0     1350 2023-05-27 07:17:07.623159 nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py
--rw-r--r--   0        0        0     1009 2023-05-26 15:21:27.440185 nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/mjs/__init__.py
--rw-r--r--   0        0        0      176 2023-05-25 15:39:25.419279 nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/naga/__init__.py
--rw-r--r--   0        0        0     3758 2023-05-27 13:45:54.389899 nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/naga/api.py
--rw-r--r--   0        0        0     3002 2023-05-27 02:36:44.852322 nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/naga/fake_api.py
--rw-r--r--   0        0        0     1066 2023-05-27 02:48:01.485010 nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/naga/model.py
--rw-r--r--   0        0        0    17472 2023-05-28 01:09:03.118081 nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/naga/service.py
--rw-r--r--   0        0        0        0 2023-05-25 16:04:02.955709 nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/utils/__init__.py
--rw-r--r--   0        0        0     1092 2023-05-25 16:06:56.701500 nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/utils/integer.py
--rw-r--r--   0        0        0        0 2023-05-26 12:48:40.974521 nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/utils/mapping.py
--rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247000 nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/utils/nonebot.py
--rw-r--r--   0        0        0       68 2023-05-26 15:50:47.559077 nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/utils/tz.py
--rw-r--r--   0        0        0      677 2023-05-28 03:26:07.996029 nonebot_plugin_nagabus-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1722 2023-05-27 05:59:01.771686 nonebot_plugin_nagabus-0.1.1/README.md
--rw-r--r--   0        0        0     2529 1970-01-01 00:00:00.000000 nonebot_plugin_nagabus-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448000 nonebot_plugin_nagabus-0.1.1.post1/LICENSE
+-rw-r--r--   0        0        0     1218 2023-05-28 04:13:44.176141 nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/__init__.py
+-rw-r--r--   0        0        0      129 2023-05-27 04:29:09.849196 nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/ac.py
+-rw-r--r--   0        0        0     1163 2023-05-28 03:26:24.392144 nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/config.py
+-rw-r--r--   0        0        0        4 2023-05-26 13:11:24.775555 nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/data/__init__.py
+-rw-r--r--   0        0        0      116 2023-05-26 11:41:42.946553 nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/data/base.py
+-rw-r--r--   0        0        0      317 2023-05-26 11:41:42.956553 nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/data/mjs.py
+-rw-r--r--   0        0        0     1697 2023-05-27 07:16:52.720509 nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/data/naga.py
+-rw-r--r--   0        0        0      775 2023-05-26 11:41:42.960551 nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/data/session.py
+-rw-r--r--   0        0        0      713 2023-05-26 15:21:27.421204 nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/data/utils/__init__.py
+-rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843000 nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/data/utils/utc_datetime.py
+-rw-r--r--   0        0        0       95 2023-05-28 01:19:53.575323 nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/matchers/__init__.py
+-rw-r--r--   0        0        0     2130 2023-05-28 01:19:53.557320 nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/matchers/errors.py
+-rw-r--r--   0        0        0     5435 2023-05-28 01:19:53.569323 nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/matchers/naga_analyze.py
+-rw-r--r--   0        0        0     2462 2023-05-28 01:19:53.563321 nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/matchers/naga_statistic.py
+-rw-r--r--   0        0        0     2278 2023-05-27 02:48:33.707764 nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/migrations/24aec3c56623_.py
+-rw-r--r--   0        0        0     1350 2023-05-27 07:17:07.623159 nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py
+-rw-r--r--   0        0        0     1009 2023-05-26 15:21:27.440185 nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/mjs/__init__.py
+-rw-r--r--   0        0        0      176 2023-05-25 15:39:25.419279 nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/naga/__init__.py
+-rw-r--r--   0        0        0     3758 2023-05-27 13:45:54.389899 nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/naga/api.py
+-rw-r--r--   0        0        0     3002 2023-05-27 02:36:44.852322 nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/naga/fake_api.py
+-rw-r--r--   0        0        0     1066 2023-05-27 02:48:01.485010 nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/naga/model.py
+-rw-r--r--   0        0        0    17472 2023-05-28 01:09:03.118081 nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/naga/service.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:04:02.955709 nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/utils/__init__.py
+-rw-r--r--   0        0        0     1092 2023-05-25 16:06:56.701500 nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/utils/integer.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:48:40.974521 nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/utils/mapping.py
+-rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247000 nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/utils/nonebot.py
+-rw-r--r--   0        0        0       68 2023-05-26 15:50:47.559077 nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/utils/tz.py
+-rw-r--r--   0        0        0      683 2023-05-28 04:14:35.468051 nonebot_plugin_nagabus-0.1.1.post1/pyproject.toml
+-rw-r--r--   0        0        0     1789 2023-05-28 03:26:24.309853 nonebot_plugin_nagabus-0.1.1.post1/README.md
+-rw-r--r--   0        0        0     2598 1970-01-01 00:00:00.000000 nonebot_plugin_nagabus-0.1.1.post1/PKG-INFO
```

### Comparing `nonebot_plugin_nagabus-0.1.1/LICENSE` & `nonebot_plugin_nagabus-0.1.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/__init__.py` & `nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 """
 nonebot-plugin-nagabus
 
 @Author         : ssttkkl
 @License        : AGPLv3
 @GitHub         : https://github.com/ssttkkl/nonebot-plugin-nagabus
 """
+from nonebot import logger
 
-from nonebot import require
+try:
+    from nonebot import require
 
-from .utils.nonebot import default_cmd_start
+    from .utils.nonebot import default_cmd_start
 
-require("nonebot_plugin_access_control")
-require("nonebot_plugin_majsoul")
-require("nonebot_plugin_datastore")
-
-from . import matchers
-
-help_text = f"""
-牌谱分析：
-{default_cmd_start}naga <雀魂牌谱链接> <东/南x局x本场>：消耗10NP解析雀魂小局
-{default_cmd_start}naga <天凤牌谱链接>：消耗50NP解析天凤半庄
-
-使用情况：
-{default_cmd_start}naga本月使用情况
-{default_cmd_start}naga上月使用情况
-
-以上命令格式中，以<>包裹的表示一个参数。
-
-详细说明：参见https://github.com/ssttkkl/nonebot-plugin-nagabus
-""".strip()
-
-from nonebot.plugin import PluginMetadata
-
-__plugin_meta__ = PluginMetadata(
-    name='NAGA公交车',
-    description='为群友提供NAGA拼车服务',
-    usage=help_text
-)
+    require("nonebot_plugin_access_control")
+    require("nonebot_plugin_majsoul")
+    require("nonebot_plugin_datastore")
+
+    from . import matchers
+
+    help_text = f"""
+    牌谱分析：
+    {default_cmd_start}naga <雀魂牌谱链接> <东/南x局x本场>：消耗10NP解析雀魂小局
+    {default_cmd_start}naga <天凤牌谱链接>：消耗50NP解析天凤半庄
+    
+    使用情况：
+    {default_cmd_start}naga本月使用情况
+    {default_cmd_start}naga上月使用情况
+    
+    以上命令格式中，以<>包裹的表示一个参数。
+    
+    详细说明：参见https://github.com/ssttkkl/nonebot-plugin-nagabus
+    """.strip()
+
+    from nonebot.plugin import PluginMetadata
+
+    __plugin_meta__ = PluginMetadata(
+        name='NAGA公交车',
+        description='为群友提供NAGA拼车服务',
+        usage=help_text
+    )
+except BaseException as e:
+    logger.exception(e)
```

### Comparing `nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/config.py` & `nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/data/naga.py` & `nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/data/naga.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/data/session.py` & `nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/data/session.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/data/utils/__init__.py` & `nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/data/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/data/utils/utc_datetime.py` & `nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/data/utils/utc_datetime.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/matchers/errors.py` & `nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/matchers/errors.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/matchers/naga_analyze.py` & `nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/matchers/naga_analyze.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/matchers/naga_statistic.py` & `nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/matchers/naga_statistic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/migrations/24aec3c56623_.py` & `nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/migrations/24aec3c56623_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py` & `nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/mjs/__init__.py` & `nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/mjs/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/naga/api.py` & `nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/naga/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/naga/fake_api.py` & `nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/naga/fake_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/naga/model.py` & `nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/naga/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/naga/service.py` & `nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/naga/service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.1/nonebot_plugin_nagabus/utils/integer.py` & `nonebot_plugin_nagabus-0.1.1.post1/nonebot_plugin_nagabus/utils/integer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.1/pyproject.toml` & `nonebot_plugin_nagabus-0.1.1.post1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-nagabus"
-version = "0.1.1"
+version = "0.1.1.post1"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_nagabus" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `nonebot_plugin_nagabus-0.1.1/README.md` & `nonebot_plugin_nagabus-0.1.1.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -45,7 +45,11 @@
     - `/naga <雀魂牌谱链接> <东/南x局x本场>`：消耗10NP解析雀魂小局
     - `/naga <天凤牌谱链接>`：消耗50NP解析天凤半庄
 - 查看使用情况：
     - `/naga本月使用情况`
     - `/naga上月使用情况`
 
 以上命令格式中，以<>包裹的表示一个参数。
+
+## Special Thanks
+
+- https://github.com/Diving-Fish/auto-naga
```

### Comparing `nonebot_plugin_nagabus-0.1.1/PKG-INFO` & `nonebot_plugin_nagabus-0.1.1.post1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nagabus
-Version: 0.1.1
+Version: 0.1.1.post1
 Summary: 
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -68,7 +68,11 @@
     - `/naga <天凤牌谱链接>`：消耗50NP解析天凤半庄
 - 查看使用情况：
     - `/naga本月使用情况`
     - `/naga上月使用情况`
 
 以上命令格式中，以<>包裹的表示一个参数。
 
+## Special Thanks
+
+- https://github.com/Diving-Fish/auto-naga
+
```

