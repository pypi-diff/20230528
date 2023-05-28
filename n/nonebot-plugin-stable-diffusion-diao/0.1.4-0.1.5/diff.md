# Comparing `tmp/nonebot_plugin_stable_diffusion_diao-0.1.4.tar.gz` & `tmp/nonebot_plugin_stable_diffusion_diao-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.1.4.tar", last modified: Sun May 28 11:36:41 2023, max compression
+gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.1.5.tar", last modified: Sun May 28 22:09:39 2023, max compression
```

## Comparing `nonebot_plugin_stable_diffusion_diao-0.1.4.tar` & `nonebot_plugin_stable_diffusion_diao-0.1.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.1.4/LICENSE
--rw-r--r--   0        0        0      686 2023-05-28 09:58:15.400842 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/__init__.py
--rw-r--r--   0        0        0    18654 2023-05-28 09:58:15.401369 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/aidraw.py
--rw-r--r--   0        0        0     6093 2023-05-28 09:58:15.401892 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
--rw-r--r--   0        0        0    65592 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
--rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
--rw-r--r--   0        0        0    15370 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/backend/base.py
--rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
--rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
--rw-r--r--   0        0        0     6321 2023-05-28 09:58:15.405664 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/backend/sd.py
--rw-r--r--   0        0        0    13617 2023-05-28 11:28:54.486210 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/config.py
--rw-r--r--   0        0        0     9282 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
--rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
--rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
--rw-r--r--   0        0        0     1328 2023-05-28 09:58:15.407673 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
--rw-r--r--   0        0        0     3751 2023-05-28 09:58:15.407673 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
--rw-r--r--   0        0        0    11304 2023-05-28 09:58:15.407673 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
--rw-r--r--   0        0        0     3668 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
--rw-r--r--   0        0        0    28380 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
--rw-r--r--   0        0        0     5964 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/extension/translation.py
--rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/fifo.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/locales/en.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/locales/jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/locales/zh.py
--rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/manage.py
--rw-r--r--   0        0        0     1479 2023-05-28 09:58:15.412189 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
--rw-r--r--   0        0        0     2314 2023-05-28 09:58:15.412189 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/utils/data.py
--rw-r--r--   0        0        0     7545 2023-05-28 09:58:15.412189 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
--rw-r--r--   0        0        0      647 2023-05-28 09:58:15.413187 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
--rw-r--r--   0        0        0      727 2023-05-28 09:58:15.413187 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/utils/save.py
--rw-r--r--   0        0        0     1994 2023-05-28 09:58:15.414188 nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/version.py
--rw-r--r--   0        0        0      701 2023-05-28 11:36:41.138126 nonebot_plugin_stable_diffusion_diao-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.1.5/LICENSE
+-rw-r--r--   0        0        0      686 2023-05-28 09:58:15.400842 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/__init__.py
+-rw-r--r--   0        0        0    18654 2023-05-28 09:58:15.401369 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/aidraw.py
+-rw-r--r--   0        0        0     6100 2023-05-28 12:48:55.161779 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
+-rw-r--r--   0        0        0    65592 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
+-rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
+-rw-r--r--   0        0        0    15370 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/backend/base.py
+-rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
+-rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
+-rw-r--r--   0        0        0     6321 2023-05-28 09:58:15.405664 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/backend/sd.py
+-rw-r--r--   0        0        0    13617 2023-05-28 11:28:54.486210 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/config.py
+-rw-r--r--   0        0        0     9282 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
+-rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
+-rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
+-rw-r--r--   0        0        0     1328 2023-05-28 09:58:15.407673 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
+-rw-r--r--   0        0        0     3751 2023-05-28 09:58:15.407673 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
+-rw-r--r--   0        0        0    11304 2023-05-28 09:58:15.407673 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
+-rw-r--r--   0        0        0     3668 2023-05-28 12:10:58.511567 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
+-rw-r--r--   0        0        0    28520 2023-05-28 12:26:36.486249 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
+-rw-r--r--   0        0        0     5964 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/extension/translation.py
+-rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/fifo.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/locales/en.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/locales/jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/locales/zh.py
+-rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/manage.py
+-rw-r--r--   0        0        0     1479 2023-05-28 09:58:15.412189 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
+-rw-r--r--   0        0        0     2314 2023-05-28 09:58:15.412189 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/utils/data.py
+-rw-r--r--   0        0        0     7545 2023-05-28 09:58:15.412189 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
+-rw-r--r--   0        0        0      647 2023-05-28 09:58:15.413187 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
+-rw-r--r--   0        0        0      727 2023-05-28 09:58:15.413187 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/utils/save.py
+-rw-r--r--   0        0        0     1994 2023-05-28 09:58:15.414188 nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/version.py
+-rw-r--r--   0        0        0      701 2023-05-28 22:09:39.160944 nonebot_plugin_stable_diffusion_diao-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.1.5/PKG-INFO
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.4/LICENSE` & `nonebot_plugin_stable_diffusion_diao-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/aidraw.py` & `nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/aidraw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py` & `nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,8 +104,8 @@
         result = await check_safe_method(fifo, [fifo.result[0]], [""], None, True, "_chatgpt")
         if isinstance(result[1], MessageSegment):
             await bot.send(event=event, message=img_msg+f"\n{fifo.img_hash}", at_sender=True, reply_message=True)
         else:
             pass
     else:
         await bot.send(event=event, message=img_msg+f"\n{fifo.img_hash}", at_sender=True, reply_message=True)
-        await save_img(fifo, img_msg, str(fifo.group_id)+"_chatgpt")
+        await save_img(fifo, fifo.result[0], str(fifo.group_id)+"_chatgpt")
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py` & `nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/backend/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/backend/base.py` & `nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/backend/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/backend/naifu.py` & `nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/backend/naifu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/backend/novelai.py` & `nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/backend/novelai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/backend/sd.py` & `nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/backend/sd.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/config.py` & `nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py` & `nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/extension/anlas.py` & `nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/extension/anlas.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/extension/control_net.py` & `nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/extension/control_net.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py` & `nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py` & `nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py` & `nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py` & `nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py` & `nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -557,15 +557,19 @@
     resp_config = await asyncio.gather(*task_list, return_exceptions=True)
     resp_tuple = all_tuple[1][2]
     today = str(datetime.date.today())
     for i, m in zip(resp_tuple, resp_config):
         work_history_list = []
         today_task = 0
         n += 1
-        if isinstance(i, (TypeError or asyncio.exceptions.TimeoutError or Exception)):
+        if isinstance(i, (aiohttp.ContentTypeError or 
+                          TypeError or 
+                          asyncio.exceptions.TimeoutError or 
+                          Exception)
+                          ):
             message.append(f"{n+1}.后端{backend_list[n]}掉线😭\t\n")
         else:
             text_message = ''
             try:
                 model = m["sd_model_checkpoint"]
             except:
                 model = ""
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/extension/translation.py` & `nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/extension/translation.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/manage.py` & `nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/manage.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/utils/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/utils/data.py` & `nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/utils/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py` & `nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py` & `nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/utils/save.py` & `nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/utils/save.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.4/nonebot_plugin_stable_diffusion_diao/version.py` & `nonebot_plugin_stable_diffusion_diao-0.1.5/nonebot_plugin_stable_diffusion_diao/version.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.4/pyproject.toml` & `nonebot_plugin_stable_diffusion_diao-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-stable-diffusion-diao"
-version = "0.1.4"
+version = "0.1.5"
 description = "主要面对stable-diffusion-webui-api的nonebot2插件"
 authors = [
     { name = "DiaoDaiaChan", email = "diaodaiachan@qq.com" },
 ]
 dependencies = [
     "aiofiles>=23.1.0",
     "aiohttp>=3.8.4",
```

