# Comparing `tmp/gptbase-0.1.tar.gz` & `tmp/gptbase-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptbase-0.1.tar", last modified: Sun May 28 09:10:11 2023, max compression
+gzip compressed data, was "gptbase-0.1.1.tar", last modified: Sun May 28 10:08:29 2023, max compression
```

## Comparing `gptbase-0.1.tar` & `gptbase-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ershan    (1000) ershan    (1000)        0 2023-05-28 09:10:11.007825 gptbase-0.1/
--rw-r--r--   0 ershan    (1000) ershan    (1000)     2061 2023-05-28 09:10:11.007825 gptbase-0.1/PKG-INFO
--rw-r--r--   0 ershan    (1000) ershan    (1000)     1620 2023-05-28 09:08:57.000000 gptbase-0.1/README.md
-drwxr-xr-x   0 ershan    (1000) ershan    (1000)        0 2023-05-28 09:10:11.007825 gptbase-0.1/gptbase/
--rw-r--r--   0 ershan    (1000) ershan    (1000)       80 2023-05-28 09:02:58.000000 gptbase-0.1/gptbase/__init__.py
--rw-r--r--   0 ershan    (1000) ershan    (1000)     1507 2023-05-28 09:02:05.000000 gptbase-0.1/gptbase/base.py
--rw-r--r--   0 ershan    (1000) ershan    (1000)     4234 2023-05-28 08:58:03.000000 gptbase-0.1/gptbase/basev2.py
--rw-r--r--   0 ershan    (1000) ershan    (1000)      409 2023-05-28 08:51:32.000000 gptbase-0.1/gptbase/chat.py
--rw-r--r--   0 ershan    (1000) ershan    (1000)      109 2023-05-28 09:02:18.000000 gptbase-0.1/gptbase/const.py
-drwxr-xr-x   0 ershan    (1000) ershan    (1000)        0 2023-05-28 09:10:11.007825 gptbase-0.1/gptbase.egg-info/
--rw-r--r--   0 ershan    (1000) ershan    (1000)     2061 2023-05-28 09:10:10.000000 gptbase-0.1/gptbase.egg-info/PKG-INFO
--rw-r--r--   0 ershan    (1000) ershan    (1000)      259 2023-05-28 09:10:10.000000 gptbase-0.1/gptbase.egg-info/SOURCES.txt
--rw-r--r--   0 ershan    (1000) ershan    (1000)        1 2023-05-28 09:10:10.000000 gptbase-0.1/gptbase.egg-info/dependency_links.txt
--rw-r--r--   0 ershan    (1000) ershan    (1000)       28 2023-05-28 09:10:10.000000 gptbase-0.1/gptbase.egg-info/requires.txt
--rw-r--r--   0 ershan    (1000) ershan    (1000)        8 2023-05-28 09:10:10.000000 gptbase-0.1/gptbase.egg-info/top_level.txt
--rw-r--r--   0 ershan    (1000) ershan    (1000)       38 2023-05-28 09:10:11.007825 gptbase-0.1/setup.cfg
--rw-r--r--   0 ershan    (1000) ershan    (1000)      782 2023-05-28 09:01:12.000000 gptbase-0.1/setup.py
+drwxr-xr-x   0 ershan    (1000) ershan    (1000)        0 2023-05-28 10:08:29.757326 gptbase-0.1.1/
+-rw-r--r--   0 ershan    (1000) ershan    (1000)     2143 2023-05-28 10:08:29.757326 gptbase-0.1.1/PKG-INFO
+-rw-r--r--   0 ershan    (1000) ershan    (1000)     1699 2023-05-28 09:17:00.000000 gptbase-0.1.1/README.md
+drwxr-xr-x   0 ershan    (1000) ershan    (1000)        0 2023-05-28 10:08:29.757326 gptbase-0.1.1/gptbase/
+-rw-r--r--   0 ershan    (1000) ershan    (1000)       80 2023-05-28 09:02:58.000000 gptbase-0.1.1/gptbase/__init__.py
+-rw-r--r--   0 ershan    (1000) ershan    (1000)     1507 2023-05-28 09:02:05.000000 gptbase-0.1.1/gptbase/base.py
+-rw-r--r--   0 ershan    (1000) ershan    (1000)     6529 2023-05-28 09:47:37.000000 gptbase-0.1.1/gptbase/basev2.py
+-rw-r--r--   0 ershan    (1000) ershan    (1000)      409 2023-05-28 08:51:32.000000 gptbase-0.1.1/gptbase/chat.py
+-rw-r--r--   0 ershan    (1000) ershan    (1000)      110 2023-05-28 09:47:37.000000 gptbase-0.1.1/gptbase/const.py
+drwxr-xr-x   0 ershan    (1000) ershan    (1000)        0 2023-05-28 10:08:29.757326 gptbase-0.1.1/gptbase.egg-info/
+-rw-r--r--   0 ershan    (1000) ershan    (1000)     2143 2023-05-28 10:08:29.000000 gptbase-0.1.1/gptbase.egg-info/PKG-INFO
+-rw-r--r--   0 ershan    (1000) ershan    (1000)      259 2023-05-28 10:08:29.000000 gptbase-0.1.1/gptbase.egg-info/SOURCES.txt
+-rw-r--r--   0 ershan    (1000) ershan    (1000)        1 2023-05-28 10:08:29.000000 gptbase-0.1.1/gptbase.egg-info/dependency_links.txt
+-rw-r--r--   0 ershan    (1000) ershan    (1000)       28 2023-05-28 10:08:29.000000 gptbase-0.1.1/gptbase.egg-info/requires.txt
+-rw-r--r--   0 ershan    (1000) ershan    (1000)        8 2023-05-28 10:08:29.000000 gptbase-0.1.1/gptbase.egg-info/top_level.txt
+-rw-r--r--   0 ershan    (1000) ershan    (1000)       38 2023-05-28 10:08:29.757326 gptbase-0.1.1/setup.cfg
+-rw-r--r--   0 ershan    (1000) ershan    (1000)      784 2023-05-28 10:07:58.000000 gptbase-0.1.1/setup.py
```

### Comparing `gptbase-0.1/PKG-INFO` & `gptbase-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,50 @@
-Metadata-Version: 2.1
-Name: gptbase
-Version: 0.1
-Summary: A package for simplified interaction with OpenAI's GPT-3 and GPT-4 models.
-Home-page: https://github.com/callmexss/gptbase
-Author: callmexss
-Author-email: callmexss@126.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
-# GPTBase
-
-Welcome to GPTBase, a Python library that provides a simple interface for using OpenAI's GPT-3.5-Turbo and GPT-4 models for text generation.
-
-## Features
-
-- Configurable parameters for chat completion.
-- Support for both individual prompts and chat conversations.
-- Stream output option for faster response times.
-- Inbuilt logging and rich printing for better visualization.
-- Customizable model choice, including GPT-3.5-Turbo, GPT-4, and other variants.
-- Easy model parameter adjustment.
+# 🚀 GPTBase
 
-## Installation
+Welcome to GPTBase! This Python library provides a straightforward and user-friendly interface to leverage OpenAI's powerful GPT-3.5-Turbo and GPT-4 models for text generation. 📚🔍
 
-You can install the GPTBase library from PyPI:
+## ✨ Features
 
-```
+- 🎛️ Configurable parameters for chat completion.
+- 💬 Support for both individual prompts and chat conversations.
+- ⚡ Stream output option for faster response times.
+- 📝 Built-in logging and rich printing for enhanced visualization.
+- 🔄 Customizable model choice, including GPT-3.5-Turbo, GPT-4, and other variants.
+- 📈 Easy model parameter adjustment.
+
+## 📦 Installation
+
+You can easily install the GPTBase library from PyPI with a single command line:
+
+```bash
 pip install gptbase
 ```
 
-Then import it in your Python script:
+Once installed, import it in your Python script:
 
 ```python
 from gptbase.basev2 import ChatAssistant, CompletionParameters
 ```
 
-## Usage
+## 📚 Usage
 
-The library includes two main classes: `Assistant` for individual prompts and `ChatAssistant` for multi-turn chat conversations.
+The library includes two powerful classes: `Assistant` for individual prompts and `ChatAssistant` for engaging, multi-turn chat conversations.
 
-Here is a simple example of how to use the `ChatAssistant` class:
+Here's a snippet showcasing a simple usage of the `ChatAssistant` class:
 
 ```python
 from gptbase.basev2 import ChatAssistant, CompletionParameters
 
 cm = CompletionParameters(stream=True)
 assistant = ChatAssistant(memory_turns=3)
 message = assistant.chat("I want to learn Python", cm)
 ```
 
-For more examples and usage, please refer to the documentation.
+For more examples and a deeper dive into usage, please refer to the detailed documentation. 📘
 
-## Support
+## 🙋 Support
 
-If you have any questions or issues, feel free to contact us.
+If you have any questions, run into any issues, or just need a little help, don't hesitate to reach out. We're here to help! 🤝
 
-### Short Description
+---
 
-GPTBase is a versatile Python library for the OpenAI GPT-3.5-Turbo and GPT-4 models. It supports both individual prompts and chat conversations, with customizable parameters for output control. Other features include stream output for faster response times, built-in logging, and rich printing for better visualization.
+Whether you're a veteran developer or just getting started, GPTBase is a powerful tool for any text generation task. Give it a try today! 🌟
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gptbase-0.1/gptbase/base.py` & `gptbase-0.1.1/gptbase/base.py`

 * *Files identical despite different names*

### Comparing `gptbase-0.1/setup.py` & `gptbase-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="gptbase",
-    version="0.1",
+    version="0.1.1",
     author="callmexss",
     author_email="callmexss@126.com",
     description="A package for simplified interaction with OpenAI's GPT-3 and GPT-4 models.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/callmexss/gptbase",
     packages=find_packages(include=["gptbase"]),
@@ -18,9 +18,9 @@
         "rich==13.0.1",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.9',
+    python_requires=">=3.9",
 )
```

