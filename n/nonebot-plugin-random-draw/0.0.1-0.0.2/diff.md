# Comparing `tmp/nonebot_plugin_random_draw-0.0.1.tar.gz` & `tmp/nonebot_plugin_random_draw-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_random_draw-0.0.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_random_draw-0.0.2.tar", max compression
```

## Comparing `nonebot_plugin_random_draw-0.0.1.tar` & `nonebot_plugin_random_draw-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1084 2022-12-03 13:20:36.036837 nonebot_plugin_random_draw-0.0.1/LICENSE
--rw-r--r--   0        0        0    20850 2023-05-28 04:27:22.333607 nonebot_plugin_random_draw-0.0.1/nonebot_plugin_random_draw/__init__.py
--rw-r--r--   0        0        0      980 2023-05-28 04:32:54.474525 nonebot_plugin_random_draw-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5660 2023-05-28 04:35:31.088660 nonebot_plugin_random_draw-0.0.1/README.md
--rw-r--r--   0        0        0     6443 1970-01-01 00:00:00.000000 nonebot_plugin_random_draw-0.0.1/setup.py
--rw-r--r--   0        0        0     6413 1970-01-01 00:00:00.000000 nonebot_plugin_random_draw-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2022-12-03 13:20:36.036837 nonebot_plugin_random_draw-0.0.2/LICENSE
+-rw-r--r--   0        0        0    21050 2023-05-28 05:43:43.600557 nonebot_plugin_random_draw-0.0.2/nonebot_plugin_random_draw/__init__.py
+-rw-r--r--   0        0        0      980 2023-05-28 06:27:47.158019 nonebot_plugin_random_draw-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5763 2023-05-28 05:40:33.394241 nonebot_plugin_random_draw-0.0.2/README.md
+-rw-r--r--   0        0        0     6546 1970-01-01 00:00:00.000000 nonebot_plugin_random_draw-0.0.2/setup.py
+-rw-r--r--   0        0        0     6512 1970-01-01 00:00:00.000000 nonebot_plugin_random_draw-0.0.2/PKG-INFO
```

### Comparing `nonebot_plugin_random_draw-0.0.1/LICENSE` & `nonebot_plugin_random_draw-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_random_draw-0.0.1/nonebot_plugin_random_draw/__init__.py` & `nonebot_plugin_random_draw-0.0.2/nonebot_plugin_random_draw/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 from nonebot.plugin import PluginMetadata
 
 
 help_text = f"""
 功能说明：命令列表（命令前缀自行匹配）
 获取帮助：随机抽取帮助
 创建随抽组，一个群可以有多个组：随抽组创建 <组名>
-往指定的随抽组中添加待抽内容：随抽添加 <组号> <内容>
-删除指定随抽组中的待抽内容：随抽删除 <组号> <内容>
+往指定的随抽组中添加待抽内容（可多个，用空格分隔）：随抽添加 <组号> <内容>
+删除指定随抽组中的待抽内容（可多个，用空格分隔）：随抽删除 <组号> <内容>
 删除指定组号的随抽组：随抽组删除 <组号>
 查看本群所有的随抽组内容（含组号和组名）：随抽组列表
 查看指定组号的所有待抽内容：随抽列表 <组号>
 在指定随抽组中随机抽取一个待抽内容：随抽 <组号>
 清空本群中所有的随抽组（慎用）：随抽组清空
 清空指定随抽组中所有的待抽内容（慎用）：随抽清空 <组号>
 """.strip()
@@ -44,15 +44,15 @@
 global_config = nonebot.get_driver().config
 
 # 数据存储路径
 root_dir = "data"
 data_dir = root_dir + "/nonebot_plugin_random_draw"
 data_path = ""
 
-cmd0 = on_command("随机抽取帮助")
+cmd0 = on_command("随抽帮助", aliases={"随机抽取组创建"})
 cmd1 = on_command("随抽组创建", aliases={"随机抽取组创建"}, permission=SUPERUSER | GROUP_ADMIN | GROUP_OWNER)
 cmd2 = on_command("随抽添加", aliases={"随机抽取添加"})
 cmd3 = on_command("随抽删除", aliases={"随机抽取删除"})
 cmd4 = on_command("随抽组删除", aliases={"随机抽取组删除"})
 cmd5 = on_command("随抽组列表", aliases={"随机抽取组列表"})
 cmd6 = on_command("随抽列表", aliases={"随机抽取列表"})
 cmd7 = on_command("随抽", aliases={"随机抽取"})
@@ -143,43 +143,55 @@
     content = msg.extract_plain_text()
     content = content.split()
 
     group_id = event.group_id
 
     data_path = await check_data_file(group_id)
 
-    if len(content) != 2:
+    if len(content) < 2:
         msg = '命令错误，命令：/随抽添加 <组号> <内容>'
         await cmd2.finish(Message(f'{msg}'), reply_message=True)
 
 
     group_num = content[0]
-    content_str = content[1]
+    # 删除组号
+    del content[0]
+    # content_str = content[1]
     # qq = event.get_user_id()
 
     data_json = {}
 
     try:
         # 打开JSON文件
         with open(data_path, 'r', encoding="utf-8") as f:
             # 读取文件内容并解析JSON
             data_json = json.load(f)
         
             # 判断是否存在
-            if group_num in data_json:             
+            if group_num not in data_json:
+                msg = "不存在此随抽组，请先创建随抽组。"
+                await cmd2.send(Message(f'{msg}'), reply_message=True)
+
+            data_arr = []
+
+            for data in content:
                 for users in data_json[group_num]["内容"]:
                     # 重复性检测
-                    if users == content_str:
-                        msg = '组号：' + group_num + "，已存在 " + content_str + "，请勿重复添加！"
-                        await cmd2.finish(Message(f'{msg}'), reply_message=True)
-
-                data_json[group_num]["内容"].append(content_str)
-            else:
-                msg = '命令错误，添加的组号不存在，请先确认随抽组列表，命令：/随抽组列表'
-                await cmd2.finish(Message(f'{msg}'), reply_message=True)
+                    if users == data:
+                        data_arr.append(data)
+                        break
+
+                data_json[group_num]["内容"].append(data)
+            
+            if len(data_arr) != 0:
+                msg = '组号：' + group_num + "，已存在 "
+                for data in data_arr:
+                    msg = msg + data + " "
+                msg = msg + "，请勿重复添加！"
+                await cmd2.send(Message(f'{msg}'), reply_message=True)
 
         # 将处理后的JSON数据写入文件
         with open(data_path, 'w', encoding="utf-8") as f:
             json.dump(data_json, f, ensure_ascii=False)
 
         await cmd2.finish('添加成功~', reply_message=True)
     except FinishedException:
@@ -197,20 +209,21 @@
 
     group_id = event.group_id
 
     content = content.split()
 
     data_path = await check_data_file(group_id)
 
-    if len(content) != 2:
+    if len(content) < 2:
         msg = '命令错误，命令：/随抽删除 <组号> <内容>'
         await cmd2.finish(Message(f'{msg}'), reply_message=True)
 
     group_num = content[0]
-    content_str = content[1]
+    # content_str = content[1]
+    del content[0]
 
     try:
         data_json = None
 
         # 打开JSON文件
         with open(data_path, 'r', encoding="utf-8") as f:
             # 读取文件内容并解析JSON
@@ -224,25 +237,23 @@
             # 如果是空数据
             if len(data_json[group_num]) == 0:
                 msg = '当前随抽组无内容，无需删除。'
                 await cmd3.finish(Message(f'{msg}'), reply_message=True)
 
             # qq = event.get_user_id()
 
-            if "内容" in data_json[group_num] and content_str in data_json[group_num]["内容"]:
-                data_json[group_num]["内容"].remove(content_str)
-                # 将处理后的JSON数据写入文件
-                with open(data_path, 'w', encoding="utf-8") as f:
-                    json.dump(data_json, f, ensure_ascii=False)
+            for content_str in content:
+                if content_str in data_json[group_num]["内容"]:
+                    data_json[group_num]["内容"].remove(content_str)
+                    # 将处理后的JSON数据写入文件
+                    with open(data_path, 'w', encoding="utf-8") as f:
+                        json.dump(data_json, f, ensure_ascii=False)
 
-                msg = "随抽删除成功~"
-                await cmd3.send(Message(f'{msg}'), reply_message=True)
-            else:
-                msg = '不存在 ' + content_str + '，无需删除。'
-                await cmd3.finish(Message(f'{msg}'), reply_message=True)
+            msg = "随抽删除匹配的内容成功~"
+            await cmd3.send(Message(f'{msg}'), reply_message=True)
     except FinishedException:
         pass
     except Exception as e:
         logger.info(e)
         msg = '随抽删除失败！（请看后台日志排查问题）'
         await cmd3.finish(Message(f'{msg}'), reply_message=True)
```

### Comparing `nonebot_plugin_random_draw-0.0.1/pyproject.toml` & `nonebot_plugin_random_draw-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-random_draw"
-version = "0.0.1"
+version = "0.0.2"
 description = "通过添加各种想要抽取的内容，最后进行随机抽取。"
 authors = ["Ikaros <327209194@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_random_draw"}]
 homepage = "https://github.com/Ikaros-521/nonebot_plugin_random_draw"
 repository = "https://github.com/Ikaros-521/nonebot_plugin_random_draw"
```

### Comparing `nonebot_plugin_random_draw-0.0.1/README.md` & `nonebot_plugin_random_draw-0.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -81,25 +81,25 @@
 
 
 ## 🎉 功能
   
 
 ## 👉 命令
 
-### /随机抽取帮助
-命令结构：```/随机抽取帮助```  
-例如：```/随机抽取帮助```  
+### /随抽帮助
+命令结构：```/随抽帮助```  
+例如：```/随抽帮助```  
 功能：返回所有命令的使用方式。  
 bot返回内容：  
 ```
 功能说明：命令列表（命令前缀自行匹配）
-获取帮助：随机抽取帮助
+获取帮助：随抽帮助
 创建随抽组，一个群可以有多个组：随抽组创建 <组名>
-往指定的随抽组中添加待抽内容：随抽添加 <组号> <内容>
-删除指定随抽组中的待抽内容：随抽删除 <组号> <内容>
+往指定的随抽组中添加待抽内容（可多个，用空格分隔）：随抽添加 <组号> <内容>
+删除指定随抽组中的待抽内容（可多个，用空格分隔）：随抽删除 <组号> <内容>
 删除指定组号的随抽组：随抽组删除 <组号>
 查看本群所有的随抽组内容（含组号和组名）：随抽组列表
 查看指定组号的所有待抽内容：随抽列表 <组号>
 在指定随抽组中随机抽取一个待抽内容：随抽 <组号>
 清空本群中所有的随抽组（慎用）：随抽组清空
 清空指定随抽组中所有的待抽内容（慎用）：随抽清空 <组号>
 ```
@@ -115,14 +115,18 @@
 <details>
 <summary>展开/收起</summary>
 
 ### 0.0.1
 
 - 插件初次发布  
 
+### 0.0.2
+
+- 增加批量添加和删除内容的功能
+
 </details>
 
 ## 致谢
 - [nonebot-plugin-template](https://github.com/A-kirami/nonebot-plugin-template)
 
 ## 项目打包上传至pypi
```

#### html2text {}

```diff
@@ -19,32 +19,34 @@
 æå¼ nonebot2 é¡¹ç®ç ```bot.py``` æä»¶, å¨å¶ä¸­åå¥
 ```nonebot.load_plugin('nonebot_plugin_random_draw')```
 å½ç¶ï¼å¦ææ¯é»è®¤nb-
 cliåå»ºçnonebot2çè¯ï¼å¨botè·¯å¾```pyproject.toml```ç```
 [tool.nonebot]```ç```plugins```ä¸­æ·»å ```nonebot_plugin_random_draw```å³å¯
 pyproject.tomléç½®ä¾å¦ï¼ ``` [tool.nonebot] plugin_dirs = ["src/plugins"]
 plugins = ["nonebot_plugin_random_draw"] ``` ## ð§ éç½® ## ð åè½ ##
-ð å½ä»¤ ### /éæºæ½åå¸®å© å½ä»¤ç»æï¼```/éæºæ½åå¸®å©```
-ä¾å¦ï¼```/éæºæ½åå¸®å©```
-åè½ï¼è¿åææå½ä»¤çä½¿ç¨æ¹å¼ã botè¿ååå®¹ï¼ ```
+ð å½ä»¤ ### /éæ½å¸®å© å½ä»¤ç»æï¼```/éæ½å¸®å©``` ä¾å¦ï¼```/
+éæ½å¸®å©``` åè½ï¼è¿åææå½ä»¤çä½¿ç¨æ¹å¼ã
+botè¿ååå®¹ï¼ ```
 åè½è¯´æï¼å½ä»¤åè¡¨ï¼å½ä»¤åç¼èªè¡å¹éï¼
-è·åå¸®å©ï¼éæºæ½åå¸®å©
+è·åå¸®å©ï¼éæ½å¸®å©
 åå»ºéæ½ç»ï¼ä¸ä¸ªç¾¤å¯ä»¥æå¤ä¸ªç»ï¼éæ½ç»åå»º <ç»å>
-å¾æå®çéæ½ç»ä¸­æ·»å å¾æ½åå®¹ï¼éæ½æ·»å  <ç»å·> <åå®¹>
-å é¤æå®éæ½ç»ä¸­çå¾æ½åå®¹ï¼éæ½å é¤ <ç»å·> <åå®¹>
-å é¤æå®ç»å·çéæ½ç»ï¼éæ½ç»å é¤ <ç»å·>
+å¾æå®çéæ½ç»ä¸­æ·»å å¾æ½åå®¹ï¼å¯å¤ä¸ªï¼ç¨ç©ºæ ¼åéï¼ï¼éæ½æ·»å 
+<ç»å·> <åå®¹>
+å é¤æå®éæ½ç»ä¸­çå¾æ½åå®¹ï¼å¯å¤ä¸ªï¼ç¨ç©ºæ ¼åéï¼ï¼éæ½å é¤
+<ç»å·> <åå®¹> å é¤æå®ç»å·çéæ½ç»ï¼éæ½ç»å é¤ <ç»å·>
 æ¥çæ¬ç¾¤ææçéæ½ç»åå®¹ï¼å«ç»å·åç»åï¼ï¼éæ½ç»åè¡¨
 æ¥çæå®ç»å·çææå¾æ½åå®¹ï¼éæ½åè¡¨ <ç»å·>
 å¨æå®éæ½ç»ä¸­éæºæ½åä¸ä¸ªå¾æ½åå®¹ï¼éæ½ <ç»å·>
 æ¸ç©ºæ¬ç¾¤ä¸­ææçéæ½ç»ï¼æç¨ï¼ï¼éæ½ç»æ¸ç©º
 æ¸ç©ºæå®éæ½ç»ä¸­ææçå¾æ½åå®¹ï¼æç¨ï¼ï¼éæ½æ¸ç©º
 <ç»å·> ``` ### å¶ä»å½ä»¤æå¾åäºï¼ç´æ¥çå¾å§ ![](docs/
 result.png) ## â æå± ## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 0.0.1 -
-æä»¶åæ¬¡åå¸  ## è´è°¢ - [nonebot-plugin-template](https://github.com/A-
-kirami/nonebot-plugin-template) ## é¡¹ç®æåä¸ä¼ è³pypi å®ç½ï¼https://
+æä»¶åæ¬¡åå¸ ### 0.0.2 - å¢å æ¹éæ·»å åå é¤åå®¹çåè½  ##
+è´è°¢ - [nonebot-plugin-template](https://github.com/A-kirami/nonebot-plugin-
+template) ## é¡¹ç®æåä¸ä¼ è³pypi å®ç½ï¼https://
 pypi.orgï¼æ³¨åè´¦å·ï¼å¨ç³»ç»ç¨æ·æ ¹ç®å½ä¸åå»º`.pypirc`ï¼éç½®
 ``` [distutils] index-servers=pypi [pypi] repository = https://upload.pypi.org/
 legacy/ username = ç¨æ·å password = å¯ç  ``` ### poetry ``` # åè
 https://www.freesion.com/article/58051228882/ # poetry config pypi-token.pypi #
 1ãå®è£poetry pip install poetry #
 2ãåå§åéç½®æä»¶ï¼æ ¹æ®æç¤ºå¡«åï¼ poetry init #
 3ãå¾®è°éç½®æä»¶pyproject.toml # 4ãè¿è¡ poetry install, å¯çæ
```

### Comparing `nonebot_plugin_random_draw-0.0.1/setup.py` & `nonebot_plugin_random_draw-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['nonebot-adapter-onebot>=2.1.3,<3.0.0', 'nonebot2>=2.0.0b5,<3.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-random-draw',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': '通过添加各种想要抽取的内容，最后进行随机抽取。',
-    'long_description': '<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot_plugin_random_draw\n\n_✨ NoneBot 随机抽取设定内容 插件 ✨_\n\n\n<a href="https://github.com/Ikaros-521/nonebot_plugin_random_draw/stargazers">\n    <img alt="GitHub stars" src="https://img.shields.io/github/stars/Ikaros-521/nonebot_plugin_random_draw?color=%09%2300BFFF&style=flat-square">\n</a>\n<a href="https://github.com/Ikaros-521/nonebot_plugin_random_draw/issues">\n    <img alt="GitHub issues" src="https://img.shields.io/github/issues/Ikaros-521/nonebot_plugin_random_draw?color=Emerald%20green&style=flat-square">\n</a>\n<a href="https://github.com/Ikaros-521/nonebot_plugin_random_draw/network">\n    <img alt="GitHub forks" src="https://img.shields.io/github/forks/Ikaros-521/nonebot_plugin_random_draw?color=%2300BFFF&style=flat-square">\n</a>\n<a href="./LICENSE">\n    <img src="https://img.shields.io/github/license/Ikaros-521/nonebot_plugin_random_draw.svg" alt="license">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_random_draw">\n    <img src="https://img.shields.io/pypi/v/nonebot_plugin_random_draw.svg" alt="pypi">\n</a>\n<a href="https://www.python.org">\n    <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">\n</a>\n\n</div>\n\n## 📖 介绍\n\n通过添加各种想要抽取的内容，最后进行随机抽取。  \n\n## 🔧 开发环境\nNonebot2：2.0.0rc3  \npython：3.8.13  \n操作系统：Windows10（Linux兼容性问题不大）  \n编辑器：VS Code  \n\n## 💿 安装  \n\n### 1. nb-cli安装\n\n在你bot工程的文件夹下，运行cmd（运行路径要对啊），执行nb命令安装插件，插件配置会自动添加至配置文件  \n```\nnb plugin install nonebot_plugin_random_draw\n```\n\n### 2. 本地安装\n\n将项目clone到你的机器人插件下的对应插件目录内（一般为机器人文件夹下的`src/plugins`），然后把`nonebot_plugin_random_draw`文件夹里的内容拷贝至上一级目录即可。  \nclone命令参考（得先装`git`，懂的都懂）：\n```\ngit clone https://github.com/Ikaros-521/nonebot_plugin_random_draw.git\n``` \n也可以直接下载压缩包到插件目录解压，然后同样提取`nonebot_plugin_random_draw`至上一级目录。  \n目录结构： ```你的bot/src/plugins/nonebot_plugin_random_draw/__init__.py```  \n\n\n### 3. pip安装\n```\npip install nonebot_plugin_random_draw\n```  \n打开 nonebot2 项目的 ```bot.py``` 文件, 在其中写入  \n```nonebot.load_plugin(\'nonebot_plugin_random_draw\')```  \n当然，如果是默认nb-cli创建的nonebot2的话，在bot路径```pyproject.toml```的```[tool.nonebot]```的```plugins```中添加```nonebot_plugin_random_draw```即可  \npyproject.toml配置例如：  \n``` \n[tool.nonebot]\nplugin_dirs = ["src/plugins"]\nplugins = ["nonebot_plugin_random_draw"]\n``` \n\n\n## 🔧 配置\n\n\n## 🎉 功能\n  \n\n## 👉 命令\n\n### /随机抽取帮助\n命令结构：```/随机抽取帮助```  \n例如：```/随机抽取帮助```  \n功能：返回所有命令的使用方式。  \nbot返回内容：  \n```\n功能说明：命令列表（命令前缀自行匹配）\n获取帮助：随机抽取帮助\n创建随抽组，一个群可以有多个组：随抽组创建 <组名>\n往指定的随抽组中添加待抽内容：随抽添加 <组号> <内容>\n删除指定随抽组中的待抽内容：随抽删除 <组号> <内容>\n删除指定组号的随抽组：随抽组删除 <组号>\n查看本群所有的随抽组内容（含组号和组名）：随抽组列表\n查看指定组号的所有待抽内容：随抽列表 <组号>\n在指定随抽组中随机抽取一个待抽内容：随抽 <组号>\n清空本群中所有的随抽组（慎用）：随抽组清空\n清空指定随抽组中所有的待抽内容（慎用）：随抽清空 <组号>\n```\n\n### 其他命令懒得写了，直接看图吧\n![](docs/result.png)\n\n## ⚙ 拓展\n \n\n## 📝 更新日志\n\n<details>\n<summary>展开/收起</summary>\n\n### 0.0.1\n\n- 插件初次发布  \n\n</details>\n\n## 致谢\n- [nonebot-plugin-template](https://github.com/A-kirami/nonebot-plugin-template)\n\n## 项目打包上传至pypi\n\n官网：https://pypi.org，注册账号，在系统用户根目录下创建`.pypirc`，配置  \n``` \n[distutils] \nindex-servers=pypi \n \n[pypi] repository = https://upload.pypi.org/legacy/ \nusername = 用户名 \npassword = 密码\n```\n\n### poetry\n\n```\n# 参考 https://www.freesion.com/article/58051228882/\n# poetry config pypi-token.pypi\n\n# 1、安装poetry\npip install poetry\n\n# 2、初始化配置文件（根据提示填写）\npoetry init\n\n# 3、微调配置文件pyproject.toml\n\n# 4、运行 poetry install, 可生成 “poetry.lock” 文件（可跳过）\npoetry install\n\n# 5、编译，生成dist\npoetry build\n\n# 6、发布(poetry config pypi-token.pypi 配置token)\npoetry publish\n\n```\n\n### twine\n\n```\n# 参考 https://www.cnblogs.com/danhuai/p/14915042.html\n#创建setup.py文件 填写相关信息\n\n# 1、可以先升级打包工具\npip install --upgrade setuptools wheel twine\n\n# 2、打包\npython setup.py sdist bdist_wheel\n\n# 3、可以先检查一下包\ntwine check dist/*\n\n# 4、上传包到pypi（需输入用户名、密码）\ntwine upload dist/*\n```\n',
+    'long_description': '<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot_plugin_random_draw\n\n_✨ NoneBot 随机抽取设定内容 插件 ✨_\n\n\n<a href="https://github.com/Ikaros-521/nonebot_plugin_random_draw/stargazers">\n    <img alt="GitHub stars" src="https://img.shields.io/github/stars/Ikaros-521/nonebot_plugin_random_draw?color=%09%2300BFFF&style=flat-square">\n</a>\n<a href="https://github.com/Ikaros-521/nonebot_plugin_random_draw/issues">\n    <img alt="GitHub issues" src="https://img.shields.io/github/issues/Ikaros-521/nonebot_plugin_random_draw?color=Emerald%20green&style=flat-square">\n</a>\n<a href="https://github.com/Ikaros-521/nonebot_plugin_random_draw/network">\n    <img alt="GitHub forks" src="https://img.shields.io/github/forks/Ikaros-521/nonebot_plugin_random_draw?color=%2300BFFF&style=flat-square">\n</a>\n<a href="./LICENSE">\n    <img src="https://img.shields.io/github/license/Ikaros-521/nonebot_plugin_random_draw.svg" alt="license">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_random_draw">\n    <img src="https://img.shields.io/pypi/v/nonebot_plugin_random_draw.svg" alt="pypi">\n</a>\n<a href="https://www.python.org">\n    <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">\n</a>\n\n</div>\n\n## 📖 介绍\n\n通过添加各种想要抽取的内容，最后进行随机抽取。  \n\n## 🔧 开发环境\nNonebot2：2.0.0rc3  \npython：3.8.13  \n操作系统：Windows10（Linux兼容性问题不大）  \n编辑器：VS Code  \n\n## 💿 安装  \n\n### 1. nb-cli安装\n\n在你bot工程的文件夹下，运行cmd（运行路径要对啊），执行nb命令安装插件，插件配置会自动添加至配置文件  \n```\nnb plugin install nonebot_plugin_random_draw\n```\n\n### 2. 本地安装\n\n将项目clone到你的机器人插件下的对应插件目录内（一般为机器人文件夹下的`src/plugins`），然后把`nonebot_plugin_random_draw`文件夹里的内容拷贝至上一级目录即可。  \nclone命令参考（得先装`git`，懂的都懂）：\n```\ngit clone https://github.com/Ikaros-521/nonebot_plugin_random_draw.git\n``` \n也可以直接下载压缩包到插件目录解压，然后同样提取`nonebot_plugin_random_draw`至上一级目录。  \n目录结构： ```你的bot/src/plugins/nonebot_plugin_random_draw/__init__.py```  \n\n\n### 3. pip安装\n```\npip install nonebot_plugin_random_draw\n```  \n打开 nonebot2 项目的 ```bot.py``` 文件, 在其中写入  \n```nonebot.load_plugin(\'nonebot_plugin_random_draw\')```  \n当然，如果是默认nb-cli创建的nonebot2的话，在bot路径```pyproject.toml```的```[tool.nonebot]```的```plugins```中添加```nonebot_plugin_random_draw```即可  \npyproject.toml配置例如：  \n``` \n[tool.nonebot]\nplugin_dirs = ["src/plugins"]\nplugins = ["nonebot_plugin_random_draw"]\n``` \n\n\n## 🔧 配置\n\n\n## 🎉 功能\n  \n\n## 👉 命令\n\n### /随抽帮助\n命令结构：```/随抽帮助```  \n例如：```/随抽帮助```  \n功能：返回所有命令的使用方式。  \nbot返回内容：  \n```\n功能说明：命令列表（命令前缀自行匹配）\n获取帮助：随抽帮助\n创建随抽组，一个群可以有多个组：随抽组创建 <组名>\n往指定的随抽组中添加待抽内容（可多个，用空格分隔）：随抽添加 <组号> <内容>\n删除指定随抽组中的待抽内容（可多个，用空格分隔）：随抽删除 <组号> <内容>\n删除指定组号的随抽组：随抽组删除 <组号>\n查看本群所有的随抽组内容（含组号和组名）：随抽组列表\n查看指定组号的所有待抽内容：随抽列表 <组号>\n在指定随抽组中随机抽取一个待抽内容：随抽 <组号>\n清空本群中所有的随抽组（慎用）：随抽组清空\n清空指定随抽组中所有的待抽内容（慎用）：随抽清空 <组号>\n```\n\n### 其他命令懒得写了，直接看图吧\n![](docs/result.png)\n\n## ⚙ 拓展\n \n\n## 📝 更新日志\n\n<details>\n<summary>展开/收起</summary>\n\n### 0.0.1\n\n- 插件初次发布  \n\n### 0.0.2\n\n- 增加批量添加和删除内容的功能\n\n</details>\n\n## 致谢\n- [nonebot-plugin-template](https://github.com/A-kirami/nonebot-plugin-template)\n\n## 项目打包上传至pypi\n\n官网：https://pypi.org，注册账号，在系统用户根目录下创建`.pypirc`，配置  \n``` \n[distutils] \nindex-servers=pypi \n \n[pypi] repository = https://upload.pypi.org/legacy/ \nusername = 用户名 \npassword = 密码\n```\n\n### poetry\n\n```\n# 参考 https://www.freesion.com/article/58051228882/\n# poetry config pypi-token.pypi\n\n# 1、安装poetry\npip install poetry\n\n# 2、初始化配置文件（根据提示填写）\npoetry init\n\n# 3、微调配置文件pyproject.toml\n\n# 4、运行 poetry install, 可生成 “poetry.lock” 文件（可跳过）\npoetry install\n\n# 5、编译，生成dist\npoetry build\n\n# 6、发布(poetry config pypi-token.pypi 配置token)\npoetry publish\n\n```\n\n### twine\n\n```\n# 参考 https://www.cnblogs.com/danhuai/p/14915042.html\n#创建setup.py文件 填写相关信息\n\n# 1、可以先升级打包工具\npip install --upgrade setuptools wheel twine\n\n# 2、打包\npython setup.py sdist bdist_wheel\n\n# 3、可以先检查一下包\ntwine check dist/*\n\n# 4、上传包到pypi（需输入用户名、密码）\ntwine upload dist/*\n```\n',
     'author': 'Ikaros',
     'author_email': '327209194@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Ikaros-521/nonebot_plugin_random_draw',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['nonebot_plugin_random_draw'] package_data = \ {'': ['*']} install_requires =
 \ ['nonebot-adapter-onebot>=2.1.3,<3.0.0', 'nonebot2>=2.0.0b5,<3.0.0']
-setup_kwargs = { 'name': 'nonebot-plugin-random-draw', 'version': '0.0.1',
+setup_kwargs = { 'name': 'nonebot-plugin-random-draw', 'version': '0.0.2',
 'description':
 'éè¿æ·»å åç§æ³è¦æ½åçåå®¹ï¼æåè¿è¡éæºæ½åã',
 'long_description': '
                            \n [NoneBotPluginLogo]\n
                                       \n
                               [NoneBotPluginText]
                                       \n
@@ -31,28 +31,29 @@
 æä»¶, å¨å¶ä¸­åå¥ \n```nonebot.load_plugin
 (\'nonebot_plugin_random_draw\')``` \nå½ç¶ï¼å¦ææ¯é»è®¤nb-
 cliåå»ºçnonebot2çè¯ï¼å¨botè·¯å¾```pyproject.toml```ç```
 [tool.nonebot]```ç```plugins```ä¸­æ·»å ```nonebot_plugin_random_draw```å³å¯
 \npyproject.tomléç½®ä¾å¦ï¼ \n``` \n[tool.nonebot]\nplugin_dirs = ["src/
 plugins"]\nplugins = ["nonebot_plugin_random_draw"]\n``` \n\n\n## ð§
 éç½®\n\n\n## ð åè½\n \n\n## ð å½ä»¤\n\n### /
-éæºæ½åå¸®å©\nå½ä»¤ç»æï¼```/éæºæ½åå¸®å©``` \nä¾å¦ï¼```/
-éæºæ½åå¸®å©``` \nåè½ï¼è¿åææå½ä»¤çä½¿ç¨æ¹å¼ã
-\nbotè¿ååå®¹ï¼
-\n```\nåè½è¯´æï¼å½ä»¤åè¡¨ï¼å½ä»¤åç¼èªè¡å¹éï¼\nè·åå¸®å©ï¼éæºæ½åå¸®å©\nåå»ºéæ½ç»ï¼ä¸ä¸ªç¾¤å¯ä»¥æå¤ä¸ªç»ï¼éæ½ç»åå»º
-<ç»å>\nå¾æå®çéæ½ç»ä¸­æ·»å å¾æ½åå®¹ï¼éæ½æ·»å  <ç»å·>
-<åå®¹>\nå é¤æå®éæ½ç»ä¸­çå¾æ½åå®¹ï¼éæ½å é¤ <ç»å·>
-<åå®¹>\nå é¤æå®ç»å·çéæ½ç»ï¼éæ½ç»å é¤
+éæ½å¸®å©\nå½ä»¤ç»æï¼```/éæ½å¸®å©``` \nä¾å¦ï¼```/éæ½å¸®å©```
+\nåè½ï¼è¿åææå½ä»¤çä½¿ç¨æ¹å¼ã \nbotè¿ååå®¹ï¼
+\n```\nåè½è¯´æï¼å½ä»¤åè¡¨ï¼å½ä»¤åç¼èªè¡å¹éï¼\nè·åå¸®å©ï¼éæ½å¸®å©\nåå»ºéæ½ç»ï¼ä¸ä¸ªç¾¤å¯ä»¥æå¤ä¸ªç»ï¼éæ½ç»åå»º
+<ç»å>\nå¾æå®çéæ½ç»ä¸­æ·»å å¾æ½åå®¹ï¼å¯å¤ä¸ªï¼ç¨ç©ºæ ¼åéï¼ï¼éæ½æ·»å 
+<ç»å·>
+<åå®¹>\nå é¤æå®éæ½ç»ä¸­çå¾æ½åå®¹ï¼å¯å¤ä¸ªï¼ç¨ç©ºæ ¼åéï¼ï¼éæ½å é¤
+<ç»å·> <åå®¹>\nå é¤æå®ç»å·çéæ½ç»ï¼éæ½ç»å é¤
 <ç»å·>\næ¥çæ¬ç¾¤ææçéæ½ç»åå®¹ï¼å«ç»å·åç»åï¼ï¼éæ½ç»åè¡¨\næ¥çæå®ç»å·çææå¾æ½åå®¹ï¼éæ½åè¡¨
 <ç»å·>\nå¨æå®éæ½ç»ä¸­éæºæ½åä¸ä¸ªå¾æ½åå®¹ï¼éæ½
 <ç»å·>\næ¸ç©ºæ¬ç¾¤ä¸­ææçéæ½ç»ï¼æç¨ï¼ï¼éæ½ç»æ¸ç©º\næ¸ç©ºæå®éæ½ç»ä¸­ææçå¾æ½åå®¹ï¼æç¨ï¼ï¼éæ½æ¸ç©º
 <ç»å·>\n```\n\n### å¶ä»å½ä»¤æå¾åäºï¼ç´æ¥çå¾å§\n![](docs/
 result.png)\n\n## â æå±\n \n\n## ð æ´æ°æ¥å¿\n\n\nå±å¼/
-æ¶èµ·\n\n### 0.0.1\n\n- æä»¶åæ¬¡åå¸ \n\n\n\n## è´è°¢\n- [nonebot-
-plugin-template](https://github.com/A-kirami/nonebot-plugin-template)\n\n##
+æ¶èµ·\n\n### 0.0.1\n\n- æä»¶åæ¬¡åå¸ \n\n### 0.0.2\n\n-
+å¢å æ¹éæ·»å åå é¤åå®¹çåè½\n\n\n\n## è´è°¢\n- [nonebot-plugin-
+template](https://github.com/A-kirami/nonebot-plugin-template)\n\n##
 é¡¹ç®æåä¸ä¼ è³pypi\n\nå®ç½ï¼https://
 pypi.orgï¼æ³¨åè´¦å·ï¼å¨ç³»ç»ç¨æ·æ ¹ç®å½ä¸åå»º`.pypirc`ï¼éç½®
 \n``` \n[distutils] \nindex-servers=pypi \n \n[pypi] repository = https://
 upload.pypi.org/legacy/ \nusername = ç¨æ·å \npassword = å¯ç \n```\n\n###
 poetry\n\n```\n# åè https://www.freesion.com/article/58051228882/\n# poetry
 config pypi-token.pypi\n\n# 1ãå®è£poetry\npip install poetry\n\n#
 2ãåå§åéç½®æä»¶ï¼æ ¹æ®æç¤ºå¡«åï¼\npoetry init\n\n#
```

### Comparing `nonebot_plugin_random_draw-0.0.1/PKG-INFO` & `nonebot_plugin_random_draw-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-random-draw
-Version: 0.0.1
+Version: 0.0.2
 Summary: 通过添加各种想要抽取的内容，最后进行随机抽取。
 Home-page: https://github.com/Ikaros-521/nonebot_plugin_random_draw
 License: MIT
 Author: Ikaros
 Author-email: 327209194@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -102,25 +102,25 @@
 
 
 ## 🎉 功能
   
 
 ## 👉 命令
 
-### /随机抽取帮助
-命令结构：```/随机抽取帮助```  
-例如：```/随机抽取帮助```  
+### /随抽帮助
+命令结构：```/随抽帮助```  
+例如：```/随抽帮助```  
 功能：返回所有命令的使用方式。  
 bot返回内容：  
 ```
 功能说明：命令列表（命令前缀自行匹配）
-获取帮助：随机抽取帮助
+获取帮助：随抽帮助
 创建随抽组，一个群可以有多个组：随抽组创建 <组名>
-往指定的随抽组中添加待抽内容：随抽添加 <组号> <内容>
-删除指定随抽组中的待抽内容：随抽删除 <组号> <内容>
+往指定的随抽组中添加待抽内容（可多个，用空格分隔）：随抽添加 <组号> <内容>
+删除指定随抽组中的待抽内容（可多个，用空格分隔）：随抽删除 <组号> <内容>
 删除指定组号的随抽组：随抽组删除 <组号>
 查看本群所有的随抽组内容（含组号和组名）：随抽组列表
 查看指定组号的所有待抽内容：随抽列表 <组号>
 在指定随抽组中随机抽取一个待抽内容：随抽 <组号>
 清空本群中所有的随抽组（慎用）：随抽组清空
 清空指定随抽组中所有的待抽内容（慎用）：随抽清空 <组号>
 ```
@@ -136,14 +136,18 @@
 <details>
 <summary>展开/收起</summary>
 
 ### 0.0.1
 
 - 插件初次发布  
 
+### 0.0.2
+
+- 增加批量添加和删除内容的功能
+
 </details>
 
 ## 致谢
 - [nonebot-plugin-template](https://github.com/A-kirami/nonebot-plugin-template)
 
 ## 项目打包上传至pypi
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-random-draw Version: 0.0.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-random-draw Version: 0.0.2 Summary:
 éè¿æ·»å åç§æ³è¦æ½åçåå®¹ï¼æåè¿è¡éæºæ½åã Home-
 page: https://github.com/Ikaros-521/nonebot_plugin_random_draw License: MIT
 Author: Ikaros Author-email: 327209194@qq.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
@@ -32,32 +32,34 @@
 æå¼ nonebot2 é¡¹ç®ç ```bot.py``` æä»¶, å¨å¶ä¸­åå¥
 ```nonebot.load_plugin('nonebot_plugin_random_draw')```
 å½ç¶ï¼å¦ææ¯é»è®¤nb-
 cliåå»ºçnonebot2çè¯ï¼å¨botè·¯å¾```pyproject.toml```ç```
 [tool.nonebot]```ç```plugins```ä¸­æ·»å ```nonebot_plugin_random_draw```å³å¯
 pyproject.tomléç½®ä¾å¦ï¼ ``` [tool.nonebot] plugin_dirs = ["src/plugins"]
 plugins = ["nonebot_plugin_random_draw"] ``` ## ð§ éç½® ## ð åè½ ##
-ð å½ä»¤ ### /éæºæ½åå¸®å© å½ä»¤ç»æï¼```/éæºæ½åå¸®å©```
-ä¾å¦ï¼```/éæºæ½åå¸®å©```
-åè½ï¼è¿åææå½ä»¤çä½¿ç¨æ¹å¼ã botè¿ååå®¹ï¼ ```
+ð å½ä»¤ ### /éæ½å¸®å© å½ä»¤ç»æï¼```/éæ½å¸®å©``` ä¾å¦ï¼```/
+éæ½å¸®å©``` åè½ï¼è¿åææå½ä»¤çä½¿ç¨æ¹å¼ã
+botè¿ååå®¹ï¼ ```
 åè½è¯´æï¼å½ä»¤åè¡¨ï¼å½ä»¤åç¼èªè¡å¹éï¼
-è·åå¸®å©ï¼éæºæ½åå¸®å©
+è·åå¸®å©ï¼éæ½å¸®å©
 åå»ºéæ½ç»ï¼ä¸ä¸ªç¾¤å¯ä»¥æå¤ä¸ªç»ï¼éæ½ç»åå»º <ç»å>
-å¾æå®çéæ½ç»ä¸­æ·»å å¾æ½åå®¹ï¼éæ½æ·»å  <ç»å·> <åå®¹>
-å é¤æå®éæ½ç»ä¸­çå¾æ½åå®¹ï¼éæ½å é¤ <ç»å·> <åå®¹>
-å é¤æå®ç»å·çéæ½ç»ï¼éæ½ç»å é¤ <ç»å·>
+å¾æå®çéæ½ç»ä¸­æ·»å å¾æ½åå®¹ï¼å¯å¤ä¸ªï¼ç¨ç©ºæ ¼åéï¼ï¼éæ½æ·»å 
+<ç»å·> <åå®¹>
+å é¤æå®éæ½ç»ä¸­çå¾æ½åå®¹ï¼å¯å¤ä¸ªï¼ç¨ç©ºæ ¼åéï¼ï¼éæ½å é¤
+<ç»å·> <åå®¹> å é¤æå®ç»å·çéæ½ç»ï¼éæ½ç»å é¤ <ç»å·>
 æ¥çæ¬ç¾¤ææçéæ½ç»åå®¹ï¼å«ç»å·åç»åï¼ï¼éæ½ç»åè¡¨
 æ¥çæå®ç»å·çææå¾æ½åå®¹ï¼éæ½åè¡¨ <ç»å·>
 å¨æå®éæ½ç»ä¸­éæºæ½åä¸ä¸ªå¾æ½åå®¹ï¼éæ½ <ç»å·>
 æ¸ç©ºæ¬ç¾¤ä¸­ææçéæ½ç»ï¼æç¨ï¼ï¼éæ½ç»æ¸ç©º
 æ¸ç©ºæå®éæ½ç»ä¸­ææçå¾æ½åå®¹ï¼æç¨ï¼ï¼éæ½æ¸ç©º
 <ç»å·> ``` ### å¶ä»å½ä»¤æå¾åäºï¼ç´æ¥çå¾å§ ![](docs/
 result.png) ## â æå± ## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 0.0.1 -
-æä»¶åæ¬¡åå¸  ## è´è°¢ - [nonebot-plugin-template](https://github.com/A-
-kirami/nonebot-plugin-template) ## é¡¹ç®æåä¸ä¼ è³pypi å®ç½ï¼https://
+æä»¶åæ¬¡åå¸ ### 0.0.2 - å¢å æ¹éæ·»å åå é¤åå®¹çåè½  ##
+è´è°¢ - [nonebot-plugin-template](https://github.com/A-kirami/nonebot-plugin-
+template) ## é¡¹ç®æåä¸ä¼ è³pypi å®ç½ï¼https://
 pypi.orgï¼æ³¨åè´¦å·ï¼å¨ç³»ç»ç¨æ·æ ¹ç®å½ä¸åå»º`.pypirc`ï¼éç½®
 ``` [distutils] index-servers=pypi [pypi] repository = https://upload.pypi.org/
 legacy/ username = ç¨æ·å password = å¯ç  ``` ### poetry ``` # åè
 https://www.freesion.com/article/58051228882/ # poetry config pypi-token.pypi #
 1ãå®è£poetry pip install poetry #
 2ãåå§åéç½®æä»¶ï¼æ ¹æ®æç¤ºå¡«åï¼ poetry init #
 3ãå¾®è°éç½®æä»¶pyproject.toml # 4ãè¿è¡ poetry install, å¯çæ
```

