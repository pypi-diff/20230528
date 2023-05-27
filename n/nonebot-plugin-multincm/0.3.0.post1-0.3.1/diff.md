# Comparing `tmp/nonebot_plugin_multincm-0.3.0.post1.tar.gz` & `tmp/nonebot_plugin_multincm-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_multincm-0.3.0.post1.tar", last modified: Thu May 18 20:22:33 2023, max compression
+gzip compressed data, was "nonebot_plugin_multincm-0.3.1.tar", last modified: Sat May 27 22:18:39 2023, max compression
```

## Comparing `nonebot_plugin_multincm-0.3.0.post1.tar` & `nonebot_plugin_multincm-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1069 2023-05-18 20:22:20.169310 nonebot_plugin_multincm-0.3.0.post1/LICENSE
--rw-r--r--   0        0        0     7087 2023-05-18 20:22:20.169310 nonebot_plugin_multincm-0.3.0.post1/README.md
--rw-r--r--   0        0        0     1652 2023-05-18 20:22:20.169310 nonebot_plugin_multincm-0.3.0.post1/nonebot_plugin_multincm/__init__.py
--rw-r--r--   0        0        0    11595 2023-05-18 20:22:20.169310 nonebot_plugin_multincm-0.3.0.post1/nonebot_plugin_multincm/__main__.py
--rw-r--r--   0        0        0      512 2023-05-18 20:22:20.169310 nonebot_plugin_multincm-0.3.0.post1/nonebot_plugin_multincm/config.py
--rw-r--r--   0        0        0      134 2023-05-18 20:22:20.169310 nonebot_plugin_multincm-0.3.0.post1/nonebot_plugin_multincm/const.py
--rw-r--r--   0        0        0     5500 2023-05-18 20:22:20.169310 nonebot_plugin_multincm-0.3.0.post1/nonebot_plugin_multincm/data_source.py
--rw-r--r--   0        0        0    11617 2023-05-18 20:22:20.169310 nonebot_plugin_multincm-0.3.0.post1/nonebot_plugin_multincm/draw.py
--rw-r--r--   0        0        0     2957 2023-05-18 20:22:20.169310 nonebot_plugin_multincm-0.3.0.post1/nonebot_plugin_multincm/lrc_parser.py
--rw-r--r--   0        0        0     2228 2023-05-18 20:22:20.169310 nonebot_plugin_multincm-0.3.0.post1/nonebot_plugin_multincm/msg_cache.py
--rw-r--r--   0        0        0   212591 2023-05-18 20:22:20.173310 nonebot_plugin_multincm-0.3.0.post1/nonebot_plugin_multincm/res/bg.jpg
--rw-r--r--   0        0        0     2997 2023-05-18 20:22:20.181310 nonebot_plugin_multincm-0.3.0.post1/nonebot_plugin_multincm/types.py
--rw-r--r--   0        0        0      851 2023-05-18 20:22:20.181310 nonebot_plugin_multincm-0.3.0.post1/nonebot_plugin_multincm/utils.py
--rw-r--r--   0        0        0      873 2023-05-18 20:22:33.749376 nonebot_plugin_multincm-0.3.0.post1/pyproject.toml
--rw-r--r--   0        0        0     8043 1970-01-01 00:00:00.000000 nonebot_plugin_multincm-0.3.0.post1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-27 22:18:17.113726 nonebot_plugin_multincm-0.3.1/LICENSE
+-rw-r--r--   0        0        0     7380 2023-05-27 22:18:17.113726 nonebot_plugin_multincm-0.3.1/README.md
+-rw-r--r--   0        0        0     1646 2023-05-27 22:18:17.113726 nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/__init__.py
+-rw-r--r--   0        0        0    11552 2023-05-27 22:18:17.113726 nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/__main__.py
+-rw-r--r--   0        0        0      512 2023-05-27 22:18:17.113726 nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/config.py
+-rw-r--r--   0        0        0      134 2023-05-27 22:18:17.113726 nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/const.py
+-rw-r--r--   0        0        0     5500 2023-05-27 22:18:17.113726 nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/data_source.py
+-rw-r--r--   0        0        0    11669 2023-05-27 22:18:17.113726 nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/draw.py
+-rw-r--r--   0        0        0     2957 2023-05-27 22:18:17.113726 nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/lrc_parser.py
+-rw-r--r--   0        0        0     2228 2023-05-27 22:18:17.113726 nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/msg_cache.py
+-rw-r--r--   0        0        0   212591 2023-05-27 22:18:17.117726 nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/res/bg.jpg
+-rw-r--r--   0        0        0     3007 2023-05-27 22:18:17.117726 nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/types.py
+-rw-r--r--   0        0        0      851 2023-05-27 22:18:17.117726 nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/utils.py
+-rw-r--r--   0        0        0      867 2023-05-27 22:18:39.233830 nonebot_plugin_multincm-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     8330 1970-01-01 00:00:00.000000 nonebot_plugin_multincm-0.3.1/PKG-INFO
```

### Comparing `nonebot_plugin_multincm-0.3.0.post1/LICENSE` & `nonebot_plugin_multincm-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.0.post1/README.md` & `nonebot_plugin_multincm-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -167,14 +167,20 @@
   - 别名：`link`、`url`
 
 ### Tip
 
 - 点击 Bot 发送的音乐卡片会跳转到音乐直链，可以直接下载
 - 使用需要回复音乐卡片的指令时，如果没有回复，会自动使用你触发发送的最近一个音乐卡片的信息
 
+## 🤔 Q & A
+
+### Q: 我可以把插件变成单选点歌吗？
+
+A: 可以，把配置项 `NCM_LIST_LIMIT` 设置为 `1` 即可。因为插件在检测到搜索结果仅有一个时，会将它直接发送出来。我们在这里利用了这个特性。
+
 ## 📞 联系
 
 QQ：3076823485  
 Telegram：[@lgc2333](https://t.me/lgc2333)  
 吹水群：[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp)  
 邮箱：<lgc2333@126.com>
 
@@ -202,14 +208,18 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.3.1
+
+- 修复电台相关 bug
+
 ### 0.3.0
 
 - 支持电台节目的解析与点播
 
 ### 0.2.5
 
 - `解析`、`歌词`、`链接` 指令可以直接根据 Bot 发送的上个音乐卡片作出回应了
```

#### html2text {}

```diff
@@ -53,26 +53,30 @@
 å«åï¼`resolve`ã`parse`ã`get` - æ­è¯ [åå¤ é³ä¹å¡ç / é¾æ¥] -
 ä»ç»ï¼è·åè¯¥é³ä¹çæ­è¯ï¼ä»¥å¾çå½¢å¼åé -
 å«åï¼`lrc`ã`lyric`ã`lyrics` - é¾æ¥ [åå¤ é³ä¹å¡ç] -
 ä»ç»ï¼è·å Bot åéçé³ä¹å¡ççç½æäºé¾æ¥ -
 å«åï¼`link`ã`url` ### Tip - ç¹å» Bot
 åéçé³ä¹å¡çä¼è·³è½¬å°é³ä¹ç´é¾ï¼å¯ä»¥ç´æ¥ä¸è½½ -
 ä½¿ç¨éè¦åå¤é³ä¹å¡ççæä»¤æ¶ï¼å¦ææ²¡æåå¤ï¼ä¼èªå¨ä½¿ç¨ä½ è§¦ååéçæè¿ä¸ä¸ªé³ä¹å¡ççä¿¡æ¯
+## ð¤ Q & A ### Q: æå¯ä»¥ææä»¶åæåéç¹æ­åï¼ A:
+å¯ä»¥ï¼æéç½®é¡¹ `NCM_LIST_LIMIT` è®¾ç½®ä¸º `1`
+å³å¯ãå ä¸ºæä»¶å¨æ£æµå°æç´¢ç»æä»æä¸ä¸ªæ¶ï¼ä¼å°å®ç´æ¥åéåºæ¥ãæä»¬å¨è¿éå©ç¨äºè¿ä¸ªç¹æ§ã
 ## ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333)
 å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [mos9527/pyncm](https://github.com/mos9527/pyncm)
 é¡¹ç®ä½¿ç¨çç½æäº API è°ç¨åº ### [Binaryify/NeteaseCloudMusicApi]
 (https://github.com/Binaryify/NeteaseCloudMusicApi) é¡¹ç®çµå°ç¸å³ API
 æ¥æº ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-utils) è¶å¥½ç¨ç
 Pillow è¾å©åº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.0 -
-æ¯æçµå°èç®çè§£æä¸ç¹æ­ ### 0.2.5 - `è§£æ`ã`æ­è¯`ã`é¾æ¥`
-æä»¤å¯ä»¥ç´æ¥æ ¹æ® Bot åéçä¸ä¸ªé³ä¹å¡çä½åºååºäº -
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.1 - ä¿®å¤çµå°ç¸å³ bug ###
+0.3.0 - æ¯æçµå°èç®çè§£æä¸ç¹æ­ ### 0.2.5 -
+`è§£æ`ã`æ­è¯`ã`é¾æ¥` æä»¤å¯ä»¥ç´æ¥æ ¹æ® Bot
+åéçä¸ä¸ªé³ä¹å¡çä½åºååºäº -
 æ­è¯è§£æä¼åå¹¶å¤è¡ç©ºè¡åå»æé¦å°¾ç©ºè¡äº -
 ç°å¨æä»¶ä¼å®æ¶æ¸çèªèº«åå­ä¸­çç¼å­äº ### 0.2.4 -
 ä¿®å¤ä¸ä¸ªæ­è¯è§£æ bug ### 0.2.3 - å¾®è°æ­æ²åè¡¨æç -
 å¾®è°æä»¶å¸®å©ææ¬ ### 0.2.2 - ä¿®å¤ææ­ `KeyError` ### 0.2.1 -
 å é¤æ­è¯å°¾é¨çç©ºè¡ä¸å¤ä½åå²çº¿ ### 0.2.0 - æ°å¢äºä¸ä¸ªæä»¤
 `è§£æ`ã`æ­è¯`ã`é¾æ¥` - ç¹æ­æä»¤æ¯æç´æ¥è¾å¥é³ä¹ ID
```

### Comparing `nonebot_plugin_multincm-0.3.0.post1/nonebot_plugin_multincm/__init__.py` & `nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from nonebot.plugin import PluginMetadata, require
 
 require("nonebot_plugin_apscheduler")
 
 from . import __main__ as __main__  # noqa: E402
 from .config import ConfigModel  # noqa: E402
 
-__version__ = "0.3.0.post1"
+__version__ = "0.3.1"
 __plugin_meta__ = PluginMetadata(
     "MultiNCM",
     "网易云多选点歌",
     (
         "指令列表：\n"
         "▶ 点歌 [歌曲名 / 音乐 ID]\n"
         "    ▷ 介绍：搜索歌曲。当输入音乐 ID 时会直接发送对应音乐\n"
```

### Comparing `nonebot_plugin_multincm-0.3.0.post1/nonebot_plugin_multincm/__main__.py` & `nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,15 +189,15 @@
     index = ori_index % config.ncm_list_limit
 
     res = cache.get(page_index)
     if not (res):
         return None
 
     results = res.songs if isinstance(res, SongSearchResult) else res.resources
-    if not (0 <= index < len(results)):
+    if (not results) or (not (0 <= index < len(results))):
         return None
 
     got = results[index]
     if isinstance(got, VoiceResource):
         return got.baseInfo
     return got
 
@@ -213,28 +213,27 @@
     calling = CALLING_MAP[song_type]
 
     if not (res := cache.get(page)):
         try:
             func = search_song if song_type == "song" else search_voice
             res = await func(param, page=page)
         except:
-            logger.exception("搜索歌曲失败")
-            await matcher.finish("搜索歌曲失败，请检查后台输出")
-
-        if not (res.songCount if isinstance(res, SongSearchResult) else res.totalCount):
-            await matcher.finish("没搜到任何歌曲捏")
+            logger.exception(f"搜索{calling}失败")
+            await matcher.finish(f"搜索{calling}失败，请检查后台输出")
 
     is_song = isinstance(res, SongSearchResult)
     total_count = res.songCount if is_song else res.totalCount
+    results = res.songs if is_song else res.resources
+    if not results:
+        await matcher.finish(f"没搜到任何{calling}捏")
 
     state["page"] = page
     cache[page] = res
     state["page_max"] = ceil(total_count / config.ncm_list_limit)
 
-    results = res.songs if is_song else res.resources
     if page == 1 and len(results) == 1:
         await get_cache_by_index(cache, 1)
 
     try:
         pic = draw_search_res(res, page)
     except:
         logger.exception(f"绘制{calling}列表失败")
```

### Comparing `nonebot_plugin_multincm-0.3.0.post1/nonebot_plugin_multincm/config.py` & `nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.0.post1/nonebot_plugin_multincm/data_source.py` & `nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.0.post1/nonebot_plugin_multincm/draw.py` & `nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/draw.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,14 +222,17 @@
     )
 
 
 def get_voice_search_res_table(
     res: VoiceSearchResult,
     index_offset: int = 0,
 ) -> Tuple[List[TableHead], List[List[str]]]:
+    if not res.resources:
+        raise ValueError
+
     return (
         [
             TableHead("序号", align="right"),
             TableHead("节目", max_width=config.ncm_max_name_len),
             TableHead("电台", max_width=config.ncm_max_name_len),
             TableHead("台主", max_width=config.ncm_max_artist_len),
             TableHead("时长", align="center"),
```

### Comparing `nonebot_plugin_multincm-0.3.0.post1/nonebot_plugin_multincm/lrc_parser.py` & `nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/lrc_parser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.0.post1/nonebot_plugin_multincm/msg_cache.py` & `nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/msg_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.0.post1/nonebot_plugin_multincm/res/bg.jpg` & `nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/res/bg.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.0.post1/nonebot_plugin_multincm/types.py` & `nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,10 +129,10 @@
 
 
 class VoiceResource(BaseModel):
     baseInfo: VoiceBaseInfo  # noqa: N815
 
 
 class VoiceSearchResult(BaseModel):
-    resources: List[VoiceResource]
+    resources: Optional[List[VoiceResource]]
     totalCount: int  # noqa: N815
     searchQcReminder: Optional[SearchQcReminder]  # noqa: N815
```

### Comparing `nonebot_plugin_multincm-0.3.0.post1/nonebot_plugin_multincm/utils.py` & `nonebot_plugin_multincm-0.3.1/nonebot_plugin_multincm/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.0.post1/pyproject.toml` & `nonebot_plugin_multincm-0.3.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-multincm"
-version = "0.3.0.post1"
+version = "0.3.1"
 description = "NCM Song Searcher"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0-rc.1",
     "nonebot-adapter-onebot>=2.2.0",
```

### Comparing `nonebot_plugin_multincm-0.3.0.post1/PKG-INFO` & `nonebot_plugin_multincm-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-multincm
-Version: 0.3.0.post1
+Version: 0.3.1
 Summary: NCM Song Searcher
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Requires-Python: <4.0,>=3.8
 Requires-Dist: nonebot2>=2.0.0-rc.1
@@ -193,14 +193,20 @@
   - 别名：`link`、`url`
 
 ### Tip
 
 - 点击 Bot 发送的音乐卡片会跳转到音乐直链，可以直接下载
 - 使用需要回复音乐卡片的指令时，如果没有回复，会自动使用你触发发送的最近一个音乐卡片的信息
 
+## 🤔 Q & A
+
+### Q: 我可以把插件变成单选点歌吗？
+
+A: 可以，把配置项 `NCM_LIST_LIMIT` 设置为 `1` 即可。因为插件在检测到搜索结果仅有一个时，会将它直接发送出来。我们在这里利用了这个特性。
+
 ## 📞 联系
 
 QQ：3076823485  
 Telegram：[@lgc2333](https://t.me/lgc2333)  
 吹水群：[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp)  
 邮箱：<lgc2333@126.com>
 
@@ -228,14 +234,18 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.3.1
+
+- 修复电台相关 bug
+
 ### 0.3.0
 
 - 支持电台节目的解析与点播
 
 ### 0.2.5
 
 - `解析`、`歌词`、`链接` 指令可以直接根据 Bot 发送的上个音乐卡片作出回应了
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-multincm Version: 0.3.0.post1
-Summary: NCM Song Searcher Home-page: https://github.com/lgc-NB2Dev/nonebot-
-plugin-multincm Author-Email: student_2333
+Metadata-Version: 2.1 Name: nonebot-plugin-multincm Version: 0.3.1 Summary: NCM
+Song Searcher Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
+Author-Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-multincm Requires-Python: <4.0,>=3.8 Requires-Dist:
 nonebot2>=2.0.0-rc.1 Requires-Dist: nonebot-adapter-onebot>=2.2.0 Requires-
 Dist: pydantic>=1.10.4 Requires-Dist: pil-utils>=0.1.7 Requires-Dist:
 pyncm>=1.6.8.9.1 Requires-Dist: typing-extensions>=4.5.0 Requires-Dist:
 anyio>=3.6.2 Requires-Dist: nonebot-plugin-apscheduler>=0.2.0 Requires-Dist:
 pip>=23.0.1; extra == "dev" Requires-Dist: setuptools>=67.6.1; extra == "dev"
@@ -67,26 +67,30 @@
 å«åï¼`resolve`ã`parse`ã`get` - æ­è¯ [åå¤ é³ä¹å¡ç / é¾æ¥] -
 ä»ç»ï¼è·åè¯¥é³ä¹çæ­è¯ï¼ä»¥å¾çå½¢å¼åé -
 å«åï¼`lrc`ã`lyric`ã`lyrics` - é¾æ¥ [åå¤ é³ä¹å¡ç] -
 ä»ç»ï¼è·å Bot åéçé³ä¹å¡ççç½æäºé¾æ¥ -
 å«åï¼`link`ã`url` ### Tip - ç¹å» Bot
 åéçé³ä¹å¡çä¼è·³è½¬å°é³ä¹ç´é¾ï¼å¯ä»¥ç´æ¥ä¸è½½ -
 ä½¿ç¨éè¦åå¤é³ä¹å¡ççæä»¤æ¶ï¼å¦ææ²¡æåå¤ï¼ä¼èªå¨ä½¿ç¨ä½ è§¦ååéçæè¿ä¸ä¸ªé³ä¹å¡ççä¿¡æ¯
+## ð¤ Q & A ### Q: æå¯ä»¥ææä»¶åæåéç¹æ­åï¼ A:
+å¯ä»¥ï¼æéç½®é¡¹ `NCM_LIST_LIMIT` è®¾ç½®ä¸º `1`
+å³å¯ãå ä¸ºæä»¶å¨æ£æµå°æç´¢ç»æä»æä¸ä¸ªæ¶ï¼ä¼å°å®ç´æ¥åéåºæ¥ãæä»¬å¨è¿éå©ç¨äºè¿ä¸ªç¹æ§ã
 ## ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333)
 å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [mos9527/pyncm](https://github.com/mos9527/pyncm)
 é¡¹ç®ä½¿ç¨çç½æäº API è°ç¨åº ### [Binaryify/NeteaseCloudMusicApi]
 (https://github.com/Binaryify/NeteaseCloudMusicApi) é¡¹ç®çµå°ç¸å³ API
 æ¥æº ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-utils) è¶å¥½ç¨ç
 Pillow è¾å©åº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.0 -
-æ¯æçµå°èç®çè§£æä¸ç¹æ­ ### 0.2.5 - `è§£æ`ã`æ­è¯`ã`é¾æ¥`
-æä»¤å¯ä»¥ç´æ¥æ ¹æ® Bot åéçä¸ä¸ªé³ä¹å¡çä½åºååºäº -
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.1 - ä¿®å¤çµå°ç¸å³ bug ###
+0.3.0 - æ¯æçµå°èç®çè§£æä¸ç¹æ­ ### 0.2.5 -
+`è§£æ`ã`æ­è¯`ã`é¾æ¥` æä»¤å¯ä»¥ç´æ¥æ ¹æ® Bot
+åéçä¸ä¸ªé³ä¹å¡çä½åºååºäº -
 æ­è¯è§£æä¼åå¹¶å¤è¡ç©ºè¡åå»æé¦å°¾ç©ºè¡äº -
 ç°å¨æä»¶ä¼å®æ¶æ¸çèªèº«åå­ä¸­çç¼å­äº ### 0.2.4 -
 ä¿®å¤ä¸ä¸ªæ­è¯è§£æ bug ### 0.2.3 - å¾®è°æ­æ²åè¡¨æç -
 å¾®è°æä»¶å¸®å©ææ¬ ### 0.2.2 - ä¿®å¤ææ­ `KeyError` ### 0.2.1 -
 å é¤æ­è¯å°¾é¨çç©ºè¡ä¸å¤ä½åå²çº¿ ### 0.2.0 - æ°å¢äºä¸ä¸ªæä»¤
 `è§£æ`ã`æ­è¯`ã`é¾æ¥` - ç¹æ­æä»¤æ¯æç´æ¥è¾å¥é³ä¹ ID
```

