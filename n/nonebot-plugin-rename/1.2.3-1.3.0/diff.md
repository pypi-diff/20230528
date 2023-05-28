# Comparing `tmp/nonebot_plugin_rename-1.2.3.tar.gz` & `tmp/nonebot_plugin_rename-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_rename-1.2.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_rename-1.3.0.tar", max compression
```

## Comparing `nonebot_plugin_rename-1.2.3.tar` & `nonebot_plugin_rename-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1066 2023-05-17 04:38:07.406701 nonebot_plugin_rename-1.2.3/LICENSE
--rw-r--r--   0        0        0     5230 2023-05-17 04:38:07.406701 nonebot_plugin_rename-1.2.3/README.md
--rw-r--r--   0        0        0      363 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/__init__.py
--rw-r--r--   0        0        0      293 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/__init__.py
--rw-r--r--   0        0        0      789 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/gaokao_time.py
--rw-r--r--   0        0        0     1020 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/genshin_time.py
--rw-r--r--   0        0        0      689 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/get_times.py
--rw-r--r--   0        0        0      925 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/hot_search.py
--rw-r--r--   0        0        0      408 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/message.py
--rw-r--r--   0        0        0      607 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/one_word.py
--rw-r--r--   0        0        0      893 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/starrail_time.py
--rw-r--r--   0        0        0      604 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/status.py
--rw-r--r--   0        0        0      338 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/config.py
--rw-r--r--   0        0        0     9234 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/main.py
--rw-r--r--   0        0        0      187 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/utils/__init__.py
--rw-r--r--   0        0        0      479 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/utils/card_choice.py
--rw-r--r--   0        0        0      838 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/utils/card_name.py
--rw-r--r--   0        0        0      643 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/utils/download.py
--rw-r--r--   0        0        0     1534 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/utils/draw.py
--rw-r--r--   0        0        0      423 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/utils/my_yaml.py
--rw-r--r--   0        0        0      663 2023-05-17 04:38:07.442701 nonebot_plugin_rename-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     6135 1970-01-01 00:00:00.000000 nonebot_plugin_rename-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-28 09:33:04.939643 nonebot_plugin_rename-1.3.0/LICENSE
+-rw-r--r--   0        0        0     5286 2023-05-28 09:33:04.939643 nonebot_plugin_rename-1.3.0/README.md
+-rw-r--r--   0        0        0      363 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/__init__.py
+-rw-r--r--   0        0        0      293 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/__init__.py
+-rw-r--r--   0        0        0      844 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/gaokao_time.py
+-rw-r--r--   0        0        0     1020 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/genshin_time.py
+-rw-r--r--   0        0        0      689 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/get_times.py
+-rw-r--r--   0        0        0      925 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/hot_search.py
+-rw-r--r--   0        0        0      408 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/message.py
+-rw-r--r--   0        0        0      607 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/one_word.py
+-rw-r--r--   0        0        0      893 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/starrail_time.py
+-rw-r--r--   0        0        0      604 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/status.py
+-rw-r--r--   0        0        0      376 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/config.py
+-rw-r--r--   0        0        0     9234 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/main.py
+-rw-r--r--   0        0        0      187 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/utils/__init__.py
+-rw-r--r--   0        0        0      479 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/utils/card_choice.py
+-rw-r--r--   0        0        0      838 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/utils/card_name.py
+-rw-r--r--   0        0        0     1096 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/utils/download.py
+-rw-r--r--   0        0        0     1534 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/utils/draw.py
+-rw-r--r--   0        0        0      423 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/utils/my_yaml.py
+-rw-r--r--   0        0        0      701 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6272 1970-01-01 00:00:00.000000 nonebot_plugin_rename-1.3.0/PKG-INFO
```

### Comparing `nonebot_plugin_rename-1.2.3/LICENSE` & `nonebot_plugin_rename-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.2.3/README.md` & `nonebot_plugin_rename-1.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -92,22 +92,23 @@
 **请注意不要将两个间隔时间都设为0!!!!!!**
 
 **由于qq群名片特殊性,间隔太短可能意义并不大反而容易导致风控,建议在30分钟以上**
 
 ## 🎉目前已实现的群名片功能
 <details>
 <summary>一图流</summary>
-<img src="https://cdn.staticaly.com/gh/forchannot/mypicgo@main/20230418/image.1l16rm6rtbkw.jpg" alt="help">
+<img src="https://cdn.staticaly.com/gh/forchannot/mypicgo@main/20230517/2b2b6734352a6ef94ff64cf1b7d8922d.5rr8s2fnai80.webp" alt="help">
 </details>
 
 <details>
 <summary>时间</summary>
 <pre>
 -- 高考时间
 -- 原神版本剩余时间
+-- 星铁版本剩余时间
 -- 北京时间
 -- 古代计时制时间
 </pre>
 </details>
 
 <details>
 <summary>热搜</summary>
```

#### html2text {}

```diff
@@ -34,14 +34,15 @@
 æ¯å¦åè®¸ä¸åä¸ªbotä¼è¯å¯ä»¥è®¾ç½®ææbotæå¨çç¾¤åç | bool |
 | is_show_aps_info_log | æ¯å¦æ¾ç¤ºå®æ¶ä»»å¡çinfoçº§å«æ¥å¿ | bool |
 **è¯·æ³¨æä¸è¦å°ä¸¤ä¸ªé´éæ¶é´é½è®¾ä¸º0!!!!!!**
 **ç±äºqqç¾¤åçç¹æ®æ§,é´éå¤ªç­å¯è½æä¹å¹¶ä¸å¤§åèå®¹æå¯¼è´é£æ§,å»ºè®®å¨30åéä»¥ä¸**
 ## ðç®åå·²å®ç°çç¾¤åçåè½  ä¸å¾æµ [help]   æ¶é´
 -- é«èæ¶é´
 -- åç¥çæ¬å©ä½æ¶é´
+-- æéçæ¬å©ä½æ¶é´
 -- åäº¬æ¶é´
 -- å¤ä»£è®¡æ¶å¶æ¶é´
   ç­æ
 -- Bç«ç­æ
 -- å¾®åç­æ
 -- æé³ç­æ
 -- ç¾åº¦ç­æ
```

### Comparing `nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/gaokao_time.py` & `nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/gaokao_time.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # Description: 获取高考倒计时
 
 from datetime import datetime
 
 
 def gk() -> str:
     # 基准时间
+    year = 2023
     baseTime = (
         datetime.strptime("2023-6-7 9:00:00", "%Y-%m-%d %H:%M:%S").timestamp() * 1000
     )
     nowTime = datetime.now().timestamp() * 1000
     # 获取持续时间
     duringTime = baseTime - nowTime
     while duringTime <= 0:
-        # 时间+365天
+        # 时间+365天 年份+1年
         duringTime += 365 * 24 * 60 * 60 * 1000
+        year += 1
     # 获取天数并取整
     days = int(duringTime / (24 * 3600 * 1000))
     leave1 = duringTime % (24 * 3600 * 1000)
     # 获取小时数并取整
     hours = int(leave1 / (3600 * 1000))
     leave2 = leave1 % (3600 * 1000)
     # 获取分钟数并取整
     minutes = int(leave2 / (60 * 1000))
-    return f"离高考还有{days}天{hours}小时{minutes}分钟"
+    return f"离{year}年高考还有{days}天{hours}小时{minutes}分钟"
```

### Comparing `nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/genshin_time.py` & `nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/genshin_time.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/get_times.py` & `nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/get_times.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/hot_search.py` & `nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/hot_search.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/one_word.py` & `nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/one_word.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/starrail_time.py` & `nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/starrail_time.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/status.py` & `nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/status.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/main.py` & `nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/utils/card_name.py` & `nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/utils/card_name.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/utils/draw.py` & `nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/utils/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.2.3/pyproject.toml` & `nonebot_plugin_rename-1.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-rename"
-version = "1.2.3"
+version = "1.3.0"
 description = "更改qq机器人的群名片，内置多种有趣名片"
 authors = ["forchannot <yy320206@gmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_rename"}]
 
 [[tool.poetry.source]]
@@ -17,12 +17,14 @@
 httpx = "^0.23.3"
 nonebot-adapter-onebot = "^2.2.2"
 nonebot-plugin-apscheduler = "^0.2.0"
 psutil = "^5.9.5"
 pyyaml = "^6.0"
 pillow = "^9.5.0"
 aiohttp = "^3.8.1"
+aiofiles = "^23.1.0"
+tqdm = "^4.65.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_rename-1.2.3/PKG-INFO` & `nonebot_plugin_rename-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-rename
-Version: 1.2.3
+Version: 1.3.0
 Summary: 更改qq机器人的群名片，内置多种有趣名片
 License: GPL-3.0
 Author: forchannot
 Author-email: yy320206@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.2,<3.0.0)
 Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0,<0.3.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://ghproxy.com/https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://ghproxy.com/https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
@@ -115,22 +117,23 @@
 **请注意不要将两个间隔时间都设为0!!!!!!**
 
 **由于qq群名片特殊性,间隔太短可能意义并不大反而容易导致风控,建议在30分钟以上**
 
 ## 🎉目前已实现的群名片功能
 <details>
 <summary>一图流</summary>
-<img src="https://cdn.staticaly.com/gh/forchannot/mypicgo@main/20230418/image.1l16rm6rtbkw.jpg" alt="help">
+<img src="https://cdn.staticaly.com/gh/forchannot/mypicgo@main/20230517/2b2b6734352a6ef94ff64cf1b7d8922d.5rr8s2fnai80.webp" alt="help">
 </details>
 
 <details>
 <summary>时间</summary>
 <pre>
 -- 高考时间
 -- 原神版本剩余时间
+-- 星铁版本剩余时间
 -- 北京时间
 -- 古代计时制时间
 </pre>
 </details>
 
 <details>
 <summary>热搜</summary>
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-rename Version: 1.2.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-rename Version: 1.3.0 Summary:
 æ´æ¹qqæºå¨äººçç¾¤åçï¼åç½®å¤ç§æè¶£åç License: GPL-3.0
 Author: forchannot Author-email: yy320206@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: aiohttp (>=3.8.1,<4.0.0) Requires-
-Dist: httpx (>=0.23.3,<0.24.0) Requires-Dist: nonebot-adapter-onebot
-(>=2.2.2,<3.0.0) Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0,<0.3.0)
-Requires-Dist: pillow (>=9.5.0,<10.0.0) Requires-Dist: psutil (>=5.9.5,<6.0.0)
-Requires-Dist: pyyaml (>=6.0,<7.0) Description-Content-Type: text/markdown
+Language :: Python :: 3.11 Requires-Dist: aiofiles (>=23.1.0,<24.0.0) Requires-
+Dist: aiohttp (>=3.8.1,<4.0.0) Requires-Dist: httpx (>=0.23.3,<0.24.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.2.2,<3.0.0) Requires-Dist: nonebot-
+plugin-apscheduler (>=0.2.0,<0.3.0) Requires-Dist: pillow (>=9.5.0,<10.0.0)
+Requires-Dist: psutil (>=5.9.5,<6.0.0) Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0) Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                          # nonebot-plugin-rename _â¨
 éè¿å®æ¶ä»»å¡æ´æ¹botæå¨ç¾¤èªå·±çç¾¤åç,åç½®äºå ç§å¸¸è§çç¾¤åçå¹¶ä¸åæ­¥æ¯æäºå¤bot,æ¬¢è¿**pr**æ°çç¾¤åç!
                         â¨_ [license] [pypi] [python]
  * [nonebot-plugin-rename](#nonebot-plugin-rename) * [ðç®ä»](#ç®ä») *
 [ðè®¸å¯](#è®¸å¯) * [ð¿ å®è£æ¹æ³](#-å®è£æ¹æ³) *
@@ -46,14 +47,15 @@
 æ¯å¦åè®¸ä¸åä¸ªbotä¼è¯å¯ä»¥è®¾ç½®ææbotæå¨çç¾¤åç | bool |
 | is_show_aps_info_log | æ¯å¦æ¾ç¤ºå®æ¶ä»»å¡çinfoçº§å«æ¥å¿ | bool |
 **è¯·æ³¨æä¸è¦å°ä¸¤ä¸ªé´éæ¶é´é½è®¾ä¸º0!!!!!!**
 **ç±äºqqç¾¤åçç¹æ®æ§,é´éå¤ªç­å¯è½æä¹å¹¶ä¸å¤§åèå®¹æå¯¼è´é£æ§,å»ºè®®å¨30åéä»¥ä¸**
 ## ðç®åå·²å®ç°çç¾¤åçåè½  ä¸å¾æµ [help]   æ¶é´
 -- é«èæ¶é´
 -- åç¥çæ¬å©ä½æ¶é´
+-- æéçæ¬å©ä½æ¶é´
 -- åäº¬æ¶é´
 -- å¤ä»£è®¡æ¶å¶æ¶é´
   ç­æ
 -- Bç«ç­æ
 -- å¾®åç­æ
 -- æé³ç­æ
 -- ç¾åº¦ç­æ
```

