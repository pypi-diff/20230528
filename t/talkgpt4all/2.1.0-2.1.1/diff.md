# Comparing `tmp/talkgpt4all-2.1.0.tar.gz` & `tmp/talkgpt4all-2.1.1.tar.gz`

## Comparing `talkgpt4all-2.1.0.tar` & `talkgpt4all-2.1.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 talkgpt4all-2.1.0/requirements.txt
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 talkgpt4all-2.1.0/src/talkgpt4all/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 talkgpt4all-2.1.0/src/talkgpt4all/chat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 talkgpt4all-2.1.0/tests/example_test.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 talkgpt4all-2.1.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 talkgpt4all-2.1.0/LICENSE
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 talkgpt4all-2.1.0/README.md
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 talkgpt4all-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 talkgpt4all-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 talkgpt4all-2.1.1/BUILD.md
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 talkgpt4all-2.1.1/requirements.txt
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 talkgpt4all-2.1.1/src/talkgpt4all/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 talkgpt4all-2.1.1/src/talkgpt4all/chat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 talkgpt4all-2.1.1/tests/example_test.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 talkgpt4all-2.1.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 talkgpt4all-2.1.1/LICENSE
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 talkgpt4all-2.1.1/README.md
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 talkgpt4all-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 talkgpt4all-2.1.1/PKG-INFO
```

### Comparing `talkgpt4all-2.1.0/src/talkgpt4all/__init__.py` & `talkgpt4all-2.1.1/src/talkgpt4all/__init__.py`

 * *Files identical despite different names*

### Comparing `talkgpt4all-2.1.0/src/talkgpt4all/chat.py` & `talkgpt4all-2.1.1/src/talkgpt4all/chat.py`

 * *Files identical despite different names*

### Comparing `talkgpt4all-2.1.0/.gitignore` & `talkgpt4all-2.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `talkgpt4all-2.1.0/LICENSE` & `talkgpt4all-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `talkgpt4all-2.1.0/README.md` & `talkgpt4all-2.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -4,30 +4,36 @@
 [Video demo](https://www.zhihu.com/zvideo/1625779747656515584).
 
 Please check more details in this [blog post (in Chinese)](https://zhuanlan.zhihu.com/p/632592897).
 
 If you are looking for the older version of talkGPT4All, please checkout to [dev/v1.0.0](https://github.com/vra/talkGPT4All/tree/dev/v1.0.0) branch.
 
 ## Installation
-### Install Python Requirements
+
+### Install using pip (Recommend)
+talkgpt4all is on PyPI, you can install it using simple one command:
+```bash
+pip install talkgpt4all
+```
+### Install from source code
 Clone the code:
 ```bash
 git clone https://github.com/vra/talkGPT4All.git <ROOT>
 ```
 
 Install the dependencies and talkGPT4All in a python virtual environment:
 ```bash
 cd <ROOT>
 python -m venv talkgpt4all
 source talkgpt4all/bin/activate
 pip install -U pip
 pip install -r requirements.txt
 ```
 
-### Prepare Text to Voice program
+## Extra dependencies for Linux users
 We use [pyttsx3](https://github.com/nateshmbhat/pyttsx3) to convert text to voice. Please note that on Linux ，You need to install dependencies:
 ```bash
 sudo apt update && sudo apt install -y espeak ffmpeg libespeak1
 ```
 
 ## Usage
 Open a terminal and type `talkgpt4all` to begin:
@@ -69,15 +75,15 @@
 ```
 
 ### Tune voice rate
 You can tune the voice rate using `--voice-rate <rate>`, default rate is 165. the larger the speak faster.
 
 e.g.,
 ```bash
-python chat.py --whisper-model-type large --voice-rate 150
+talkgpt4all --whisper-model-type large --voice-rate 150
 ```
 
 ## RoadMap
 + [x] Add source building for llama.cpp, with more flexible interface.
 + [x] More LLMs
 + [x] Add support for contextual information during chating.
 + [ ] Test code on Linux，Mac Intel and WSL2.
```

### Comparing `talkgpt4all-2.1.0/pyproject.toml` & `talkgpt4all-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "talkgpt4all"
-version = "2.1.0"
+version = "2.1.1"
 authors = [
   { name="Yunfeng Wang", email="wyf.brz@gmail.com" },
 ]
 description = "A voice chatbot based on GPT4All and OpenAI Whisper, running on your PC locally"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `talkgpt4all-2.1.0/PKG-INFO` & `talkgpt4all-2.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkgpt4all
-Version: 2.1.0
+Version: 2.1.1
 Summary: A voice chatbot based on GPT4All and OpenAI Whisper, running on your PC locally
 Project-URL: Homepage, https://github.com/vra/talkGPT4All
 Project-URL: Bug Tracker, https://github.com/vra/talkGPT4All/issues
 Author-email: Yunfeng Wang <wyf.brz@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,30 +24,36 @@
 [Video demo](https://www.zhihu.com/zvideo/1625779747656515584).
 
 Please check more details in this [blog post (in Chinese)](https://zhuanlan.zhihu.com/p/632592897).
 
 If you are looking for the older version of talkGPT4All, please checkout to [dev/v1.0.0](https://github.com/vra/talkGPT4All/tree/dev/v1.0.0) branch.
 
 ## Installation
-### Install Python Requirements
+
+### Install using pip (Recommend)
+talkgpt4all is on PyPI, you can install it using simple one command:
+```bash
+pip install talkgpt4all
+```
+### Install from source code
 Clone the code:
 ```bash
 git clone https://github.com/vra/talkGPT4All.git <ROOT>
 ```
 
 Install the dependencies and talkGPT4All in a python virtual environment:
 ```bash
 cd <ROOT>
 python -m venv talkgpt4all
 source talkgpt4all/bin/activate
 pip install -U pip
 pip install -r requirements.txt
 ```
 
-### Prepare Text to Voice program
+## Extra dependencies for Linux users
 We use [pyttsx3](https://github.com/nateshmbhat/pyttsx3) to convert text to voice. Please note that on Linux ，You need to install dependencies:
 ```bash
 sudo apt update && sudo apt install -y espeak ffmpeg libespeak1
 ```
 
 ## Usage
 Open a terminal and type `talkgpt4all` to begin:
@@ -89,15 +95,15 @@
 ```
 
 ### Tune voice rate
 You can tune the voice rate using `--voice-rate <rate>`, default rate is 165. the larger the speak faster.
 
 e.g.,
 ```bash
-python chat.py --whisper-model-type large --voice-rate 150
+talkgpt4all --whisper-model-type large --voice-rate 150
 ```
 
 ## RoadMap
 + [x] Add source building for llama.cpp, with more flexible interface.
 + [x] More LLMs
 + [x] Add support for contextual information during chating.
 + [ ] Test code on Linux，Mac Intel and WSL2.
```

