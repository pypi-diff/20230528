# Comparing `tmp/promptlayer-0.1.82.tar.gz` & `tmp/promptlayer-0.1.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/promptlayer-0.1.82.tar", last modified: Wed May 24 19:32:30 2023, max compression
+gzip compressed data, was "dist/promptlayer-0.1.83.tar", last modified: Sun May 28 18:41:21 2023, max compression
```

## Comparing `promptlayer-0.1.82.tar` & `promptlayer-0.1.83.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-24 19:32:30.496979 promptlayer-0.1.82/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    11357 2023-01-26 22:51:29.000000 promptlayer-0.1.82/LICENSE
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-05-24 19:32:30.496641 promptlayer-0.1.82/PKG-INFO
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3891 2023-01-26 22:51:29.000000 promptlayer-0.1.82/README.md
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-24 19:32:30.490775 promptlayer-0.1.82/promptlayer/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      496 2023-05-24 19:31:54.000000 promptlayer-0.1.82/promptlayer/__init__.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-24 19:32:30.492558 promptlayer-0.1.82/promptlayer/langchain/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        0 2023-02-01 20:15:14.000000 promptlayer-0.1.82/promptlayer/langchain/__init__.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-24 19:32:30.493140 promptlayer-0.1.82/promptlayer/langchain/llms/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       26 2023-02-01 20:08:36.000000 promptlayer-0.1.82/promptlayer/langchain/llms/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     2012 2023-02-15 16:07:17.000000 promptlayer-0.1.82/promptlayer/langchain/llms/openai.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     2689 2023-03-27 21:24:30.000000 promptlayer-0.1.82/promptlayer/promptlayer.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-24 19:32:30.494162 promptlayer-0.1.82/promptlayer/prompts/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      124 2023-02-16 22:50:19.000000 promptlayer-0.1.82/promptlayer/prompts/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1285 2023-03-31 18:02:42.000000 promptlayer-0.1.82/promptlayer/prompts/prompts.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-24 19:32:30.495293 promptlayer-0.1.82/promptlayer/track/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       59 2023-03-13 20:43:03.000000 promptlayer-0.1.82/promptlayer/track/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1239 2023-05-12 18:10:56.000000 promptlayer-0.1.82/promptlayer/track/track.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    13445 2023-05-24 19:31:54.000000 promptlayer-0.1.82/promptlayer/utils.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-24 19:32:30.492224 promptlayer-0.1.82/promptlayer.egg-info/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-05-24 19:32:30.000000 promptlayer-0.1.82/promptlayer.egg-info/PKG-INFO
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      502 2023-05-24 19:32:30.000000 promptlayer-0.1.82/promptlayer.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        1 2023-05-24 19:32:30.000000 promptlayer-0.1.82/promptlayer.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       26 2023-05-24 19:32:30.000000 promptlayer-0.1.82/promptlayer.egg-info/requires.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       12 2023-05-24 19:32:30.000000 promptlayer-0.1.82/promptlayer.egg-info/top_level.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       38 2023-05-24 19:32:30.497134 promptlayer-0.1.82/setup.cfg
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      832 2023-05-24 19:32:04.000000 promptlayer-0.1.82/setup.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-28 18:41:21.419518 promptlayer-0.1.83/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    11357 2023-01-26 22:51:29.000000 promptlayer-0.1.83/LICENSE
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-05-28 18:41:21.419171 promptlayer-0.1.83/PKG-INFO
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3891 2023-01-26 22:51:29.000000 promptlayer-0.1.83/README.md
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-28 18:41:21.410863 promptlayer-0.1.83/promptlayer/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      496 2023-05-24 19:31:54.000000 promptlayer-0.1.83/promptlayer/__init__.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-28 18:41:21.414068 promptlayer-0.1.83/promptlayer/langchain/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        0 2023-02-01 20:15:14.000000 promptlayer-0.1.83/promptlayer/langchain/__init__.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-28 18:41:21.415305 promptlayer-0.1.83/promptlayer/langchain/llms/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       26 2023-02-01 20:08:36.000000 promptlayer-0.1.83/promptlayer/langchain/llms/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     2012 2023-02-15 16:07:17.000000 promptlayer-0.1.83/promptlayer/langchain/llms/openai.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     2689 2023-03-27 21:24:30.000000 promptlayer-0.1.83/promptlayer/promptlayer.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-28 18:41:21.416686 promptlayer-0.1.83/promptlayer/prompts/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      124 2023-02-16 22:50:19.000000 promptlayer-0.1.83/promptlayer/prompts/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1285 2023-03-31 18:02:42.000000 promptlayer-0.1.83/promptlayer/prompts/prompts.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-28 18:41:21.418259 promptlayer-0.1.83/promptlayer/track/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       59 2023-03-13 20:43:03.000000 promptlayer-0.1.83/promptlayer/track/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1239 2023-05-12 18:10:56.000000 promptlayer-0.1.83/promptlayer/track/track.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    13445 2023-05-24 19:31:54.000000 promptlayer-0.1.83/promptlayer/utils.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-28 18:41:21.413598 promptlayer-0.1.83/promptlayer.egg-info/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-05-28 18:41:21.000000 promptlayer-0.1.83/promptlayer.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      502 2023-05-28 18:41:21.000000 promptlayer-0.1.83/promptlayer.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        1 2023-05-28 18:41:21.000000 promptlayer-0.1.83/promptlayer.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       36 2023-05-28 18:41:21.000000 promptlayer-0.1.83/promptlayer.egg-info/requires.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       12 2023-05-28 18:41:21.000000 promptlayer-0.1.83/promptlayer.egg-info/top_level.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       38 2023-05-28 18:41:21.419626 promptlayer-0.1.83/setup.cfg
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      860 2023-05-28 18:40:49.000000 promptlayer-0.1.83/setup.py
```

### Comparing `promptlayer-0.1.82/LICENSE` & `promptlayer-0.1.83/LICENSE`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.82/PKG-INFO` & `promptlayer-0.1.83/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptlayer
-Version: 0.1.82
+Version: 0.1.83
 Summary: PromptLayer is a package to keep track of your GPT models training
 Home-page: https://www.promptlayer.com
 Author: Magniv
 Author-email: hello@magniv.io
 License: UNKNOWN
 Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: promptlayer Version: 0.1.82 Summary: PromptLayer is
+Metadata-Version: 2.1 Name: promptlayer Version: 0.1.83 Summary: PromptLayer is
 a package to keep track of your GPT models training Home-page: https://
 www.promptlayer.com Author: Magniv Author-email: hello@magniv.io License:
 UNKNOWN Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-
 Docs-db0e6f50cacf4564a6d09824ba17a629 Description:
 # ð° PromptLayer **The first platform built for prompt engineers** [Python]
                           [Docs] [Demo_with_Loom] ---
 [PromptLayer](https://promptlayer.com/) is the first platform that allows you
```

### Comparing `promptlayer-0.1.82/README.md` & `promptlayer-0.1.83/README.md`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.82/promptlayer/langchain/llms/openai.py` & `promptlayer-0.1.83/promptlayer/langchain/llms/openai.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.82/promptlayer/promptlayer.py` & `promptlayer-0.1.83/promptlayer/promptlayer.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.82/promptlayer/prompts/prompts.py` & `promptlayer-0.1.83/promptlayer/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.82/promptlayer/track/track.py` & `promptlayer-0.1.83/promptlayer/track/track.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.82/promptlayer/utils.py` & `promptlayer-0.1.83/promptlayer/utils.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.82/promptlayer.egg-info/PKG-INFO` & `promptlayer-0.1.83/promptlayer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptlayer
-Version: 0.1.82
+Version: 0.1.83
 Summary: PromptLayer is a package to keep track of your GPT models training
 Home-page: https://www.promptlayer.com
 Author: Magniv
 Author-email: hello@magniv.io
 License: UNKNOWN
 Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: promptlayer Version: 0.1.82 Summary: PromptLayer is
+Metadata-Version: 2.1 Name: promptlayer Version: 0.1.83 Summary: PromptLayer is
 a package to keep track of your GPT models training Home-page: https://
 www.promptlayer.com Author: Magniv Author-email: hello@magniv.io License:
 UNKNOWN Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-
 Docs-db0e6f50cacf4564a6d09824ba17a629 Description:
 # ð° PromptLayer **The first platform built for prompt engineers** [Python]
                           [Docs] [Demo_with_Loom] ---
 [PromptLayer](https://promptlayer.com/) is the first platform that allows you
```

### Comparing `promptlayer-0.1.82/setup.py` & `promptlayer-0.1.83/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from setuptools import find_packages, setup
 
 try:
     # read the contents of your README file
     from pathlib import Path
+
     this_directory = Path(__file__).parent
     long_description = (this_directory / "README.md").read_text()
 except:
     long_description = ""
 
 setup(
     name="promptlayer",
     description="PromptLayer is a package to keep track of your GPT models training",
     long_description=long_description,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     author="Magniv",
     author_email="hello@magniv.io",
     url="https://www.promptlayer.com",
-    project_urls={"Documentation": "https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629",},
-    version="0.1.82",
+    project_urls={
+        "Documentation": "https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629",
+    },
+    version="0.1.83",
     py_modules=["promptlayer"],
     packages=find_packages(),
-    install_requires=["requests", "openai", "langchain"],
+    install_requires=["requests", "openai", "langchain", "anthropic"],
 )
```

