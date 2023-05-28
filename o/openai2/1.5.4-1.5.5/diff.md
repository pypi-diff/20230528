# Comparing `tmp/openai2-1.5.4.tar.gz` & `tmp/openai2-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai2-1.5.4.tar", last modified: Tue May  2 03:05:00 2023, max compression
+gzip compressed data, was "openai2-1.5.5.tar", last modified: Sun May 28 04:57:48 2023, max compression
```

## Comparing `openai2-1.5.4.tar` & `openai2-1.5.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    10953 2023-03-07 16:01:05.491907 openai2-1.5.4/LICENSE
--rw-r--r--   0        0        0     2323 2023-05-02 03:00:54.676633 openai2-1.5.4/README.md
--rw-r--r--   0        0        0     1083 2020-12-22 18:45:03.000000 openai2-1.5.4/openai2/Licenses of dependent packages/openai/LICENSE
--rw-r--r--   0        0        0       25 2023-03-07 03:18:11.476857 openai2-1.5.4/openai2/__init__.py
--rw-r--r--   0        0        0     2047 2023-05-02 02:37:21.759092 openai2-1.5.4/openai2/openai2.py
--rw-r--r--   0        0        0      634 2023-05-02 03:01:32.472779 openai2-1.5.4/pyproject.toml
--rw-r--r--   0        0        0     2690 1970-01-01 00:00:00.000000 openai2-1.5.4/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-03-07 16:01:05.491907 openai2-1.5.5/LICENSE
+-rw-r--r--   0        0        0     2866 2023-05-28 04:47:47.511099 openai2-1.5.5/README.md
+-rw-r--r--   0        0        0     1083 2020-12-22 18:45:03.000000 openai2-1.5.5/openai2/Licenses of dependent packages/openai/LICENSE
+-rw-r--r--   0        0        0       25 2023-03-07 03:18:11.476857 openai2-1.5.5/openai2/__init__.py
+-rw-r--r--   0        0        0     2577 2023-05-28 04:22:51.712836 openai2-1.5.5/openai2/openai2.py
+-rw-r--r--   0        0        0      634 2023-05-28 04:50:00.858650 openai2-1.5.5/pyproject.toml
+-rw-r--r--   0        0        0     3238 1970-01-01 00:00:00.000000 openai2-1.5.5/PKG-INFO
```

### Comparing `openai2-1.5.4/LICENSE` & `openai2-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openai2-1.5.4/openai2/Licenses of dependent packages/openai/LICENSE` & `openai2-1.5.5/openai2/Licenses of dependent packages/openai/LICENSE`

 * *Files identical despite different names*

### Comparing `openai2-1.5.4/openai2/openai2.py` & `openai2-1.5.5/openai2/openai2.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,20 +27,34 @@
 
     def rollback(self, n=1):
         self.messages[-2*n:] = []
         for x in self.messages[-2:]:
             print(f"[{x['role']}]: {x['content']}")
     
     def request(self, text:str):
-        completion = openai.ChatCompletion.create(
-            api_key = self.api_key,
-            model = self.model,
-            messages = self.messages + [{"role": "user", "content": text}],
-             **self.kwargs
-        )
+        completion = openai.ChatCompletion.create(**{
+            'api_key': self.api_key,
+            'model': self.model,
+            'messages': self.messages + [{"role": "user", "content": text}],
+            **self.kwargs
+        })
+        answer:str = completion.choices[0].message['content']
+        self.messages += [
+            {"role": "user", "content": text},
+            {"role": "assistant", "content": answer}
+        ]
+        return answer
+
+    async def asy_request(self, text:str):
+        completion = await openai.ChatCompletion.acreate(**{
+            'api_key': self.api_key,
+            'model': self.model,
+            'messages': self.messages + [{"role": "user", "content": text}],
+            **self.kwargs
+        })
         answer:str = completion.choices[0].message['content']
         self.messages += [
             {"role": "user", "content": text},
             {"role": "assistant", "content": answer}
         ]
         return answer
```

### Comparing `openai2-1.5.4/pyproject.toml` & `openai2-1.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "openai2"
-version = "1.5.4"
+version = "1.5.5"
 description = "根据openai官方接口‘openai’改造的‘openai2’，比官方接口更好用一点。"
 dependencies = ["openai >=0.27.0"]
 keywords = ["openai2", "openai"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
```

### Comparing `openai2-1.5.4/PKG-INFO` & `openai2-1.5.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: openai2
-Version: 1.5.4
+Version: 1.5.5
 Summary: 根据openai官方接口‘openai’改造的‘openai2’，比官方接口更好用一点。
 Keywords: openai2,openai
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: openai >=0.27.0
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/openai2#readme
 
 # 项目描述
 
-根据openai官方接口‘openai’改造的‘openai2’，比官方接口更好用一点。
+根据 openai 官方接口‘openai’改造的‘openai2’，比官方接口更好用一点。
 
 # 安装
 
 ```
 pip install openai2
 ```
 
@@ -24,98 +24,93 @@
 
 [获取链接1](https://platform.openai.com/account/api-keys)
 
 [获取链接2](https://www.baidu.com/s?wd=%E8%8E%B7%E5%8F%96%20openai%20api_key)
 
 # 教程
 
-导入：
+##### 导入
 
 ```python
 from openai2 import Chat
 ```
 
-创建对话：
+##### 创建对话
 
 ```python
 api_key = 'api_key'  # 更换成自己的api_key
 
-talk_1 = Chat(api_key=api_key, model="gpt-3.5-turbo")
-talk_2 = Chat(api_key=api_key, model="gpt-3.5-turbo")
+Tony = Chat(api_key=api_key, model="gpt-3.5-turbo")
+Lucy = Chat(api_key=api_key, model="gpt-3.5-turbo")  # 每个实例可使用 相同 或者 不同 的api_key
 ```
 
-对话：
+##### 对话
 
 ```python
-talk_1.request('数字1的后面是几?')
-# >>> 2
-talk_2.request('数字101的后面是几?')
-# >>> 102
+Tony.request('数字1的后面是几?')  # >>> 2
+Lucy.request('数字101的后面是几?')  # >>> 102
 
-talk_1.request('再往后是几?')
-# >>> 3
-talk_2.request('再往后是几?')
-# >>> 103
+Tony.request('再往后是几?')  # >>> 3
+Lucy.request('再往后是几?')  # >>> 103
 ```
 
-存档：
+##### 存档
 
 ```python
-talk_1.dump('./talk_record.json')
+Tony.dump('./talk_record.json')
 ```
 
-载入存档：
+##### 载入存档
 
 ```python
-new_talk = Chat(api_key=api_key, model="gpt-3.5-turbo")
-new_talk.load('./talk_record.json')
-new_talk.request('再往后呢?')
-# >>> 4
+Jenny = Chat(api_key=api_key, model="gpt-3.5-turbo")
+Jenny.load('./talk_record.json')
+
+Jenny.request('再往后呢?')  # >>> 4
 ```
 
-对话回滚：
+##### 对话回滚
 
 ```python
-talk_4 = Chat(api_key=api_key, model="gpt-3.5-turbo")
-
-talk_4.request('数字1的后面是几?')
-# >>> 2
+Anna = Chat(api_key=api_key, model="gpt-3.5-turbo")
 
-talk_4.request('再往后是几?')
-# >>> 3
-
-talk_4.request('再往后呢?')
-# >>> 4
+Anna.request('数字1的后面是几?')  # >>> 2
+Anna.request('再往后是几?')  # >>> 3
+Anna.request('再往后呢?')  # >>> 4
 
 # 回滚
-talk_4.rollback()
-# >>> [user]: 再往后是几?
-# >>> [assistant]: 3
+Anna.rollback()  # >>> [user]:再往后是几?  [assistant]:3
 
 # 再回滚
-talk_4.rollback()
-# >>> [user]: 数字1的后面是几?
-# >>> [assistant]: 2
+Anna.rollback()  # >>> [user]:数字1的后面是几?  [assistant]:2
 
-talk_4.request('再往后是几?')
-# >>> 3
+Anna.request('再往后是几?')  # >>> 3
 ```
 
-修改api_key：
+注：
+
+执行1次 `Anna.rollback(n=10)` 等效于执行10次 `Anna.rollback()`  。
+
+##### 修改api_key
 
 ```python
-talk_4.api_key = 'new api_key'
+Anna.api_key = 'new api_key'
 ```
 
+##### 更多方法
+
+openai2.Chat 底层调用了 [openai.ChatCompletion.create](https://platform.openai.com/docs/api-reference/chat/create?lang=python)，在实例化时，支持 openai.ChatCompletion.create 的所有参数，例如：`Chat(api_key=api_key, model="gpt-3.5-turbo", max_tokens=100)` 。
+
 # Bug提交、功能提议
 
-您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg) 与我联系。
+您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg) 与我联系。
 
 # 关于作者
 
 作者：许灿标
 
 邮箱：lcctoor@outlook.com
 
-[主页](https://github.com/lcctoor/me/blob/main/home.md) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg) | [Python技术微信交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg)
+[主页](https://github.com/lcctoor/me#readme) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg) | [微信公众号](https://raw.githubusercontent.com/lcctoor/me/main/author/WechatSubscribeQR-max.jpg) | [Python技术微信交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg)
 
 开源项目：[让 Python 更简单一点](https://github.com/lcctoor/lccpy#readme)
+
```

