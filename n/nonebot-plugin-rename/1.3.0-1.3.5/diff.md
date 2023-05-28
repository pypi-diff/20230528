# Comparing `tmp/nonebot_plugin_rename-1.3.0.tar.gz` & `tmp/nonebot_plugin_rename-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_rename-1.3.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_rename-1.3.5.tar", max compression
```

## Comparing `nonebot_plugin_rename-1.3.0.tar` & `nonebot_plugin_rename-1.3.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1066 2023-05-28 09:33:04.939643 nonebot_plugin_rename-1.3.0/LICENSE
--rw-r--r--   0        0        0     5286 2023-05-28 09:33:04.939643 nonebot_plugin_rename-1.3.0/README.md
--rw-r--r--   0        0        0      363 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/__init__.py
--rw-r--r--   0        0        0      293 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/__init__.py
--rw-r--r--   0        0        0      844 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/gaokao_time.py
--rw-r--r--   0        0        0     1020 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/genshin_time.py
--rw-r--r--   0        0        0      689 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/get_times.py
--rw-r--r--   0        0        0      925 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/hot_search.py
--rw-r--r--   0        0        0      408 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/message.py
--rw-r--r--   0        0        0      607 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/one_word.py
--rw-r--r--   0        0        0      893 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/starrail_time.py
--rw-r--r--   0        0        0      604 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/status.py
--rw-r--r--   0        0        0      376 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/config.py
--rw-r--r--   0        0        0     9234 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/main.py
--rw-r--r--   0        0        0      187 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/utils/__init__.py
--rw-r--r--   0        0        0      479 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/utils/card_choice.py
--rw-r--r--   0        0        0      838 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/utils/card_name.py
--rw-r--r--   0        0        0     1096 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/utils/download.py
--rw-r--r--   0        0        0     1534 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/utils/draw.py
--rw-r--r--   0        0        0      423 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/utils/my_yaml.py
--rw-r--r--   0        0        0      701 2023-05-28 09:33:04.947643 nonebot_plugin_rename-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     6272 1970-01-01 00:00:00.000000 nonebot_plugin_rename-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-28 10:21:41.708293 nonebot_plugin_rename-1.3.5/LICENSE
+-rw-r--r--   0        0        0     5286 2023-05-28 10:21:41.708293 nonebot_plugin_rename-1.3.5/README.md
+-rw-r--r--   0        0        0      363 2023-05-28 10:21:41.708293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/__init__.py
+-rw-r--r--   0        0        0      293 2023-05-28 10:21:41.708293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/__init__.py
+-rw-r--r--   0        0        0      844 2023-05-28 10:21:41.708293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/gaokao_time.py
+-rw-r--r--   0        0        0     1020 2023-05-28 10:21:41.708293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/genshin_time.py
+-rw-r--r--   0        0        0      689 2023-05-28 10:21:41.708293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/get_times.py
+-rw-r--r--   0        0        0      925 2023-05-28 10:21:41.708293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/hot_search.py
+-rw-r--r--   0        0        0      408 2023-05-28 10:21:41.708293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/message.py
+-rw-r--r--   0        0        0      607 2023-05-28 10:21:41.708293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/one_word.py
+-rw-r--r--   0        0        0      893 2023-05-28 10:21:41.708293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/starrail_time.py
+-rw-r--r--   0        0        0      604 2023-05-28 10:21:41.708293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/status.py
+-rw-r--r--   0        0        0      376 2023-05-28 10:21:41.708293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/config.py
+-rw-r--r--   0        0        0  1878036 2023-05-28 10:21:41.724293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/fonts/draw.ttf
+-rw-r--r--   0        0        0     8894 2023-05-28 10:21:41.724293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/main.py
+-rw-r--r--   0        0        0      151 2023-05-28 10:21:41.724293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/utils/__init__.py
+-rw-r--r--   0        0        0      479 2023-05-28 10:21:41.724293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/utils/card_choice.py
+-rw-r--r--   0        0        0      838 2023-05-28 10:21:41.724293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/utils/card_name.py
+-rw-r--r--   0        0        0     1529 2023-05-28 10:21:41.724293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/utils/draw.py
+-rw-r--r--   0        0        0      423 2023-05-28 10:21:41.724293 nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/utils/my_yaml.py
+-rw-r--r--   0        0        0      644 2023-05-28 10:21:41.724293 nonebot_plugin_rename-1.3.5/pyproject.toml
+-rw-r--r--   0        0        0     6151 1970-01-01 00:00:00.000000 nonebot_plugin_rename-1.3.5/PKG-INFO
```

### Comparing `nonebot_plugin_rename-1.3.0/LICENSE` & `nonebot_plugin_rename-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.0/README.md` & `nonebot_plugin_rename-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/gaokao_time.py` & `nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/gaokao_time.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/genshin_time.py` & `nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/genshin_time.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/get_times.py` & `nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/get_times.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/hot_search.py` & `nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/hot_search.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/one_word.py` & `nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/one_word.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/starrail_time.py` & `nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/starrail_time.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/card/status.py` & `nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/card/status.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/main.py` & `nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from nonebot.params import CommandArg
 from nonebot.permission import SUPERUSER
 
 from .config import Config
 from .utils import (
     card_list,
     choice_card,
-    download_file,
     generate_card_image,
     read_yaml,
     write_yaml,
 )
 
 require("nonebot_plugin_apscheduler")
 from nonebot_plugin_apscheduler import scheduler # noqa
@@ -244,13 +243,7 @@
 # bot启动时执行
 @driver.on_startup
 async def init_group_card():
     if not (yml_file / "group_card.yaml").exists():
         yml_file.mkdir(parents=True, exist_ok=True)
         (yml_file / "group_card.yaml").touch()
         logger.info("创建group_card.yaml文件成功")
-    if not (yml_file / "fonts" / "draw.ttf").exists():
-        (yml_file / "fonts").mkdir(parents=True, exist_ok=True)
-        await download_file(
-            url="https://fastly.jsdelivr.net/gh/forchannot/nonebot_plugin_rename@main/data/fonts/draw.ttf",
-            file_path=yml_file / "fonts" / "draw.ttf",
-        )
```

### Comparing `nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/utils/card_name.py` & `nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/utils/card_name.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.0/nonebot_plugin_rename/utils/draw.py` & `nonebot_plugin_rename-1.3.5/nonebot_plugin_rename/utils/draw.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from io import BytesIO
 from pathlib import Path
 
 from PIL import Image, ImageDraw, ImageFont
 
 from .card_name import card_list
 
-font_path = Path.cwd() / "data" / "group_card" / "fonts" / "draw.ttf"
+
+font_path = Path(__file__).parent.parent / "fonts" / "draw.ttf"
 
 
 def generate_card_image(
     font: Path = font_path,
     font_size: int = 20,
     title_left: str = "群名片序号",
     title_right: str = "群名片描述",
```

### Comparing `nonebot_plugin_rename-1.3.0/pyproject.toml` & `nonebot_plugin_rename-1.3.5/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-rename"
-version = "1.3.0"
+version = "1.3.5"
 description = "更改qq机器人的群名片，内置多种有趣名片"
 authors = ["forchannot <yy320206@gmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_rename"}]
 
 [[tool.poetry.source]]
@@ -16,15 +16,12 @@
 python = "^3.8"
 httpx = "^0.23.3"
 nonebot-adapter-onebot = "^2.2.2"
 nonebot-plugin-apscheduler = "^0.2.0"
 psutil = "^5.9.5"
 pyyaml = "^6.0"
 pillow = "^9.5.0"
-aiohttp = "^3.8.1"
-aiofiles = "^23.1.0"
-tqdm = "^4.65.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_rename-1.3.0/PKG-INFO` & `nonebot_plugin_rename-1.3.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-rename
-Version: 1.3.0
+Version: 1.3.5
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
-Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
-Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.2,<3.0.0)
 Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0,<0.3.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://ghproxy.com/https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://ghproxy.com/https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
```

#### html2text {}

```diff
@@ -1,20 +1,19 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-rename Version: 1.3.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-rename Version: 1.3.5 Summary:
 æ´æ¹qqæºå¨äººçç¾¤åçï¼åç½®å¤ç§æè¶£åç License: GPL-3.0
 Author: forchannot Author-email: yy320206@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: aiofiles (>=23.1.0,<24.0.0) Requires-
-Dist: aiohttp (>=3.8.1,<4.0.0) Requires-Dist: httpx (>=0.23.3,<0.24.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.2.2,<3.0.0) Requires-Dist: nonebot-
-plugin-apscheduler (>=0.2.0,<0.3.0) Requires-Dist: pillow (>=9.5.0,<10.0.0)
-Requires-Dist: psutil (>=5.9.5,<6.0.0) Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: tqdm (>=4.65.0,<5.0.0) Description-Content-Type: text/markdown
+Language :: Python :: 3.11 Requires-Dist: httpx (>=0.23.3,<0.24.0) Requires-
+Dist: nonebot-adapter-onebot (>=2.2.2,<3.0.0) Requires-Dist: nonebot-plugin-
+apscheduler (>=0.2.0,<0.3.0) Requires-Dist: pillow (>=9.5.0,<10.0.0) Requires-
+Dist: psutil (>=5.9.5,<6.0.0) Requires-Dist: pyyaml (>=6.0,<7.0) Description-
+Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                          # nonebot-plugin-rename _â¨
 éè¿å®æ¶ä»»å¡æ´æ¹botæå¨ç¾¤èªå·±çç¾¤åç,åç½®äºå ç§å¸¸è§çç¾¤åçå¹¶ä¸åæ­¥æ¯æäºå¤bot,æ¬¢è¿**pr**æ°çç¾¤åç!
                         â¨_ [license] [pypi] [python]
  * [nonebot-plugin-rename](#nonebot-plugin-rename) * [ðç®ä»](#ç®ä») *
 [ðè®¸å¯](#è®¸å¯) * [ð¿ å®è£æ¹æ³](#-å®è£æ¹æ³) *
```

