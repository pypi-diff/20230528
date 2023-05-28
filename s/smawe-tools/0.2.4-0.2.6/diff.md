# Comparing `tmp/smawe_tools-0.2.4.tar.gz` & `tmp/smawe_tools-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smawe_tools-0.2.4.tar", last modified: Thu Apr  6 12:28:17 2023, max compression
+gzip compressed data, was "smawe_tools-0.2.6.tar", last modified: Sun May 28 10:29:16 2023, max compression
```

## Comparing `smawe_tools-0.2.4.tar` & `smawe_tools-0.2.6.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 12:28:17.548912 smawe_tools-0.2.4/
--rw-rw-rw-   0        0        0     1091 2023-01-15 03:19:33.000000 smawe_tools-0.2.4/LICENSE
--rw-rw-rw-   0        0        0     4922 2023-04-06 12:28:17.547913 smawe_tools-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     4445 2023-04-06 12:27:07.000000 smawe_tools-0.2.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-06 12:28:17.548912 smawe_tools-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1019 2023-04-04 10:22:33.000000 smawe_tools-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-06 12:28:17.527913 smawe_tools-0.2.4/smawe_tools/
--rw-rw-rw-   0        0        0      194 2023-04-04 09:49:25.000000 smawe_tools-0.2.4/smawe_tools/__init__.py
--rw-rw-rw-   0        0        0       76 2023-04-06 12:27:07.000000 smawe_tools-0.2.4/smawe_tools/__version__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 12:28:17.537913 smawe_tools-0.2.4/smawe_tools/exception/
--rw-rw-rw-   0        0        0       98 2023-04-02 12:50:55.000000 smawe_tools-0.2.4/smawe_tools/exception/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 12:28:17.540913 smawe_tools-0.2.4/smawe_tools/net/
--rw-rw-rw-   0        0        0       29 2023-03-29 05:15:59.000000 smawe_tools-0.2.4/smawe_tools/net/__init__.py
--rw-rw-rw-   0        0        0     2905 2023-04-04 10:22:33.000000 smawe_tools-0.2.4/smawe_tools/net/network_tool.py
-drwxrwxrwx   0        0        0        0 2023-04-06 12:28:17.543913 smawe_tools-0.2.4/smawe_tools/retrying/
--rw-rw-rw-   0        0        0       26 2023-04-04 07:07:45.000000 smawe_tools-0.2.4/smawe_tools/retrying/__init__.py
--rw-rw-rw-   0        0        0     2889 2023-04-04 14:50:18.000000 smawe_tools-0.2.4/smawe_tools/retrying/retry.py
--rw-rw-rw-   0        0        0      654 2023-04-04 09:21:43.000000 smawe_tools-0.2.4/smawe_tools/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-06 12:28:17.544913 smawe_tools-0.2.4/smawe_tools/struct/
--rw-rw-rw-   0        0        0      946 2023-04-06 10:03:49.000000 smawe_tools-0.2.4/smawe_tools/struct/__init__.py
--rw-rw-rw-   0        0        0     2842 2023-03-19 15:58:44.000000 smawe_tools-0.2.4/smawe_tools/tool.py
-drwxrwxrwx   0        0        0        0 2023-04-06 12:28:17.535912 smawe_tools-0.2.4/smawe_tools.egg-info/
--rw-rw-rw-   0        0        0     4922 2023-04-06 12:28:17.000000 smawe_tools-0.2.4/smawe_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      497 2023-04-06 12:28:17.000000 smawe_tools-0.2.4/smawe_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 12:28:17.000000 smawe_tools-0.2.4/smawe_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-06 12:28:17.000000 smawe_tools-0.2.4/smawe_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-06 12:28:17.000000 smawe_tools-0.2.4/smawe_tools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-06 12:28:17.545914 smawe_tools-0.2.4/tests/
--rw-rw-rw-   0        0        0       79 2023-04-06 12:20:07.000000 smawe_tools-0.2.4/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:29:16.507922 smawe_tools-0.2.6/
+-rw-rw-rw-   0        0        0     1091 2023-01-15 03:19:33.000000 smawe_tools-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0     5955 2023-05-28 10:29:16.506919 smawe_tools-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5478 2023-05-27 14:13:31.000000 smawe_tools-0.2.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-28 10:29:16.507922 smawe_tools-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1019 2023-04-04 10:22:33.000000 smawe_tools-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:29:16.488070 smawe_tools-0.2.6/smawe_tools/
+-rw-rw-rw-   0        0        0      194 2023-05-27 14:06:38.000000 smawe_tools-0.2.6/smawe_tools/__init__.py
+-rw-rw-rw-   0        0        0       76 2023-05-28 10:27:58.000000 smawe_tools-0.2.6/smawe_tools/__version__.py
+-rw-rw-rw-   0        0        0     6799 2023-05-28 10:27:58.000000 smawe_tools-0.2.6/smawe_tools/config.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:29:16.496749 smawe_tools-0.2.6/smawe_tools/exception/
+-rw-rw-rw-   0        0        0       98 2023-04-02 12:50:55.000000 smawe_tools-0.2.6/smawe_tools/exception/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:29:16.500027 smawe_tools-0.2.6/smawe_tools/net/
+-rw-rw-rw-   0        0        0       29 2023-03-29 05:15:59.000000 smawe_tools-0.2.6/smawe_tools/net/__init__.py
+-rw-rw-rw-   0        0        0     2905 2023-04-04 10:22:33.000000 smawe_tools-0.2.6/smawe_tools/net/network_tool.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:29:16.502919 smawe_tools-0.2.6/smawe_tools/retrying/
+-rw-rw-rw-   0        0        0       26 2023-04-04 07:07:45.000000 smawe_tools-0.2.6/smawe_tools/retrying/__init__.py
+-rw-rw-rw-   0        0        0     2889 2023-04-09 10:10:02.000000 smawe_tools-0.2.6/smawe_tools/retrying/retry.py
+-rw-rw-rw-   0        0        0      670 2023-04-18 02:48:31.000000 smawe_tools-0.2.6/smawe_tools/settings.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:29:16.503922 smawe_tools-0.2.6/smawe_tools/struct/
+-rw-rw-rw-   0        0        0      946 2023-04-06 10:03:49.000000 smawe_tools-0.2.6/smawe_tools/struct/__init__.py
+-rw-rw-rw-   0        0        0     2842 2023-04-19 07:48:57.000000 smawe_tools-0.2.6/smawe_tools/tool.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:29:16.495750 smawe_tools-0.2.6/smawe_tools.egg-info/
+-rw-rw-rw-   0        0        0     5955 2023-05-28 10:29:16.000000 smawe_tools-0.2.6/smawe_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      519 2023-05-28 10:29:16.000000 smawe_tools-0.2.6/smawe_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 10:29:16.000000 smawe_tools-0.2.6/smawe_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-28 10:29:16.000000 smawe_tools-0.2.6/smawe_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-28 10:29:16.000000 smawe_tools-0.2.6/smawe_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 10:29:16.505922 smawe_tools-0.2.6/tests/
+-rw-rw-rw-   0        0        0     1512 2023-05-28 10:19:26.000000 smawe_tools-0.2.6/tests/test.py
```

### Comparing `smawe_tools-0.2.4/LICENSE` & `smawe_tools-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.2.4/PKG-INFO` & `smawe_tools-0.2.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,24 @@
-Metadata-Version: 2.1
-Name: smawe_tools
-Version: 0.2.4
-Summary: small tool
-Author: Samwe
-Author-email: 1281722462@qq.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.5.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ### ***本文档是由作者本人编写，难免会出现一些小问题，例如打错字等，发现后会及时改正***
-## 核心功能
-
-> 提供了一个rename()函数, 对目录中的文件进行重命名  
-格式为第xxx章  
-第某某章必须在一亿章以下  
-例如:  
-    &ensp;&ensp;&ensp;&ensp;第一百章.txt -> 第100章.txt   
-    &ensp;&ensp;&ensp;&ensp;第两千零一章.txt -> 第2001章.txt
 
 ---
 
 ### **核心函数**
 以下函数都可以从smawe_tools包中进行导入  
 例如: from smawe_tools import retry  
+
+- rename(src=""):  
+    对src路径指定的目录中的文件进行重命名  
+    格式为第xxx章  
+    第某某章必须在一亿章以下  
+    例如:  
+        &ensp;&ensp;&ensp;&ensp;第一百章.txt -> 第100章.txt   
+        &ensp;&ensp;&ensp;&ensp;第两千零一章.txt -> 第2001章.txt  
+
+
 - text_conversion(s):  
     功能: 文本转换  
     描述: 如果s为空, 则返回0.  
     参数s: str
     返回值: 整数
     列如:  
         &ensp;&ensp;&ensp;&ensp;两千零一 -> 2001  
@@ -54,19 +41,19 @@
     stop_max_attempt_number: 停止时的最大重试次数，超出次数后还发生异常，则抛出MaxRetryError异常  
     wait_random_min：随机等待的最小时间(单位毫秒)  
     wait_random_max: 随机等待的最大时间(单位毫秒)  
     retry_exception: 要重试的异常类型，默认为Exception
   
 - modify_encoding():   
     此函数要从smawe_tools.settings模块进行导入, 如: 
-    ```
+    ~~~ python
     from smawe_tools.settings import modify_encoding 
     # 直接调用即可
     modify_encoding()  
-    ```
+    ~~~
     调用此函数可以修正以下此类的错误:  
     UnicodeEncodeError: 'gbk' codec can't encode character '\xa0' in position 188608: illegal multibyte sequence
     
 ---
 
 **启用默认日志**  
 *默认日志级别为logging.INFO*
@@ -119,14 +106,15 @@
     ...     pass
     ... # 如果发生异常，则进行重试，每次重试前休眠1-3s的随机时间
     ...
     >>>
 
 ---
 #### 示例2
+
     >>> from smawe_tools import retry
     >>> @retry(3, 1000, 2000, ValueError)
     ... def test(a, b):
     ...     print(1)
     ...     print(2)
     ...     print(a, b)
     ...     raise ValueError()
@@ -136,7 +124,43 @@
     ... def test(a, b):
     ...     print(1)
     ...     print(2)
     ...     print(a, b)
     ...     raise ValueError()
     ...
     >>> test(1, 2) #发生IndexError就进行重试
+
+---
+此包还提供了一个对配置进行读取和保存的子模块smawe_tools.config  
+简单使用如下:  
+```python
+from smawe_tools.config import Config
+
+config = Config()
+# 切换节，设置选项和值
+config.switch_to_section("s1").set("k1", "v1")
+config.switch_to_section("s2").set("k2", "v2")
+config.switch_to_section("s3").set("k3", "v3")
+# 切换到默认节"DEFAULT"
+config.switch_to_section("DEFAULT").set("accept", "true")
+# 保存配置
+config.save_config("test.ini")
+```
+读取配置
+
+```python
+from smawe_tools.config import Config
+
+config = Config()
+config.read_config("test.ini")
+# 获取配置中的值
+print(config.get("s1", "k1"))
+print(config.get("s1", "kk1", fallback="vv2"))
+# 获取默认节中的值, 将其转为布尔值
+print(config.get_boolean("s1", "accept"))
+
+# 将其它值转为布尔值
+config.boolean_states = {"access": "agree"}
+
+config.set("s1", "can", "access")
+print(config.switch_to_section("s1").get_boolean("can"))
+```
```

### Comparing `smawe_tools-0.2.4/setup.py` & `smawe_tools-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.2.4/smawe_tools/net/network_tool.py` & `smawe_tools-0.2.6/smawe_tools/net/network_tool.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.2.4/smawe_tools/retrying/retry.py` & `smawe_tools-0.2.6/smawe_tools/retrying/retry.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.2.4/smawe_tools/settings.py` & `smawe_tools-0.2.6/smawe_tools/settings.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 except ModuleNotFoundError:
     pass
 
 _IS_LESS_THEN_PY39 = float(".".join(platform.python_version_tuple()[:-1])) < 3.9
 if _IS_LESS_THEN_PY39:
     import typing
     List = typing.List
+    del typing
 else:
     List = list
 
 # 'Linux', 'Darwin', 'Java', 'Windows'
 OS_NAME = platform.system()
```

### Comparing `smawe_tools-0.2.4/smawe_tools/struct/__init__.py` & `smawe_tools-0.2.6/smawe_tools/struct/__init__.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.2.4/smawe_tools/tool.py` & `smawe_tools-0.2.6/smawe_tools/tool.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.2.4/smawe_tools.egg-info/PKG-INFO` & `smawe_tools-0.2.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
-Name: smawe-tools
-Version: 0.2.4
+Name: smawe_tools
+Version: 0.2.6
 Summary: small tool
 Author: Samwe
 Author-email: 1281722462@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.5.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### ***本文档是由作者本人编写，难免会出现一些小问题，例如打错字等，发现后会及时改正***
-## 核心功能
-
-> 提供了一个rename()函数, 对目录中的文件进行重命名  
-格式为第xxx章  
-第某某章必须在一亿章以下  
-例如:  
-    &ensp;&ensp;&ensp;&ensp;第一百章.txt -> 第100章.txt   
-    &ensp;&ensp;&ensp;&ensp;第两千零一章.txt -> 第2001章.txt
 
 ---
 
 ### **核心函数**
 以下函数都可以从smawe_tools包中进行导入  
 例如: from smawe_tools import retry  
+
+- rename(src=""):  
+    对src路径指定的目录中的文件进行重命名  
+    格式为第xxx章  
+    第某某章必须在一亿章以下  
+    例如:  
+        &ensp;&ensp;&ensp;&ensp;第一百章.txt -> 第100章.txt   
+        &ensp;&ensp;&ensp;&ensp;第两千零一章.txt -> 第2001章.txt  
+
+
 - text_conversion(s):  
     功能: 文本转换  
     描述: 如果s为空, 则返回0.  
     参数s: str
     返回值: 整数
     列如:  
         &ensp;&ensp;&ensp;&ensp;两千零一 -> 2001  
@@ -54,19 +56,19 @@
     stop_max_attempt_number: 停止时的最大重试次数，超出次数后还发生异常，则抛出MaxRetryError异常  
     wait_random_min：随机等待的最小时间(单位毫秒)  
     wait_random_max: 随机等待的最大时间(单位毫秒)  
     retry_exception: 要重试的异常类型，默认为Exception
   
 - modify_encoding():   
     此函数要从smawe_tools.settings模块进行导入, 如: 
-    ```
+    ~~~ python
     from smawe_tools.settings import modify_encoding 
     # 直接调用即可
     modify_encoding()  
-    ```
+    ~~~
     调用此函数可以修正以下此类的错误:  
     UnicodeEncodeError: 'gbk' codec can't encode character '\xa0' in position 188608: illegal multibyte sequence
     
 ---
 
 **启用默认日志**  
 *默认日志级别为logging.INFO*
@@ -119,14 +121,15 @@
     ...     pass
     ... # 如果发生异常，则进行重试，每次重试前休眠1-3s的随机时间
     ...
     >>>
 
 ---
 #### 示例2
+
     >>> from smawe_tools import retry
     >>> @retry(3, 1000, 2000, ValueError)
     ... def test(a, b):
     ...     print(1)
     ...     print(2)
     ...     print(a, b)
     ...     raise ValueError()
@@ -136,7 +139,43 @@
     ... def test(a, b):
     ...     print(1)
     ...     print(2)
     ...     print(a, b)
     ...     raise ValueError()
     ...
     >>> test(1, 2) #发生IndexError就进行重试
+
+---
+此包还提供了一个对配置进行读取和保存的子模块smawe_tools.config  
+简单使用如下:  
+```python
+from smawe_tools.config import Config
+
+config = Config()
+# 切换节，设置选项和值
+config.switch_to_section("s1").set("k1", "v1")
+config.switch_to_section("s2").set("k2", "v2")
+config.switch_to_section("s3").set("k3", "v3")
+# 切换到默认节"DEFAULT"
+config.switch_to_section("DEFAULT").set("accept", "true")
+# 保存配置
+config.save_config("test.ini")
+```
+读取配置
+
+```python
+from smawe_tools.config import Config
+
+config = Config()
+config.read_config("test.ini")
+# 获取配置中的值
+print(config.get("s1", "k1"))
+print(config.get("s1", "kk1", fallback="vv2"))
+# 获取默认节中的值, 将其转为布尔值
+print(config.get_boolean("s1", "accept"))
+
+# 将其它值转为布尔值
+config.boolean_states = {"access": "agree"}
+
+config.set("s1", "can", "access")
+print(config.switch_to_section("s1").get_boolean("can"))
+```
```

