# Comparing `tmp/ChatGPTWeb-0.0.8.tar.gz` & `tmp/ChatGPTWeb-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChatGPTWeb-0.0.8.tar", last modified: Fri May 19 06:22:32 2023, max compression
+gzip compressed data, was "ChatGPTWeb-0.0.9.tar", last modified: Sun May 28 12:31:45 2023, max compression
```

## Comparing `ChatGPTWeb-0.0.8.tar` & `ChatGPTWeb-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 06:22:32.237189 ChatGPTWeb-0.0.8/
-drwxrwxrwx   0        0        0        0 2023-05-19 06:22:32.232193 ChatGPTWeb-0.0.8/ChatGPTWeb/
--rw-rw-rw-   0        0        0    23949 2023-05-19 06:02:57.000000 ChatGPTWeb-0.0.8/ChatGPTWeb/ChatGPTWeb.py
--rw-rw-rw-   0        0        0       56 2023-04-08 08:59:30.000000 ChatGPTWeb-0.0.8/ChatGPTWeb/__init__.py
--rw-rw-rw-   0        0        0     1998 2023-05-19 06:20:46.000000 ChatGPTWeb-0.0.8/ChatGPTWeb/__main__.py
--rw-rw-rw-   0        0        0     6418 2023-05-19 06:18:09.000000 ChatGPTWeb-0.0.8/ChatGPTWeb/config.py
-drwxrwxrwx   0        0        0        0 2023-05-19 06:22:32.235190 ChatGPTWeb-0.0.8/ChatGPTWeb.egg-info/
--rw-rw-rw-   0        0        0     3516 2023-05-19 06:22:32.000000 ChatGPTWeb-0.0.8/ChatGPTWeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-05-19 06:22:32.000000 ChatGPTWeb-0.0.8/ChatGPTWeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 06:22:32.000000 ChatGPTWeb-0.0.8/ChatGPTWeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-19 06:22:32.000000 ChatGPTWeb-0.0.8/ChatGPTWeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-19 06:22:32.000000 ChatGPTWeb-0.0.8/ChatGPTWeb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-04-07 06:03:43.000000 ChatGPTWeb-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     3516 2023-05-19 06:22:32.236191 ChatGPTWeb-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3161 2023-04-13 13:42:59.000000 ChatGPTWeb-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-05-19 06:22:32.237189 ChatGPTWeb-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      660 2023-05-19 06:21:44.000000 ChatGPTWeb-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:31:45.591768 ChatGPTWeb-0.0.9/
+drwxrwxrwx   0        0        0        0 2023-05-28 12:31:45.585257 ChatGPTWeb-0.0.9/ChatGPTWeb/
+-rw-rw-rw-   0        0        0    23995 2023-05-28 12:31:06.000000 ChatGPTWeb-0.0.9/ChatGPTWeb/ChatGPTWeb.py
+-rw-rw-rw-   0        0        0       56 2023-04-08 08:59:30.000000 ChatGPTWeb-0.0.9/ChatGPTWeb/__init__.py
+-rw-rw-rw-   0        0        0     1998 2023-05-19 06:20:46.000000 ChatGPTWeb-0.0.9/ChatGPTWeb/__main__.py
+-rw-rw-rw-   0        0        0     6418 2023-05-19 06:18:09.000000 ChatGPTWeb-0.0.9/ChatGPTWeb/config.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:31:45.589767 ChatGPTWeb-0.0.9/ChatGPTWeb.egg-info/
+-rw-rw-rw-   0        0        0     3516 2023-05-28 12:31:45.000000 ChatGPTWeb-0.0.9/ChatGPTWeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-05-28 12:31:45.000000 ChatGPTWeb-0.0.9/ChatGPTWeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 12:31:45.000000 ChatGPTWeb-0.0.9/ChatGPTWeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-28 12:31:45.000000 ChatGPTWeb-0.0.9/ChatGPTWeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-28 12:31:45.000000 ChatGPTWeb-0.0.9/ChatGPTWeb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-04-07 06:03:43.000000 ChatGPTWeb-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3516 2023-05-28 12:31:45.590768 ChatGPTWeb-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3161 2023-04-13 13:42:59.000000 ChatGPTWeb-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-28 12:31:45.591768 ChatGPTWeb-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      660 2023-05-28 12:31:33.000000 ChatGPTWeb-0.0.9/setup.py
```

### Comparing `ChatGPTWeb-0.0.8/ChatGPTWeb/ChatGPTWeb.py` & `ChatGPTWeb-0.0.9/ChatGPTWeb/ChatGPTWeb.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                 "value": x
             } for x in session_token]
         else:
             raise ValueError("session_token is empty!")
         self.manage = {
             "start":False,
             "browser_contexts":[],
-            "access_token":[],
+            "access_token":["" for x in range(0,len(self.cookie))],
             "status":{}
         }
         
         '''start:bool 全部启动完毕
         
         browser_contexts：list 浏览器环境列表
         
@@ -258,15 +258,15 @@
                 access_token = json_data['accessToken']
             except:
                 access_token = None
                 self.logger.debug(f"{str(context_index)}'s have cf checkbox?retry {str(retry)} ")
             #await page.screenshot(path=f"{str(context_index)}'s have cf checkbox?retry {str(retry)} .png")
             #continue
             
-        self.manage["access_token"].append(access_token)
+        self.manage["access_token"][context_index] = access_token
         if access_token:
             self.manage["status"][str(context_index)] = True
             self.logger.info(f"context {context_index} start!")
         else:
             self.manage["status"][str(context_index)] = False
             await page.screenshot(path=f"context {context_index} faild!.png")
             self.logger.info(f"context {context_index} faild!")
```

### Comparing `ChatGPTWeb-0.0.8/ChatGPTWeb/__main__.py` & `ChatGPTWeb-0.0.9/ChatGPTWeb/__main__.py`

 * *Files identical despite different names*

### Comparing `ChatGPTWeb-0.0.8/ChatGPTWeb/config.py` & `ChatGPTWeb-0.0.9/ChatGPTWeb/config.py`

 * *Files identical despite different names*

### Comparing `ChatGPTWeb-0.0.8/ChatGPTWeb.egg-info/PKG-INFO` & `ChatGPTWeb-0.0.9/ChatGPTWeb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatGPTWeb
-Version: 0.0.8
+Version: 0.0.9
 Summary: a ChatGPT API,no web ui
 Home-page: https://github.com/nek0us/ChatGPT
 Author: nek0us
 Author-email: nekouss@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `ChatGPTWeb-0.0.8/LICENSE` & `ChatGPTWeb-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ChatGPTWeb-0.0.8/PKG-INFO` & `ChatGPTWeb-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatGPTWeb
-Version: 0.0.8
+Version: 0.0.9
 Summary: a ChatGPT API,no web ui
 Home-page: https://github.com/nek0us/ChatGPT
 Author: nek0us
 Author-email: nekouss@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `ChatGPTWeb-0.0.8/README.md` & `ChatGPTWeb-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ChatGPTWeb-0.0.8/setup.py` & `ChatGPTWeb-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r",encoding="utf8") as readme_file:
     readme = readme_file.read()
 
 requirements = ["playwright","aioconsole"] 
 
 setup(
     name="ChatGPTWeb",
-    version="0.0.8",
+    version="0.0.9",
     author="nek0us",
     author_email="nekouss@gmail.com",
     description="a ChatGPT API,no web ui",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/nek0us/ChatGPT",
     packages=find_packages(),
```

