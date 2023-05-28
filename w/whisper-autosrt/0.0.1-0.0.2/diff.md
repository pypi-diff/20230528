# Comparing `tmp/whisper_autosrt-0.0.1.tar.gz` & `tmp/whisper_autosrt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper_autosrt-0.0.1.tar", last modified: Sat May 27 16:40:25 2023, max compression
+gzip compressed data, was "whisper_autosrt-0.0.2.tar", last modified: Sun May 28 10:45:49 2023, max compression
```

## Comparing `whisper_autosrt-0.0.1.tar` & `whisper_autosrt-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 16:40:25.403530 whisper_autosrt-0.0.1/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 whisper_autosrt-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 whisper_autosrt-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1996 2023-05-27 16:40:25.404278 whisper_autosrt-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 whisper_autosrt-0.0.1/README.md
--rw-rw-rw-   0        0        0      147 2023-05-27 16:40:25.406526 whisper_autosrt-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1467 2023-05-27 16:38:14.000000 whisper_autosrt-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-27 16:40:25.355579 whisper_autosrt-0.0.1/whisper_autosrt/
--rw-rw-rw-   0        0        0    78028 2023-05-27 15:39:12.000000 whisper_autosrt-0.0.1/whisper_autosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 16:40:25.402032 whisper_autosrt-0.0.1/whisper_autosrt.egg-info/
--rw-rw-rw-   0        0        0     1996 2023-05-27 16:40:25.000000 whisper_autosrt-0.0.1/whisper_autosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-05-27 16:40:25.000000 whisper_autosrt-0.0.1/whisper_autosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 16:40:25.000000 whisper_autosrt-0.0.1/whisper_autosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-05-27 16:40:25.000000 whisper_autosrt-0.0.1/whisper_autosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      113 2023-05-27 16:40:25.000000 whisper_autosrt-0.0.1/whisper_autosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-27 16:40:25.000000 whisper_autosrt-0.0.1/whisper_autosrt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 10:45:49.039622 whisper_autosrt-0.0.2/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 whisper_autosrt-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 whisper_autosrt-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2009 2023-05-28 10:45:49.040370 whisper_autosrt-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4700 2023-05-27 16:57:41.000000 whisper_autosrt-0.0.2/README.md
+-rw-rw-rw-   0        0        0      147 2023-05-28 10:45:49.044119 whisper_autosrt-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1466 2023-05-27 17:47:37.000000 whisper_autosrt-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:45:48.973850 whisper_autosrt-0.0.2/whisper_autosrt/
+-rw-rw-rw-   0        0        0    78004 2023-05-27 17:33:39.000000 whisper_autosrt-0.0.2/whisper_autosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:45:49.036625 whisper_autosrt-0.0.2/whisper_autosrt.egg-info/
+-rw-rw-rw-   0        0        0     2009 2023-05-28 10:45:48.000000 whisper_autosrt-0.0.2/whisper_autosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-05-28 10:45:48.000000 whisper_autosrt-0.0.2/whisper_autosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 10:45:48.000000 whisper_autosrt-0.0.2/whisper_autosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-05-28 10:45:48.000000 whisper_autosrt-0.0.2/whisper_autosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      122 2023-05-28 10:45:48.000000 whisper_autosrt-0.0.2/whisper_autosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-28 10:45:48.000000 whisper_autosrt-0.0.2/whisper_autosrt.egg-info/top_level.txt
```

### Comparing `whisper_autosrt-0.0.1/LICENSE` & `whisper_autosrt-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_autosrt-0.0.1/PKG-INFO` & `whisper_autosrt-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: whisper_autosrt
-Version: 0.0.1
-Summary: a utility for automatic speech recognition and subtitle generation
+Version: 0.0.2
+Summary: a command line utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/whisper_autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `whisper_autosrt-0.0.1/README.md` & `whisper_autosrt-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,125 +1,118 @@
-# autosrt <a href="https://pypi.python.org/pypi/autosrt"><img src="https://img.shields.io/pypi/v/autosrt.svg"></img></a>
+# whisper_autosrt <a href="https://pypi.python.org/pypi/whisper_autosrt"><img src="https://img.shields.io/pypi/v/whisper_autosrt.svg"></img></a>
   
 ### Auto generate subtitle files for any video / audio files
-autosrt is a simple command line tool made with python to auto generate subtitle/closed caption for any video or audio files and translate it automatically for free using a simple unofficial online Google Translate API.
-
-This script is a modified version of original autosub made by Anastasis Germanidis at https://github.com/agermanidis/autosub
-
-### UPDATE NOTES
-Since version 1.2.2 I tried to make some class modules, so in case you want to use them in your own project you can just import them. They are Language, WavConverter, SpeechRegionFinder, FLACConverter, SpeechRecognizer, SentenceTranslator, SubtitleFormatter, and SubtitleWriter. You can import them like this :
-```
-from autosrt import Language, WavConverter, SpeechRegionFinder, FLACConverter, SpeechRecognizer, SentenceTranslator, \
-    SubtitleFormatter,  SubtitleWriter
-```
-
-You can learn how to use them by playing around with those scripts inside test folder. Check every def function on each class to know how to use them. They are not to difficult to understand.
-
-If you are on Linux OS don't forget to install libmagic C library to make python_magic modules work properly by typing this at console terminal :
-```
-sudo apt install -y libmagic1
-```
+whisper_autosrt is a simple command line tool made with python to auto generate subtitle/closed caption for any video or audio files using OpenAI whisper module and translate it automatically for free using a simple unofficial online Google Translate API.
 
 ### Installation
 If you don't have python on your Windows system you can get compiled version from this git release assets
-https://github.com/botbahlul/autosrt/releases
+https://github.com/botbahlul/whisper_autosrt/releases
 
-Just extract those ffmpeg.exe and autosrt.exe into a folder that has been added to PATH ENVIRONTMET for example in C:\Windows\system32
+Just extract those ffmpeg.exe and whisper_autosrt.exe into a folder that has been added to PATH ENVIRONTMET for example in C:\Windows\system32
 
 You can get latest version of ffmpeg from https://www.ffmpeg.org/
 
 In Linux you have to install this script with python (version minimal 3.8 ) and install ffmpeg with your linux package manager for example in debian based linux distribution you can type :
 
 ```
 sudo apt update
 sudo apt install -y ffmpeg
 ```
 
-To install this autosrt, just type :
+To install this whisper_autosrt, just type :
 ```
-pip install autosrt
+pip install whisper_autosrt
 ```
 
-You can try to compile that autosrt.py script in win/linux folder into a single executable file with pyinstaller by typing these :
+You can try to compile that whisper_autosrt.py script in win/linux folder into a single executable file with pyinstaller by typing these :
 ```
 pip install pyinstaller
-pyinstaller --onefile autosrt.py
+pyinstaller --onefile whisper_autosrt.py
 ```
 
 The executable compiled file will be placed by pyinstaller into dist subfolder of your current working folder, so you can just rename and put that compiled file into a folder that has been added to your PATH ENVIRONTMENT so you can execute it from anywhere
 
 I was succesfuly compiled it in Windows 10 with pyinstaller-5.1 and Pyhton-3.10.4, and python-3.8.12 in Debian 9
 
 Another alternative way to install this script with python is by cloning this git (or downloading this git as zip then extract it into a folder), and then just type :
 
 ```
 pip install wheel
-python setup.py build
 python setup.py bdist_wheel
 ```
 
-Then check the name of the whl file created in dist folder. In case the filename is autosrt-1.2.2-py2.py3-none-any.whl then you can install that whl file with pip :
+Then check the name of the whl file created in dist folder. In case the filename is whisper_autosrt-0.0.1-py2.py3-none-any.whl then you can install that whl file with pip :
 ```
 cd dist
-pip install autosrt-1.2.2-py2.py3-none-any.whl
+pip install whisper_autosrt-0.0.1-py2.py3-none-any.whl
 ```
 
 You can also install this script (or any pip package) in ANDROID DEVICES via PYTHON package in TERMUX APP
 
 https://github.com/termux/termux-app/releases/tag/v0.118.0
 
 Choose the right apk for your device, install it, then open it
 
-Type these commands to get python, pip, this autosrt, (and any other pip packages) :
+Type these commands to get python, pip, this whisper_autosrt, (and any other pip packages) :
 
 ```
 termux-setup-storage
 pkg update -y
 pkg install -y python
 pkg install -y ffmpeg
-pip install autosrt
+pip install whisper_autosrt
 ```
 
 ### Simple usage example 
 
 ```
-autosrt --list-languages
-autosrt -S zh-CN -D en "Episode 1.mp4"
+whisper_autosrt --list-whisper-languages
+whisper_autosrt --list-google-languages
+whisper_autosrt -S zh -D en "Episode 1.mp4"
+```
+
+For multiple video/audio files you can use wildcard e.g:
+```
+whisper_autosrt -S zh -D en "C:\Movies\*.mp4"
 ```
 
-For multiple video/audio files (starts from version 1.1.0), you can use wildcard
+or separate them with space character e.g:
 ```
-autosrt -S zh-CN -D en "C:\Movies\*.mp4"
+whisper_autosrt -S zh -D en "Episode 1.mp4" "Episode 2.mp4"
 ```
 
 If you don't need translations just type :
 ```
-autosrt -S zh-CN "Episode 1.mp4"
+whisper_autosrt -S zh "Episode 1.mp4"
 ```
 
 ### Usage
 
 ```
-usage: autosrt [-h] [-S SRC_LANGUAGE] [-D DST_LANGUAGE] [-ll] [-o OUTPUT] [-F FORMAT] [-lf] [-C CONCURRENCY] [-v] [source_path ...]
+usage: whisper_autosrt [-h] [-m MODEL_NAME] [-lm] [-S SRC_LANGUAGE] [-D DST_LANGUAGE] [-lwl] [-lgl] [-F FORMAT] [-lf]
+                       [-C CONCURRENCY] [-v]
+                       [source_path ...]
 
 positional arguments:
-  source_path           File path of the video or audio files to generate subtitles files (use wildcard for multiple files or
-                        separate them with a space character)
+  source_path           Path to the video or audio files to generate subtitles files (use wildcard for multiple files or separate
+                        them with a space character e.g. "file 1.mp4" "file 2.mp4")
 
 options:
   -h, --help            show this help message and exit
+  -m MODEL_NAME, --model-name MODEL_NAME
+                        name of the Whisper model to use
+  -lm, --list-models    List of Whisper models name
   -S SRC_LANGUAGE, --src-language SRC_LANGUAGE
                         Language code of the audio language spoken in video/audio source_path
   -D DST_LANGUAGE, --dst-language DST_LANGUAGE
                         Desired translation language code for the subtitles
-  -ll, --list-languages
-                        List all supported languages
-  -o OUTPUT, --output OUTPUT
-                        Output file path for subtitles (by default, subtitles are saved in the same directory and named with the
-                        source_path base name)
+  -lwl, --list-whisper-languages
+                        List all whisper supported languages
+  -lgl, --list-google-languages
+                        List all google translate supported languages
   -F FORMAT, --format FORMAT
                         Desired subtitle format
   -lf, --list-formats   List all supported subtitle formats
   -C CONCURRENCY, --concurrency CONCURRENCY
                         Number of concurrent API requests to make
   -v, --version         show program's version number and exit
 ```
```

#### html2text {}

```diff
@@ -1,64 +1,57 @@
-# autosrt [https://img.shields.io/pypi/v/autosrt.svg] ### Auto generate
-subtitle files for any video / audio files autosrt is a simple command line
-tool made with python to auto generate subtitle/closed caption for any video or
-audio files and translate it automatically for free using a simple unofficial
-online Google Translate API. This script is a modified version of original
-autosub made by Anastasis Germanidis at https://github.com/agermanidis/autosub
-### UPDATE NOTES Since version 1.2.2 I tried to make some class modules, so in
-case you want to use them in your own project you can just import them. They
-are Language, WavConverter, SpeechRegionFinder, FLACConverter,
-SpeechRecognizer, SentenceTranslator, SubtitleFormatter, and SubtitleWriter.
-You can import them like this : ``` from autosrt import Language, WavConverter,
-SpeechRegionFinder, FLACConverter, SpeechRecognizer, SentenceTranslator, \
-SubtitleFormatter, SubtitleWriter ``` You can learn how to use them by playing
-around with those scripts inside test folder. Check every def function on each
-class to know how to use them. They are not to difficult to understand. If you
-are on Linux OS don't forget to install libmagic C library to make python_magic
-modules work properly by typing this at console terminal : ``` sudo apt install
--y libmagic1 ``` ### Installation If you don't have python on your Windows
-system you can get compiled version from this git release assets https://
-github.com/botbahlul/autosrt/releases Just extract those ffmpeg.exe and
-autosrt.exe into a folder that has been added to PATH ENVIRONTMET for example
-in C:\Windows\system32 You can get latest version of ffmpeg from https://
+# whisper_autosrt [https://img.shields.io/pypi/v/whisper_autosrt.svg] ### Auto
+generate subtitle files for any video / audio files whisper_autosrt is a simple
+command line tool made with python to auto generate subtitle/closed caption for
+any video or audio files using OpenAI whisper module and translate it
+automatically for free using a simple unofficial online Google Translate API.
+### Installation If you don't have python on your Windows system you can get
+compiled version from this git release assets https://github.com/botbahlul/
+whisper_autosrt/releases Just extract those ffmpeg.exe and whisper_autosrt.exe
+into a folder that has been added to PATH ENVIRONTMET for example in C:
+\Windows\system32 You can get latest version of ffmpeg from https://
 www.ffmpeg.org/ In Linux you have to install this script with python (version
 minimal 3.8 ) and install ffmpeg with your linux package manager for example in
 debian based linux distribution you can type : ``` sudo apt update sudo apt
-install -y ffmpeg ``` To install this autosrt, just type : ``` pip install
-autosrt ``` You can try to compile that autosrt.py script in win/linux folder
-into a single executable file with pyinstaller by typing these : ``` pip
-install pyinstaller pyinstaller --onefile autosrt.py ``` The executable
-compiled file will be placed by pyinstaller into dist subfolder of your current
-working folder, so you can just rename and put that compiled file into a folder
-that has been added to your PATH ENVIRONTMENT so you can execute it from
-anywhere I was succesfuly compiled it in Windows 10 with pyinstaller-5.1 and
-Pyhton-3.10.4, and python-3.8.12 in Debian 9 Another alternative way to install
-this script with python is by cloning this git (or downloading this git as zip
-then extract it into a folder), and then just type : ``` pip install wheel
-python setup.py build python setup.py bdist_wheel ``` Then check the name of
-the whl file created in dist folder. In case the filename is autosrt-1.2.2-
-py2.py3-none-any.whl then you can install that whl file with pip : ``` cd dist
-pip install autosrt-1.2.2-py2.py3-none-any.whl ``` You can also install this
-script (or any pip package) in ANDROID DEVICES via PYTHON package in TERMUX APP
-https://github.com/termux/termux-app/releases/tag/v0.118.0 Choose the right apk
-for your device, install it, then open it Type these commands to get python,
-pip, this autosrt, (and any other pip packages) : ``` termux-setup-storage pkg
-update -y pkg install -y python pkg install -y ffmpeg pip install autosrt ```
-### Simple usage example ``` autosrt --list-languages autosrt -S zh-CN -D en
-"Episode 1.mp4" ``` For multiple video/audio files (starts from version 1.1.0),
-you can use wildcard ``` autosrt -S zh-CN -D en "C:\Movies\*.mp4" ``` If you
-don't need translations just type : ``` autosrt -S zh-CN "Episode 1.mp4" ```
-### Usage ``` usage: autosrt [-h] [-S SRC_LANGUAGE] [-D DST_LANGUAGE] [-ll] [-
-o OUTPUT] [-F FORMAT] [-lf] [-C CONCURRENCY] [-v] [source_path ...] positional
-arguments: source_path File path of the video or audio files to generate
-subtitles files (use wildcard for multiple files or separate them with a space
-character) options: -h, --help show this help message and exit -S SRC_LANGUAGE,
---src-language SRC_LANGUAGE Language code of the audio language spoken in
-video/audio source_path -D DST_LANGUAGE, --dst-language DST_LANGUAGE Desired
-translation language code for the subtitles -ll, --list-languages List all
-supported languages -o OUTPUT, --output OUTPUT Output file path for subtitles
-(by default, subtitles are saved in the same directory and named with the
-source_path base name) -F FORMAT, --format FORMAT Desired subtitle format -lf,
---list-formats List all supported subtitle formats -C CONCURRENCY, --
-concurrency CONCURRENCY Number of concurrent API requests to make -v, --version
-show program's version number and exit ``` ### License MIT Check my other
-SPEECH RECOGNITIION + TRANSLATE PROJECTS in https://botbahlul.github.io
+install -y ffmpeg ``` To install this whisper_autosrt, just type : ``` pip
+install whisper_autosrt ``` You can try to compile that whisper_autosrt.py
+script in win/linux folder into a single executable file with pyinstaller by
+typing these : ``` pip install pyinstaller pyinstaller --onefile
+whisper_autosrt.py ``` The executable compiled file will be placed by
+pyinstaller into dist subfolder of your current working folder, so you can just
+rename and put that compiled file into a folder that has been added to your
+PATH ENVIRONTMENT so you can execute it from anywhere I was succesfuly compiled
+it in Windows 10 with pyinstaller-5.1 and Pyhton-3.10.4, and python-3.8.12 in
+Debian 9 Another alternative way to install this script with python is by
+cloning this git (or downloading this git as zip then extract it into a
+folder), and then just type : ``` pip install wheel python setup.py bdist_wheel
+``` Then check the name of the whl file created in dist folder. In case the
+filename is whisper_autosrt-0.0.1-py2.py3-none-any.whl then you can install
+that whl file with pip : ``` cd dist pip install whisper_autosrt-0.0.1-py2.py3-
+none-any.whl ``` You can also install this script (or any pip package) in
+ANDROID DEVICES via PYTHON package in TERMUX APP https://github.com/termux/
+termux-app/releases/tag/v0.118.0 Choose the right apk for your device, install
+it, then open it Type these commands to get python, pip, this whisper_autosrt,
+(and any other pip packages) : ``` termux-setup-storage pkg update -y pkg
+install -y python pkg install -y ffmpeg pip install whisper_autosrt ``` ###
+Simple usage example ``` whisper_autosrt --list-whisper-languages
+whisper_autosrt --list-google-languages whisper_autosrt -S zh -D en "Episode
+1.mp4" ``` For multiple video/audio files you can use wildcard e.g: ```
+whisper_autosrt -S zh -D en "C:\Movies\*.mp4" ``` or separate them with space
+character e.g: ``` whisper_autosrt -S zh -D en "Episode 1.mp4" "Episode 2.mp4"
+``` If you don't need translations just type : ``` whisper_autosrt -S zh
+"Episode 1.mp4" ``` ### Usage ``` usage: whisper_autosrt [-h] [-m MODEL_NAME]
+[-lm] [-S SRC_LANGUAGE] [-D DST_LANGUAGE] [-lwl] [-lgl] [-F FORMAT] [-lf] [-
+C CONCURRENCY] [-v] [source_path ...] positional arguments: source_path Path to
+the video or audio files to generate subtitles files (use wildcard for multiple
+files or separate them with a space character e.g. "file 1.mp4" "file 2.mp4")
+options: -h, --help show this help message and exit -m MODEL_NAME, --model-name
+MODEL_NAME name of the Whisper model to use -lm, --list-models List of Whisper
+models name -S SRC_LANGUAGE, --src-language SRC_LANGUAGE Language code of the
+audio language spoken in video/audio source_path -D DST_LANGUAGE, --dst-
+language DST_LANGUAGE Desired translation language code for the subtitles -lwl,
+--list-whisper-languages List all whisper supported languages -lgl, --list-
+google-languages List all google translate supported languages -F FORMAT, --
+format FORMAT Desired subtitle format -lf, --list-formats List all supported
+subtitle formats -C CONCURRENCY, --concurrency CONCURRENCY Number of concurrent
+API requests to make -v, --version show program's version number and exit ```
+### License MIT Check my other SPEECH RECOGNITIION + TRANSLATE PROJECTS in
+https://botbahlul.github.io
```

### Comparing `whisper_autosrt-0.0.1/setup.py` & `whisper_autosrt-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 from __future__ import unicode_literals
 import sys
 
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
@@ -16,25 +15,25 @@
     'It supports a variety of input and output languages and can currently produce subtitles '
     'in SRT, VTT, JSON, and RAW format.'
 )
 
 install_requires=[
     "requests>=2.3.0",
     "httpx>=0.24.0",
-    "urllib3 >=1.26.0,<2.0",
+    "urllib3 >=1.26.0,<3.0",
     "pysrt>=1.0.1",
     "six>=1.11.0",
     "progressbar2>=3.34.3",
-    "whisper>=1.1.10",
+    "openai_whisper>=20230314",
 ]
 
 setup(
     name="whisper_autosrt",
     version=VERSION,
-    description="a utility for automatic speech recognition and subtitle generation",
+    description="a command line utility for automatic speech recognition and subtitle generation",
     long_description = long_description,
     author="Bot Bahlul",
     author_email="bot.bahlul@gmail.com",
     url="https://github.com/botbahlul/whisper_autosrt",
     packages=["whisper_autosrt"],
     entry_points={
         "console_scripts": [
```

### Comparing `whisper_autosrt-0.0.1/whisper_autosrt/__init__.py` & `whisper_autosrt-0.0.2/whisper_autosrt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,4877 +1,4876 @@
-00000000: 2321 2f75 7372 2f62 696e 2f65 6e76 2070  #!/usr/bin/env p
-00000010: 7974 686f 6e33 0d0a 2320 4f52 4947 494e  ython3..# ORIGIN
-00000020: 414c 2041 5554 4f53 5542 2049 4d50 4f52  AL AUTOSUB IMPOR
-00000030: 5453 0d0a 6672 6f6d 205f 5f66 7574 7572  TS..from __futur
-00000040: 655f 5f20 696d 706f 7274 2061 6273 6f6c  e__ import absol
-00000050: 7574 655f 696d 706f 7274 2c20 7072 696e  ute_import, prin
-00000060: 745f 6675 6e63 7469 6f6e 2c20 756e 6963  t_function, unic
-00000070: 6f64 655f 6c69 7465 7261 6c73 0d0a 696d  ode_literals..im
-00000080: 706f 7274 2061 7267 7061 7273 650d 0a69  port argparse..i
-00000090: 6d70 6f72 7420 6175 6469 6f6f 700d 0a69  mport audioop..i
-000000a0: 6d70 6f72 7420 6d61 7468 0d0a 696d 706f  mport math..impo
-000000b0: 7274 206d 756c 7469 7072 6f63 6573 7369  rt multiprocessi
-000000c0: 6e67 0d0a 696d 706f 7274 206f 730d 0a69  ng..import os..i
-000000d0: 6d70 6f72 7420 7375 6270 726f 6365 7373  mport subprocess
-000000e0: 0d0a 696d 706f 7274 2073 7973 0d0a 696d  ..import sys..im
-000000f0: 706f 7274 2074 656d 7066 696c 650d 0a69  port tempfile..i
-00000100: 6d70 6f72 7420 7761 7665 0d0a 696d 706f  mport wave..impo
-00000110: 7274 206a 736f 6e0d 0a69 6d70 6f72 7420  rt json..import 
-00000120: 7265 7175 6573 7473 0d0a 7472 793a 0d0a  requests..try:..
-00000130: 2020 2020 6672 6f6d 206a 736f 6e2e 6465      from json.de
-00000140: 636f 6465 7220 696d 706f 7274 204a 534f  coder import JSO
-00000150: 4e44 6563 6f64 6545 7272 6f72 0d0a 6578  NDecodeError..ex
-00000160: 6365 7074 2049 6d70 6f72 7445 7272 6f72  cept ImportError
-00000170: 3a0d 0a20 2020 204a 534f 4e44 6563 6f64  :..    JSONDecod
-00000180: 6545 7272 6f72 203d 2056 616c 7565 4572  eError = ValueEr
-00000190: 726f 720d 0a66 726f 6d20 7072 6f67 7265  ror..from progre
-000001a0: 7373 6261 7220 696d 706f 7274 2050 726f  ssbar import Pro
-000001b0: 6772 6573 7342 6172 2c20 5065 7263 656e  gressBar, Percen
-000001c0: 7461 6765 2c20 4261 722c 2045 5441 0d0a  tage, Bar, ETA..
-000001d0: 696d 706f 7274 2070 7973 7274 0d0a 696d  import pysrt..im
-000001e0: 706f 7274 2073 6978 0d0a 2320 4144 4449  port six..# ADDI
-000001f0: 5449 4f4e 414c 2049 4d50 4f52 540d 0a66  TIONAL IMPORT..f
-00000200: 726f 6d20 676c 6f62 2069 6d70 6f72 7420  rom glob import 
-00000210: 676c 6f62 2c20 6573 6361 7065 0d0a 696d  glob, escape..im
-00000220: 706f 7274 2074 696d 650d 0a66 726f 6d20  port time..from 
-00000230: 6461 7465 7469 6d65 2069 6d70 6f72 7420  datetime import 
-00000240: 6461 7465 7469 6d65 2c20 7469 6d65 6465  datetime, timede
-00000250: 6c74 610d 0a66 726f 6d20 7061 7468 6c69  lta..from pathli
-00000260: 6220 696d 706f 7274 2050 6174 680d 0a69  b import Path..i
-00000270: 6d70 6f72 7420 7761 726e 696e 6773 0d0a  mport warnings..
-00000280: 7761 726e 696e 6773 2e66 696c 7465 7277  warnings.filterw
-00000290: 6172 6e69 6e67 7328 2269 676e 6f72 6522  arnings("ignore"
-000002a0: 2c20 6d65 7373 6167 653d 222e 2a54 6865  , message=".*The
-000002b0: 2027 6e6f 7079 7468 6f6e 2720 6b65 7977   'nopython' keyw
-000002c0: 6f72 642e 2a22 290d 0a69 6d70 6f72 7420  ord.*")..import 
-000002d0: 7768 6973 7065 720d 0a0d 0a0d 0a56 4552  whisper......VER
-000002e0: 5349 4f4e 203d 2022 302e 302e 3122 0d0a  SION = "0.0.1"..
-000002f0: 0d0a 233d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ..#=============
+00000000: 2320 4f52 4947 494e 414c 2041 5554 4f53  # ORIGINAL AUTOS
+00000010: 5542 2049 4d50 4f52 5453 0d0a 6672 6f6d  UB IMPORTS..from
+00000020: 205f 5f66 7574 7572 655f 5f20 696d 706f   __future__ impo
+00000030: 7274 2061 6273 6f6c 7574 655f 696d 706f  rt absolute_impo
+00000040: 7274 2c20 7072 696e 745f 6675 6e63 7469  rt, print_functi
+00000050: 6f6e 2c20 756e 6963 6f64 655f 6c69 7465  on, unicode_lite
+00000060: 7261 6c73 0d0a 696d 706f 7274 2061 7267  rals..import arg
+00000070: 7061 7273 650d 0a69 6d70 6f72 7420 6175  parse..import au
+00000080: 6469 6f6f 700d 0a69 6d70 6f72 7420 6d61  dioop..import ma
+00000090: 7468 0d0a 696d 706f 7274 206d 756c 7469  th..import multi
+000000a0: 7072 6f63 6573 7369 6e67 0d0a 696d 706f  processing..impo
+000000b0: 7274 206f 730d 0a69 6d70 6f72 7420 7375  rt os..import su
+000000c0: 6270 726f 6365 7373 0d0a 696d 706f 7274  bprocess..import
+000000d0: 2073 7973 0d0a 696d 706f 7274 2074 656d   sys..import tem
+000000e0: 7066 696c 650d 0a69 6d70 6f72 7420 7761  pfile..import wa
+000000f0: 7665 0d0a 696d 706f 7274 206a 736f 6e0d  ve..import json.
+00000100: 0a69 6d70 6f72 7420 7265 7175 6573 7473  .import requests
+00000110: 0d0a 7472 793a 0d0a 2020 2020 6672 6f6d  ..try:..    from
+00000120: 206a 736f 6e2e 6465 636f 6465 7220 696d   json.decoder im
+00000130: 706f 7274 204a 534f 4e44 6563 6f64 6545  port JSONDecodeE
+00000140: 7272 6f72 0d0a 6578 6365 7074 2049 6d70  rror..except Imp
+00000150: 6f72 7445 7272 6f72 3a0d 0a20 2020 204a  ortError:..    J
+00000160: 534f 4e44 6563 6f64 6545 7272 6f72 203d  SONDecodeError =
+00000170: 2056 616c 7565 4572 726f 720d 0a66 726f   ValueError..fro
+00000180: 6d20 7072 6f67 7265 7373 6261 7220 696d  m progressbar im
+00000190: 706f 7274 2050 726f 6772 6573 7342 6172  port ProgressBar
+000001a0: 2c20 5065 7263 656e 7461 6765 2c20 4261  , Percentage, Ba
+000001b0: 722c 2045 5441 0d0a 696d 706f 7274 2070  r, ETA..import p
+000001c0: 7973 7274 0d0a 696d 706f 7274 2073 6978  ysrt..import six
+000001d0: 0d0a 2320 4144 4449 5449 4f4e 414c 2049  ..# ADDITIONAL I
+000001e0: 4d50 4f52 540d 0a66 726f 6d20 676c 6f62  MPORT..from glob
+000001f0: 2069 6d70 6f72 7420 676c 6f62 2c20 6573   import glob, es
+00000200: 6361 7065 0d0a 696d 706f 7274 2074 696d  cape..import tim
+00000210: 650d 0a66 726f 6d20 6461 7465 7469 6d65  e..from datetime
+00000220: 2069 6d70 6f72 7420 6461 7465 7469 6d65   import datetime
+00000230: 2c20 7469 6d65 6465 6c74 610d 0a66 726f  , timedelta..fro
+00000240: 6d20 7061 7468 6c69 6220 696d 706f 7274  m pathlib import
+00000250: 2050 6174 680d 0a69 6d70 6f72 7420 7761   Path..import wa
+00000260: 726e 696e 6773 0d0a 7761 726e 696e 6773  rnings..warnings
+00000270: 2e66 696c 7465 7277 6172 6e69 6e67 7328  .filterwarnings(
+00000280: 2269 676e 6f72 6522 2c20 6d65 7373 6167  "ignore", messag
+00000290: 653d 222e 2a54 6865 2027 6e6f 7079 7468  e=".*The 'nopyth
+000002a0: 6f6e 2720 6b65 7977 6f72 642e 2a22 290d  on' keyword.*").
+000002b0: 0a69 6d70 6f72 7420 7768 6973 7065 720d  .import whisper.
+000002c0: 0a0d 0a0d 0a56 4552 5349 4f4e 203d 2022  .....VERSION = "
+000002d0: 302e 302e 3222 0d0a 0d0a 233d 3d3d 3d3d  0.0.2"....#=====
+000002e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000002f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00000300: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000310: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000320: 3d3d 3d3d 3d3d 3d3d 3d3d 3d20 6666 6d70  =========== ffmp
-00000330: 6567 5f70 726f 6772 6573 735f 7969 656c  eg_progress_yiel
-00000340: 6420 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  d ==============
+00000310: 3d3d 3d20 6666 6d70 6567 5f70 726f 6772  === ffmpeg_progr
+00000320: 6573 735f 7969 656c 6420 3d3d 3d3d 3d3d  ess_yield ======
+00000330: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000340: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00000350: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000360: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000370: 3d3d 3d3d 3d3d 3d3d 3d3d 230d 0a0d 0a69  ==========#....i
-00000380: 6d70 6f72 7420 7265 0d0a 2369 6d70 6f72  mport re..#impor
-00000390: 7420 7375 6270 726f 6365 7373 0d0a 6672  t subprocess..fr
-000003a0: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
-000003b0: 2041 6e79 2c20 4361 6c6c 6162 6c65 2c20   Any, Callable, 
-000003c0: 4974 6572 6174 6f72 2c20 4c69 7374 2c20  Iterator, List, 
-000003d0: 4f70 7469 6f6e 616c 2c20 556e 696f 6e0d  Optional, Union.
-000003e0: 0a0d 0a0d 0a64 6566 2074 6f5f 6d73 282a  .....def to_ms(*
-000003f0: 2a6b 7761 7267 733a 2055 6e69 6f6e 5b66  *kwargs: Union[f
-00000400: 6c6f 6174 2c20 696e 742c 2073 7472 5d29  loat, int, str])
-00000410: 202d 3e20 696e 743a 0d0a 2020 2020 686f   -> int:..    ho
-00000420: 7572 203d 2069 6e74 286b 7761 7267 732e  ur = int(kwargs.
-00000430: 6765 7428 2268 6f75 7222 2c20 3029 290d  get("hour", 0)).
-00000440: 0a20 2020 206d 696e 7574 6520 3d20 696e  .    minute = in
-00000450: 7428 6b77 6172 6773 2e67 6574 2822 6d69  t(kwargs.get("mi
-00000460: 6e22 2c20 3029 290d 0a20 2020 2073 6563  n", 0))..    sec
-00000470: 203d 2069 6e74 286b 7761 7267 732e 6765   = int(kwargs.ge
-00000480: 7428 2273 6563 222c 2030 2929 0d0a 2020  t("sec", 0))..  
-00000490: 2020 6d73 203d 2069 6e74 286b 7761 7267    ms = int(kwarg
-000004a0: 732e 6765 7428 226d 7322 2c20 3029 290d  s.get("ms", 0)).
-000004b0: 0a0d 0a20 2020 2072 6574 7572 6e20 2868  ...    return (h
-000004c0: 6f75 7220 2a20 3630 202a 2036 3020 2a20  our * 60 * 60 * 
-000004d0: 3130 3030 2920 2b20 286d 696e 7574 6520  1000) + (minute 
-000004e0: 2a20 3630 202a 2031 3030 3029 202b 2028  * 60 * 1000) + (
-000004f0: 7365 6320 2a20 3130 3030 2920 2b20 6d73  sec * 1000) + ms
-00000500: 0d0a 0d0a 0d0a 6465 6620 5f70 726f 6265  ......def _probe
-00000510: 5f64 7572 6174 696f 6e28 636d 643a 204c  _duration(cmd: L
-00000520: 6973 745b 7374 725d 2920 2d3e 204f 7074  ist[str]) -> Opt
-00000530: 696f 6e61 6c5b 696e 745d 3a0d 0a20 2020  ional[int]:..   
-00000540: 2027 2727 0d0a 2020 2020 4765 7420 7468   '''..    Get th
-00000550: 6520 6475 7261 7469 6f6e 2076 6961 2066  e duration via f
-00000560: 6670 726f 6265 2066 726f 6d20 696e 7075  fprobe from inpu
-00000570: 7420 6d65 6469 6120 6669 6c65 0d0a 2020  t media file..  
-00000580: 2020 696e 2063 6173 6520 6666 6d70 6567    in case ffmpeg
-00000590: 2077 6173 2072 756e 2077 6974 6820 6c6f   was run with lo
-000005a0: 676c 6576 656c 3d65 7272 6f72 2e0d 0a0d  glevel=error....
-000005b0: 0a20 2020 2041 7267 733a 0d0a 2020 2020  .    Args:..    
-000005c0: 2020 2020 636d 6420 284c 6973 745b 7374      cmd (List[st
-000005d0: 725d 293a 2041 206c 6973 7420 6f66 2063  r]): A list of c
-000005e0: 6f6d 6d61 6e64 206c 696e 6520 656c 656d  ommand line elem
-000005f0: 656e 7473 2c20 652e 672e 205b 2266 666d  ents, e.g. ["ffm
-00000600: 7065 6722 2c20 222d 6922 2c20 2e2e 2e5d  peg", "-i", ...]
-00000610: 0d0a 0d0a 2020 2020 5265 7475 726e 733a  ....    Returns:
-00000620: 0d0a 2020 2020 2020 2020 4f70 7469 6f6e  ..        Option
-00000630: 616c 5b69 6e74 5d3a 2054 6865 2064 7572  al[int]: The dur
-00000640: 6174 696f 6e20 696e 206d 696c 6c69 7365  ation in millise
-00000650: 636f 6e64 732e 0d0a 2020 2020 2727 270d  conds...    '''.
-00000660: 0a0d 0a20 2020 2064 6566 205f 6765 745f  ...    def _get_
-00000670: 6669 6c65 5f6e 616d 6528 636d 643a 204c  file_name(cmd: L
-00000680: 6973 745b 7374 725d 2920 2d3e 204f 7074  ist[str]) -> Opt
-00000690: 696f 6e61 6c5b 7374 725d 3a0d 0a20 2020  ional[str]:..   
-000006a0: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
-000006b0: 2020 2020 2020 2069 6478 203d 2063 6d64         idx = cmd
-000006c0: 2e69 6e64 6578 2822 2d69 2229 0d0a 2020  .index("-i")..  
-000006d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000006e0: 2063 6d64 5b69 6478 202b 2031 5d0d 0a20   cmd[idx + 1].. 
-000006f0: 2020 2020 2020 2065 7863 6570 7420 5661         except Va
-00000700: 6c75 6545 7272 6f72 3a0d 0a20 2020 2020  lueError:..     
-00000710: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-00000720: 6e65 0d0a 0d0a 2020 2020 6669 6c65 5f6e  ne....    file_n
-00000730: 616d 6520 3d20 5f67 6574 5f66 696c 655f  ame = _get_file_
-00000740: 6e61 6d65 2863 6d64 290d 0a20 2020 2069  name(cmd)..    i
-00000750: 6620 6669 6c65 5f6e 616d 6520 6973 204e  f file_name is N
-00000760: 6f6e 653a 0d0a 2020 2020 2020 2020 7265  one:..        re
-00000770: 7475 726e 204e 6f6e 650d 0a0d 0a20 2020  turn None....   
-00000780: 2074 7279 3a0d 0a20 2020 2020 2020 2069   try:..        i
-00000790: 6620 7379 732e 706c 6174 666f 726d 203d  f sys.platform =
-000007a0: 3d20 2277 696e 3332 223a 0d0a 2020 2020  = "win32":..    
-000007b0: 2020 2020 2020 2020 6f75 7470 7574 203d          output =
-000007c0: 2073 7562 7072 6f63 6573 732e 6368 6563   subprocess.chec
-000007d0: 6b5f 6f75 7470 7574 280d 0a20 2020 2020  k_output(..     
-000007e0: 2020 2020 2020 2020 2020 205b 0d0a 2020             [..  
-000007f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000800: 2020 2266 6670 726f 6265 222c 0d0a 2020    "ffprobe",..  
-00000810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000820: 2020 222d 6c6f 676c 6576 656c 222c 0d0a    "-loglevel",..
-00000830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000840: 2020 2020 222d 3122 2c0d 0a20 2020 2020      "-1",..     
-00000850: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000860: 2d68 6964 655f 6261 6e6e 6572 222c 0d0a  -hide_banner",..
-00000870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000880: 2020 2020 222d 7368 6f77 5f65 6e74 7269      "-show_entri
-00000890: 6573 222c 0d0a 2020 2020 2020 2020 2020  es",..          
-000008a0: 2020 2020 2020 2020 2020 2266 6f72 6d61            "forma
-000008b0: 743d 6475 7261 7469 6f6e 222c 0d0a 2020  t=duration",..  
-000008c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008d0: 2020 222d 6f66 222c 0d0a 2020 2020 2020    "-of",..      
-000008e0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-000008f0: 6566 6175 6c74 3d6e 6f70 7269 6e74 5f77  efault=noprint_w
-00000900: 7261 7070 6572 733d 313a 6e6f 6b65 793d  rappers=1:nokey=
-00000910: 3122 2c0d 0a20 2020 2020 2020 2020 2020  1",..           
-00000920: 2020 2020 2020 2020 2066 696c 655f 6e61           file_na
-00000930: 6d65 2c0d 0a20 2020 2020 2020 2020 2020  me,..           
-00000940: 2020 2020 205d 2c0d 0a20 2020 2020 2020       ],..       
-00000950: 2020 2020 2020 2020 2075 6e69 7665 7273           univers
-00000960: 616c 5f6e 6577 6c69 6e65 733d 5472 7565  al_newlines=True
-00000970: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000980: 2020 2063 7265 6174 696f 6e66 6c61 6773     creationflags
-00000990: 3d73 7562 7072 6f63 6573 732e 4352 4541  =subprocess.CREA
-000009a0: 5445 5f4e 4f5f 5749 4e44 4f57 2c0d 0a20  TE_NO_WINDOW,.. 
-000009b0: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
-000009c0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-000009d0: 2020 2020 2020 2020 206f 7574 7075 7420           output 
-000009e0: 3d20 7375 6270 726f 6365 7373 2e63 6865  = subprocess.che
-000009f0: 636b 5f6f 7574 7075 7428 0d0a 2020 2020  ck_output(..    
-00000a00: 2020 2020 2020 2020 2020 2020 5b0d 0a20              [.. 
-00000a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a20: 2020 2022 6666 7072 6f62 6522 2c0d 0a20     "ffprobe",.. 
-00000a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a40: 2020 2022 2d6c 6f67 6c65 7665 6c22 2c0d     "-loglevel",.
-00000a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000a60: 2020 2020 2022 2d31 222c 0d0a 2020 2020       "-1",..    
-00000a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a80: 222d 6869 6465 5f62 616e 6e65 7222 2c0d  "-hide_banner",.
-00000a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000aa0: 2020 2020 2022 2d73 686f 775f 656e 7472       "-show_entr
-00000ab0: 6965 7322 2c0d 0a20 2020 2020 2020 2020  ies",..         
-00000ac0: 2020 2020 2020 2020 2020 2022 666f 726d             "form
-00000ad0: 6174 3d64 7572 6174 696f 6e22 2c0d 0a20  at=duration",.. 
-00000ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000af0: 2020 2022 2d6f 6622 2c0d 0a20 2020 2020     "-of",..     
-00000b00: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000b10: 6465 6661 756c 743d 6e6f 7072 696e 745f  default=noprint_
-00000b20: 7772 6170 7065 7273 3d31 3a6e 6f6b 6579  wrappers=1:nokey
-00000b30: 3d31 222c 0d0a 2020 2020 2020 2020 2020  =1",..          
-00000b40: 2020 2020 2020 2020 2020 6669 6c65 5f6e            file_n
-00000b50: 616d 652c 0d0a 2020 2020 2020 2020 2020  ame,..          
-00000b60: 2020 2020 2020 5d2c 0d0a 2020 2020 2020        ],..      
-00000b70: 2020 2020 2020 2020 2020 756e 6976 6572            univer
-00000b80: 7361 6c5f 6e65 776c 696e 6573 3d54 7275  sal_newlines=Tru
-00000b90: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00000ba0: 290d 0a0d 0a20 2020 2020 2020 2072 6574  )....        ret
-00000bb0: 7572 6e20 696e 7428 666c 6f61 7428 6f75  urn int(float(ou
-00000bc0: 7470 7574 2e73 7472 6970 2829 2920 2a20  tput.strip()) * 
-00000bd0: 3130 3030 290d 0a20 2020 2065 7863 6570  1000)..    excep
-00000be0: 7420 4578 6365 7074 696f 6e3a 0d0a 2020  t Exception:..  
-00000bf0: 2020 2020 2020 2320 544f 444f 3a20 6164        # TODO: ad
-00000c00: 6420 6c6f 6767 696e 670d 0a20 2020 2020  d logging..     
-00000c10: 2020 2072 6574 7572 6e20 4e6f 6e65 0d0a     return None..
-00000c20: 0d0a 0d0a 6465 6620 5f75 7365 735f 6572  ....def _uses_er
-00000c30: 726f 725f 6c6f 676c 6576 656c 2863 6d64  ror_loglevel(cmd
-00000c40: 3a20 4c69 7374 5b73 7472 5d29 202d 3e20  : List[str]) -> 
-00000c50: 626f 6f6c 3a0d 0a20 2020 2074 7279 3a0d  bool:..    try:.
-00000c60: 0a20 2020 2020 2020 2069 6478 203d 2063  .        idx = c
-00000c70: 6d64 2e69 6e64 6578 2822 2d6c 6f67 6c65  md.index("-logle
-00000c80: 7665 6c22 290d 0a20 2020 2020 2020 2069  vel")..        i
-00000c90: 6620 636d 645b 6964 7820 2b20 315d 203d  f cmd[idx + 1] =
-00000ca0: 3d20 2265 7272 6f72 223a 0d0a 2020 2020  = "error":..    
-00000cb0: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-00000cc0: 7275 650d 0a20 2020 2020 2020 2065 6c73  rue..        els
-00000cd0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00000ce0: 7265 7475 726e 2046 616c 7365 0d0a 2020  return False..  
-00000cf0: 2020 6578 6365 7074 2056 616c 7565 4572    except ValueEr
-00000d00: 726f 723a 0d0a 2020 2020 2020 2020 7265  ror:..        re
-00000d10: 7475 726e 2046 616c 7365 0d0a 0d0a 0d0a  turn False......
-00000d20: 636c 6173 7320 4666 6d70 6567 5072 6f67  class FfmpegProg
-00000d30: 7265 7373 3a0d 0a20 2020 2044 5552 5f52  ress:..    DUR_R
-00000d40: 4547 4558 203d 2072 652e 636f 6d70 696c  EGEX = re.compil
-00000d50: 6528 0d0a 2020 2020 2020 2020 7222 4475  e(..        r"Du
-00000d60: 7261 7469 6f6e 3a20 283f 503c 686f 7572  ration: (?P<hour
-00000d70: 3e5c 647b 327d 293a 283f 503c 6d69 6e3e  >\d{2}):(?P<min>
-00000d80: 5c64 7b32 7d29 3a28 3f50 3c73 6563 3e5c  \d{2}):(?P<sec>\
-00000d90: 647b 327d 295c 2e28 3f50 3c6d 733e 5c64  d{2})\.(?P<ms>\d
-00000da0: 7b32 7d29 220d 0a20 2020 2029 0d0a 2020  {2})"..    )..  
-00000db0: 2020 5449 4d45 5f52 4547 4558 203d 2072    TIME_REGEX = r
-00000dc0: 652e 636f 6d70 696c 6528 0d0a 2020 2020  e.compile(..    
-00000dd0: 2020 2020 7222 6f75 745f 7469 6d65 3d28      r"out_time=(
-00000de0: 3f50 3c68 6f75 723e 5c64 7b32 7d29 3a28  ?P<hour>\d{2}):(
-00000df0: 3f50 3c6d 696e 3e5c 647b 327d 293a 283f  ?P<min>\d{2}):(?
-00000e00: 503c 7365 633e 5c64 7b32 7d29 5c2e 283f  P<sec>\d{2})\.(?
-00000e10: 503c 6d73 3e5c 647b 327d 2922 0d0a 2020  P<ms>\d{2})"..  
-00000e20: 2020 290d 0a0d 0a20 2020 2064 6566 205f    )....    def _
-00000e30: 5f69 6e69 745f 5f28 7365 6c66 2c20 636d  _init__(self, cm
-00000e40: 643a 204c 6973 745b 7374 725d 2c20 6472  d: List[str], dr
-00000e50: 795f 7275 6e3a 2062 6f6f 6c20 3d20 4661  y_run: bool = Fa
-00000e60: 6c73 6529 202d 3e20 4e6f 6e65 3a0d 0a20  lse) -> None:.. 
-00000e70: 2020 2020 2020 2027 2727 496e 6974 6961         '''Initia
-00000e80: 6c69 7a65 2074 6865 2046 666d 7065 6750  lize the FfmpegP
-00000e90: 726f 6772 6573 7320 636c 6173 732e 0d0a  rogress class...
-00000ea0: 0d0a 2020 2020 2020 2020 4172 6773 3a0d  ..        Args:.
-00000eb0: 0a20 2020 2020 2020 2020 2020 2063 6d64  .            cmd
-00000ec0: 2028 4c69 7374 5b73 7472 5d29 3a20 4120   (List[str]): A 
-00000ed0: 6c69 7374 206f 6620 636f 6d6d 616e 6420  list of command 
-00000ee0: 6c69 6e65 2065 6c65 6d65 6e74 732c 2065  line elements, e
-00000ef0: 2e67 2e20 5b22 6666 6d70 6567 222c 2022  .g. ["ffmpeg", "
-00000f00: 2d69 222c 202e 2e2e 5d0d 0a20 2020 2020  -i", ...]..     
-00000f10: 2020 2020 2020 2064 7279 5f72 756e 2028         dry_run (
-00000f20: 626f 6f6c 2c20 6f70 7469 6f6e 616c 293a  bool, optional):
-00000f30: 204f 6e6c 7920 7368 6f77 2077 6861 7420   Only show what 
-00000f40: 776f 756c 6420 6265 2064 6f6e 652e 2044  would be done. D
-00000f50: 6566 6175 6c74 7320 746f 2046 616c 7365  efaults to False
-00000f60: 2e0d 0a20 2020 2020 2020 2027 2727 0d0a  ...        '''..
-00000f70: 2020 2020 2020 2020 7365 6c66 2e63 6d64          self.cmd
-00000f80: 203d 2063 6d64 0d0a 2020 2020 2020 2020   = cmd..        
-00000f90: 7365 6c66 2e73 7464 6572 723a 2055 6e69  self.stderr: Uni
-00000fa0: 6f6e 5b73 7472 2c20 4e6f 6e65 5d20 3d20  on[str, None] = 
-00000fb0: 4e6f 6e65 0d0a 2020 2020 2020 2020 7365  None..        se
-00000fc0: 6c66 2e64 7279 5f72 756e 203d 2064 7279  lf.dry_run = dry
-00000fd0: 5f72 756e 0d0a 2020 2020 2020 2020 7365  _run..        se
-00000fe0: 6c66 2e70 726f 6365 7373 3a20 416e 7920  lf.process: Any 
-00000ff0: 3d20 4e6f 6e65 0d0a 2020 2020 2020 2020  = None..        
-00001000: 7365 6c66 2e73 7464 6572 725f 6361 6c6c  self.stderr_call
-00001010: 6261 636b 3a20 556e 696f 6e5b 4361 6c6c  back: Union[Call
-00001020: 6162 6c65 5b5b 7374 725d 2c20 4e6f 6e65  able[[str], None
-00001030: 5d2c 204e 6f6e 655d 203d 204e 6f6e 650d  ], None] = None.
-00001040: 0a20 2020 2020 2020 2069 6620 7379 732e  .        if sys.
-00001050: 706c 6174 666f 726d 203d 3d20 2277 696e  platform == "win
-00001060: 3332 223a 0d0a 2020 2020 2020 2020 2020  32":..          
-00001070: 2020 7365 6c66 2e62 6173 655f 706f 7065    self.base_pope
-00001080: 6e5f 6b77 6172 6773 203d 207b 0d0a 2020  n_kwargs = {..  
-00001090: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-000010a0: 7464 696e 223a 2073 7562 7072 6f63 6573  tdin": subproces
-000010b0: 732e 5049 5045 2c20 2023 2041 7070 6c79  s.PIPE,  # Apply
-000010c0: 2073 7464 696e 2069 736f 6c61 7469 6f6e   stdin isolation
-000010d0: 2062 7920 6372 6561 7469 6e67 2073 6570   by creating sep
-000010e0: 6172 6174 6520 7069 7065 2e0d 0a20 2020  arate pipe...   
-000010f0: 2020 2020 2020 2020 2020 2020 2022 7374               "st
-00001100: 646f 7574 223a 2073 7562 7072 6f63 6573  dout": subproces
-00001110: 732e 5049 5045 2c0d 0a20 2020 2020 2020  s.PIPE,..       
-00001120: 2020 2020 2020 2020 2022 7374 6465 7272           "stderr
-00001130: 223a 2073 7562 7072 6f63 6573 732e 5354  ": subprocess.ST
-00001140: 444f 5554 2c0d 0a20 2020 2020 2020 2020  DOUT,..         
-00001150: 2020 2020 2020 2022 756e 6976 6572 7361         "universa
-00001160: 6c5f 6e65 776c 696e 6573 223a 2046 616c  l_newlines": Fal
-00001170: 7365 2c0d 0a20 2020 2020 2020 2020 2020  se,..           
-00001180: 2020 2020 2022 7368 656c 6c22 3a20 5472       "shell": Tr
-00001190: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
-000011a0: 207d 0d0a 2020 2020 2020 2020 656c 7365   }..        else
-000011b0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-000011c0: 656c 662e 6261 7365 5f70 6f70 656e 5f6b  elf.base_popen_k
-000011d0: 7761 7267 7320 3d20 7b0d 0a20 2020 2020  wargs = {..     
-000011e0: 2020 2020 2020 2020 2020 2022 7374 6469             "stdi
-000011f0: 6e22 3a20 7375 6270 726f 6365 7373 2e50  n": subprocess.P
-00001200: 4950 452c 2020 2320 4170 706c 7920 7374  IPE,  # Apply st
-00001210: 6469 6e20 6973 6f6c 6174 696f 6e20 6279  din isolation by
-00001220: 2063 7265 6174 696e 6720 7365 7061 7261   creating separa
-00001230: 7465 2070 6970 652e 0d0a 2020 2020 2020  te pipe...      
-00001240: 2020 2020 2020 2020 2020 2273 7464 6f75            "stdou
-00001250: 7422 3a20 7375 6270 726f 6365 7373 2e50  t": subprocess.P
-00001260: 4950 452c 0d0a 2020 2020 2020 2020 2020  IPE,..          
-00001270: 2020 2020 2020 2273 7464 6572 7222 3a20        "stderr": 
-00001280: 7375 6270 726f 6365 7373 2e53 5444 4f55  subprocess.STDOU
-00001290: 542c 0d0a 2020 2020 2020 2020 2020 2020  T,..            
-000012a0: 2020 2020 2275 6e69 7665 7273 616c 5f6e      "universal_n
-000012b0: 6577 6c69 6e65 7322 3a20 4661 6c73 652c  ewlines": False,
-000012c0: 0d0a 2020 2020 2020 2020 2020 2020 7d0d  ..            }.
-000012d0: 0a0d 0a20 2020 2064 6566 2073 6574 5f73  ...    def set_s
-000012e0: 7464 6572 725f 6361 6c6c 6261 636b 2873  tderr_callback(s
-000012f0: 656c 662c 2063 616c 6c62 6163 6b3a 2043  elf, callback: C
-00001300: 616c 6c61 626c 655b 5b73 7472 5d2c 204e  allable[[str], N
-00001310: 6f6e 655d 2920 2d3e 204e 6f6e 653a 0d0a  one]) -> None:..
-00001320: 2020 2020 2020 2020 2727 270d 0a20 2020          '''..   
-00001330: 2020 2020 2053 6574 2061 2063 616c 6c62       Set a callb
-00001340: 6163 6b20 6675 6e63 7469 6f6e 2074 6f20  ack function to 
-00001350: 6265 2063 616c 6c65 6420 6f6e 2073 7464  be called on std
-00001360: 6572 7220 6f75 7470 7574 2e0d 0a20 2020  err output...   
-00001370: 2020 2020 2054 6865 2063 616c 6c62 6163       The callbac
-00001380: 6b20 6675 6e63 7469 6f6e 206d 7573 7420  k function must 
-00001390: 6163 6365 7074 2061 2073 696e 676c 6520  accept a single 
-000013a0: 7374 7269 6e67 2061 7267 756d 656e 742e  string argument.
-000013b0: 0d0a 2020 2020 2020 2020 4e6f 7465 2074  ..        Note t
-000013c0: 6861 7420 7468 6973 2069 7320 6361 6c6c  hat this is call
-000013d0: 6564 206f 6e20 6576 6572 7920 6c69 6e65  ed on every line
-000013e0: 206f 6620 7374 6465 7272 206f 7574 7075   of stderr outpu
-000013f0: 742c 2073 6f20 6974 2063 616e 2062 6520  t, so it can be 
-00001400: 6361 6c6c 6564 2061 206c 6f74 2e0d 0a20  called a lot... 
-00001410: 2020 2020 2020 2041 6c73 6f20 6e6f 7465         Also note
-00001420: 2074 6861 7420 7374 646f 7574 2f73 7464   that stdout/std
-00001430: 6572 7220 6172 6520 6a6f 696e 6564 2069  err are joined i
-00001440: 6e74 6f20 6f6e 6520 7374 7265 616d 2c20  nto one stream, 
-00001450: 736f 2079 6f75 206d 6967 6874 2067 6574  so you might get
-00001460: 2073 7464 6f75 7420 6f75 7470 7574 2069   stdout output i
-00001470: 6e20 7468 6520 6361 6c6c 6261 636b 2e0d  n the callback..
-00001480: 0a0d 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-00001490: 0d0a 2020 2020 2020 2020 2020 2020 6361  ..            ca
-000014a0: 6c6c 6261 636b 2028 4361 6c6c 6162 6c65  llback (Callable
-000014b0: 5b5b 7374 725d 2c20 4e6f 6e65 5d29 3a20  [[str], None]): 
-000014c0: 4120 6361 6c6c 6261 636b 2066 756e 6374  A callback funct
-000014d0: 696f 6e20 7468 6174 2061 6363 6570 7473  ion that accepts
-000014e0: 2061 2073 696e 676c 6520 7374 7269 6e67   a single string
-000014f0: 2061 7267 756d 656e 742e 0d0a 2020 2020   argument...    
-00001500: 2020 2020 2727 270d 0a20 2020 2020 2020      '''..       
-00001510: 2069 6620 6e6f 7420 6361 6c6c 6162 6c65   if not callable
-00001520: 2863 616c 6c62 6163 6b29 206f 7220 6c65  (callback) or le
-00001530: 6e28 6361 6c6c 6261 636b 2e5f 5f63 6f64  n(callback.__cod
-00001540: 655f 5f2e 636f 5f76 6172 6e61 6d65 7329  e__.co_varnames)
-00001550: 2021 3d20 313a 0d0a 2020 2020 2020 2020   != 1:..        
-00001560: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00001570: 7272 6f72 280d 0a20 2020 2020 2020 2020  rror(..         
-00001580: 2020 2020 2020 2022 4361 6c6c 6261 636b         "Callback
-00001590: 206d 7573 7420 6265 2061 2066 756e 6374   must be a funct
-000015a0: 696f 6e20 7468 6174 2061 6363 6570 7473  ion that accepts
-000015b0: 206f 6e6c 7920 6f6e 6520 6172 6775 6d65   only one argume
-000015c0: 6e74 220d 0a20 2020 2020 2020 2020 2020  nt"..           
-000015d0: 2029 0d0a 0d0a 2020 2020 2020 2020 7365   )....        se
-000015e0: 6c66 2e73 7464 6572 725f 6361 6c6c 6261  lf.stderr_callba
-000015f0: 636b 203d 2063 616c 6c62 6163 6b0d 0a0d  ck = callback...
-00001600: 0a20 2020 2064 6566 2072 756e 5f63 6f6d  .    def run_com
-00001610: 6d61 6e64 5f77 6974 685f 7072 6f67 7265  mand_with_progre
-00001620: 7373 280d 0a20 2020 2020 2020 2073 656c  ss(..        sel
-00001630: 662c 2070 6f70 656e 5f6b 7761 7267 733d  f, popen_kwargs=
-00001640: 4e6f 6e65 2c20 6475 7261 7469 6f6e 5f6f  None, duration_o
-00001650: 7665 7272 6964 653a 2055 6e69 6f6e 5b66  verride: Union[f
-00001660: 6c6f 6174 2c20 4e6f 6e65 5d20 3d20 4e6f  loat, None] = No
-00001670: 6e65 0d0a 2020 2020 2920 2d3e 2049 7465  ne..    ) -> Ite
-00001680: 7261 746f 725b 696e 745d 3a0d 0a20 2020  rator[int]:..   
-00001690: 2020 2020 2027 2727 0d0a 2020 2020 2020       '''..      
-000016a0: 2020 5275 6e20 616e 2066 666d 7065 6720    Run an ffmpeg 
-000016b0: 636f 6d6d 616e 642c 2074 7279 696e 6720  command, trying 
-000016c0: 746f 2063 6170 7475 7265 2074 6865 2070  to capture the p
-000016d0: 726f 6365 7373 206f 7574 7075 7420 616e  rocess output an
-000016e0: 6420 6361 6c63 756c 6174 650d 0a20 2020  d calculate..   
-000016f0: 2020 2020 2074 6865 2064 7572 6174 696f       the duratio
-00001700: 6e20 2f20 7072 6f67 7265 7373 2e0d 0a20  n / progress... 
-00001710: 2020 2020 2020 2059 6965 6c64 7320 7468         Yields th
-00001720: 6520 7072 6f67 7265 7373 2069 6e20 7065  e progress in pe
-00001730: 7263 656e 742e 0d0a 0d0a 2020 2020 2020  rcent.....      
-00001740: 2020 4172 6773 3a0d 0a20 2020 2020 2020    Args:..       
-00001750: 2020 2020 2070 6f70 656e 5f6b 7761 7267       popen_kwarg
-00001760: 7320 2864 6963 742c 206f 7074 696f 6e61  s (dict, optiona
-00001770: 6c29 3a20 4120 6469 6374 2074 6f20 7370  l): A dict to sp
-00001780: 6563 6966 7920 6578 7472 6120 6172 6775  ecify extra argu
-00001790: 6d65 6e74 7320 746f 2074 6865 2070 6f70  ments to the pop
-000017a0: 656e 2063 616c 6c2c 2065 2e67 2e20 7b20  en call, e.g. { 
-000017b0: 6372 6561 7469 6f6e 666c 6167 733a 2043  creationflags: C
-000017c0: 5245 4154 455f 4e4f 5f57 494e 444f 5720  REATE_NO_WINDOW 
-000017d0: 7d0d 0a20 2020 2020 2020 2020 2020 2064  }..            d
-000017e0: 7572 6174 696f 6e5f 6f76 6572 7269 6465  uration_override
-000017f0: 2028 666c 6f61 742c 206f 7074 696f 6e61   (float, optiona
-00001800: 6c29 3a20 5468 6520 6475 7261 7469 6f6e  l): The duration
-00001810: 2069 6e20 7365 636f 6e64 732e 2049 6620   in seconds. If 
-00001820: 6e6f 7420 7370 6563 6966 6965 642c 2069  not specified, i
-00001830: 7420 7769 6c6c 2062 6520 6361 6c63 756c  t will be calcul
-00001840: 6174 6564 2066 726f 6d20 7468 6520 6666  ated from the ff
-00001850: 6d70 6567 206f 7574 7075 742e 0d0a 0d0a  mpeg output.....
-00001860: 2020 2020 2020 2020 5261 6973 6573 3a0d          Raises:.
-00001870: 0a20 2020 2020 2020 2020 2020 2052 756e  .            Run
-00001880: 7469 6d65 4572 726f 723a 2049 6620 7468  timeError: If th
-00001890: 6520 636f 6d6d 616e 6420 6661 696c 732c  e command fails,
-000018a0: 2061 6e20 6578 6365 7074 696f 6e20 6973   an exception is
-000018b0: 2072 6169 7365 642e 0d0a 0d0a 2020 2020   raised.....    
-000018c0: 2020 2020 5969 656c 6473 3a0d 0a20 2020      Yields:..   
-000018d0: 2020 2020 2020 2020 2049 7465 7261 746f           Iterato
-000018e0: 725b 696e 745d 3a20 4120 6765 6e65 7261  r[int]: A genera
-000018f0: 746f 7220 7468 6174 2079 6965 6c64 7320  tor that yields 
-00001900: 7468 6520 7072 6f67 7265 7373 2069 6e20  the progress in 
-00001910: 7065 7263 656e 742e 0d0a 2020 2020 2020  percent...      
-00001920: 2020 2727 270d 0a20 2020 2020 2020 2069    '''..        i
-00001930: 6620 7365 6c66 2e64 7279 5f72 756e 3a0d  f self.dry_run:.
-00001940: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00001950: 7572 6e20 7365 6c66 2e63 6d64 0d0a 0d0a  urn self.cmd....
-00001960: 2020 2020 2020 2020 746f 7461 6c5f 6475          total_du
-00001970: 723a 2055 6e69 6f6e 5b4e 6f6e 652c 2069  r: Union[None, i
-00001980: 6e74 5d20 3d20 4e6f 6e65 0d0a 2020 2020  nt] = None..    
-00001990: 2020 2020 6966 205f 7573 6573 5f65 7272      if _uses_err
-000019a0: 6f72 5f6c 6f67 6c65 7665 6c28 7365 6c66  or_loglevel(self
-000019b0: 2e63 6d64 293a 0d0a 2020 2020 2020 2020  .cmd):..        
-000019c0: 2020 2020 746f 7461 6c5f 6475 7220 3d20      total_dur = 
-000019d0: 5f70 726f 6265 5f64 7572 6174 696f 6e28  _probe_duration(
-000019e0: 7365 6c66 2e63 6d64 290d 0a0d 0a20 2020  self.cmd)....   
-000019f0: 2020 2020 2063 6d64 5f77 6974 685f 7072       cmd_with_pr
-00001a00: 6f67 7265 7373 203d 2028 0d0a 2020 2020  ogress = (..    
-00001a10: 2020 2020 2020 2020 5b73 656c 662e 636d          [self.cm
-00001a20: 645b 305d 5d20 2b20 5b22 2d70 726f 6772  d[0]] + ["-progr
-00001a30: 6573 7322 2c20 222d 222c 2022 2d6e 6f73  ess", "-", "-nos
-00001a40: 7461 7473 225d 202b 2073 656c 662e 636d  tats"] + self.cm
-00001a50: 645b 313a 5d0d 0a20 2020 2020 2020 2029  d[1:]..        )
-00001a60: 0d0a 0d0a 2020 2020 2020 2020 7374 6465  ....        stde
-00001a70: 7272 203d 205b 5d0d 0a20 2020 2020 2020  rr = []..       
-00001a80: 2062 6173 655f 706f 7065 6e5f 6b77 6172   base_popen_kwar
-00001a90: 6773 203d 2073 656c 662e 6261 7365 5f70  gs = self.base_p
-00001aa0: 6f70 656e 5f6b 7761 7267 732e 636f 7079  open_kwargs.copy
-00001ab0: 2829 0d0a 2020 2020 2020 2020 6966 2070  ()..        if p
-00001ac0: 6f70 656e 5f6b 7761 7267 7320 6973 206e  open_kwargs is n
-00001ad0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-00001ae0: 2020 2020 2020 6261 7365 5f70 6f70 656e        base_popen
-00001af0: 5f6b 7761 7267 732e 7570 6461 7465 2870  _kwargs.update(p
-00001b00: 6f70 656e 5f6b 7761 7267 7329 0d0a 0d0a  open_kwargs)....
-00001b10: 2020 2020 2020 2020 6966 2073 7973 2e70          if sys.p
-00001b20: 6c61 7466 6f72 6d20 3d3d 2022 7769 6e64  latform == "wind
-00001b30: 3332 223a 0d0a 2020 2020 2020 2020 2020  32":..          
-00001b40: 2020 7365 6c66 2e70 726f 6365 7373 203d    self.process =
-00001b50: 2073 7562 7072 6f63 6573 732e 506f 7065   subprocess.Pope
-00001b60: 6e28 0d0a 2020 2020 2020 2020 2020 2020  n(..            
-00001b70: 2020 2020 636d 645f 7769 7468 5f70 726f      cmd_with_pro
-00001b80: 6772 6573 732c 0d0a 2020 2020 2020 2020  gress,..        
-00001b90: 2020 2020 2020 2020 2a2a 6261 7365 5f70          **base_p
-00001ba0: 6f70 656e 5f6b 7761 7267 732c 0d0a 2020  open_kwargs,..  
-00001bb0: 2020 2020 2020 2020 2020 2020 2020 6372                cr
-00001bc0: 6561 7469 6f6e 666c 6167 733d 7375 6270  eationflags=subp
-00001bd0: 726f 6365 7373 2e43 5245 4154 455f 4e4f  rocess.CREATE_NO
-00001be0: 5f57 494e 444f 572c 0d0a 2020 2020 2020  _WINDOW,..      
-00001bf0: 2020 2020 2020 2920 2023 2074 7970 653a        )  # type:
-00001c00: 2069 676e 6f72 650d 0a20 2020 2020 2020   ignore..       
-00001c10: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00001c20: 2020 2020 7365 6c66 2e70 726f 6365 7373      self.process
-00001c30: 203d 2073 7562 7072 6f63 6573 732e 506f   = subprocess.Po
-00001c40: 7065 6e28 0d0a 2020 2020 2020 2020 2020  pen(..          
-00001c50: 2020 2020 2020 636d 645f 7769 7468 5f70        cmd_with_p
-00001c60: 726f 6772 6573 732c 0d0a 2020 2020 2020  rogress,..      
-00001c70: 2020 2020 2020 2020 2020 2a2a 6261 7365            **base
-00001c80: 5f70 6f70 656e 5f6b 7761 7267 732c 0d0a  _popen_kwargs,..
-00001c90: 2020 2020 2020 2020 2020 2020 2920 2023              )  #
-00001ca0: 2074 7970 653a 2069 676e 6f72 650d 0a0d   type: ignore...
-00001cb0: 0a20 2020 2020 2020 2079 6965 6c64 2030  .        yield 0
-00001cc0: 0d0a 0d0a 2020 2020 2020 2020 7768 696c  ....        whil
-00001cd0: 6520 5472 7565 3a0d 0a20 2020 2020 2020  e True:..       
-00001ce0: 2020 2020 2069 6620 7365 6c66 2e70 726f       if self.pro
-00001cf0: 6365 7373 2e73 7464 6f75 7420 6973 204e  cess.stdout is N
-00001d00: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00001d10: 2020 2020 2020 636f 6e74 696e 7565 0d0a        continue..
-00001d20: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
-00001d30: 6465 7272 5f6c 696e 6520 3d20 280d 0a20  derr_line = (.. 
-00001d40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00001d50: 656c 662e 7072 6f63 6573 732e 7374 646f  elf.process.stdo
-00001d60: 7574 2e72 6561 646c 696e 6528 292e 6465  ut.readline().de
-00001d70: 636f 6465 2822 7574 662d 3822 2c20 6572  code("utf-8", er
-00001d80: 726f 7273 3d22 7265 706c 6163 6522 292e  rors="replace").
-00001d90: 7374 7269 7028 290d 0a20 2020 2020 2020  strip()..       
-00001da0: 2020 2020 2029 0d0a 0d0a 2020 2020 2020       )....      
-00001db0: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
-00001dc0: 6465 7272 5f63 616c 6c62 6163 6b3a 0d0a  derr_callback:..
-00001dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001de0: 7365 6c66 2e73 7464 6572 725f 6361 6c6c  self.stderr_call
-00001df0: 6261 636b 2873 7464 6572 725f 6c69 6e65  back(stderr_line
-00001e00: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00001e10: 2069 6620 7374 6465 7272 5f6c 696e 6520   if stderr_line 
-00001e20: 3d3d 2027 2720 616e 6420 7365 6c66 2e70  == '' and self.p
-00001e30: 726f 6365 7373 2e70 6f6c 6c28 2920 6973  rocess.poll() is
-00001e40: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-00001e50: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-00001e60: 6b0d 0a0d 0a20 2020 2020 2020 2020 2020  k....           
-00001e70: 2073 7464 6572 722e 6170 7065 6e64 2873   stderr.append(s
-00001e80: 7464 6572 725f 6c69 6e65 2e73 7472 6970  tderr_line.strip
-00001e90: 2829 290d 0a0d 0a20 2020 2020 2020 2020  ())....         
-00001ea0: 2020 2073 656c 662e 7374 6465 7272 203d     self.stderr =
-00001eb0: 2022 5c6e 222e 6a6f 696e 2873 7464 6572   "\n".join(stder
-00001ec0: 7229 0d0a 0d0a 2020 2020 2020 2020 2020  r)....          
-00001ed0: 2020 6966 2074 6f74 616c 5f64 7572 2069    if total_dur i
-00001ee0: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
-00001ef0: 2020 2020 2020 2020 2074 6f74 616c 5f64           total_d
-00001f00: 7572 5f6d 6174 6368 203d 2073 656c 662e  ur_match = self.
-00001f10: 4455 525f 5245 4745 582e 7365 6172 6368  DUR_REGEX.search
-00001f20: 2873 7464 6572 725f 6c69 6e65 290d 0a20  (stderr_line).. 
-00001f30: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00001f40: 6620 746f 7461 6c5f 6475 725f 6d61 7463  f total_dur_matc
-00001f50: 683a 0d0a 2020 2020 2020 2020 2020 2020  h:..            
-00001f60: 2020 2020 2020 2020 746f 7461 6c5f 6475          total_du
-00001f70: 7220 3d20 746f 5f6d 7328 2a2a 746f 7461  r = to_ms(**tota
-00001f80: 6c5f 6475 725f 6d61 7463 682e 6772 6f75  l_dur_match.grou
-00001f90: 7064 6963 7428 2929 0d0a 2020 2020 2020  pdict())..      
-00001fa0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00001fb0: 6e74 696e 7565 0d0a 2020 2020 2020 2020  ntinue..        
-00001fc0: 2020 2020 2020 2020 656c 6966 2064 7572          elif dur
-00001fd0: 6174 696f 6e5f 6f76 6572 7269 6465 2069  ation_override i
-00001fe0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
-00001ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002000: 2023 2075 7365 2074 6865 206f 7665 7272   # use the overr
-00002010: 6964 6520 2873 686f 756c 6420 6170 706c  ide (should appl
-00002020: 7920 696e 2074 6865 2066 6972 7374 206c  y in the first l
-00002030: 6f6f 7029 0d0a 2020 2020 2020 2020 2020  oop)..          
-00002040: 2020 2020 2020 2020 2020 746f 7461 6c5f            total_
-00002050: 6475 7220 3d20 696e 7428 6475 7261 7469  dur = int(durati
-00002060: 6f6e 5f6f 7665 7272 6964 6520 2a20 3130  on_override * 10
-00002070: 3030 290d 0a20 2020 2020 2020 2020 2020  00)..           
-00002080: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-00002090: 650d 0a0d 0a20 2020 2020 2020 2020 2020  e....           
-000020a0: 2069 6620 746f 7461 6c5f 6475 723a 0d0a   if total_dur:..
-000020b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020c0: 7072 6f67 7265 7373 5f74 696d 6520 3d20  progress_time = 
-000020d0: 4666 6d70 6567 5072 6f67 7265 7373 2e54  FfmpegProgress.T
-000020e0: 494d 455f 5245 4745 582e 7365 6172 6368  IME_REGEX.search
-000020f0: 2873 7464 6572 725f 6c69 6e65 290d 0a20  (stderr_line).. 
-00002100: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00002110: 6620 7072 6f67 7265 7373 5f74 696d 653a  f progress_time:
-00002120: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002130: 2020 2020 2020 656c 6170 7365 645f 7469        elapsed_ti
-00002140: 6d65 203d 2074 6f5f 6d73 282a 2a70 726f  me = to_ms(**pro
-00002150: 6772 6573 735f 7469 6d65 2e67 726f 7570  gress_time.group
-00002160: 6469 6374 2829 290d 0a20 2020 2020 2020  dict())..       
-00002170: 2020 2020 2020 2020 2020 2020 2079 6965               yie
-00002180: 6c64 2069 6e74 2865 6c61 7073 6564 5f74  ld int(elapsed_t
-00002190: 696d 6520 2a20 3130 302f 2074 6f74 616c  ime * 100/ total
-000021a0: 5f64 7572 290d 0a0d 0a20 2020 2020 2020  _dur)....       
-000021b0: 2069 6620 7365 6c66 2e70 726f 6365 7373   if self.process
-000021c0: 2069 7320 4e6f 6e65 206f 7220 7365 6c66   is None or self
-000021d0: 2e70 726f 6365 7373 2e72 6574 7572 6e63  .process.returnc
-000021e0: 6f64 6520 213d 2030 3a0d 0a20 2020 2020  ode != 0:..     
-000021f0: 2020 2020 2020 2023 7072 696e 7428 7365         #print(se
-00002200: 6c66 2e70 726f 6365 7373 290d 0a20 2020  lf.process)..   
-00002210: 2020 2020 2020 2020 2023 7072 696e 7428           #print(
-00002220: 7365 6c66 2e70 726f 6365 7373 2e72 6574  self.process.ret
-00002230: 7572 6e63 6f64 6529 0d0a 2020 2020 2020  urncode)..      
-00002240: 2020 2020 2020 5f70 7265 7474 795f 7374        _pretty_st
-00002250: 6465 7272 203d 2022 5c6e 222e 6a6f 696e  derr = "\n".join
-00002260: 2873 7464 6572 7229 0d0a 2020 2020 2020  (stderr)..      
-00002270: 2020 2020 2020 7261 6973 6520 5275 6e74        raise Runt
-00002280: 696d 6545 7272 6f72 2866 2245 7272 6f72  imeError(f"Error
-00002290: 2072 756e 6e69 6e67 2063 6f6d 6d61 6e64   running command
-000022a0: 207b 7365 6c66 2e63 6d64 7d3a 207b 5f70   {self.cmd}: {_p
-000022b0: 7265 7474 795f 7374 6465 7272 7d22 290d  retty_stderr}").
-000022c0: 0a0d 0a20 2020 2020 2020 2079 6965 6c64  ...        yield
-000022d0: 2031 3030 0d0a 2020 2020 2020 2020 7365   100..        se
-000022e0: 6c66 2e70 726f 6365 7373 203d 204e 6f6e  lf.process = Non
-000022f0: 650d 0a0d 0a20 2020 2064 6566 2071 7569  e....    def qui
-00002300: 745f 6772 6163 6566 756c 6c79 2873 656c  t_gracefully(sel
-00002310: 6629 202d 3e20 4e6f 6e65 3a0d 0a20 2020  f) -> None:..   
-00002320: 2020 2020 2027 2727 0d0a 2020 2020 2020       '''..      
-00002330: 2020 5175 6974 2074 6865 2066 666d 7065    Quit the ffmpe
-00002340: 6720 7072 6f63 6573 7320 6279 2073 656e  g process by sen
-00002350: 6469 6e67 2027 7127 0d0a 0d0a 2020 2020  ding 'q'....    
-00002360: 2020 2020 5261 6973 6573 3a0d 0a20 2020      Raises:..   
-00002370: 2020 2020 2020 2020 2052 756e 7469 6d65           Runtime
-00002380: 4572 726f 723a 2049 6620 6e6f 2070 726f  Error: If no pro
-00002390: 6365 7373 2069 7320 666f 756e 642e 0d0a  cess is found...
-000023a0: 2020 2020 2020 2020 2727 270d 0a20 2020          '''..   
-000023b0: 2020 2020 2069 6620 7365 6c66 2e70 726f       if self.pro
-000023c0: 6365 7373 2069 7320 4e6f 6e65 3a0d 0a20  cess is None:.. 
-000023d0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-000023e0: 2052 756e 7469 6d65 4572 726f 7228 224e   RuntimeError("N
-000023f0: 6f20 7072 6f63 6573 7320 666f 756e 642e  o process found.
-00002400: 2044 6964 2079 6f75 2072 756e 2074 6865   Did you run the
-00002410: 2063 6f6d 6d61 6e64 3f22 290d 0a0d 0a20   command?").... 
-00002420: 2020 2020 2020 2073 656c 662e 7072 6f63         self.proc
-00002430: 6573 732e 636f 6d6d 756e 6963 6174 6528  ess.communicate(
-00002440: 696e 7075 743d 6222 7122 290d 0a20 2020  input=b"q")..   
-00002450: 2020 2020 2073 656c 662e 7072 6f63 6573       self.proces
-00002460: 732e 6b69 6c6c 2829 0d0a 2020 2020 2020  s.kill()..      
-00002470: 2020 7365 6c66 2e70 726f 6365 7373 203d    self.process =
-00002480: 204e 6f6e 650d 0a0d 0a20 2020 2064 6566   None....    def
-00002490: 2071 7569 7428 7365 6c66 2920 2d3e 204e   quit(self) -> N
-000024a0: 6f6e 653a 0d0a 2020 2020 2020 2020 2727  one:..        ''
-000024b0: 270d 0a20 2020 2020 2020 2051 7569 7420  '..        Quit 
-000024c0: 7468 6520 6666 6d70 6567 2070 726f 6365  the ffmpeg proce
-000024d0: 7373 2062 7920 7365 6e64 696e 6720 5349  ss by sending SI
-000024e0: 474b 494c 4c2e 0d0a 0d0a 2020 2020 2020  GKILL.....      
-000024f0: 2020 5261 6973 6573 3a0d 0a20 2020 2020    Raises:..     
-00002500: 2020 2020 2020 2052 756e 7469 6d65 4572         RuntimeEr
-00002510: 726f 723a 2049 6620 6e6f 2070 726f 6365  ror: If no proce
-00002520: 7373 2069 7320 666f 756e 642e 0d0a 2020  ss is found...  
-00002530: 2020 2020 2020 2727 270d 0a20 2020 2020        '''..     
-00002540: 2020 2069 6620 7365 6c66 2e70 726f 6365     if self.proce
-00002550: 7373 2069 7320 4e6f 6e65 3a0d 0a20 2020  ss is None:..   
-00002560: 2020 2020 2020 2020 2072 6169 7365 2052           raise R
-00002570: 756e 7469 6d65 4572 726f 7228 224e 6f20  untimeError("No 
-00002580: 7072 6f63 6573 7320 666f 756e 642e 2044  process found. D
-00002590: 6964 2079 6f75 2072 756e 2074 6865 2063  id you run the c
-000025a0: 6f6d 6d61 6e64 3f22 290d 0a0d 0a20 2020  ommand?")....   
-000025b0: 2020 2020 2073 656c 662e 7072 6f63 6573       self.proces
-000025c0: 732e 6b69 6c6c 2829 0d0a 2020 2020 2020  s.kill()..      
-000025d0: 2020 7365 6c66 2e70 726f 6365 7373 203d    self.process =
-000025e0: 204e 6f6e 650d 0a0d 0a0d 0a23 3d3d 3d3d   None......#====
+00000360: 3d3d 230d 0a0d 0a69 6d70 6f72 7420 7265  ==#....import re
+00000370: 0d0a 2369 6d70 6f72 7420 7375 6270 726f  ..#import subpro
+00000380: 6365 7373 0d0a 6672 6f6d 2074 7970 696e  cess..from typin
+00000390: 6720 696d 706f 7274 2041 6e79 2c20 4361  g import Any, Ca
+000003a0: 6c6c 6162 6c65 2c20 4974 6572 6174 6f72  llable, Iterator
+000003b0: 2c20 4c69 7374 2c20 4f70 7469 6f6e 616c  , List, Optional
+000003c0: 2c20 556e 696f 6e0d 0a0d 0a0d 0a64 6566  , Union......def
+000003d0: 2074 6f5f 6d73 282a 2a6b 7761 7267 733a   to_ms(**kwargs:
+000003e0: 2055 6e69 6f6e 5b66 6c6f 6174 2c20 696e   Union[float, in
+000003f0: 742c 2073 7472 5d29 202d 3e20 696e 743a  t, str]) -> int:
+00000400: 0d0a 2020 2020 686f 7572 203d 2069 6e74  ..    hour = int
+00000410: 286b 7761 7267 732e 6765 7428 2268 6f75  (kwargs.get("hou
+00000420: 7222 2c20 3029 290d 0a20 2020 206d 696e  r", 0))..    min
+00000430: 7574 6520 3d20 696e 7428 6b77 6172 6773  ute = int(kwargs
+00000440: 2e67 6574 2822 6d69 6e22 2c20 3029 290d  .get("min", 0)).
+00000450: 0a20 2020 2073 6563 203d 2069 6e74 286b  .    sec = int(k
+00000460: 7761 7267 732e 6765 7428 2273 6563 222c  wargs.get("sec",
+00000470: 2030 2929 0d0a 2020 2020 6d73 203d 2069   0))..    ms = i
+00000480: 6e74 286b 7761 7267 732e 6765 7428 226d  nt(kwargs.get("m
+00000490: 7322 2c20 3029 290d 0a0d 0a20 2020 2072  s", 0))....    r
+000004a0: 6574 7572 6e20 2868 6f75 7220 2a20 3630  eturn (hour * 60
+000004b0: 202a 2036 3020 2a20 3130 3030 2920 2b20   * 60 * 1000) + 
+000004c0: 286d 696e 7574 6520 2a20 3630 202a 2031  (minute * 60 * 1
+000004d0: 3030 3029 202b 2028 7365 6320 2a20 3130  000) + (sec * 10
+000004e0: 3030 2920 2b20 6d73 0d0a 0d0a 0d0a 6465  00) + ms......de
+000004f0: 6620 5f70 726f 6265 5f64 7572 6174 696f  f _probe_duratio
+00000500: 6e28 636d 643a 204c 6973 745b 7374 725d  n(cmd: List[str]
+00000510: 2920 2d3e 204f 7074 696f 6e61 6c5b 696e  ) -> Optional[in
+00000520: 745d 3a0d 0a20 2020 2027 2727 0d0a 2020  t]:..    '''..  
+00000530: 2020 4765 7420 7468 6520 6475 7261 7469    Get the durati
+00000540: 6f6e 2076 6961 2066 6670 726f 6265 2066  on via ffprobe f
+00000550: 726f 6d20 696e 7075 7420 6d65 6469 6120  rom input media 
+00000560: 6669 6c65 0d0a 2020 2020 696e 2063 6173  file..    in cas
+00000570: 6520 6666 6d70 6567 2077 6173 2072 756e  e ffmpeg was run
+00000580: 2077 6974 6820 6c6f 676c 6576 656c 3d65   with loglevel=e
+00000590: 7272 6f72 2e0d 0a0d 0a20 2020 2041 7267  rror.....    Arg
+000005a0: 733a 0d0a 2020 2020 2020 2020 636d 6420  s:..        cmd 
+000005b0: 284c 6973 745b 7374 725d 293a 2041 206c  (List[str]): A l
+000005c0: 6973 7420 6f66 2063 6f6d 6d61 6e64 206c  ist of command l
+000005d0: 696e 6520 656c 656d 656e 7473 2c20 652e  ine elements, e.
+000005e0: 672e 205b 2266 666d 7065 6722 2c20 222d  g. ["ffmpeg", "-
+000005f0: 6922 2c20 2e2e 2e5d 0d0a 0d0a 2020 2020  i", ...]....    
+00000600: 5265 7475 726e 733a 0d0a 2020 2020 2020  Returns:..      
+00000610: 2020 4f70 7469 6f6e 616c 5b69 6e74 5d3a    Optional[int]:
+00000620: 2054 6865 2064 7572 6174 696f 6e20 696e   The duration in
+00000630: 206d 696c 6c69 7365 636f 6e64 732e 0d0a   milliseconds...
+00000640: 2020 2020 2727 270d 0a0d 0a20 2020 2064      '''....    d
+00000650: 6566 205f 6765 745f 6669 6c65 5f6e 616d  ef _get_file_nam
+00000660: 6528 636d 643a 204c 6973 745b 7374 725d  e(cmd: List[str]
+00000670: 2920 2d3e 204f 7074 696f 6e61 6c5b 7374  ) -> Optional[st
+00000680: 725d 3a0d 0a20 2020 2020 2020 2074 7279  r]:..        try
+00000690: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
+000006a0: 6478 203d 2063 6d64 2e69 6e64 6578 2822  dx = cmd.index("
+000006b0: 2d69 2229 0d0a 2020 2020 2020 2020 2020  -i")..          
+000006c0: 2020 7265 7475 726e 2063 6d64 5b69 6478    return cmd[idx
+000006d0: 202b 2031 5d0d 0a20 2020 2020 2020 2065   + 1]..        e
+000006e0: 7863 6570 7420 5661 6c75 6545 7272 6f72  xcept ValueError
+000006f0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00000700: 6574 7572 6e20 4e6f 6e65 0d0a 0d0a 2020  eturn None....  
+00000710: 2020 6669 6c65 5f6e 616d 6520 3d20 5f67    file_name = _g
+00000720: 6574 5f66 696c 655f 6e61 6d65 2863 6d64  et_file_name(cmd
+00000730: 290d 0a20 2020 2069 6620 6669 6c65 5f6e  )..    if file_n
+00000740: 616d 6520 6973 204e 6f6e 653a 0d0a 2020  ame is None:..  
+00000750: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
+00000760: 650d 0a0d 0a20 2020 2074 7279 3a0d 0a20  e....    try:.. 
+00000770: 2020 2020 2020 2069 6620 7379 732e 706c         if sys.pl
+00000780: 6174 666f 726d 203d 3d20 2277 696e 3332  atform == "win32
+00000790: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
+000007a0: 6f75 7470 7574 203d 2073 7562 7072 6f63  output = subproc
+000007b0: 6573 732e 6368 6563 6b5f 6f75 7470 7574  ess.check_output
+000007c0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+000007d0: 2020 205b 0d0a 2020 2020 2020 2020 2020     [..          
+000007e0: 2020 2020 2020 2020 2020 2266 6670 726f            "ffpro
+000007f0: 6265 222c 0d0a 2020 2020 2020 2020 2020  be",..          
+00000800: 2020 2020 2020 2020 2020 222d 6c6f 676c            "-logl
+00000810: 6576 656c 222c 0d0a 2020 2020 2020 2020  evel",..        
+00000820: 2020 2020 2020 2020 2020 2020 222d 3122              "-1"
+00000830: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000840: 2020 2020 2020 2022 2d68 6964 655f 6261         "-hide_ba
+00000850: 6e6e 6572 222c 0d0a 2020 2020 2020 2020  nner",..        
+00000860: 2020 2020 2020 2020 2020 2020 222d 7368              "-sh
+00000870: 6f77 5f65 6e74 7269 6573 222c 0d0a 2020  ow_entries",..  
+00000880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000890: 2020 2266 6f72 6d61 743d 6475 7261 7469    "format=durati
+000008a0: 6f6e 222c 0d0a 2020 2020 2020 2020 2020  on",..          
+000008b0: 2020 2020 2020 2020 2020 222d 6f66 222c            "-of",
+000008c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000008d0: 2020 2020 2020 2264 6566 6175 6c74 3d6e        "default=n
+000008e0: 6f70 7269 6e74 5f77 7261 7070 6572 733d  oprint_wrappers=
+000008f0: 313a 6e6f 6b65 793d 3122 2c0d 0a20 2020  1:nokey=1",..   
+00000900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000910: 2066 696c 655f 6e61 6d65 2c0d 0a20 2020   file_name,..   
+00000920: 2020 2020 2020 2020 2020 2020 205d 2c0d               ],.
+00000930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000940: 2075 6e69 7665 7273 616c 5f6e 6577 6c69   universal_newli
+00000950: 6e65 733d 5472 7565 2c0d 0a20 2020 2020  nes=True,..     
+00000960: 2020 2020 2020 2020 2020 2063 7265 6174             creat
+00000970: 696f 6e66 6c61 6773 3d73 7562 7072 6f63  ionflags=subproc
+00000980: 6573 732e 4352 4541 5445 5f4e 4f5f 5749  ess.CREATE_NO_WI
+00000990: 4e44 4f57 2c0d 0a20 2020 2020 2020 2020  NDOW,..         
+000009a0: 2020 2029 0d0a 2020 2020 2020 2020 656c     )..        el
+000009b0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+000009c0: 206f 7574 7075 7420 3d20 7375 6270 726f   output = subpro
+000009d0: 6365 7373 2e63 6865 636b 5f6f 7574 7075  cess.check_outpu
+000009e0: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
+000009f0: 2020 2020 5b0d 0a20 2020 2020 2020 2020      [..         
+00000a00: 2020 2020 2020 2020 2020 2022 6666 7072             "ffpr
+00000a10: 6f62 6522 2c0d 0a20 2020 2020 2020 2020  obe",..         
+00000a20: 2020 2020 2020 2020 2020 2022 2d6c 6f67             "-log
+00000a30: 6c65 7665 6c22 2c0d 0a20 2020 2020 2020  level",..       
+00000a40: 2020 2020 2020 2020 2020 2020 2022 2d31               "-1
+00000a50: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00000a60: 2020 2020 2020 2020 222d 6869 6465 5f62          "-hide_b
+00000a70: 616e 6e65 7222 2c0d 0a20 2020 2020 2020  anner",..       
+00000a80: 2020 2020 2020 2020 2020 2020 2022 2d73               "-s
+00000a90: 686f 775f 656e 7472 6965 7322 2c0d 0a20  how_entries",.. 
+00000aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ab0: 2020 2022 666f 726d 6174 3d64 7572 6174     "format=durat
+00000ac0: 696f 6e22 2c0d 0a20 2020 2020 2020 2020  ion",..         
+00000ad0: 2020 2020 2020 2020 2020 2022 2d6f 6622             "-of"
+00000ae0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000af0: 2020 2020 2020 2022 6465 6661 756c 743d         "default=
+00000b00: 6e6f 7072 696e 745f 7772 6170 7065 7273  noprint_wrappers
+00000b10: 3d31 3a6e 6f6b 6579 3d31 222c 0d0a 2020  =1:nokey=1",..  
+00000b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b30: 2020 6669 6c65 5f6e 616d 652c 0d0a 2020    file_name,..  
+00000b40: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
+00000b50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000b60: 2020 756e 6976 6572 7361 6c5f 6e65 776c    universal_newl
+00000b70: 696e 6573 3d54 7275 652c 0d0a 2020 2020  ines=True,..    
+00000b80: 2020 2020 2020 2020 290d 0a0d 0a20 2020          )....   
+00000b90: 2020 2020 2072 6574 7572 6e20 696e 7428       return int(
+00000ba0: 666c 6f61 7428 6f75 7470 7574 2e73 7472  float(output.str
+00000bb0: 6970 2829 2920 2a20 3130 3030 290d 0a20  ip()) * 1000).. 
+00000bc0: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+00000bd0: 696f 6e3a 0d0a 2020 2020 2020 2020 2320  ion:..        # 
+00000be0: 544f 444f 3a20 6164 6420 6c6f 6767 696e  TODO: add loggin
+00000bf0: 670d 0a20 2020 2020 2020 2072 6574 7572  g..        retur
+00000c00: 6e20 4e6f 6e65 0d0a 0d0a 0d0a 6465 6620  n None......def 
+00000c10: 5f75 7365 735f 6572 726f 725f 6c6f 676c  _uses_error_logl
+00000c20: 6576 656c 2863 6d64 3a20 4c69 7374 5b73  evel(cmd: List[s
+00000c30: 7472 5d29 202d 3e20 626f 6f6c 3a0d 0a20  tr]) -> bool:.. 
+00000c40: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
+00000c50: 2069 6478 203d 2063 6d64 2e69 6e64 6578   idx = cmd.index
+00000c60: 2822 2d6c 6f67 6c65 7665 6c22 290d 0a20  ("-loglevel").. 
+00000c70: 2020 2020 2020 2069 6620 636d 645b 6964         if cmd[id
+00000c80: 7820 2b20 315d 203d 3d20 2265 7272 6f72  x + 1] == "error
+00000c90: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
+00000ca0: 7265 7475 726e 2054 7275 650d 0a20 2020  return True..   
+00000cb0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00000cc0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+00000cd0: 616c 7365 0d0a 2020 2020 6578 6365 7074  alse..    except
+00000ce0: 2056 616c 7565 4572 726f 723a 0d0a 2020   ValueError:..  
+00000cf0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+00000d00: 7365 0d0a 0d0a 0d0a 636c 6173 7320 4666  se......class Ff
+00000d10: 6d70 6567 5072 6f67 7265 7373 3a0d 0a20  mpegProgress:.. 
+00000d20: 2020 2044 5552 5f52 4547 4558 203d 2072     DUR_REGEX = r
+00000d30: 652e 636f 6d70 696c 6528 0d0a 2020 2020  e.compile(..    
+00000d40: 2020 2020 7222 4475 7261 7469 6f6e 3a20      r"Duration: 
+00000d50: 283f 503c 686f 7572 3e5c 647b 327d 293a  (?P<hour>\d{2}):
+00000d60: 283f 503c 6d69 6e3e 5c64 7b32 7d29 3a28  (?P<min>\d{2}):(
+00000d70: 3f50 3c73 6563 3e5c 647b 327d 295c 2e28  ?P<sec>\d{2})\.(
+00000d80: 3f50 3c6d 733e 5c64 7b32 7d29 220d 0a20  ?P<ms>\d{2})".. 
+00000d90: 2020 2029 0d0a 2020 2020 5449 4d45 5f52     )..    TIME_R
+00000da0: 4547 4558 203d 2072 652e 636f 6d70 696c  EGEX = re.compil
+00000db0: 6528 0d0a 2020 2020 2020 2020 7222 6f75  e(..        r"ou
+00000dc0: 745f 7469 6d65 3d28 3f50 3c68 6f75 723e  t_time=(?P<hour>
+00000dd0: 5c64 7b32 7d29 3a28 3f50 3c6d 696e 3e5c  \d{2}):(?P<min>\
+00000de0: 647b 327d 293a 283f 503c 7365 633e 5c64  d{2}):(?P<sec>\d
+00000df0: 7b32 7d29 5c2e 283f 503c 6d73 3e5c 647b  {2})\.(?P<ms>\d{
+00000e00: 327d 2922 0d0a 2020 2020 290d 0a0d 0a20  2})"..    ).... 
+00000e10: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00000e20: 7365 6c66 2c20 636d 643a 204c 6973 745b  self, cmd: List[
+00000e30: 7374 725d 2c20 6472 795f 7275 6e3a 2062  str], dry_run: b
+00000e40: 6f6f 6c20 3d20 4661 6c73 6529 202d 3e20  ool = False) -> 
+00000e50: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2027  None:..        '
+00000e60: 2727 496e 6974 6961 6c69 7a65 2074 6865  ''Initialize the
+00000e70: 2046 666d 7065 6750 726f 6772 6573 7320   FfmpegProgress 
+00000e80: 636c 6173 732e 0d0a 0d0a 2020 2020 2020  class.....      
+00000e90: 2020 4172 6773 3a0d 0a20 2020 2020 2020    Args:..       
+00000ea0: 2020 2020 2063 6d64 2028 4c69 7374 5b73       cmd (List[s
+00000eb0: 7472 5d29 3a20 4120 6c69 7374 206f 6620  tr]): A list of 
+00000ec0: 636f 6d6d 616e 6420 6c69 6e65 2065 6c65  command line ele
+00000ed0: 6d65 6e74 732c 2065 2e67 2e20 5b22 6666  ments, e.g. ["ff
+00000ee0: 6d70 6567 222c 2022 2d69 222c 202e 2e2e  mpeg", "-i", ...
+00000ef0: 5d0d 0a20 2020 2020 2020 2020 2020 2064  ]..            d
+00000f00: 7279 5f72 756e 2028 626f 6f6c 2c20 6f70  ry_run (bool, op
+00000f10: 7469 6f6e 616c 293a 204f 6e6c 7920 7368  tional): Only sh
+00000f20: 6f77 2077 6861 7420 776f 756c 6420 6265  ow what would be
+00000f30: 2064 6f6e 652e 2044 6566 6175 6c74 7320   done. Defaults 
+00000f40: 746f 2046 616c 7365 2e0d 0a20 2020 2020  to False...     
+00000f50: 2020 2027 2727 0d0a 2020 2020 2020 2020     '''..        
+00000f60: 7365 6c66 2e63 6d64 203d 2063 6d64 0d0a  self.cmd = cmd..
+00000f70: 2020 2020 2020 2020 7365 6c66 2e73 7464          self.std
+00000f80: 6572 723a 2055 6e69 6f6e 5b73 7472 2c20  err: Union[str, 
+00000f90: 4e6f 6e65 5d20 3d20 4e6f 6e65 0d0a 2020  None] = None..  
+00000fa0: 2020 2020 2020 7365 6c66 2e64 7279 5f72        self.dry_r
+00000fb0: 756e 203d 2064 7279 5f72 756e 0d0a 2020  un = dry_run..  
+00000fc0: 2020 2020 2020 7365 6c66 2e70 726f 6365        self.proce
+00000fd0: 7373 3a20 416e 7920 3d20 4e6f 6e65 0d0a  ss: Any = None..
+00000fe0: 2020 2020 2020 2020 7365 6c66 2e73 7464          self.std
+00000ff0: 6572 725f 6361 6c6c 6261 636b 3a20 556e  err_callback: Un
+00001000: 696f 6e5b 4361 6c6c 6162 6c65 5b5b 7374  ion[Callable[[st
+00001010: 725d 2c20 4e6f 6e65 5d2c 204e 6f6e 655d  r], None], None]
+00001020: 203d 204e 6f6e 650d 0a20 2020 2020 2020   = None..       
+00001030: 2069 6620 7379 732e 706c 6174 666f 726d   if sys.platform
+00001040: 203d 3d20 2277 696e 3332 223a 0d0a 2020   == "win32":..  
+00001050: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+00001060: 6173 655f 706f 7065 6e5f 6b77 6172 6773  ase_popen_kwargs
+00001070: 203d 207b 0d0a 2020 2020 2020 2020 2020   = {..          
+00001080: 2020 2020 2020 2273 7464 696e 223a 2073        "stdin": s
+00001090: 7562 7072 6f63 6573 732e 5049 5045 2c20  ubprocess.PIPE, 
+000010a0: 2023 2041 7070 6c79 2073 7464 696e 2069   # Apply stdin i
+000010b0: 736f 6c61 7469 6f6e 2062 7920 6372 6561  solation by crea
+000010c0: 7469 6e67 2073 6570 6172 6174 6520 7069  ting separate pi
+000010d0: 7065 2e0d 0a20 2020 2020 2020 2020 2020  pe...           
+000010e0: 2020 2020 2022 7374 646f 7574 223a 2073       "stdout": s
+000010f0: 7562 7072 6f63 6573 732e 5049 5045 2c0d  ubprocess.PIPE,.
+00001100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001110: 2022 7374 6465 7272 223a 2073 7562 7072   "stderr": subpr
+00001120: 6f63 6573 732e 5354 444f 5554 2c0d 0a20  ocess.STDOUT,.. 
+00001130: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001140: 756e 6976 6572 7361 6c5f 6e65 776c 696e  universal_newlin
+00001150: 6573 223a 2046 616c 7365 2c0d 0a20 2020  es": False,..   
+00001160: 2020 2020 2020 2020 2020 2020 2022 7368               "sh
+00001170: 656c 6c22 3a20 5472 7565 2c0d 0a20 2020  ell": True,..   
+00001180: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
+00001190: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+000011a0: 2020 2020 2020 2073 656c 662e 6261 7365         self.base
+000011b0: 5f70 6f70 656e 5f6b 7761 7267 7320 3d20  _popen_kwargs = 
+000011c0: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
+000011d0: 2020 2022 7374 6469 6e22 3a20 7375 6270     "stdin": subp
+000011e0: 726f 6365 7373 2e50 4950 452c 2020 2320  rocess.PIPE,  # 
+000011f0: 4170 706c 7920 7374 6469 6e20 6973 6f6c  Apply stdin isol
+00001200: 6174 696f 6e20 6279 2063 7265 6174 696e  ation by creatin
+00001210: 6720 7365 7061 7261 7465 2070 6970 652e  g separate pipe.
+00001220: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001230: 2020 2273 7464 6f75 7422 3a20 7375 6270    "stdout": subp
+00001240: 726f 6365 7373 2e50 4950 452c 0d0a 2020  rocess.PIPE,..  
+00001250: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+00001260: 7464 6572 7222 3a20 7375 6270 726f 6365  tderr": subproce
+00001270: 7373 2e53 5444 4f55 542c 0d0a 2020 2020  ss.STDOUT,..    
+00001280: 2020 2020 2020 2020 2020 2020 2275 6e69              "uni
+00001290: 7665 7273 616c 5f6e 6577 6c69 6e65 7322  versal_newlines"
+000012a0: 3a20 4661 6c73 652c 0d0a 2020 2020 2020  : False,..      
+000012b0: 2020 2020 2020 7d0d 0a0d 0a20 2020 2064        }....    d
+000012c0: 6566 2073 6574 5f73 7464 6572 725f 6361  ef set_stderr_ca
+000012d0: 6c6c 6261 636b 2873 656c 662c 2063 616c  llback(self, cal
+000012e0: 6c62 6163 6b3a 2043 616c 6c61 626c 655b  lback: Callable[
+000012f0: 5b73 7472 5d2c 204e 6f6e 655d 2920 2d3e  [str], None]) ->
+00001300: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00001310: 2727 270d 0a20 2020 2020 2020 2053 6574  '''..        Set
+00001320: 2061 2063 616c 6c62 6163 6b20 6675 6e63   a callback func
+00001330: 7469 6f6e 2074 6f20 6265 2063 616c 6c65  tion to be calle
+00001340: 6420 6f6e 2073 7464 6572 7220 6f75 7470  d on stderr outp
+00001350: 7574 2e0d 0a20 2020 2020 2020 2054 6865  ut...        The
+00001360: 2063 616c 6c62 6163 6b20 6675 6e63 7469   callback functi
+00001370: 6f6e 206d 7573 7420 6163 6365 7074 2061  on must accept a
+00001380: 2073 696e 676c 6520 7374 7269 6e67 2061   single string a
+00001390: 7267 756d 656e 742e 0d0a 2020 2020 2020  rgument...      
+000013a0: 2020 4e6f 7465 2074 6861 7420 7468 6973    Note that this
+000013b0: 2069 7320 6361 6c6c 6564 206f 6e20 6576   is called on ev
+000013c0: 6572 7920 6c69 6e65 206f 6620 7374 6465  ery line of stde
+000013d0: 7272 206f 7574 7075 742c 2073 6f20 6974  rr output, so it
+000013e0: 2063 616e 2062 6520 6361 6c6c 6564 2061   can be called a
+000013f0: 206c 6f74 2e0d 0a20 2020 2020 2020 2041   lot...        A
+00001400: 6c73 6f20 6e6f 7465 2074 6861 7420 7374  lso note that st
+00001410: 646f 7574 2f73 7464 6572 7220 6172 6520  dout/stderr are 
+00001420: 6a6f 696e 6564 2069 6e74 6f20 6f6e 6520  joined into one 
+00001430: 7374 7265 616d 2c20 736f 2079 6f75 206d  stream, so you m
+00001440: 6967 6874 2067 6574 2073 7464 6f75 7420  ight get stdout 
+00001450: 6f75 7470 7574 2069 6e20 7468 6520 6361  output in the ca
+00001460: 6c6c 6261 636b 2e0d 0a0d 0a20 2020 2020  llback.....     
+00001470: 2020 2041 7267 733a 0d0a 2020 2020 2020     Args:..      
+00001480: 2020 2020 2020 6361 6c6c 6261 636b 2028        callback (
+00001490: 4361 6c6c 6162 6c65 5b5b 7374 725d 2c20  Callable[[str], 
+000014a0: 4e6f 6e65 5d29 3a20 4120 6361 6c6c 6261  None]): A callba
+000014b0: 636b 2066 756e 6374 696f 6e20 7468 6174  ck function that
+000014c0: 2061 6363 6570 7473 2061 2073 696e 676c   accepts a singl
+000014d0: 6520 7374 7269 6e67 2061 7267 756d 656e  e string argumen
+000014e0: 742e 0d0a 2020 2020 2020 2020 2727 270d  t...        '''.
+000014f0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00001500: 6361 6c6c 6162 6c65 2863 616c 6c62 6163  callable(callbac
+00001510: 6b29 206f 7220 6c65 6e28 6361 6c6c 6261  k) or len(callba
+00001520: 636b 2e5f 5f63 6f64 655f 5f2e 636f 5f76  ck.__code__.co_v
+00001530: 6172 6e61 6d65 7329 2021 3d20 313a 0d0a  arnames) != 1:..
+00001540: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00001550: 6520 5661 6c75 6545 7272 6f72 280d 0a20  e ValueError(.. 
+00001560: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001570: 4361 6c6c 6261 636b 206d 7573 7420 6265  Callback must be
+00001580: 2061 2066 756e 6374 696f 6e20 7468 6174   a function that
+00001590: 2061 6363 6570 7473 206f 6e6c 7920 6f6e   accepts only on
+000015a0: 6520 6172 6775 6d65 6e74 220d 0a20 2020  e argument"..   
+000015b0: 2020 2020 2020 2020 2029 0d0a 0d0a 2020           )....  
+000015c0: 2020 2020 2020 7365 6c66 2e73 7464 6572        self.stder
+000015d0: 725f 6361 6c6c 6261 636b 203d 2063 616c  r_callback = cal
+000015e0: 6c62 6163 6b0d 0a0d 0a20 2020 2064 6566  lback....    def
+000015f0: 2072 756e 5f63 6f6d 6d61 6e64 5f77 6974   run_command_wit
+00001600: 685f 7072 6f67 7265 7373 280d 0a20 2020  h_progress(..   
+00001610: 2020 2020 2073 656c 662c 2070 6f70 656e       self, popen
+00001620: 5f6b 7761 7267 733d 4e6f 6e65 2c20 6475  _kwargs=None, du
+00001630: 7261 7469 6f6e 5f6f 7665 7272 6964 653a  ration_override:
+00001640: 2055 6e69 6f6e 5b66 6c6f 6174 2c20 4e6f   Union[float, No
+00001650: 6e65 5d20 3d20 4e6f 6e65 0d0a 2020 2020  ne] = None..    
+00001660: 2920 2d3e 2049 7465 7261 746f 725b 696e  ) -> Iterator[in
+00001670: 745d 3a0d 0a20 2020 2020 2020 2027 2727  t]:..        '''
+00001680: 0d0a 2020 2020 2020 2020 5275 6e20 616e  ..        Run an
+00001690: 2066 666d 7065 6720 636f 6d6d 616e 642c   ffmpeg command,
+000016a0: 2074 7279 696e 6720 746f 2063 6170 7475   trying to captu
+000016b0: 7265 2074 6865 2070 726f 6365 7373 206f  re the process o
+000016c0: 7574 7075 7420 616e 6420 6361 6c63 756c  utput and calcul
+000016d0: 6174 650d 0a20 2020 2020 2020 2074 6865  ate..        the
+000016e0: 2064 7572 6174 696f 6e20 2f20 7072 6f67   duration / prog
+000016f0: 7265 7373 2e0d 0a20 2020 2020 2020 2059  ress...        Y
+00001700: 6965 6c64 7320 7468 6520 7072 6f67 7265  ields the progre
+00001710: 7373 2069 6e20 7065 7263 656e 742e 0d0a  ss in percent...
+00001720: 0d0a 2020 2020 2020 2020 4172 6773 3a0d  ..        Args:.
+00001730: 0a20 2020 2020 2020 2020 2020 2070 6f70  .            pop
+00001740: 656e 5f6b 7761 7267 7320 2864 6963 742c  en_kwargs (dict,
+00001750: 206f 7074 696f 6e61 6c29 3a20 4120 6469   optional): A di
+00001760: 6374 2074 6f20 7370 6563 6966 7920 6578  ct to specify ex
+00001770: 7472 6120 6172 6775 6d65 6e74 7320 746f  tra arguments to
+00001780: 2074 6865 2070 6f70 656e 2063 616c 6c2c   the popen call,
+00001790: 2065 2e67 2e20 7b20 6372 6561 7469 6f6e   e.g. { creation
+000017a0: 666c 6167 733a 2043 5245 4154 455f 4e4f  flags: CREATE_NO
+000017b0: 5f57 494e 444f 5720 7d0d 0a20 2020 2020  _WINDOW }..     
+000017c0: 2020 2020 2020 2064 7572 6174 696f 6e5f         duration_
+000017d0: 6f76 6572 7269 6465 2028 666c 6f61 742c  override (float,
+000017e0: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
+000017f0: 6475 7261 7469 6f6e 2069 6e20 7365 636f  duration in seco
+00001800: 6e64 732e 2049 6620 6e6f 7420 7370 6563  nds. If not spec
+00001810: 6966 6965 642c 2069 7420 7769 6c6c 2062  ified, it will b
+00001820: 6520 6361 6c63 756c 6174 6564 2066 726f  e calculated fro
+00001830: 6d20 7468 6520 6666 6d70 6567 206f 7574  m the ffmpeg out
+00001840: 7075 742e 0d0a 0d0a 2020 2020 2020 2020  put.....        
+00001850: 5261 6973 6573 3a0d 0a20 2020 2020 2020  Raises:..       
+00001860: 2020 2020 2052 756e 7469 6d65 4572 726f       RuntimeErro
+00001870: 723a 2049 6620 7468 6520 636f 6d6d 616e  r: If the comman
+00001880: 6420 6661 696c 732c 2061 6e20 6578 6365  d fails, an exce
+00001890: 7074 696f 6e20 6973 2072 6169 7365 642e  ption is raised.
+000018a0: 0d0a 0d0a 2020 2020 2020 2020 5969 656c  ....        Yiel
+000018b0: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
+000018c0: 2049 7465 7261 746f 725b 696e 745d 3a20   Iterator[int]: 
+000018d0: 4120 6765 6e65 7261 746f 7220 7468 6174  A generator that
+000018e0: 2079 6965 6c64 7320 7468 6520 7072 6f67   yields the prog
+000018f0: 7265 7373 2069 6e20 7065 7263 656e 742e  ress in percent.
+00001900: 0d0a 2020 2020 2020 2020 2727 270d 0a20  ..        '''.. 
+00001910: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
+00001920: 7279 5f72 756e 3a0d 0a20 2020 2020 2020  ry_run:..       
+00001930: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00001940: 2e63 6d64 0d0a 0d0a 2020 2020 2020 2020  .cmd....        
+00001950: 746f 7461 6c5f 6475 723a 2055 6e69 6f6e  total_dur: Union
+00001960: 5b4e 6f6e 652c 2069 6e74 5d20 3d20 4e6f  [None, int] = No
+00001970: 6e65 0d0a 2020 2020 2020 2020 6966 205f  ne..        if _
+00001980: 7573 6573 5f65 7272 6f72 5f6c 6f67 6c65  uses_error_logle
+00001990: 7665 6c28 7365 6c66 2e63 6d64 293a 0d0a  vel(self.cmd):..
+000019a0: 2020 2020 2020 2020 2020 2020 746f 7461              tota
+000019b0: 6c5f 6475 7220 3d20 5f70 726f 6265 5f64  l_dur = _probe_d
+000019c0: 7572 6174 696f 6e28 7365 6c66 2e63 6d64  uration(self.cmd
+000019d0: 290d 0a0d 0a20 2020 2020 2020 2063 6d64  )....        cmd
+000019e0: 5f77 6974 685f 7072 6f67 7265 7373 203d  _with_progress =
+000019f0: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+00001a00: 5b73 656c 662e 636d 645b 305d 5d20 2b20  [self.cmd[0]] + 
+00001a10: 5b22 2d70 726f 6772 6573 7322 2c20 222d  ["-progress", "-
+00001a20: 222c 2022 2d6e 6f73 7461 7473 225d 202b  ", "-nostats"] +
+00001a30: 2073 656c 662e 636d 645b 313a 5d0d 0a20   self.cmd[1:].. 
+00001a40: 2020 2020 2020 2029 0d0a 0d0a 2020 2020         )....    
+00001a50: 2020 2020 7374 6465 7272 203d 205b 5d0d      stderr = [].
+00001a60: 0a20 2020 2020 2020 2062 6173 655f 706f  .        base_po
+00001a70: 7065 6e5f 6b77 6172 6773 203d 2073 656c  pen_kwargs = sel
+00001a80: 662e 6261 7365 5f70 6f70 656e 5f6b 7761  f.base_popen_kwa
+00001a90: 7267 732e 636f 7079 2829 0d0a 2020 2020  rgs.copy()..    
+00001aa0: 2020 2020 6966 2070 6f70 656e 5f6b 7761      if popen_kwa
+00001ab0: 7267 7320 6973 206e 6f74 204e 6f6e 653a  rgs is not None:
+00001ac0: 0d0a 2020 2020 2020 2020 2020 2020 6261  ..            ba
+00001ad0: 7365 5f70 6f70 656e 5f6b 7761 7267 732e  se_popen_kwargs.
+00001ae0: 7570 6461 7465 2870 6f70 656e 5f6b 7761  update(popen_kwa
+00001af0: 7267 7329 0d0a 0d0a 2020 2020 2020 2020  rgs)....        
+00001b00: 6966 2073 7973 2e70 6c61 7466 6f72 6d20  if sys.platform 
+00001b10: 3d3d 2022 7769 6e64 3332 223a 0d0a 2020  == "wind32":..  
+00001b20: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+00001b30: 726f 6365 7373 203d 2073 7562 7072 6f63  rocess = subproc
+00001b40: 6573 732e 506f 7065 6e28 0d0a 2020 2020  ess.Popen(..    
+00001b50: 2020 2020 2020 2020 2020 2020 636d 645f              cmd_
+00001b60: 7769 7468 5f70 726f 6772 6573 732c 0d0a  with_progress,..
+00001b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b80: 2a2a 6261 7365 5f70 6f70 656e 5f6b 7761  **base_popen_kwa
+00001b90: 7267 732c 0d0a 2020 2020 2020 2020 2020  rgs,..          
+00001ba0: 2020 2020 2020 6372 6561 7469 6f6e 666c        creationfl
+00001bb0: 6167 733d 7375 6270 726f 6365 7373 2e43  ags=subprocess.C
+00001bc0: 5245 4154 455f 4e4f 5f57 494e 444f 572c  REATE_NO_WINDOW,
+00001bd0: 0d0a 2020 2020 2020 2020 2020 2020 2920  ..            ) 
+00001be0: 2023 2074 7970 653a 2069 676e 6f72 650d   # type: ignore.
+00001bf0: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
+00001c00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00001c10: 2e70 726f 6365 7373 203d 2073 7562 7072  .process = subpr
+00001c20: 6f63 6573 732e 506f 7065 6e28 0d0a 2020  ocess.Popen(..  
+00001c30: 2020 2020 2020 2020 2020 2020 2020 636d                cm
+00001c40: 645f 7769 7468 5f70 726f 6772 6573 732c  d_with_progress,
+00001c50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001c60: 2020 2a2a 6261 7365 5f70 6f70 656e 5f6b    **base_popen_k
+00001c70: 7761 7267 732c 0d0a 2020 2020 2020 2020  wargs,..        
+00001c80: 2020 2020 2920 2023 2074 7970 653a 2069      )  # type: i
+00001c90: 676e 6f72 650d 0a0d 0a20 2020 2020 2020  gnore....       
+00001ca0: 2079 6965 6c64 2030 0d0a 0d0a 2020 2020   yield 0....    
+00001cb0: 2020 2020 7768 696c 6520 5472 7565 3a0d      while True:.
+00001cc0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00001cd0: 7365 6c66 2e70 726f 6365 7373 2e73 7464  self.process.std
+00001ce0: 6f75 7420 6973 204e 6f6e 653a 0d0a 2020  out is None:..  
+00001cf0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00001d00: 6e74 696e 7565 0d0a 0d0a 2020 2020 2020  ntinue....      
+00001d10: 2020 2020 2020 7374 6465 7272 5f6c 696e        stderr_lin
+00001d20: 6520 3d20 280d 0a20 2020 2020 2020 2020  e = (..         
+00001d30: 2020 2020 2020 2073 656c 662e 7072 6f63         self.proc
+00001d40: 6573 732e 7374 646f 7574 2e72 6561 646c  ess.stdout.readl
+00001d50: 696e 6528 292e 6465 636f 6465 2822 7574  ine().decode("ut
+00001d60: 662d 3822 2c20 6572 726f 7273 3d22 7265  f-8", errors="re
+00001d70: 706c 6163 6522 292e 7374 7269 7028 290d  place").strip().
+00001d80: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
+00001d90: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00001da0: 2073 656c 662e 7374 6465 7272 5f63 616c   self.stderr_cal
+00001db0: 6c62 6163 6b3a 0d0a 2020 2020 2020 2020  lback:..        
+00001dc0: 2020 2020 2020 2020 7365 6c66 2e73 7464          self.std
+00001dd0: 6572 725f 6361 6c6c 6261 636b 2873 7464  err_callback(std
+00001de0: 6572 725f 6c69 6e65 290d 0a0d 0a20 2020  err_line)....   
+00001df0: 2020 2020 2020 2020 2069 6620 7374 6465           if stde
+00001e00: 7272 5f6c 696e 6520 3d3d 2027 2720 616e  rr_line == '' an
+00001e10: 6420 7365 6c66 2e70 726f 6365 7373 2e70  d self.process.p
+00001e20: 6f6c 6c28 2920 6973 206e 6f74 204e 6f6e  oll() is not Non
+00001e30: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00001e40: 2020 2020 6272 6561 6b0d 0a0d 0a20 2020      break....   
+00001e50: 2020 2020 2020 2020 2073 7464 6572 722e           stderr.
+00001e60: 6170 7065 6e64 2873 7464 6572 725f 6c69  append(stderr_li
+00001e70: 6e65 2e73 7472 6970 2829 290d 0a0d 0a20  ne.strip()).... 
+00001e80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00001e90: 7374 6465 7272 203d 2022 5c6e 222e 6a6f  stderr = "\n".jo
+00001ea0: 696e 2873 7464 6572 7229 0d0a 0d0a 2020  in(stderr)....  
+00001eb0: 2020 2020 2020 2020 2020 6966 2074 6f74            if tot
+00001ec0: 616c 5f64 7572 2069 7320 4e6f 6e65 3a0d  al_dur is None:.
+00001ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001ee0: 2074 6f74 616c 5f64 7572 5f6d 6174 6368   total_dur_match
+00001ef0: 203d 2073 656c 662e 4455 525f 5245 4745   = self.DUR_REGE
+00001f00: 582e 7365 6172 6368 2873 7464 6572 725f  X.search(stderr_
+00001f10: 6c69 6e65 290d 0a20 2020 2020 2020 2020  line)..         
+00001f20: 2020 2020 2020 2069 6620 746f 7461 6c5f         if total_
+00001f30: 6475 725f 6d61 7463 683a 0d0a 2020 2020  dur_match:..    
+00001f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f50: 746f 7461 6c5f 6475 7220 3d20 746f 5f6d  total_dur = to_m
+00001f60: 7328 2a2a 746f 7461 6c5f 6475 725f 6d61  s(**total_dur_ma
+00001f70: 7463 682e 6772 6f75 7064 6963 7428 2929  tch.groupdict())
+00001f80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001f90: 2020 2020 2020 636f 6e74 696e 7565 0d0a        continue..
+00001fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fb0: 656c 6966 2064 7572 6174 696f 6e5f 6f76  elif duration_ov
+00001fc0: 6572 7269 6465 2069 7320 6e6f 7420 4e6f  erride is not No
+00001fd0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00001fe0: 2020 2020 2020 2020 2023 2075 7365 2074           # use t
+00001ff0: 6865 206f 7665 7272 6964 6520 2873 686f  he override (sho
+00002000: 756c 6420 6170 706c 7920 696e 2074 6865  uld apply in the
+00002010: 2066 6972 7374 206c 6f6f 7029 0d0a 2020   first loop)..  
+00002020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002030: 2020 746f 7461 6c5f 6475 7220 3d20 696e    total_dur = in
+00002040: 7428 6475 7261 7469 6f6e 5f6f 7665 7272  t(duration_overr
+00002050: 6964 6520 2a20 3130 3030 290d 0a20 2020  ide * 1000)..   
+00002060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002070: 2063 6f6e 7469 6e75 650d 0a0d 0a20 2020   continue....   
+00002080: 2020 2020 2020 2020 2069 6620 746f 7461           if tota
+00002090: 6c5f 6475 723a 0d0a 2020 2020 2020 2020  l_dur:..        
+000020a0: 2020 2020 2020 2020 7072 6f67 7265 7373          progress
+000020b0: 5f74 696d 6520 3d20 4666 6d70 6567 5072  _time = FfmpegPr
+000020c0: 6f67 7265 7373 2e54 494d 455f 5245 4745  ogress.TIME_REGE
+000020d0: 582e 7365 6172 6368 2873 7464 6572 725f  X.search(stderr_
+000020e0: 6c69 6e65 290d 0a20 2020 2020 2020 2020  line)..         
+000020f0: 2020 2020 2020 2069 6620 7072 6f67 7265         if progre
+00002100: 7373 5f74 696d 653a 0d0a 2020 2020 2020  ss_time:..      
+00002110: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00002120: 6170 7365 645f 7469 6d65 203d 2074 6f5f  apsed_time = to_
+00002130: 6d73 282a 2a70 726f 6772 6573 735f 7469  ms(**progress_ti
+00002140: 6d65 2e67 726f 7570 6469 6374 2829 290d  me.groupdict()).
+00002150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002160: 2020 2020 2079 6965 6c64 2069 6e74 2865       yield int(e
+00002170: 6c61 7073 6564 5f74 696d 6520 2a20 3130  lapsed_time * 10
+00002180: 302f 2074 6f74 616c 5f64 7572 290d 0a0d  0/ total_dur)...
+00002190: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000021a0: 2e70 726f 6365 7373 2069 7320 4e6f 6e65  .process is None
+000021b0: 206f 7220 7365 6c66 2e70 726f 6365 7373   or self.process
+000021c0: 2e72 6574 7572 6e63 6f64 6520 213d 2030  .returncode != 0
+000021d0: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
+000021e0: 7072 696e 7428 7365 6c66 2e70 726f 6365  print(self.proce
+000021f0: 7373 290d 0a20 2020 2020 2020 2020 2020  ss)..           
+00002200: 2023 7072 696e 7428 7365 6c66 2e70 726f   #print(self.pro
+00002210: 6365 7373 2e72 6574 7572 6e63 6f64 6529  cess.returncode)
+00002220: 0d0a 2020 2020 2020 2020 2020 2020 5f70  ..            _p
+00002230: 7265 7474 795f 7374 6465 7272 203d 2022  retty_stderr = "
+00002240: 5c6e 222e 6a6f 696e 2873 7464 6572 7229  \n".join(stderr)
+00002250: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
+00002260: 6973 6520 5275 6e74 696d 6545 7272 6f72  ise RuntimeError
+00002270: 2866 2245 7272 6f72 2072 756e 6e69 6e67  (f"Error running
+00002280: 2063 6f6d 6d61 6e64 207b 7365 6c66 2e63   command {self.c
+00002290: 6d64 7d3a 207b 5f70 7265 7474 795f 7374  md}: {_pretty_st
+000022a0: 6465 7272 7d22 290d 0a0d 0a20 2020 2020  derr}")....     
+000022b0: 2020 2079 6965 6c64 2031 3030 0d0a 2020     yield 100..  
+000022c0: 2020 2020 2020 7365 6c66 2e70 726f 6365        self.proce
+000022d0: 7373 203d 204e 6f6e 650d 0a0d 0a20 2020  ss = None....   
+000022e0: 2064 6566 2071 7569 745f 6772 6163 6566   def quit_gracef
+000022f0: 756c 6c79 2873 656c 6629 202d 3e20 4e6f  ully(self) -> No
+00002300: 6e65 3a0d 0a20 2020 2020 2020 2027 2727  ne:..        '''
+00002310: 0d0a 2020 2020 2020 2020 5175 6974 2074  ..        Quit t
+00002320: 6865 2066 666d 7065 6720 7072 6f63 6573  he ffmpeg proces
+00002330: 7320 6279 2073 656e 6469 6e67 2027 7127  s by sending 'q'
+00002340: 0d0a 0d0a 2020 2020 2020 2020 5261 6973  ....        Rais
+00002350: 6573 3a0d 0a20 2020 2020 2020 2020 2020  es:..           
+00002360: 2052 756e 7469 6d65 4572 726f 723a 2049   RuntimeError: I
+00002370: 6620 6e6f 2070 726f 6365 7373 2069 7320  f no process is 
+00002380: 666f 756e 642e 0d0a 2020 2020 2020 2020  found...        
+00002390: 2727 270d 0a20 2020 2020 2020 2069 6620  '''..        if 
+000023a0: 7365 6c66 2e70 726f 6365 7373 2069 7320  self.process is 
+000023b0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+000023c0: 2020 2072 6169 7365 2052 756e 7469 6d65     raise Runtime
+000023d0: 4572 726f 7228 224e 6f20 7072 6f63 6573  Error("No proces
+000023e0: 7320 666f 756e 642e 2044 6964 2079 6f75  s found. Did you
+000023f0: 2072 756e 2074 6865 2063 6f6d 6d61 6e64   run the command
+00002400: 3f22 290d 0a0d 0a20 2020 2020 2020 2073  ?")....        s
+00002410: 656c 662e 7072 6f63 6573 732e 636f 6d6d  elf.process.comm
+00002420: 756e 6963 6174 6528 696e 7075 743d 6222  unicate(input=b"
+00002430: 7122 290d 0a20 2020 2020 2020 2073 656c  q")..        sel
+00002440: 662e 7072 6f63 6573 732e 6b69 6c6c 2829  f.process.kill()
+00002450: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
+00002460: 726f 6365 7373 203d 204e 6f6e 650d 0a0d  rocess = None...
+00002470: 0a20 2020 2064 6566 2071 7569 7428 7365  .    def quit(se
+00002480: 6c66 2920 2d3e 204e 6f6e 653a 0d0a 2020  lf) -> None:..  
+00002490: 2020 2020 2020 2727 270d 0a20 2020 2020        '''..     
+000024a0: 2020 2051 7569 7420 7468 6520 6666 6d70     Quit the ffmp
+000024b0: 6567 2070 726f 6365 7373 2062 7920 7365  eg process by se
+000024c0: 6e64 696e 6720 5349 474b 494c 4c2e 0d0a  nding SIGKILL...
+000024d0: 0d0a 2020 2020 2020 2020 5261 6973 6573  ..        Raises
+000024e0: 3a0d 0a20 2020 2020 2020 2020 2020 2052  :..            R
+000024f0: 756e 7469 6d65 4572 726f 723a 2049 6620  untimeError: If 
+00002500: 6e6f 2070 726f 6365 7373 2069 7320 666f  no process is fo
+00002510: 756e 642e 0d0a 2020 2020 2020 2020 2727  und...        ''
+00002520: 270d 0a20 2020 2020 2020 2069 6620 7365  '..        if se
+00002530: 6c66 2e70 726f 6365 7373 2069 7320 4e6f  lf.process is No
+00002540: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00002550: 2072 6169 7365 2052 756e 7469 6d65 4572   raise RuntimeEr
+00002560: 726f 7228 224e 6f20 7072 6f63 6573 7320  ror("No process 
+00002570: 666f 756e 642e 2044 6964 2079 6f75 2072  found. Did you r
+00002580: 756e 2074 6865 2063 6f6d 6d61 6e64 3f22  un the command?"
+00002590: 290d 0a0d 0a20 2020 2020 2020 2073 656c  )....        sel
+000025a0: 662e 7072 6f63 6573 732e 6b69 6c6c 2829  f.process.kill()
+000025b0: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
+000025c0: 726f 6365 7373 203d 204e 6f6e 650d 0a0d  rocess = None...
+000025d0: 0a0d 0a23 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ...#============
+000025e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 000025f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00002600: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00002610: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00002620: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00002630: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00002640: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00002650: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00002660: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00002670: 3d3d 3d23 0d0a 0d0a 0d0a 6465 6620 7374  ===#......def st
-00002680: 6f70 5f66 666d 7065 675f 7769 6e64 6f77  op_ffmpeg_window
-00002690: 7328 6572 726f 725f 6d65 7373 6167 6573  s(error_messages
-000026a0: 5f63 616c 6c62 6163 6b3d 4e6f 6e65 293a  _callback=None):
-000026b0: 0d0a 2020 2020 7472 793a 0d0a 2020 2020  ..    try:..    
-000026c0: 2020 2020 7461 736b 6c69 7374 5f6f 7574      tasklist_out
-000026d0: 7075 7420 3d20 7375 6270 726f 6365 7373  put = subprocess
-000026e0: 2e63 6865 636b 5f6f 7574 7075 7428 5b27  .check_output(['
-000026f0: 7461 736b 6c69 7374 275d 2c20 6372 6561  tasklist'], crea
-00002700: 7469 6f6e 666c 6167 733d 7375 6270 726f  tionflags=subpro
-00002710: 6365 7373 2e43 5245 4154 455f 4e4f 5f57  cess.CREATE_NO_W
-00002720: 494e 444f 5729 2e64 6563 6f64 6528 2775  INDOW).decode('u
-00002730: 7466 2d38 2729 0d0a 2020 2020 2020 2020  tf-8')..        
-00002740: 6666 6d70 6567 5f70 6964 203d 204e 6f6e  ffmpeg_pid = Non
-00002750: 650d 0a20 2020 2020 2020 2066 6f72 206c  e..        for l
-00002760: 696e 6520 696e 2074 6173 6b6c 6973 745f  ine in tasklist_
-00002770: 6f75 7470 7574 2e73 706c 6974 2827 5c6e  output.split('\n
-00002780: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
-00002790: 2069 6620 2266 666d 7065 6722 2069 6e20   if "ffmpeg" in 
-000027a0: 6c69 6e65 3a0d 0a20 2020 2020 2020 2020  line:..         
-000027b0: 2020 2020 2020 2066 666d 7065 675f 7069         ffmpeg_pi
-000027c0: 6420 3d20 6c69 6e65 2e73 706c 6974 2829  d = line.split()
-000027d0: 5b31 5d0d 0a20 2020 2020 2020 2020 2020  [1]..           
-000027e0: 2020 2020 2062 7265 616b 0d0a 2020 2020       break..    
-000027f0: 2020 2020 6966 2066 666d 7065 675f 7069      if ffmpeg_pi
-00002800: 643a 0d0a 2020 2020 2020 2020 2020 2020  d:..            
-00002810: 6465 766e 756c 6c20 3d20 6f70 656e 286f  devnull = open(o
-00002820: 732e 6465 766e 756c 6c2c 2027 7727 290d  s.devnull, 'w').
-00002830: 0a20 2020 2020 2020 2020 2020 2073 7562  .            sub
-00002840: 7072 6f63 6573 732e 506f 7065 6e28 5b27  process.Popen(['
-00002850: 7461 736b 6b69 6c6c 272c 2027 2f46 272c  taskkill', '/F',
-00002860: 2027 2f54 272c 2027 2f50 4944 272c 2066   '/T', '/PID', f
-00002870: 666d 7065 675f 7069 645d 2c20 7374 646f  fmpeg_pid], stdo
-00002880: 7574 3d73 7562 7072 6f63 6573 732e 5049  ut=subprocess.PI
-00002890: 5045 2c20 7374 6465 7272 3d73 7562 7072  PE, stderr=subpr
-000028a0: 6f63 6573 732e 5354 444f 5554 2c20 7368  ocess.STDOUT, sh
-000028b0: 656c 6c3d 5472 7565 2c20 6372 6561 7469  ell=True, creati
-000028c0: 6f6e 666c 6167 733d 7375 6270 726f 6365  onflags=subproce
-000028d0: 7373 2e43 5245 4154 455f 4e4f 5f57 494e  ss.CREATE_NO_WIN
-000028e0: 444f 5729 0d0a 0d0a 2020 2020 6578 6365  DOW)....    exce
-000028f0: 7074 204b 6579 626f 6172 6449 6e74 6572  pt KeyboardInter
-00002900: 7275 7074 3a0d 0a20 2020 2020 2020 2069  rupt:..        i
-00002910: 6620 6572 726f 725f 6d65 7373 6167 6573  f error_messages
-00002920: 5f63 616c 6c62 6163 6b3a 0d0a 2020 2020  _callback:..    
-00002930: 2020 2020 2020 2020 6572 726f 725f 6d65          error_me
-00002940: 7373 6167 6573 5f63 616c 6c62 6163 6b28  ssages_callback(
-00002950: 2243 616e 6365 6c6c 696e 6720 616c 6c20  "Cancelling all 
-00002960: 7461 736b 7322 290d 0a20 2020 2020 2020  tasks")..       
-00002970: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00002980: 2020 2020 7072 696e 7428 2243 616e 6365      print("Cance
-00002990: 6c6c 696e 6720 616c 6c20 7461 736b 7322  lling all tasks"
-000029a0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-000029b0: 6e0d 0a0d 0a20 2020 2065 7863 6570 7420  n....    except 
-000029c0: 4578 6365 7074 696f 6e20 6173 2065 3a0d  Exception as e:.
-000029d0: 0a20 2020 2020 2020 2069 6620 6572 726f  .        if erro
-000029e0: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
-000029f0: 6163 6b3a 0d0a 2020 2020 2020 2020 2020  ack:..          
-00002a00: 2020 6572 726f 725f 6d65 7373 6167 6573    error_messages
-00002a10: 5f63 616c 6c62 6163 6b28 6529 0d0a 2020  _callback(e)..  
-00002a20: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00002a30: 2020 2020 2020 2020 2070 7269 6e74 2865           print(e
-00002a40: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00002a50: 6e0d 0a0d 0a0d 0a64 6566 2073 746f 705f  n......def stop_
-00002a60: 6666 6d70 6567 5f6c 696e 7578 2865 7272  ffmpeg_linux(err
-00002a70: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
-00002a80: 6261 636b 3d4e 6f6e 6529 3a0d 0a20 2020  back=None):..   
-00002a90: 2070 726f 6365 7373 5f6e 616d 6520 3d20   process_name = 
-00002aa0: 2766 666d 7065 6727 0d0a 2020 2020 7472  'ffmpeg'..    tr
-00002ab0: 793a 0d0a 2020 2020 2020 2020 6f75 7470  y:..        outp
-00002ac0: 7574 203d 2073 7562 7072 6f63 6573 732e  ut = subprocess.
-00002ad0: 6368 6563 6b5f 6f75 7470 7574 285b 2770  check_output(['p
-00002ae0: 7327 2c20 272d 6566 275d 290d 0a20 2020  s', '-ef'])..   
-00002af0: 2020 2020 2070 6964 203d 205b 6c69 6e65       pid = [line
-00002b00: 2e73 706c 6974 2829 5b31 5d20 666f 7220  .split()[1] for 
-00002b10: 6c69 6e65 2069 6e20 6f75 7470 7574 2e64  line in output.d
-00002b20: 6563 6f64 6528 2775 7466 2d38 2729 2e73  ecode('utf-8').s
-00002b30: 706c 6974 2827 5c6e 2729 2069 6620 7072  plit('\n') if pr
-00002b40: 6f63 6573 735f 6e61 6d65 2069 6e20 6c69  ocess_name in li
-00002b50: 6e65 5d5b 305d 0d0a 2020 2020 2020 2020  ne][0]..        
-00002b60: 7375 6270 726f 6365 7373 2e63 616c 6c28  subprocess.call(
-00002b70: 5b27 6b69 6c6c 272c 2027 2d39 272c 2073  ['kill', '-9', s
-00002b80: 7472 2870 6964 295d 290d 0a20 2020 2020  tr(pid)])..     
-00002b90: 2020 2023 7072 696e 7428 6622 7b70 726f     #print(f"{pro
-00002ba0: 6365 7373 5f6e 616d 657d 2068 6173 2062  cess_name} has b
-00002bb0: 6565 6e20 6b69 6c6c 6564 2229 0d0a 2020  een killed")..  
-00002bc0: 2020 6578 6365 7074 2049 6e64 6578 4572    except IndexEr
-00002bd0: 726f 723a 0d0a 2020 2020 2020 2020 2370  ror:..        #p
-00002be0: 7269 6e74 2866 227b 7072 6f63 6573 735f  rint(f"{process_
-00002bf0: 6e61 6d65 7d20 6973 206e 6f74 2072 756e  name} is not run
-00002c00: 6e69 6e67 2229 0d0a 2020 2020 2020 2020  ning")..        
-00002c10: 7061 7373 0d0a 0d0a 2020 2020 6578 6365  pass....    exce
-00002c20: 7074 204b 6579 626f 6172 6449 6e74 6572  pt KeyboardInter
-00002c30: 7275 7074 3a0d 0a20 2020 2020 2020 2069  rupt:..        i
-00002c40: 6620 6572 726f 725f 6d65 7373 6167 6573  f error_messages
-00002c50: 5f63 616c 6c62 6163 6b3a 0d0a 2020 2020  _callback:..    
-00002c60: 2020 2020 2020 2020 6572 726f 725f 6d65          error_me
-00002c70: 7373 6167 6573 5f63 616c 6c62 6163 6b28  ssages_callback(
-00002c80: 2243 616e 6365 6c6c 696e 6720 616c 6c20  "Cancelling all 
-00002c90: 7461 736b 7322 290d 0a20 2020 2020 2020  tasks")..       
-00002ca0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00002cb0: 2020 2020 7072 696e 7428 2243 616e 6365      print("Cance
-00002cc0: 6c6c 696e 6720 616c 6c20 7461 736b 7322  lling all tasks"
-00002cd0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00002ce0: 6e0d 0a0d 0a20 2020 2065 7863 6570 7420  n....    except 
-00002cf0: 4578 6365 7074 696f 6e20 6173 2065 3a0d  Exception as e:.
-00002d00: 0a20 2020 2020 2020 2069 6620 6572 726f  .        if erro
-00002d10: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
-00002d20: 6163 6b3a 0d0a 2020 2020 2020 2020 2020  ack:..          
-00002d30: 2020 6572 726f 725f 6d65 7373 6167 6573    error_messages
-00002d40: 5f63 616c 6c62 6163 6b28 6529 0d0a 2020  _callback(e)..  
-00002d50: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00002d60: 2020 2020 2020 2020 2070 7269 6e74 2865           print(e
-00002d70: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00002d80: 6e0d 0a0d 0a0d 0a64 6566 2072 656d 6f76  n......def remov
-00002d90: 655f 7465 6d70 5f66 696c 6573 2865 7874  e_temp_files(ext
-00002da0: 656e 7369 6f6e 2c20 6572 726f 725f 6d65  ension, error_me
-00002db0: 7373 6167 6573 5f63 616c 6c62 6163 6b3d  ssages_callback=
-00002dc0: 4e6f 6e65 293a 0d0a 2020 2020 7472 793a  None):..    try:
-00002dd0: 0d0a 2020 2020 2020 2020 7465 6d70 5f64  ..        temp_d
-00002de0: 6972 203d 2074 656d 7066 696c 652e 6765  ir = tempfile.ge
-00002df0: 7474 656d 7064 6972 2829 0d0a 2020 2020  ttempdir()..    
-00002e00: 2020 2020 666f 7220 726f 6f74 2c20 6469      for root, di
-00002e10: 7273 2c20 6669 6c65 7320 696e 206f 732e  rs, files in os.
-00002e20: 7761 6c6b 2874 656d 705f 6469 7229 3a0d  walk(temp_dir):.
-00002e30: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00002e40: 2066 696c 6520 696e 2066 696c 6573 3a0d   file in files:.
-00002e50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002e60: 2069 6620 6669 6c65 2e65 6e64 7377 6974   if file.endswit
-00002e70: 6828 222e 2220 2b20 6578 7465 6e73 696f  h("." + extensio
-00002e80: 6e29 3a0d 0a20 2020 2020 2020 2020 2020  n):..           
-00002e90: 2020 2020 2020 2020 206f 732e 7265 6d6f           os.remo
-00002ea0: 7665 286f 732e 7061 7468 2e6a 6f69 6e28  ve(os.path.join(
-00002eb0: 726f 6f74 2c20 6669 6c65 2929 0d0a 2020  root, file))..  
-00002ec0: 2020 6578 6365 7074 204b 6579 626f 6172    except Keyboar
-00002ed0: 6449 6e74 6572 7275 7074 3a0d 0a20 2020  dInterrupt:..   
-00002ee0: 2020 2020 2069 6620 6572 726f 725f 6d65       if error_me
-00002ef0: 7373 6167 6573 5f63 616c 6c62 6163 6b3a  ssages_callback:
-00002f00: 0d0a 2020 2020 2020 2020 2020 2020 6572  ..            er
-00002f10: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
-00002f20: 6c62 6163 6b28 2243 616e 6365 6c6c 696e  lback("Cancellin
-00002f30: 6720 616c 6c20 7461 736b 7322 290d 0a20  g all tasks").. 
-00002f40: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00002f50: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00002f60: 2243 616e 6365 6c6c 696e 6720 616c 6c20  "Cancelling all 
-00002f70: 7461 736b 7322 290d 0a20 2020 2020 2020  tasks")..       
-00002f80: 2072 6574 7572 6e0d 0a0d 0a20 2020 2065   return....    e
-00002f90: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
-00002fa0: 6173 2065 3a0d 0a20 2020 2020 2020 2069  as e:..        i
-00002fb0: 6620 6572 726f 725f 6d65 7373 6167 6573  f error_messages
-00002fc0: 5f63 616c 6c62 6163 6b3a 0d0a 2020 2020  _callback:..    
-00002fd0: 2020 2020 2020 2020 6572 726f 725f 6d65          error_me
-00002fe0: 7373 6167 6573 5f63 616c 6c62 6163 6b28  ssages_callback(
-00002ff0: 6529 0d0a 2020 2020 2020 2020 656c 7365  e)..        else
-00003000: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
-00003010: 7269 6e74 2865 290d 0a20 2020 2020 2020  rint(e)..       
-00003020: 2072 6574 7572 6e0d 0a0d 0a0d 0a64 6566   return......def
-00003030: 2069 735f 7361 6d65 5f6c 616e 6775 6167   is_same_languag
-00003040: 6528 7372 632c 2064 7374 2c20 6572 726f  e(src, dst, erro
-00003050: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
-00003060: 6163 6b3d 4e6f 6e65 293a 0d0a 2020 2020  ack=None):..    
-00003070: 7472 793a 0d0a 2020 2020 2020 2020 7265  try:..        re
-00003080: 7475 726e 2073 7263 2e73 706c 6974 2822  turn src.split("
-00003090: 2d22 295b 305d 203d 3d20 6473 742e 7370  -")[0] == dst.sp
-000030a0: 6c69 7428 222d 2229 5b30 5d0d 0a20 2020  lit("-")[0]..   
-000030b0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-000030c0: 6e20 6173 2065 3a0d 0a20 2020 2020 2020  n as e:..       
-000030d0: 2069 6620 6572 726f 725f 6d65 7373 6167   if error_messag
-000030e0: 6573 5f63 616c 6c62 6163 6b3a 0d0a 2020  es_callback:..  
-000030f0: 2020 2020 2020 2020 2020 6572 726f 725f            error_
-00003100: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
-00003110: 6b28 6529 0d0a 2020 2020 2020 2020 656c  k(e)..        el
-00003120: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00003130: 2070 7269 6e74 2865 290d 0a20 2020 2020   print(e)..     
-00003140: 2020 2072 6574 7572 6e0d 0a0d 0a0d 0a64     return......d
-00003150: 6566 2063 6865 636b 5f66 696c 655f 7479  ef check_file_ty
-00003160: 7065 2866 696c 655f 7061 7468 2c20 6572  pe(file_path, er
-00003170: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
-00003180: 6c62 6163 6b3d 4e6f 6e65 293a 0d0a 2020  lback=None):..  
-00003190: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
-000031a0: 6666 7072 6f62 655f 636d 6420 3d20 5b27  ffprobe_cmd = ['
-000031b0: 6666 7072 6f62 6527 2c20 272d 7627 2c20  ffprobe', '-v', 
-000031c0: 2765 7272 6f72 272c 2027 2d73 686f 775f  'error', '-show_
-000031d0: 666f 726d 6174 272c 2027 2d73 686f 775f  format', '-show_
-000031e0: 7374 7265 616d 7327 2c20 272d 7072 696e  streams', '-prin
-000031f0: 745f 666f 726d 6174 272c 2027 6a73 6f6e  t_format', 'json
-00003200: 272c 2066 696c 655f 7061 7468 5d0d 0a20  ', file_path].. 
-00003210: 2020 2020 2020 206f 7574 7075 7420 3d20         output = 
-00003220: 4e6f 6e65 0d0a 2020 2020 2020 2020 6966  None..        if
-00003230: 2073 7973 2e70 6c61 7466 6f72 6d20 3d3d   sys.platform ==
-00003240: 2022 7769 6e33 3222 3a0d 0a20 2020 2020   "win32":..     
-00003250: 2020 2020 2020 206f 7574 7075 7420 3d20         output = 
-00003260: 7375 6270 726f 6365 7373 2e63 6865 636b  subprocess.check
-00003270: 5f6f 7574 7075 7428 6666 7072 6f62 655f  _output(ffprobe_
-00003280: 636d 642c 2063 7265 6174 696f 6e66 6c61  cmd, creationfla
-00003290: 6773 3d73 7562 7072 6f63 6573 732e 4352  gs=subprocess.CR
-000032a0: 4541 5445 5f4e 4f5f 5749 4e44 4f57 292e  EATE_NO_WINDOW).
-000032b0: 6465 636f 6465 2827 7574 662d 3827 290d  decode('utf-8').
-000032c0: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-000032d0: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
-000032e0: 7574 203d 2073 7562 7072 6f63 6573 732e  ut = subprocess.
-000032f0: 6368 6563 6b5f 6f75 7470 7574 2866 6670  check_output(ffp
-00003300: 726f 6265 5f63 6d64 292e 6465 636f 6465  robe_cmd).decode
-00003310: 2827 7574 662d 3827 290d 0a20 2020 2020  ('utf-8')..     
-00003320: 2020 2064 6174 6120 3d20 6a73 6f6e 2e6c     data = json.l
-00003330: 6f61 6473 286f 7574 7075 7429 0d0a 0d0a  oads(output)....
-00003340: 2020 2020 2020 2020 6966 2027 7374 7265          if 'stre
-00003350: 616d 7327 2069 6e20 6461 7461 3a0d 0a20  ams' in data:.. 
-00003360: 2020 2020 2020 2020 2020 2066 6f72 2073             for s
-00003370: 7472 6561 6d20 696e 2064 6174 615b 2773  tream in data['s
-00003380: 7472 6561 6d73 275d 3a0d 0a20 2020 2020  treams']:..     
-00003390: 2020 2020 2020 2020 2020 2069 6620 2763             if 'c
-000033a0: 6f64 6563 5f74 7970 6527 2069 6e20 7374  odec_type' in st
-000033b0: 7265 616d 2061 6e64 2073 7472 6561 6d5b  ream and stream[
-000033c0: 2763 6f64 6563 5f74 7970 6527 5d20 3d3d  'codec_type'] ==
-000033d0: 2027 6175 6469 6f27 3a0d 0a20 2020 2020   'audio':..     
-000033e0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000033f0: 6574 7572 6e20 2761 7564 696f 270d 0a20  eturn 'audio'.. 
-00003400: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00003410: 6c69 6620 2763 6f64 6563 5f74 7970 6527  lif 'codec_type'
-00003420: 2069 6e20 7374 7265 616d 2061 6e64 2073   in stream and s
-00003430: 7472 6561 6d5b 2763 6f64 6563 5f74 7970  tream['codec_typ
-00003440: 6527 5d20 3d3d 2027 7669 6465 6f27 3a0d  e'] == 'video':.
-00003450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003460: 2020 2020 2072 6574 7572 6e20 2776 6964       return 'vid
-00003470: 656f 270d 0a20 2020 2065 7863 6570 7420  eo'..    except 
-00003480: 2873 7562 7072 6f63 6573 732e 4361 6c6c  (subprocess.Call
-00003490: 6564 5072 6f63 6573 7345 7272 6f72 2c20  edProcessError, 
-000034a0: 6a73 6f6e 2e4a 534f 4e44 6563 6f64 6545  json.JSONDecodeE
-000034b0: 7272 6f72 293a 0d0a 2020 2020 2020 2020  rror):..        
-000034c0: 7061 7373 0d0a 0d0a 2020 2020 6578 6365  pass....    exce
-000034d0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-000034e0: 653a 0d0a 2020 2020 2020 2020 6966 2065  e:..        if e
-000034f0: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
-00003500: 6c6c 6261 636b 3a0d 0a20 2020 2020 2020  llback:..       
-00003510: 2020 2020 2065 7272 6f72 5f6d 6573 7361       error_messa
-00003520: 6765 735f 6361 6c6c 6261 636b 2865 290d  ges_callback(e).
-00003530: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-00003540: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00003550: 7428 6529 0d0a 0d0a 2020 2020 7265 7475  t(e)....    retu
-00003560: 726e 204e 6f6e 650d 0a0d 0a0d 0a63 6c61  rn None......cla
-00003570: 7373 2057 6869 7370 6572 4c61 6e67 7561  ss WhisperLangua
-00003580: 6765 3a0d 0a20 2020 2064 6566 205f 5f69  ge:..    def __i
-00003590: 6e69 745f 5f28 7365 6c66 293a 0d0a 2020  nit__(self):..  
-000035a0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-000035b0: 636f 6465 7320 3d20 5b5d 0d0a 2020 2020  codes = []..    
-000035c0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-000035d0: 6465 732e 6170 7065 6e64 2822 6166 2229  des.append("af")
-000035e0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-000035f0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00003600: 2822 7371 2229 0d0a 2020 2020 2020 2020  ("sq")..        
-00003610: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-00003620: 6170 7065 6e64 2822 616d 2229 0d0a 2020  append("am")..  
-00003630: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00003640: 636f 6465 732e 6170 7065 6e64 2822 6172  codes.append("ar
-00003650: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00003660: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00003670: 6e64 2822 6879 2229 0d0a 2020 2020 2020  nd("hy")..      
-00003680: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00003690: 732e 6170 7065 6e64 2822 6173 2229 0d0a  s.append("as")..
-000036a0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-000036b0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-000036c0: 617a 2229 0d0a 2020 2020 2020 2020 7365  az")..        se
-000036d0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-000036e0: 7065 6e64 2822 6261 2229 0d0a 2020 2020  pend("ba")..    
-000036f0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-00003700: 6465 732e 6170 7065 6e64 2822 6575 2229  des.append("eu")
-00003710: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00003720: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00003730: 2822 6265 2229 0d0a 2020 2020 2020 2020  ("be")..        
-00003740: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-00003750: 6170 7065 6e64 2822 626e 2229 0d0a 2020  append("bn")..  
-00003760: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00003770: 636f 6465 732e 6170 7065 6e64 2822 6273  codes.append("bs
-00003780: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00003790: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-000037a0: 6e64 2822 6272 2229 0d0a 2020 2020 2020  nd("br")..      
-000037b0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-000037c0: 732e 6170 7065 6e64 2822 6267 2229 0d0a  s.append("bg")..
-000037d0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-000037e0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-000037f0: 6361 2229 0d0a 2020 2020 2020 2020 7365  ca")..        se
-00003800: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00003810: 7065 6e64 2822 7a68 2229 0d0a 2020 2020  pend("zh")..    
-00003820: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-00003830: 6465 732e 6170 7065 6e64 2822 6872 2229  des.append("hr")
-00003840: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00003850: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00003860: 2822 6373 2229 0d0a 2020 2020 2020 2020  ("cs")..        
-00003870: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-00003880: 6170 7065 6e64 2822 6461 2229 0d0a 2020  append("da")..  
-00003890: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-000038a0: 636f 6465 732e 6170 7065 6e64 2822 6e6c  codes.append("nl
-000038b0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-000038c0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-000038d0: 6e64 2822 656e 2229 0d0a 2020 2020 2020  nd("en")..      
-000038e0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-000038f0: 732e 6170 7065 6e64 2822 6574 2229 0d0a  s.append("et")..
-00003900: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00003910: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00003920: 666f 2229 0d0a 2020 2020 2020 2020 7365  fo")..        se
-00003930: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00003940: 7065 6e64 2822 6669 2229 0d0a 2020 2020  pend("fi")..    
-00003950: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-00003960: 6465 732e 6170 7065 6e64 2822 6672 2229  des.append("fr")
-00003970: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00003980: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00003990: 2822 676c 2229 0d0a 2020 2020 2020 2020  ("gl")..        
-000039a0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-000039b0: 6170 7065 6e64 2822 6b61 2229 0d0a 2020  append("ka")..  
-000039c0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-000039d0: 636f 6465 732e 6170 7065 6e64 2822 6465  codes.append("de
-000039e0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-000039f0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00003a00: 6e64 2822 656c 2229 0d0a 2020 2020 2020  nd("el")..      
-00003a10: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00003a20: 732e 6170 7065 6e64 2822 6775 2229 0d0a  s.append("gu")..
-00003a30: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00003a40: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00003a50: 6874 2229 0d0a 2020 2020 2020 2020 7365  ht")..        se
-00003a60: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00003a70: 7065 6e64 2822 6861 2229 0d0a 2020 2020  pend("ha")..    
-00003a80: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-00003a90: 6465 732e 6170 7065 6e64 2822 6861 7722  des.append("haw"
-00003aa0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00003ab0: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00003ac0: 6428 2268 6522 290d 0a20 2020 2020 2020  d("he")..       
-00003ad0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00003ae0: 2e61 7070 656e 6428 2268 6922 290d 0a20  .append("hi").. 
-00003af0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00003b00: 5f63 6f64 6573 2e61 7070 656e 6428 2268  _codes.append("h
-00003b10: 7522 290d 0a20 2020 2020 2020 2073 656c  u")..        sel
-00003b20: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00003b30: 656e 6428 2269 7322 290d 0a20 2020 2020  end("is")..     
-00003b40: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00003b50: 6573 2e61 7070 656e 6428 2269 6422 290d  es.append("id").
-00003b60: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00003b70: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00003b80: 2269 7422 290d 0a20 2020 2020 2020 2073  "it")..        s
-00003b90: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00003ba0: 7070 656e 6428 226a 6122 290d 0a20 2020  ppend("ja")..   
-00003bb0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00003bc0: 6f64 6573 2e61 7070 656e 6428 226a 7622  odes.append("jv"
-00003bd0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00003be0: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00003bf0: 6428 226b 6e22 290d 0a20 2020 2020 2020  d("kn")..       
-00003c00: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00003c10: 2e61 7070 656e 6428 226b 6b22 290d 0a20  .append("kk").. 
-00003c20: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00003c30: 5f63 6f64 6573 2e61 7070 656e 6428 226b  _codes.append("k
-00003c40: 6d22 290d 0a20 2020 2020 2020 2073 656c  m")..        sel
-00003c50: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00003c60: 656e 6428 226b 6f22 290d 0a20 2020 2020  end("ko")..     
-00003c70: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00003c80: 6573 2e61 7070 656e 6428 226c 6f22 290d  es.append("lo").
-00003c90: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00003ca0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00003cb0: 226c 6122 290d 0a20 2020 2020 2020 2073  "la")..        s
-00003cc0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00003cd0: 7070 656e 6428 226c 7622 290d 0a20 2020  ppend("lv")..   
-00003ce0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00003cf0: 6f64 6573 2e61 7070 656e 6428 226c 6e22  odes.append("ln"
-00003d00: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00003d10: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00003d20: 6428 226c 7422 290d 0a20 2020 2020 2020  d("lt")..       
-00003d30: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00003d40: 2e61 7070 656e 6428 226c 6222 290d 0a20  .append("lb").. 
-00003d50: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00003d60: 5f63 6f64 6573 2e61 7070 656e 6428 226d  _codes.append("m
-00003d70: 6b22 290d 0a20 2020 2020 2020 2073 656c  k")..        sel
-00003d80: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00003d90: 656e 6428 226d 6722 290d 0a20 2020 2020  end("mg")..     
-00003da0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00003db0: 6573 2e61 7070 656e 6428 226d 7322 290d  es.append("ms").
-00003dc0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00003dd0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00003de0: 226d 6c22 290d 0a20 2020 2020 2020 2073  "ml")..        s
-00003df0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00003e00: 7070 656e 6428 226d 7422 290d 0a20 2020  ppend("mt")..   
-00003e10: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00003e20: 6f64 6573 2e61 7070 656e 6428 226d 6922  odes.append("mi"
-00003e30: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00003e40: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00003e50: 6428 226d 7222 290d 0a20 2020 2020 2020  d("mr")..       
-00003e60: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00003e70: 2e61 7070 656e 6428 226d 6e22 290d 0a20  .append("mn").. 
-00003e80: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00003e90: 5f63 6f64 6573 2e61 7070 656e 6428 226d  _codes.append("m
-00003ea0: 7922 290d 0a20 2020 2020 2020 2073 656c  y")..        sel
-00003eb0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00003ec0: 656e 6428 226e 6522 290d 0a20 2020 2020  end("ne")..     
-00003ed0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00003ee0: 6573 2e61 7070 656e 6428 226e 6f22 290d  es.append("no").
-00003ef0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00003f00: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00003f10: 226e 6e22 290d 0a20 2020 2020 2020 2073  "nn")..        s
-00003f20: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00003f30: 7070 656e 6428 226f 6322 290d 0a20 2020  ppend("oc")..   
-00003f40: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00003f50: 6f64 6573 2e61 7070 656e 6428 2270 7322  odes.append("ps"
-00003f60: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00003f70: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00003f80: 6428 2266 6122 290d 0a20 2020 2020 2020  d("fa")..       
-00003f90: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00003fa0: 2e61 7070 656e 6428 2270 6c22 290d 0a20  .append("pl").. 
-00003fb0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00003fc0: 5f63 6f64 6573 2e61 7070 656e 6428 2270  _codes.append("p
-00003fd0: 7422 290d 0a20 2020 2020 2020 2073 656c  t")..        sel
-00003fe0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00003ff0: 656e 6428 2270 6122 290d 0a20 2020 2020  end("pa")..     
-00004000: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00004010: 6573 2e61 7070 656e 6428 2272 6f22 290d  es.append("ro").
-00004020: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00004030: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00004040: 2272 7522 290d 0a20 2020 2020 2020 2073  "ru")..        s
-00004050: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00004060: 7070 656e 6428 2273 6122 290d 0a20 2020  ppend("sa")..   
-00004070: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00004080: 6f64 6573 2e61 7070 656e 6428 2273 7222  odes.append("sr"
-00004090: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000040a0: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-000040b0: 6428 2273 6e22 290d 0a20 2020 2020 2020  d("sn")..       
-000040c0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-000040d0: 2e61 7070 656e 6428 2273 6422 290d 0a20  .append("sd").. 
-000040e0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-000040f0: 5f63 6f64 6573 2e61 7070 656e 6428 2273  _codes.append("s
-00004100: 6922 290d 0a20 2020 2020 2020 2073 656c  i")..        sel
-00004110: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00004120: 656e 6428 2273 6b22 290d 0a20 2020 2020  end("sk")..     
-00004130: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00004140: 6573 2e61 7070 656e 6428 2273 6c22 290d  es.append("sl").
-00004150: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00004160: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00004170: 2273 6f22 290d 0a20 2020 2020 2020 2073  "so")..        s
-00004180: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00004190: 7070 656e 6428 2265 7322 290d 0a20 2020  ppend("es")..   
-000041a0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-000041b0: 6f64 6573 2e61 7070 656e 6428 2273 7522  odes.append("su"
-000041c0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000041d0: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-000041e0: 6428 2273 7722 290d 0a20 2020 2020 2020  d("sw")..       
-000041f0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00004200: 2e61 7070 656e 6428 2273 7622 290d 0a20  .append("sv").. 
-00004210: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00004220: 5f63 6f64 6573 2e61 7070 656e 6428 2274  _codes.append("t
-00004230: 6c22 290d 0a20 2020 2020 2020 2073 656c  l")..        sel
-00004240: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00004250: 656e 6428 2274 6722 290d 0a20 2020 2020  end("tg")..     
-00004260: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00004270: 6573 2e61 7070 656e 6428 2274 6122 290d  es.append("ta").
-00004280: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00004290: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-000042a0: 2274 7422 290d 0a20 2020 2020 2020 2073  "tt")..        s
-000042b0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-000042c0: 7070 656e 6428 2274 6522 290d 0a20 2020  ppend("te")..   
-000042d0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-000042e0: 6f64 6573 2e61 7070 656e 6428 2274 6822  odes.append("th"
-000042f0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00004300: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00004310: 6428 2262 6f22 290d 0a20 2020 2020 2020  d("bo")..       
-00004320: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00004330: 2e61 7070 656e 6428 2274 7222 290d 0a20  .append("tr").. 
-00004340: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00004350: 5f63 6f64 6573 2e61 7070 656e 6428 2274  _codes.append("t
-00004360: 6b22 290d 0a20 2020 2020 2020 2073 656c  k")..        sel
-00004370: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00004380: 656e 6428 2275 6b22 290d 0a20 2020 2020  end("uk")..     
-00004390: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-000043a0: 6573 2e61 7070 656e 6428 2275 7222 290d  es.append("ur").
-000043b0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-000043c0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-000043d0: 2275 7a22 290d 0a20 2020 2020 2020 2073  "uz")..        s
-000043e0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-000043f0: 7070 656e 6428 2276 6922 290d 0a20 2020  ppend("vi")..   
-00004400: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00004410: 6f64 6573 2e61 7070 656e 6428 2263 7922  odes.append("cy"
-00004420: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00004430: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00004440: 6428 2279 6922 290d 0a20 2020 2020 2020  d("yi")..       
-00004450: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00004460: 2e61 7070 656e 6428 2279 6f22 290d 0a0d  .append("yo")...
-00004470: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00004480: 7374 5f6e 616d 6573 203d 205b 5d0d 0a20  st_names = [].. 
-00004490: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-000044a0: 5f6e 616d 6573 2e61 7070 656e 6428 2241  _names.append("A
-000044b0: 6672 696b 6161 6e73 2229 0d0a 2020 2020  frikaans")..    
-000044c0: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-000044d0: 6d65 732e 6170 7065 6e64 2822 416c 6261  mes.append("Alba
-000044e0: 6e69 616e 2229 0d0a 2020 2020 2020 2020  nian")..        
-000044f0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00004500: 6170 7065 6e64 2822 416d 6861 7269 6322  append("Amharic"
-00004510: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00004520: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00004530: 6428 2241 7261 6269 6322 290d 0a20 2020  d("Arabic")..   
-00004540: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00004550: 616d 6573 2e61 7070 656e 6428 2241 726d  ames.append("Arm
-00004560: 656e 6961 6e22 290d 0a20 2020 2020 2020  enian")..       
-00004570: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00004580: 2e61 7070 656e 6428 2241 7373 616d 6573  .append("Assames
-00004590: 6522 290d 0a20 2020 2020 2020 2073 656c  e")..        sel
-000045a0: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-000045b0: 656e 6428 2241 7a65 7262 6169 6a61 6e69  end("Azerbaijani
-000045c0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-000045d0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-000045e0: 6e64 2822 4261 7368 6b69 7222 290d 0a20  nd("Bashkir").. 
-000045f0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00004600: 5f6e 616d 6573 2e61 7070 656e 6428 2242  _names.append("B
-00004610: 6173 7175 6522 290d 0a20 2020 2020 2020  asque")..       
-00004620: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00004630: 2e61 7070 656e 6428 2242 656c 6172 7573  .append("Belarus
-00004640: 6961 6e22 290d 0a20 2020 2020 2020 2073  ian")..        s
-00004650: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00004660: 7070 656e 6428 2242 656e 6761 6c69 2229  ppend("Bengali")
-00004670: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00004680: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00004690: 2822 426f 736e 6961 6e22 290d 0a20 2020  ("Bosnian")..   
-000046a0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-000046b0: 616d 6573 2e61 7070 656e 6428 2242 7265  ames.append("Bre
-000046c0: 746f 6e22 290d 0a20 2020 2020 2020 2073  ton")..        s
-000046d0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-000046e0: 7070 656e 6428 2242 756c 6761 7269 616e  ppend("Bulgarian
-000046f0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00004700: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00004710: 6e64 2822 4361 7461 6c61 6e22 290d 0a20  nd("Catalan").. 
-00004720: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00004730: 5f6e 616d 6573 2e61 7070 656e 6428 2243  _names.append("C
-00004740: 6869 6e65 7365 2229 0d0a 2020 2020 2020  hinese")..      
-00004750: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00004760: 732e 6170 7065 6e64 2822 4372 6f61 7469  s.append("Croati
-00004770: 616e 2229 0d0a 2020 2020 2020 2020 7365  an")..        se
-00004780: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00004790: 7065 6e64 2822 437a 6563 6822 290d 0a20  pend("Czech").. 
-000047a0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-000047b0: 5f6e 616d 6573 2e61 7070 656e 6428 2244  _names.append("D
-000047c0: 616e 6973 6822 290d 0a20 2020 2020 2020  anish")..       
-000047d0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-000047e0: 2e61 7070 656e 6428 2244 7574 6368 2229  .append("Dutch")
-000047f0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00004800: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00004810: 2822 456e 676c 6973 6822 290d 0a20 2020  ("English")..   
-00004820: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00004830: 616d 6573 2e61 7070 656e 6428 2245 7374  ames.append("Est
-00004840: 6f6e 6961 6e22 290d 0a20 2020 2020 2020  onian")..       
-00004850: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00004860: 2e61 7070 656e 6428 2246 6172 6f65 7365  .append("Faroese
-00004870: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00004880: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00004890: 6e64 2822 4669 6e6e 6973 6822 290d 0a20  nd("Finnish").. 
-000048a0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-000048b0: 5f6e 616d 6573 2e61 7070 656e 6428 2246  _names.append("F
-000048c0: 7265 6e63 6822 290d 0a20 2020 2020 2020  rench")..       
-000048d0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-000048e0: 2e61 7070 656e 6428 2247 616c 6963 6961  .append("Galicia
-000048f0: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
-00004900: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00004910: 656e 6428 2247 656f 7267 6961 6e22 290d  end("Georgian").
-00004920: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00004930: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00004940: 2247 6572 6d61 6e22 290d 0a20 2020 2020  "German")..     
-00004950: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00004960: 6573 2e61 7070 656e 6428 2247 7265 656b  es.append("Greek
-00004970: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00004980: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00004990: 6e64 2822 4775 6a61 7261 7469 2229 0d0a  nd("Gujarati")..
-000049a0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-000049b0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-000049c0: 4861 6974 6961 6e20 4372 656f 6c65 2229  Haitian Creole")
-000049d0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-000049e0: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-000049f0: 2822 4861 7573 6122 290d 0a20 2020 2020  ("Hausa")..     
-00004a00: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00004a10: 6573 2e61 7070 656e 6428 2248 6177 6169  es.append("Hawai
-00004a20: 6961 6e22 290d 0a20 2020 2020 2020 2073  ian")..        s
-00004a30: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00004a40: 7070 656e 6428 2248 6562 7265 7722 290d  ppend("Hebrew").
-00004a50: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00004a60: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00004a70: 2248 696e 6469 2229 0d0a 2020 2020 2020  "Hindi")..      
-00004a80: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00004a90: 732e 6170 7065 6e64 2822 4875 6e67 6172  s.append("Hungar
-00004aa0: 6961 6e22 290d 0a20 2020 2020 2020 2073  ian")..        s
-00004ab0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00004ac0: 7070 656e 6428 2249 6365 6c61 6e64 6963  ppend("Icelandic
-00004ad0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00004ae0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00004af0: 6e64 2822 496e 646f 6e65 7369 616e 2229  nd("Indonesian")
-00004b00: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00004b10: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00004b20: 2822 4974 616c 6961 6e22 290d 0a20 2020  ("Italian")..   
-00004b30: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00004b40: 616d 6573 2e61 7070 656e 6428 224a 6170  ames.append("Jap
-00004b50: 616e 6573 6522 290d 0a20 2020 2020 2020  anese")..       
-00004b60: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00004b70: 2e61 7070 656e 6428 224a 6176 616e 6573  .append("Javanes
-00004b80: 6522 290d 0a20 2020 2020 2020 2073 656c  e")..        sel
-00004b90: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00004ba0: 656e 6428 224b 616e 6e61 6461 2229 0d0a  end("Kannada")..
-00004bb0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00004bc0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-00004bd0: 4b61 7a61 6b68 2229 0d0a 2020 2020 2020  Kazakh")..      
-00004be0: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00004bf0: 732e 6170 7065 6e64 2822 4b68 6d65 7222  s.append("Khmer"
-00004c00: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00004c10: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00004c20: 6428 224b 6f72 6561 6e22 290d 0a20 2020  d("Korean")..   
-00004c30: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00004c40: 616d 6573 2e61 7070 656e 6428 224c 616f  ames.append("Lao
-00004c50: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00004c60: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00004c70: 6e64 2822 4c61 7469 6e22 290d 0a20 2020  nd("Latin")..   
-00004c80: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00004c90: 616d 6573 2e61 7070 656e 6428 224c 6174  ames.append("Lat
-00004ca0: 7669 616e 2229 0d0a 2020 2020 2020 2020  vian")..        
-00004cb0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00004cc0: 6170 7065 6e64 2822 4c69 6e67 616c 6122  append("Lingala"
-00004cd0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00004ce0: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00004cf0: 6428 224c 6974 6875 616e 6961 6e22 290d  d("Lithuanian").
-00004d00: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00004d10: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00004d20: 224c 7578 656d 626f 7572 6769 7368 2229  "Luxembourgish")
-00004d30: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00004d40: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00004d50: 2822 4d61 6365 646f 6e69 616e 2229 0d0a  ("Macedonian")..
-00004d60: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00004d70: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-00004d80: 4d61 6c61 6761 7379 2229 0d0a 2020 2020  Malagasy")..    
-00004d90: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00004da0: 6d65 732e 6170 7065 6e64 2822 4d61 6c61  mes.append("Mala
-00004db0: 7922 290d 0a20 2020 2020 2020 2073 656c  y")..        sel
-00004dc0: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00004dd0: 656e 6428 224d 616c 6179 616c 616d 2229  end("Malayalam")
-00004de0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00004df0: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00004e00: 2822 4d61 6c74 6573 6522 290d 0a20 2020  ("Maltese")..   
-00004e10: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00004e20: 616d 6573 2e61 7070 656e 6428 224d 616f  ames.append("Mao
-00004e30: 7269 2229 0d0a 2020 2020 2020 2020 7365  ri")..        se
-00004e40: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00004e50: 7065 6e64 2822 4d61 7261 7468 6922 290d  pend("Marathi").
-00004e60: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00004e70: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00004e80: 224d 6f6e 676f 6c69 616e 2229 0d0a 2020  "Mongolian")..  
-00004e90: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00004ea0: 6e61 6d65 732e 6170 7065 6e64 2822 4d79  names.append("My
-00004eb0: 616e 6d61 7220 2842 7572 6d65 7365 2922  anmar (Burmese)"
-00004ec0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00004ed0: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00004ee0: 6428 224e 6570 616c 6922 290d 0a20 2020  d("Nepali")..   
-00004ef0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00004f00: 616d 6573 2e61 7070 656e 6428 224e 6f72  ames.append("Nor
-00004f10: 7765 6769 616e 2229 0d0a 2020 2020 2020  wegian")..      
-00004f20: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00004f30: 732e 6170 7065 6e64 2822 4e79 6e6f 7273  s.append("Nynors
-00004f40: 6b22 290d 0a20 2020 2020 2020 2073 656c  k")..        sel
-00004f50: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00004f60: 656e 6428 224f 6363 6974 616e 2229 0d0a  end("Occitan")..
-00004f70: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00004f80: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-00004f90: 5061 7368 746f 2229 0d0a 2020 2020 2020  Pashto")..      
-00004fa0: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00004fb0: 732e 6170 7065 6e64 2822 5065 7273 6961  s.append("Persia
-00004fc0: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
-00004fd0: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00004fe0: 656e 6428 2250 6f6c 6973 6822 290d 0a20  end("Polish").. 
-00004ff0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00005000: 5f6e 616d 6573 2e61 7070 656e 6428 2250  _names.append("P
-00005010: 6f72 7475 6775 6573 6522 290d 0a20 2020  ortuguese")..   
-00005020: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00005030: 616d 6573 2e61 7070 656e 6428 2250 756e  ames.append("Pun
-00005040: 6a61 6269 2229 0d0a 2020 2020 2020 2020  jabi")..        
-00005050: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00005060: 6170 7065 6e64 2822 526f 6d61 6e69 616e  append("Romanian
-00005070: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00005080: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00005090: 6e64 2822 5275 7373 6961 6e22 290d 0a20  nd("Russian").. 
-000050a0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-000050b0: 5f6e 616d 6573 2e61 7070 656e 6428 2253  _names.append("S
-000050c0: 616e 736b 7269 7422 290d 0a20 2020 2020  anskrit")..     
-000050d0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-000050e0: 6573 2e61 7070 656e 6428 2253 6572 6269  es.append("Serbi
-000050f0: 616e 2229 0d0a 2020 2020 2020 2020 7365  an")..        se
-00005100: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00005110: 7065 6e64 2822 5368 6f6e 6122 290d 0a20  pend("Shona").. 
-00005120: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00005130: 5f6e 616d 6573 2e61 7070 656e 6428 2253  _names.append("S
-00005140: 696e 6468 6922 290d 0a20 2020 2020 2020  indhi")..       
-00005150: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00005160: 2e61 7070 656e 6428 2253 696e 6861 6c61  .append("Sinhala
-00005170: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00005180: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00005190: 6e64 2822 536c 6f76 616b 2229 0d0a 2020  nd("Slovak")..  
-000051a0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-000051b0: 6e61 6d65 732e 6170 7065 6e64 2822 536c  names.append("Sl
-000051c0: 6f76 656e 6961 6e22 290d 0a20 2020 2020  ovenian")..     
-000051d0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-000051e0: 6573 2e61 7070 656e 6428 2253 6f6d 616c  es.append("Somal
-000051f0: 6922 290d 0a20 2020 2020 2020 2073 656c  i")..        sel
-00005200: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00005210: 656e 6428 2253 7061 6e69 7368 2229 0d0a  end("Spanish")..
-00005220: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00005230: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-00005240: 5375 6e64 616e 6573 6522 290d 0a20 2020  Sundanese")..   
-00005250: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00005260: 616d 6573 2e61 7070 656e 6428 2253 7761  ames.append("Swa
-00005270: 6869 6c69 2229 0d0a 2020 2020 2020 2020  hili")..        
-00005280: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00005290: 6170 7065 6e64 2822 5377 6564 6973 6822  append("Swedish"
-000052a0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000052b0: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-000052c0: 6428 2254 6167 616c 6f67 2229 0d0a 2020  d("Tagalog")..  
-000052d0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-000052e0: 6e61 6d65 732e 6170 7065 6e64 2822 5461  names.append("Ta
-000052f0: 6a69 6b22 290d 0a20 2020 2020 2020 2073  jik")..        s
-00005300: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00005310: 7070 656e 6428 2254 616d 696c 2229 0d0a  ppend("Tamil")..
-00005320: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00005330: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-00005340: 5461 7461 7222 290d 0a20 2020 2020 2020  Tatar")..       
-00005350: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00005360: 2e61 7070 656e 6428 2254 656c 7567 7522  .append("Telugu"
-00005370: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00005380: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00005390: 6428 2254 6861 6922 290d 0a20 2020 2020  d("Thai")..     
-000053a0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-000053b0: 6573 2e61 7070 656e 6428 2254 6962 6574  es.append("Tibet
-000053c0: 616e 2229 0d0a 2020 2020 2020 2020 7365  an")..        se
-000053d0: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-000053e0: 7065 6e64 2822 5475 726b 6973 6822 290d  pend("Turkish").
-000053f0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00005400: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00005410: 2254 7572 6b6d 656e 2229 0d0a 2020 2020  "Turkmen")..    
-00005420: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00005430: 6d65 732e 6170 7065 6e64 2822 556b 7261  mes.append("Ukra
-00005440: 696e 6961 6e22 290d 0a20 2020 2020 2020  inian")..       
-00005450: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00005460: 2e61 7070 656e 6428 2255 7264 7522 290d  .append("Urdu").
-00005470: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00005480: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00005490: 2255 7a62 656b 2229 0d0a 2020 2020 2020  "Uzbek")..      
-000054a0: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-000054b0: 732e 6170 7065 6e64 2822 5669 6574 6e61  s.append("Vietna
-000054c0: 6d65 7365 2229 0d0a 2020 2020 2020 2020  mese")..        
-000054d0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-000054e0: 6170 7065 6e64 2822 5765 6c73 6822 290d  append("Welsh").
-000054f0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00005500: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00005510: 2259 6964 6469 7368 2229 0d0a 2020 2020  "Yiddish")..    
-00005520: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00005530: 6d65 732e 6170 7065 6e64 2822 596f 7275  mes.append("Yoru
-00005540: 6261 2229 0d0a 0d0a 2020 2020 2020 2020  ba")....        
-00005550: 7365 6c66 2e63 6f64 655f 6f66 5f6e 616d  self.code_of_nam
-00005560: 6520 3d20 6469 6374 287a 6970 2873 656c  e = dict(zip(sel
-00005570: 662e 6c69 7374 5f6e 616d 6573 2c20 7365  f.list_names, se
-00005580: 6c66 2e6c 6973 745f 636f 6465 7329 290d  lf.list_codes)).
-00005590: 0a20 2020 2020 2020 2073 656c 662e 6e61  .        self.na
-000055a0: 6d65 5f6f 665f 636f 6465 203d 2064 6963  me_of_code = dic
-000055b0: 7428 7a69 7028 7365 6c66 2e6c 6973 745f  t(zip(self.list_
-000055c0: 636f 6465 732c 2073 656c 662e 6c69 7374  codes, self.list
-000055d0: 5f6e 616d 6573 2929 0d0a 0d0a 2020 2020  _names))....    
-000055e0: 2020 2020 7365 6c66 2e64 6963 7420 3d20      self.dict = 
-000055f0: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-00005600: 2020 2020 2020 2020 2020 2027 6166 273a             'af':
-00005610: 2027 4166 7269 6b61 616e 7327 2c0d 0a20   'Afrikaans',.. 
-00005620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005630: 2020 2020 2020 2027 7371 273a 2027 416c         'sq': 'Al
-00005640: 6261 6e69 616e 272c 0d0a 2020 2020 2020  banian',..      
-00005650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005660: 2020 2761 6d27 3a20 2741 6d68 6172 6963    'am': 'Amharic
-00005670: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00005680: 2020 2020 2020 2020 2020 2020 2761 7227              'ar'
-00005690: 3a20 2741 7261 6269 6327 2c0d 0a20 2020  : 'Arabic',..   
-000056a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056b0: 2020 2020 2027 6879 273a 2027 4172 6d65       'hy': 'Arme
-000056c0: 6e69 616e 272c 0d0a 2020 2020 2020 2020  nian',..        
-000056d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056e0: 2761 7327 3a20 2741 7373 616d 6573 6527  'as': 'Assamese'
-000056f0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00005700: 2020 2020 2020 2020 2020 2027 617a 273a             'az':
-00005710: 2027 417a 6572 6261 696a 616e 6927 2c0d   'Azerbaijani',.
-00005720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005730: 2020 2020 2020 2020 2027 6261 273a 2027           'ba': '
-00005740: 4261 7368 6b69 7227 2c0d 0a20 2020 2020  Bashkir',..     
-00005750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005760: 2020 2027 6575 273a 2027 4261 7371 7565     'eu': 'Basque
-00005770: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00005780: 2020 2020 2020 2020 2020 2020 2762 6527              'be'
-00005790: 3a20 2742 656c 6172 7573 6961 6e27 2c0d  : 'Belarusian',.
-000057a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000057b0: 2020 2020 2020 2020 2027 626e 273a 2027           'bn': '
-000057c0: 4265 6e67 616c 6927 2c0d 0a20 2020 2020  Bengali',..     
-000057d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057e0: 2020 2027 6273 273a 2027 426f 736e 6961     'bs': 'Bosnia
-000057f0: 6e27 2c0d 0a20 2020 2020 2020 2020 2020  n',..           
-00005800: 2020 2020 2020 2020 2020 2020 2027 6272               'br
-00005810: 273a 2027 4272 6574 6f6e 272c 0d0a 2020  ': 'Breton',..  
-00005820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005830: 2020 2020 2020 2762 6727 3a20 2742 756c        'bg': 'Bul
-00005840: 6761 7269 616e 272c 0d0a 2020 2020 2020  garian',..      
-00005850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005860: 2020 2763 6127 3a20 2743 6174 616c 616e    'ca': 'Catalan
-00005870: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00005880: 2020 2020 2020 2020 2020 2020 277a 6827              'zh'
-00005890: 3a20 2743 6869 6e65 7365 272c 0d0a 2020  : 'Chinese',..  
-000058a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058b0: 2020 2020 2020 2768 7227 3a20 2743 726f        'hr': 'Cro
-000058c0: 6174 6961 6e27 2c0d 0a20 2020 2020 2020  atian',..       
-000058d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058e0: 2027 6373 273a 2027 437a 6563 6827 2c0d   'cs': 'Czech',.
-000058f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005900: 2020 2020 2020 2020 2027 6461 273a 2027           'da': '
-00005910: 4461 6e69 7368 272c 0d0a 2020 2020 2020  Danish',..      
-00005920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005930: 2020 276e 6c27 3a20 2744 7574 6368 272c    'nl': 'Dutch',
-00005940: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005950: 2020 2020 2020 2020 2020 2765 6e27 3a20            'en': 
-00005960: 2745 6e67 6c69 7368 272c 0d0a 2020 2020  'English',..    
-00005970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005980: 2020 2020 2765 7427 3a20 2745 7374 6f6e      'et': 'Eston
-00005990: 6961 6e27 2c0d 0a20 2020 2020 2020 2020  ian',..         
-000059a0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000059b0: 666f 273a 2027 4661 726f 6573 6527 2c0d  fo': 'Faroese',.
-000059c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000059d0: 2020 2020 2020 2020 2027 6669 273a 2027           'fi': '
-000059e0: 4669 6e6e 6973 6827 2c0d 0a20 2020 2020  Finnish',..     
-000059f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a00: 2020 2027 6672 273a 2027 4672 656e 6368     'fr': 'French
-00005a10: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00005a20: 2020 2020 2020 2020 2020 2020 2767 6c27              'gl'
-00005a30: 3a20 2747 616c 6963 6961 6e27 2c0d 0a20  : 'Galician',.. 
-00005a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a50: 2020 2020 2020 2027 6b61 273a 2027 4765         'ka': 'Ge
-00005a60: 6f72 6769 616e 272c 0d0a 2020 2020 2020  orgian',..      
-00005a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a80: 2020 2764 6527 3a20 2747 6572 6d61 6e27    'de': 'German'
-00005a90: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00005aa0: 2020 2020 2020 2020 2020 2027 656c 273a             'el':
-00005ab0: 2027 4772 6565 6b27 2c0d 0a20 2020 2020   'Greek',..     
-00005ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ad0: 2020 2027 6775 273a 2027 4775 6a61 7261     'gu': 'Gujara
-00005ae0: 7469 272c 0d0a 2020 2020 2020 2020 2020  ti',..          
-00005af0: 2020 2020 2020 2020 2020 2020 2020 2768                'h
-00005b00: 7427 3a20 2748 6169 7469 616e 2043 7265  t': 'Haitian Cre
-00005b10: 6f6c 6527 2c0d 0a20 2020 2020 2020 2020  ole',..         
-00005b20: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00005b30: 6861 273a 2027 4861 7573 6127 2c0d 0a20  ha': 'Hausa',.. 
-00005b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b50: 2020 2020 2020 2027 6861 7727 3a20 2748         'haw': 'H
-00005b60: 6177 6169 6961 6e27 2c0d 0a20 2020 2020  awaiian',..     
-00005b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b80: 2020 2027 6865 273a 2027 4865 6272 6577     'he': 'Hebrew
-00005b90: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00005ba0: 2020 2020 2020 2020 2020 2020 2768 6927              'hi'
-00005bb0: 3a20 2748 696e 6469 272c 0d0a 2020 2020  : 'Hindi',..    
-00005bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005bd0: 2020 2020 2768 7527 3a20 2748 756e 6761      'hu': 'Hunga
-00005be0: 7269 616e 272c 0d0a 2020 2020 2020 2020  rian',..        
-00005bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c00: 2769 7327 3a20 2749 6365 6c61 6e64 6963  'is': 'Icelandic
-00005c10: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00005c20: 2020 2020 2020 2020 2020 2020 2769 6427              'id'
-00005c30: 3a20 2749 6e64 6f6e 6573 6961 6e27 2c0d  : 'Indonesian',.
-00005c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005c50: 2020 2020 2020 2020 2027 6974 273a 2027           'it': '
-00005c60: 4974 616c 6961 6e27 2c0d 0a20 2020 2020  Italian',..     
-00005c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c80: 2020 2027 6a61 273a 2027 4a61 7061 6e65     'ja': 'Japane
-00005c90: 7365 272c 0d0a 2020 2020 2020 2020 2020  se',..          
-00005ca0: 2020 2020 2020 2020 2020 2020 2020 276a                'j
-00005cb0: 7627 3a20 274a 6176 616e 6573 6527 2c0d  v': 'Javanese',.
-00005cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005cd0: 2020 2020 2020 2020 2027 6b6e 273a 2027           'kn': '
-00005ce0: 4b61 6e6e 6164 6127 2c0d 0a20 2020 2020  Kannada',..     
-00005cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d00: 2020 2027 6b6b 273a 2027 4b61 7a61 6b68     'kk': 'Kazakh
-00005d10: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00005d20: 2020 2020 2020 2020 2020 2020 276b 6d27              'km'
-00005d30: 3a20 274b 686d 6572 272c 0d0a 2020 2020  : 'Khmer',..    
-00005d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d50: 2020 2020 276b 6f27 3a20 274b 6f72 6561      'ko': 'Korea
-00005d60: 6e27 2c0d 0a20 2020 2020 2020 2020 2020  n',..           
-00005d70: 2020 2020 2020 2020 2020 2020 2027 6c6f               'lo
-00005d80: 273a 2027 4c61 6f27 2c0d 0a20 2020 2020  ': 'Lao',..     
-00005d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005da0: 2020 2027 6c61 273a 2027 4c61 7469 6e27     'la': 'Latin'
-00005db0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00005dc0: 2020 2020 2020 2020 2020 2027 6c76 273a             'lv':
-00005dd0: 2027 4c61 7476 6961 6e27 2c0d 0a20 2020   'Latvian',..   
-00005de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005df0: 2020 2020 2027 6c6e 273a 2027 4c69 6e67       'ln': 'Ling
-00005e00: 616c 6127 2c0d 0a20 2020 2020 2020 2020  ala',..         
-00005e10: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00005e20: 6c74 273a 2027 4c69 7468 7561 6e69 616e  lt': 'Lithuanian
-00005e30: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00005e40: 2020 2020 2020 2020 2020 2020 276c 6227              'lb'
-00005e50: 3a20 274c 7578 656d 626f 7572 6769 7368  : 'Luxembourgish
-00005e60: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00005e70: 2020 2020 2020 2020 2020 2020 276d 6b27              'mk'
-00005e80: 3a20 274d 6163 6564 6f6e 6961 6e27 2c0d  : 'Macedonian',.
-00005e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005ea0: 2020 2020 2020 2020 2027 6d67 273a 2027           'mg': '
-00005eb0: 4d61 6c61 6761 7379 272c 0d0a 2020 2020  Malagasy',..    
-00005ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ed0: 2020 2020 276d 7327 3a20 274d 616c 6179      'ms': 'Malay
-00005ee0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00005ef0: 2020 2020 2020 2020 2020 2020 276d 6c27              'ml'
-00005f00: 3a20 274d 616c 6179 616c 616d 272c 0d0a  : 'Malayalam',..
-00005f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f20: 2020 2020 2020 2020 276d 7427 3a20 274d          'mt': 'M
-00005f30: 616c 7465 7365 272c 0d0a 2020 2020 2020  altese',..      
-00005f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f50: 2020 276d 6927 3a20 274d 616f 7269 272c    'mi': 'Maori',
-00005f60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005f70: 2020 2020 2020 2020 2020 276d 7227 3a20            'mr': 
-00005f80: 274d 6172 6174 6869 272c 0d0a 2020 2020  'Marathi',..    
-00005f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fa0: 2020 2020 276d 6e27 3a20 274d 6f6e 676f      'mn': 'Mongo
-00005fb0: 6c69 616e 272c 0d0a 2020 2020 2020 2020  lian',..        
-00005fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fd0: 276d 7927 3a20 274d 7961 6e6d 6172 2028  'my': 'Myanmar (
-00005fe0: 4275 726d 6573 6529 272c 0d0a 2020 2020  Burmese)',..    
-00005ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006000: 2020 2020 276e 6527 3a20 274e 6570 616c      'ne': 'Nepal
-00006010: 6927 2c0d 0a20 2020 2020 2020 2020 2020  i',..           
-00006020: 2020 2020 2020 2020 2020 2020 2027 6e6f               'no
-00006030: 273a 2027 4e6f 7277 6567 6961 6e27 2c0d  ': 'Norwegian',.
-00006040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006050: 2020 2020 2020 2020 2027 6e6e 273a 2027           'nn': '
-00006060: 4e79 6e6f 7273 6b27 2c0d 0a20 2020 2020  Nynorsk',..     
-00006070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006080: 2020 2027 6f63 273a 2027 4f63 6369 7461     'oc': 'Occita
-00006090: 6e27 2c0d 0a20 2020 2020 2020 2020 2020  n',..           
-000060a0: 2020 2020 2020 2020 2020 2020 2027 7073               'ps
-000060b0: 273a 2027 5061 7368 746f 272c 0d0a 2020  ': 'Pashto',..  
-000060c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060d0: 2020 2020 2020 2766 6127 3a20 2750 6572        'fa': 'Per
-000060e0: 7369 616e 272c 0d0a 2020 2020 2020 2020  sian',..        
-000060f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006100: 2770 6c27 3a20 2750 6f6c 6973 6827 2c0d  'pl': 'Polish',.
-00006110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006120: 2020 2020 2020 2020 2027 7074 273a 2027           'pt': '
-00006130: 506f 7274 7567 7565 7365 272c 0d0a 2020  Portuguese',..  
-00006140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006150: 2020 2020 2020 2770 6127 3a20 2750 756e        'pa': 'Pun
-00006160: 6a61 6269 272c 0d0a 2020 2020 2020 2020  jabi',..        
-00006170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006180: 2772 6f27 3a20 2752 6f6d 616e 6961 6e27  'ro': 'Romanian'
-00006190: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000061a0: 2020 2020 2020 2020 2020 2027 7275 273a             'ru':
-000061b0: 2027 5275 7373 6961 6e27 2c0d 0a20 2020   'Russian',..   
-000061c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061d0: 2020 2020 2027 7361 273a 2027 5361 6e73       'sa': 'Sans
-000061e0: 6b72 6974 272c 0d0a 2020 2020 2020 2020  krit',..        
-000061f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006200: 2773 7227 3a20 2753 6572 6269 616e 272c  'sr': 'Serbian',
-00006210: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006220: 2020 2020 2020 2020 2020 2773 6e27 3a20            'sn': 
-00006230: 2753 686f 6e61 272c 0d0a 2020 2020 2020  'Shona',..      
-00006240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006250: 2020 2773 6427 3a20 2753 696e 6468 6927    'sd': 'Sindhi'
-00006260: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00006270: 2020 2020 2020 2020 2020 2027 7369 273a             'si':
-00006280: 2027 5369 6e68 616c 6127 2c0d 0a20 2020   'Sinhala',..   
-00006290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062a0: 2020 2020 2027 736b 273a 2027 536c 6f76       'sk': 'Slov
-000062b0: 616b 272c 0d0a 2020 2020 2020 2020 2020  ak',..          
-000062c0: 2020 2020 2020 2020 2020 2020 2020 2773                's
-000062d0: 6c27 3a20 2753 6c6f 7665 6e69 616e 272c  l': 'Slovenian',
-000062e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000062f0: 2020 2020 2020 2020 2020 2773 6f27 3a20            'so': 
-00006300: 2753 6f6d 616c 6927 2c0d 0a20 2020 2020  'Somali',..     
-00006310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006320: 2020 2027 6573 273a 2027 5370 616e 6973     'es': 'Spanis
-00006330: 6827 2c0d 0a20 2020 2020 2020 2020 2020  h',..           
-00006340: 2020 2020 2020 2020 2020 2020 2027 7375               'su
-00006350: 273a 2027 5375 6e64 616e 6573 6527 2c0d  ': 'Sundanese',.
-00006360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006370: 2020 2020 2020 2020 2027 7377 273a 2027           'sw': '
-00006380: 5377 6168 696c 6927 2c0d 0a20 2020 2020  Swahili',..     
-00006390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063a0: 2020 2027 7376 273a 2027 5377 6564 6973     'sv': 'Swedis
-000063b0: 6827 2c0d 0a20 2020 2020 2020 2020 2020  h',..           
-000063c0: 2020 2020 2020 2020 2020 2020 2027 746c               'tl
-000063d0: 273a 2027 5461 6761 6c6f 6727 2c0d 0a20  ': 'Tagalog',.. 
-000063e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063f0: 2020 2020 2020 2027 7467 273a 2027 5461         'tg': 'Ta
-00006400: 6a69 6b27 2c0d 0a20 2020 2020 2020 2020  jik',..         
-00006410: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00006420: 7461 273a 2027 5461 6d69 6c27 2c0d 0a20  ta': 'Tamil',.. 
-00006430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006440: 2020 2020 2020 2027 7474 273a 2027 5461         'tt': 'Ta
-00006450: 7461 7227 2c0d 0a20 2020 2020 2020 2020  tar',..         
-00006460: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00006470: 7465 273a 2027 5465 6c75 6775 272c 0d0a  te': 'Telugu',..
-00006480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006490: 2020 2020 2020 2020 2774 6827 3a20 2754          'th': 'T
-000064a0: 6861 6927 2c0d 0a20 2020 2020 2020 2020  hai',..         
-000064b0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000064c0: 626f 273a 2027 5469 6265 7461 6e27 2c0d  bo': 'Tibetan',.
-000064d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000064e0: 2020 2020 2020 2020 2027 7472 273a 2027           'tr': '
-000064f0: 5475 726b 6973 6827 2c0d 0a20 2020 2020  Turkish',..     
-00006500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006510: 2020 2027 746b 273a 2027 5475 726b 6d65     'tk': 'Turkme
-00006520: 6e27 2c0d 0a20 2020 2020 2020 2020 2020  n',..           
-00006530: 2020 2020 2020 2020 2020 2020 2027 756b               'uk
-00006540: 273a 2027 556b 7261 696e 6961 6e27 2c0d  ': 'Ukrainian',.
-00006550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006560: 2020 2020 2020 2020 2027 7572 273a 2027           'ur': '
-00006570: 5572 6475 272c 0d0a 2020 2020 2020 2020  Urdu',..        
-00006580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006590: 2775 7a27 3a20 2755 7a62 656b 272c 0d0a  'uz': 'Uzbek',..
-000065a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065b0: 2020 2020 2020 2020 2776 6927 3a20 2756          'vi': 'V
-000065c0: 6965 746e 616d 6573 6527 2c0d 0a20 2020  ietnamese',..   
-000065d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065e0: 2020 2020 2027 6379 273a 2027 5765 6c73       'cy': 'Wels
-000065f0: 6827 2c0d 0a20 2020 2020 2020 2020 2020  h',..           
-00006600: 2020 2020 2020 2020 2020 2020 2027 7969               'yi
-00006610: 273a 2027 5969 6464 6973 6827 2c0d 0a20  ': 'Yiddish',.. 
-00006620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006630: 2020 2020 2020 2027 796f 273a 2027 596f         'yo': 'Yo
-00006640: 7275 6261 272c 0d0a 2020 2020 2020 2020  ruba',..        
-00006650: 2020 2020 2020 2020 2020 2020 7d0d 0a0d              }...
-00006660: 0a20 2020 2064 6566 2067 6574 5f6e 616d  .    def get_nam
-00006670: 6528 7365 6c66 2c20 6765 745f 636f 6465  e(self, get_code
-00006680: 293a 0d0a 2020 2020 2020 2020 7265 7475  ):..        retu
-00006690: 726e 2073 656c 662e 6469 6374 2e67 6574  rn self.dict.get
-000066a0: 2867 6574 5f63 6f64 652e 6c6f 7765 7228  (get_code.lower(
-000066b0: 292c 2022 2229 0d0a 0d0a 2020 2020 6465  ), "")....    de
-000066c0: 6620 6765 745f 636f 6465 2873 656c 662c  f get_code(self,
-000066d0: 206c 616e 6775 6167 6529 3a0d 0a20 2020   language):..   
-000066e0: 2020 2020 2066 6f72 2067 6574 5f63 6f64       for get_cod
-000066f0: 652c 206c 616e 6720 696e 2073 656c 662e  e, lang in self.
-00006700: 6469 6374 2e69 7465 6d73 2829 3a0d 0a20  dict.items():.. 
-00006710: 2020 2020 2020 2020 2020 2069 6620 6c61             if la
-00006720: 6e67 2e6c 6f77 6572 2829 203d 3d20 6c61  ng.lower() == la
-00006730: 6e67 7561 6765 2e6c 6f77 6572 2829 3a0d  nguage.lower():.
-00006740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006750: 2072 6574 7572 6e20 6765 745f 636f 6465   return get_code
-00006760: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00006770: 2022 220d 0a0d 0a0d 0a63 6c61 7373 2047   ""......class G
-00006780: 6f6f 676c 654c 616e 6775 6167 653a 0d0a  oogleLanguage:..
-00006790: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-000067a0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-000067b0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-000067c0: 203d 205b 5d0d 0a20 2020 2020 2020 2073   = []..        s
-000067d0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-000067e0: 7070 656e 6428 2261 6622 290d 0a20 2020  ppend("af")..   
-000067f0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00006800: 6f64 6573 2e61 7070 656e 6428 2273 7122  odes.append("sq"
-00006810: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00006820: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00006830: 6428 2261 6d22 290d 0a20 2020 2020 2020  d("am")..       
-00006840: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00006850: 2e61 7070 656e 6428 2261 7222 290d 0a20  .append("ar").. 
-00006860: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00006870: 5f63 6f64 6573 2e61 7070 656e 6428 2268  _codes.append("h
-00006880: 7922 290d 0a20 2020 2020 2020 2073 656c  y")..        sel
-00006890: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-000068a0: 656e 6428 2261 7322 290d 0a20 2020 2020  end("as")..     
-000068b0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-000068c0: 6573 2e61 7070 656e 6428 2261 7922 290d  es.append("ay").
-000068d0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-000068e0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-000068f0: 2261 7a22 290d 0a20 2020 2020 2020 2073  "az")..        s
-00006900: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00006910: 7070 656e 6428 2262 6d22 290d 0a20 2020  ppend("bm")..   
-00006920: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00006930: 6f64 6573 2e61 7070 656e 6428 2265 7522  odes.append("eu"
-00006940: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00006950: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00006960: 6428 2262 6522 290d 0a20 2020 2020 2020  d("be")..       
-00006970: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00006980: 2e61 7070 656e 6428 2262 6e22 290d 0a20  .append("bn").. 
-00006990: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-000069a0: 5f63 6f64 6573 2e61 7070 656e 6428 2262  _codes.append("b
-000069b0: 686f 2229 0d0a 2020 2020 2020 2020 7365  ho")..        se
-000069c0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-000069d0: 7065 6e64 2822 6273 2229 0d0a 2020 2020  pend("bs")..    
-000069e0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-000069f0: 6465 732e 6170 7065 6e64 2822 6267 2229  des.append("bg")
-00006a00: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00006a10: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00006a20: 2822 6361 2229 0d0a 2020 2020 2020 2020  ("ca")..        
-00006a30: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-00006a40: 6170 7065 6e64 2822 6365 6222 290d 0a20  append("ceb").. 
-00006a50: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00006a60: 5f63 6f64 6573 2e61 7070 656e 6428 226e  _codes.append("n
-00006a70: 7922 290d 0a20 2020 2020 2020 2073 656c  y")..        sel
-00006a80: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00006a90: 656e 6428 227a 682d 434e 2229 0d0a 2020  end("zh-CN")..  
-00006aa0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00006ab0: 636f 6465 732e 6170 7065 6e64 2822 7a68  codes.append("zh
-00006ac0: 2d54 5722 290d 0a20 2020 2020 2020 2073  -TW")..        s
-00006ad0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00006ae0: 7070 656e 6428 2263 6f22 290d 0a20 2020  ppend("co")..   
-00006af0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00006b00: 6f64 6573 2e61 7070 656e 6428 2268 7222  odes.append("hr"
-00006b10: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00006b20: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00006b30: 6428 2263 7322 290d 0a20 2020 2020 2020  d("cs")..       
-00006b40: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00006b50: 2e61 7070 656e 6428 2264 6122 290d 0a20  .append("da").. 
-00006b60: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00006b70: 5f63 6f64 6573 2e61 7070 656e 6428 2264  _codes.append("d
-00006b80: 7622 290d 0a20 2020 2020 2020 2073 656c  v")..        sel
-00006b90: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00006ba0: 656e 6428 2264 6f69 2229 0d0a 2020 2020  end("doi")..    
-00006bb0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-00006bc0: 6465 732e 6170 7065 6e64 2822 6e6c 2229  des.append("nl")
-00006bd0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00006be0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00006bf0: 2822 656e 2229 0d0a 2020 2020 2020 2020  ("en")..        
-00006c00: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-00006c10: 6170 7065 6e64 2822 656f 2229 0d0a 2020  append("eo")..  
-00006c20: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00006c30: 636f 6465 732e 6170 7065 6e64 2822 6574  codes.append("et
-00006c40: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00006c50: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00006c60: 6e64 2822 6565 2229 0d0a 2020 2020 2020  nd("ee")..      
-00006c70: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00006c80: 732e 6170 7065 6e64 2822 6669 6c22 290d  s.append("fil").
-00006c90: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00006ca0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00006cb0: 2266 6922 290d 0a20 2020 2020 2020 2073  "fi")..        s
-00006cc0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00006cd0: 7070 656e 6428 2266 7222 290d 0a20 2020  ppend("fr")..   
-00006ce0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00006cf0: 6f64 6573 2e61 7070 656e 6428 2266 7922  odes.append("fy"
-00006d00: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00006d10: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00006d20: 6428 2267 6c22 290d 0a20 2020 2020 2020  d("gl")..       
-00006d30: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00006d40: 2e61 7070 656e 6428 226b 6122 290d 0a20  .append("ka").. 
-00006d50: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00006d60: 5f63 6f64 6573 2e61 7070 656e 6428 2264  _codes.append("d
-00006d70: 6522 290d 0a20 2020 2020 2020 2073 656c  e")..        sel
-00006d80: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00006d90: 656e 6428 2265 6c22 290d 0a20 2020 2020  end("el")..     
-00006da0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00006db0: 6573 2e61 7070 656e 6428 2267 6e22 290d  es.append("gn").
-00006dc0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00006dd0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00006de0: 2267 7522 290d 0a20 2020 2020 2020 2073  "gu")..        s
-00006df0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00006e00: 7070 656e 6428 2268 7422 290d 0a20 2020  ppend("ht")..   
-00006e10: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00006e20: 6f64 6573 2e61 7070 656e 6428 2268 6122  odes.append("ha"
-00006e30: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00006e40: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00006e50: 6428 2268 6177 2229 0d0a 2020 2020 2020  d("haw")..      
-00006e60: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00006e70: 732e 6170 7065 6e64 2822 6865 2229 0d0a  s.append("he")..
-00006e80: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00006e90: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00006ea0: 6869 2229 0d0a 2020 2020 2020 2020 7365  hi")..        se
-00006eb0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00006ec0: 7065 6e64 2822 686d 6e22 290d 0a20 2020  pend("hmn")..   
-00006ed0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00006ee0: 6f64 6573 2e61 7070 656e 6428 2268 7522  odes.append("hu"
-00006ef0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00006f00: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00006f10: 6428 2269 7322 290d 0a20 2020 2020 2020  d("is")..       
-00006f20: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00006f30: 2e61 7070 656e 6428 2269 6722 290d 0a20  .append("ig").. 
-00006f40: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00006f50: 5f63 6f64 6573 2e61 7070 656e 6428 2269  _codes.append("i
-00006f60: 6c6f 2229 0d0a 2020 2020 2020 2020 7365  lo")..        se
-00006f70: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00006f80: 7065 6e64 2822 6964 2229 0d0a 2020 2020  pend("id")..    
-00006f90: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-00006fa0: 6465 732e 6170 7065 6e64 2822 6761 2229  des.append("ga")
-00006fb0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00006fc0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00006fd0: 2822 6974 2229 0d0a 2020 2020 2020 2020  ("it")..        
-00006fe0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-00006ff0: 6170 7065 6e64 2822 6a61 2229 0d0a 2020  append("ja")..  
-00007000: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00007010: 636f 6465 732e 6170 7065 6e64 2822 6a76  codes.append("jv
-00007020: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00007030: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00007040: 6e64 2822 6b6e 2229 0d0a 2020 2020 2020  nd("kn")..      
-00007050: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00007060: 732e 6170 7065 6e64 2822 6b6b 2229 0d0a  s.append("kk")..
-00007070: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00007080: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00007090: 6b6d 2229 0d0a 2020 2020 2020 2020 7365  km")..        se
-000070a0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-000070b0: 7065 6e64 2822 7277 2229 0d0a 2020 2020  pend("rw")..    
-000070c0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-000070d0: 6465 732e 6170 7065 6e64 2822 676f 6d22  des.append("gom"
-000070e0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000070f0: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00007100: 6428 226b 6f22 290d 0a20 2020 2020 2020  d("ko")..       
-00007110: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00007120: 2e61 7070 656e 6428 226b 7269 2229 0d0a  .append("kri")..
-00007130: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00007140: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00007150: 6b6d 7222 290d 0a20 2020 2020 2020 2073  kmr")..        s
-00007160: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00007170: 7070 656e 6428 2263 6b62 2229 0d0a 2020  ppend("ckb")..  
-00007180: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00007190: 636f 6465 732e 6170 7065 6e64 2822 6b79  codes.append("ky
-000071a0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-000071b0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-000071c0: 6e64 2822 6c6f 2229 0d0a 2020 2020 2020  nd("lo")..      
-000071d0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-000071e0: 732e 6170 7065 6e64 2822 6c61 2229 0d0a  s.append("la")..
-000071f0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00007200: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00007210: 6c76 2229 0d0a 2020 2020 2020 2020 7365  lv")..        se
-00007220: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00007230: 7065 6e64 2822 6c6e 2229 0d0a 2020 2020  pend("ln")..    
-00007240: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-00007250: 6465 732e 6170 7065 6e64 2822 6c74 2229  des.append("lt")
-00007260: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00007270: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00007280: 2822 6c67 2229 0d0a 2020 2020 2020 2020  ("lg")..        
-00007290: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-000072a0: 6170 7065 6e64 2822 6c62 2229 0d0a 2020  append("lb")..  
-000072b0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-000072c0: 636f 6465 732e 6170 7065 6e64 2822 6d6b  codes.append("mk
-000072d0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-000072e0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-000072f0: 6e64 2822 6d67 2229 0d0a 2020 2020 2020  nd("mg")..      
-00007300: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00007310: 732e 6170 7065 6e64 2822 6d73 2229 0d0a  s.append("ms")..
-00007320: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00007330: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00007340: 6d6c 2229 0d0a 2020 2020 2020 2020 7365  ml")..        se
-00007350: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00007360: 7065 6e64 2822 6d74 2229 0d0a 2020 2020  pend("mt")..    
-00007370: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-00007380: 6465 732e 6170 7065 6e64 2822 6d69 2229  des.append("mi")
-00007390: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-000073a0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-000073b0: 2822 6d72 2229 0d0a 2020 2020 2020 2020  ("mr")..        
-000073c0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-000073d0: 6170 7065 6e64 2822 6d6e 692d 4d74 6569  append("mni-Mtei
-000073e0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-000073f0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00007400: 6e64 2822 6c75 7322 290d 0a20 2020 2020  nd("lus")..     
-00007410: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00007420: 6573 2e61 7070 656e 6428 226d 6e22 290d  es.append("mn").
-00007430: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00007440: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00007450: 226d 7922 290d 0a20 2020 2020 2020 2073  "my")..        s
-00007460: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00007470: 7070 656e 6428 226e 6522 290d 0a20 2020  ppend("ne")..   
-00007480: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00007490: 6f64 6573 2e61 7070 656e 6428 226e 6f22  odes.append("no"
-000074a0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000074b0: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-000074c0: 6428 226f 7222 290d 0a20 2020 2020 2020  d("or")..       
-000074d0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-000074e0: 2e61 7070 656e 6428 226f 6d22 290d 0a20  .append("om").. 
-000074f0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00007500: 5f63 6f64 6573 2e61 7070 656e 6428 2270  _codes.append("p
-00007510: 7322 290d 0a20 2020 2020 2020 2073 656c  s")..        sel
-00007520: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00007530: 656e 6428 2266 6122 290d 0a20 2020 2020  end("fa")..     
-00007540: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00007550: 6573 2e61 7070 656e 6428 2270 6c22 290d  es.append("pl").
-00007560: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00007570: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00007580: 2270 7422 290d 0a20 2020 2020 2020 2073  "pt")..        s
-00007590: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-000075a0: 7070 656e 6428 2270 6122 290d 0a20 2020  ppend("pa")..   
-000075b0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-000075c0: 6f64 6573 2e61 7070 656e 6428 2271 7522  odes.append("qu"
-000075d0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000075e0: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-000075f0: 6428 2272 6f22 290d 0a20 2020 2020 2020  d("ro")..       
-00007600: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00007610: 2e61 7070 656e 6428 2272 7522 290d 0a20  .append("ru").. 
-00007620: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00007630: 5f63 6f64 6573 2e61 7070 656e 6428 2273  _codes.append("s
-00007640: 6d22 290d 0a20 2020 2020 2020 2073 656c  m")..        sel
-00007650: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00007660: 656e 6428 2273 6122 290d 0a20 2020 2020  end("sa")..     
-00007670: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00007680: 6573 2e61 7070 656e 6428 2267 6422 290d  es.append("gd").
-00007690: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-000076a0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-000076b0: 226e 736f 2229 0d0a 2020 2020 2020 2020  "nso")..        
-000076c0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-000076d0: 6170 7065 6e64 2822 7372 2229 0d0a 2020  append("sr")..  
-000076e0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-000076f0: 636f 6465 732e 6170 7065 6e64 2822 7374  codes.append("st
-00007700: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00007710: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00007720: 6e64 2822 736e 2229 0d0a 2020 2020 2020  nd("sn")..      
-00007730: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00007740: 732e 6170 7065 6e64 2822 7364 2229 0d0a  s.append("sd")..
-00007750: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00007760: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00007770: 7369 2229 0d0a 2020 2020 2020 2020 7365  si")..        se
-00007780: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00007790: 7065 6e64 2822 736b 2229 0d0a 2020 2020  pend("sk")..    
-000077a0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-000077b0: 6465 732e 6170 7065 6e64 2822 736c 2229  des.append("sl")
-000077c0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-000077d0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-000077e0: 2822 736f 2229 0d0a 2020 2020 2020 2020  ("so")..        
-000077f0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-00007800: 6170 7065 6e64 2822 6573 2229 0d0a 2020  append("es")..  
-00007810: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00007820: 636f 6465 732e 6170 7065 6e64 2822 7375  codes.append("su
-00007830: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00007840: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00007850: 6e64 2822 7377 2229 0d0a 2020 2020 2020  nd("sw")..      
-00007860: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00007870: 732e 6170 7065 6e64 2822 7376 2229 0d0a  s.append("sv")..
-00007880: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00007890: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-000078a0: 7467 2229 0d0a 2020 2020 2020 2020 7365  tg")..        se
-000078b0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-000078c0: 7065 6e64 2822 7461 2229 0d0a 2020 2020  pend("ta")..    
-000078d0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-000078e0: 6465 732e 6170 7065 6e64 2822 7474 2229  des.append("tt")
-000078f0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00007900: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00007910: 2822 7465 2229 0d0a 2020 2020 2020 2020  ("te")..        
-00007920: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-00007930: 6170 7065 6e64 2822 7468 2229 0d0a 2020  append("th")..  
-00007940: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00007950: 636f 6465 732e 6170 7065 6e64 2822 7469  codes.append("ti
-00007960: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00007970: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00007980: 6e64 2822 7473 2229 0d0a 2020 2020 2020  nd("ts")..      
-00007990: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-000079a0: 732e 6170 7065 6e64 2822 7472 2229 0d0a  s.append("tr")..
-000079b0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-000079c0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-000079d0: 746b 2229 0d0a 2020 2020 2020 2020 7365  tk")..        se
-000079e0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-000079f0: 7065 6e64 2822 7477 2229 0d0a 2020 2020  pend("tw")..    
-00007a00: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-00007a10: 6465 732e 6170 7065 6e64 2822 756b 2229  des.append("uk")
-00007a20: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00007a30: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00007a40: 2822 7572 2229 0d0a 2020 2020 2020 2020  ("ur")..        
-00007a50: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-00007a60: 6170 7065 6e64 2822 7567 2229 0d0a 2020  append("ug")..  
-00007a70: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00007a80: 636f 6465 732e 6170 7065 6e64 2822 757a  codes.append("uz
-00007a90: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00007aa0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00007ab0: 6e64 2822 7669 2229 0d0a 2020 2020 2020  nd("vi")..      
-00007ac0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00007ad0: 732e 6170 7065 6e64 2822 6379 2229 0d0a  s.append("cy")..
-00007ae0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00007af0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00007b00: 7868 2229 0d0a 2020 2020 2020 2020 7365  xh")..        se
-00007b10: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00007b20: 7065 6e64 2822 7969 2229 0d0a 2020 2020  pend("yi")..    
-00007b30: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-00007b40: 6465 732e 6170 7065 6e64 2822 796f 2229  des.append("yo")
-00007b50: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00007b60: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00007b70: 2822 7a75 2229 0d0a 0d0a 2020 2020 2020  ("zu")....      
-00007b80: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00007b90: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-00007ba0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00007bb0: 6170 7065 6e64 2822 4166 7269 6b61 616e  append("Afrikaan
-00007bc0: 7322 290d 0a20 2020 2020 2020 2073 656c  s")..        sel
-00007bd0: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00007be0: 656e 6428 2241 6c62 616e 6961 6e22 290d  end("Albanian").
-00007bf0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00007c00: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00007c10: 2241 6d68 6172 6963 2229 0d0a 2020 2020  "Amharic")..    
-00007c20: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00007c30: 6d65 732e 6170 7065 6e64 2822 4172 6162  mes.append("Arab
-00007c40: 6963 2229 0d0a 2020 2020 2020 2020 7365  ic")..        se
-00007c50: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00007c60: 7065 6e64 2822 4172 6d65 6e69 616e 2229  pend("Armenian")
-00007c70: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00007c80: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00007c90: 2822 4173 7361 6d65 7365 2229 0d0a 2020  ("Assamese")..  
-00007ca0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00007cb0: 6e61 6d65 732e 6170 7065 6e64 2822 4179  names.append("Ay
-00007cc0: 6d61 7261 2229 0d0a 2020 2020 2020 2020  mara")..        
-00007cd0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00007ce0: 6170 7065 6e64 2822 417a 6572 6261 696a  append("Azerbaij
-00007cf0: 616e 6922 290d 0a20 2020 2020 2020 2073  ani")..        s
-00007d00: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00007d10: 7070 656e 6428 2242 616d 6261 7261 2229  ppend("Bambara")
-00007d20: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00007d30: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00007d40: 2822 4261 7371 7565 2229 0d0a 2020 2020  ("Basque")..    
-00007d50: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00007d60: 6d65 732e 6170 7065 6e64 2822 4265 6c61  mes.append("Bela
-00007d70: 7275 7369 616e 2229 0d0a 2020 2020 2020  rusian")..      
-00007d80: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00007d90: 732e 6170 7065 6e64 2822 4265 6e67 616c  s.append("Bengal
-00007da0: 6922 290d 0a20 2020 2020 2020 2073 656c  i")..        sel
-00007db0: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00007dc0: 656e 6428 2242 686f 6a70 7572 6922 290d  end("Bhojpuri").
-00007dd0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00007de0: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00007df0: 2242 6f73 6e69 616e 2229 0d0a 2020 2020  "Bosnian")..    
-00007e00: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00007e10: 6d65 732e 6170 7065 6e64 2822 4275 6c67  mes.append("Bulg
-00007e20: 6172 6961 6e22 290d 0a20 2020 2020 2020  arian")..       
-00007e30: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00007e40: 2e61 7070 656e 6428 2243 6174 616c 616e  .append("Catalan
-00007e50: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00007e60: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00007e70: 6e64 2822 4365 6275 616e 6f22 290d 0a20  nd("Cebuano").. 
-00007e80: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00007e90: 5f6e 616d 6573 2e61 7070 656e 6428 2243  _names.append("C
-00007ea0: 6869 6368 6577 6122 290d 0a20 2020 2020  hichewa")..     
-00007eb0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00007ec0: 6573 2e61 7070 656e 6428 2243 6869 6e65  es.append("Chine
-00007ed0: 7365 2028 5369 6d70 6c69 6669 6564 2922  se (Simplified)"
-00007ee0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00007ef0: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00007f00: 6428 2243 6869 6e65 7365 2028 5472 6164  d("Chinese (Trad
-00007f10: 6974 696f 6e61 6c29 2229 0d0a 2020 2020  itional)")..    
-00007f20: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00007f30: 6d65 732e 6170 7065 6e64 2822 436f 7273  mes.append("Cors
-00007f40: 6963 616e 2229 0d0a 2020 2020 2020 2020  ican")..        
-00007f50: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00007f60: 6170 7065 6e64 2822 4372 6f61 7469 616e  append("Croatian
-00007f70: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00007f80: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00007f90: 6e64 2822 437a 6563 6822 290d 0a20 2020  nd("Czech")..   
-00007fa0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00007fb0: 616d 6573 2e61 7070 656e 6428 2244 616e  ames.append("Dan
-00007fc0: 6973 6822 290d 0a20 2020 2020 2020 2073  ish")..        s
-00007fd0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00007fe0: 7070 656e 6428 2244 6869 7665 6869 2229  ppend("Dhivehi")
-00007ff0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00008000: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00008010: 2822 446f 6772 6922 290d 0a20 2020 2020  ("Dogri")..     
-00008020: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00008030: 6573 2e61 7070 656e 6428 2244 7574 6368  es.append("Dutch
-00008040: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00008050: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00008060: 6e64 2822 456e 676c 6973 6822 290d 0a20  nd("English").. 
-00008070: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00008080: 5f6e 616d 6573 2e61 7070 656e 6428 2245  _names.append("E
-00008090: 7370 6572 616e 746f 2229 0d0a 2020 2020  speranto")..    
-000080a0: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-000080b0: 6d65 732e 6170 7065 6e64 2822 4573 746f  mes.append("Esto
-000080c0: 6e69 616e 2229 0d0a 2020 2020 2020 2020  nian")..        
-000080d0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-000080e0: 6170 7065 6e64 2822 4577 6522 290d 0a20  append("Ewe").. 
-000080f0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00008100: 5f6e 616d 6573 2e61 7070 656e 6428 2246  _names.append("F
-00008110: 696c 6970 696e 6f22 290d 0a20 2020 2020  ilipino")..     
-00008120: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00008130: 6573 2e61 7070 656e 6428 2246 696e 6e69  es.append("Finni
-00008140: 7368 2229 0d0a 2020 2020 2020 2020 7365  sh")..        se
-00008150: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00008160: 7065 6e64 2822 4672 656e 6368 2229 0d0a  pend("French")..
-00008170: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00008180: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-00008190: 4672 6973 6961 6e22 290d 0a20 2020 2020  Frisian")..     
-000081a0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-000081b0: 6573 2e61 7070 656e 6428 2247 616c 6963  es.append("Galic
-000081c0: 6961 6e22 290d 0a20 2020 2020 2020 2073  ian")..        s
-000081d0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-000081e0: 7070 656e 6428 2247 656f 7267 6961 6e22  ppend("Georgian"
-000081f0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00008200: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00008210: 6428 2247 6572 6d61 6e22 290d 0a20 2020  d("German")..   
-00008220: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00008230: 616d 6573 2e61 7070 656e 6428 2247 7265  ames.append("Gre
-00008240: 656b 2229 0d0a 2020 2020 2020 2020 7365  ek")..        se
-00008250: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00008260: 7065 6e64 2822 4775 6172 616e 6922 290d  pend("Guarani").
-00008270: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00008280: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00008290: 2247 756a 6172 6174 6922 290d 0a20 2020  "Gujarati")..   
-000082a0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-000082b0: 616d 6573 2e61 7070 656e 6428 2248 6169  ames.append("Hai
-000082c0: 7469 616e 2043 7265 6f6c 6522 290d 0a20  tian Creole").. 
-000082d0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-000082e0: 5f6e 616d 6573 2e61 7070 656e 6428 2248  _names.append("H
-000082f0: 6175 7361 2229 0d0a 2020 2020 2020 2020  ausa")..        
-00008300: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00008310: 6170 7065 6e64 2822 4861 7761 6969 616e  append("Hawaiian
-00008320: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00008330: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00008340: 6e64 2822 4865 6272 6577 2229 0d0a 2020  nd("Hebrew")..  
-00008350: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00008360: 6e61 6d65 732e 6170 7065 6e64 2822 4869  names.append("Hi
-00008370: 6e64 6922 290d 0a20 2020 2020 2020 2073  ndi")..        s
-00008380: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00008390: 7070 656e 6428 2248 6d6f 6e67 2229 0d0a  ppend("Hmong")..
-000083a0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-000083b0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-000083c0: 4875 6e67 6172 6961 6e22 290d 0a20 2020  Hungarian")..   
-000083d0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-000083e0: 616d 6573 2e61 7070 656e 6428 2249 6365  ames.append("Ice
-000083f0: 6c61 6e64 6963 2229 0d0a 2020 2020 2020  landic")..      
-00008400: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00008410: 732e 6170 7065 6e64 2822 4967 626f 2229  s.append("Igbo")
-00008420: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00008430: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00008440: 2822 496c 6f63 616e 6f22 290d 0a20 2020  ("Ilocano")..   
-00008450: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00008460: 616d 6573 2e61 7070 656e 6428 2249 6e64  ames.append("Ind
-00008470: 6f6e 6573 6961 6e22 290d 0a20 2020 2020  onesian")..     
-00008480: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00008490: 6573 2e61 7070 656e 6428 2249 7269 7368  es.append("Irish
-000084a0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-000084b0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-000084c0: 6e64 2822 4974 616c 6961 6e22 290d 0a20  nd("Italian").. 
-000084d0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-000084e0: 5f6e 616d 6573 2e61 7070 656e 6428 224a  _names.append("J
-000084f0: 6170 616e 6573 6522 290d 0a20 2020 2020  apanese")..     
-00008500: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00008510: 6573 2e61 7070 656e 6428 224a 6176 616e  es.append("Javan
-00008520: 6573 6522 290d 0a20 2020 2020 2020 2073  ese")..        s
-00008530: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00008540: 7070 656e 6428 224b 616e 6e61 6461 2229  ppend("Kannada")
-00008550: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00008560: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00008570: 2822 4b61 7a61 6b68 2229 0d0a 2020 2020  ("Kazakh")..    
-00008580: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00008590: 6d65 732e 6170 7065 6e64 2822 4b68 6d65  mes.append("Khme
-000085a0: 7222 290d 0a20 2020 2020 2020 2073 656c  r")..        sel
-000085b0: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-000085c0: 656e 6428 224b 696e 7961 7277 616e 6461  end("Kinyarwanda
-000085d0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-000085e0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-000085f0: 6e64 2822 4b6f 6e6b 616e 6922 290d 0a20  nd("Konkani").. 
-00008600: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00008610: 5f6e 616d 6573 2e61 7070 656e 6428 224b  _names.append("K
-00008620: 6f72 6561 6e22 290d 0a20 2020 2020 2020  orean")..       
-00008630: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00008640: 2e61 7070 656e 6428 224b 7269 6f22 290d  .append("Krio").
-00008650: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00008660: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00008670: 224b 7572 6469 7368 2028 4b75 726d 616e  "Kurdish (Kurman
-00008680: 6a69 2922 290d 0a20 2020 2020 2020 2073  ji)")..        s
-00008690: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-000086a0: 7070 656e 6428 224b 7572 6469 7368 2028  ppend("Kurdish (
-000086b0: 536f 7261 6e69 2922 290d 0a20 2020 2020  Sorani)")..     
-000086c0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-000086d0: 6573 2e61 7070 656e 6428 224b 7972 6779  es.append("Kyrgy
-000086e0: 7a22 290d 0a20 2020 2020 2020 2073 656c  z")..        sel
-000086f0: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00008700: 656e 6428 224c 616f 2229 0d0a 2020 2020  end("Lao")..    
-00008710: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00008720: 6d65 732e 6170 7065 6e64 2822 4c61 7469  mes.append("Lati
-00008730: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
-00008740: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00008750: 656e 6428 224c 6174 7669 616e 2229 0d0a  end("Latvian")..
-00008760: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00008770: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-00008780: 4c69 6e67 616c 6122 290d 0a20 2020 2020  Lingala")..     
-00008790: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-000087a0: 6573 2e61 7070 656e 6428 224c 6974 6875  es.append("Lithu
-000087b0: 616e 6961 6e22 290d 0a20 2020 2020 2020  anian")..       
-000087c0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-000087d0: 2e61 7070 656e 6428 224c 7567 616e 6461  .append("Luganda
-000087e0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-000087f0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00008800: 6e64 2822 4c75 7865 6d62 6f75 7267 6973  nd("Luxembourgis
-00008810: 6822 290d 0a20 2020 2020 2020 2073 656c  h")..        sel
-00008820: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00008830: 656e 6428 224d 6163 6564 6f6e 6961 6e22  end("Macedonian"
-00008840: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00008850: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00008860: 6428 224d 616c 6167 6173 7922 290d 0a20  d("Malagasy").. 
-00008870: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00008880: 5f6e 616d 6573 2e61 7070 656e 6428 224d  _names.append("M
-00008890: 616c 6179 2229 0d0a 2020 2020 2020 2020  alay")..        
-000088a0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-000088b0: 6170 7065 6e64 2822 4d61 6c61 7961 6c61  append("Malayala
-000088c0: 6d22 290d 0a20 2020 2020 2020 2073 656c  m")..        sel
-000088d0: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-000088e0: 656e 6428 224d 616c 7465 7365 2229 0d0a  end("Maltese")..
-000088f0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00008900: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-00008910: 4d61 6f72 6922 290d 0a20 2020 2020 2020  Maori")..       
-00008920: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00008930: 2e61 7070 656e 6428 224d 6172 6174 6869  .append("Marathi
-00008940: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00008950: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00008960: 6e64 2822 4d65 6974 6569 6c6f 6e20 284d  nd("Meiteilon (M
-00008970: 616e 6970 7572 6929 2229 0d0a 2020 2020  anipuri)")..    
-00008980: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00008990: 6d65 732e 6170 7065 6e64 2822 4d69 7a6f  mes.append("Mizo
-000089a0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-000089b0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-000089c0: 6e64 2822 4d6f 6e67 6f6c 6961 6e22 290d  nd("Mongolian").
-000089d0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-000089e0: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-000089f0: 224d 7961 6e6d 6172 2028 4275 726d 6573  "Myanmar (Burmes
-00008a00: 6529 2229 0d0a 2020 2020 2020 2020 7365  e)")..        se
-00008a10: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00008a20: 7065 6e64 2822 4e65 7061 6c69 2229 0d0a  pend("Nepali")..
-00008a30: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00008a40: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-00008a50: 4e6f 7277 6567 6961 6e22 290d 0a20 2020  Norwegian")..   
-00008a60: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00008a70: 616d 6573 2e61 7070 656e 6428 224f 6469  ames.append("Odi
-00008a80: 7961 2028 4f72 6979 6129 2229 0d0a 2020  ya (Oriya)")..  
-00008a90: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00008aa0: 6e61 6d65 732e 6170 7065 6e64 2822 4f72  names.append("Or
-00008ab0: 6f6d 6f22 290d 0a20 2020 2020 2020 2073  omo")..        s
-00008ac0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00008ad0: 7070 656e 6428 2250 6173 6874 6f22 290d  ppend("Pashto").
-00008ae0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00008af0: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00008b00: 2250 6572 7369 616e 2229 0d0a 2020 2020  "Persian")..    
-00008b10: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00008b20: 6d65 732e 6170 7065 6e64 2822 506f 6c69  mes.append("Poli
-00008b30: 7368 2229 0d0a 2020 2020 2020 2020 7365  sh")..        se
-00008b40: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00008b50: 7065 6e64 2822 506f 7274 7567 7565 7365  pend("Portuguese
-00008b60: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00008b70: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00008b80: 6e64 2822 5075 6e6a 6162 6922 290d 0a20  nd("Punjabi").. 
-00008b90: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00008ba0: 5f6e 616d 6573 2e61 7070 656e 6428 2251  _names.append("Q
-00008bb0: 7565 6368 7561 2229 0d0a 2020 2020 2020  uechua")..      
-00008bc0: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00008bd0: 732e 6170 7065 6e64 2822 526f 6d61 6e69  s.append("Romani
-00008be0: 616e 2229 0d0a 2020 2020 2020 2020 7365  an")..        se
-00008bf0: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00008c00: 7065 6e64 2822 5275 7373 6961 6e22 290d  pend("Russian").
-00008c10: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00008c20: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00008c30: 2253 616d 6f61 6e22 290d 0a20 2020 2020  "Samoan")..     
-00008c40: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00008c50: 6573 2e61 7070 656e 6428 2253 616e 736b  es.append("Sansk
-00008c60: 7269 7422 290d 0a20 2020 2020 2020 2073  rit")..        s
-00008c70: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00008c80: 7070 656e 6428 2253 636f 7473 2047 6165  ppend("Scots Gae
-00008c90: 6c69 6322 290d 0a20 2020 2020 2020 2073  lic")..        s
-00008ca0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00008cb0: 7070 656e 6428 2253 6570 6564 6922 290d  ppend("Sepedi").
-00008cc0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00008cd0: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00008ce0: 2253 6572 6269 616e 2229 0d0a 2020 2020  "Serbian")..    
-00008cf0: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00008d00: 6d65 732e 6170 7065 6e64 2822 5365 736f  mes.append("Seso
-00008d10: 7468 6f22 290d 0a20 2020 2020 2020 2073  tho")..        s
-00008d20: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00008d30: 7070 656e 6428 2253 686f 6e61 2229 0d0a  ppend("Shona")..
-00008d40: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00008d50: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-00008d60: 5369 6e64 6869 2229 0d0a 2020 2020 2020  Sindhi")..      
-00008d70: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00008d80: 732e 6170 7065 6e64 2822 5369 6e68 616c  s.append("Sinhal
-00008d90: 6122 290d 0a20 2020 2020 2020 2073 656c  a")..        sel
-00008da0: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00008db0: 656e 6428 2253 6c6f 7661 6b22 290d 0a20  end("Slovak").. 
-00008dc0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00008dd0: 5f6e 616d 6573 2e61 7070 656e 6428 2253  _names.append("S
-00008de0: 6c6f 7665 6e69 616e 2229 0d0a 2020 2020  lovenian")..    
-00008df0: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00008e00: 6d65 732e 6170 7065 6e64 2822 536f 6d61  mes.append("Soma
-00008e10: 6c69 2229 0d0a 2020 2020 2020 2020 7365  li")..        se
-00008e20: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00008e30: 7065 6e64 2822 5370 616e 6973 6822 290d  pend("Spanish").
-00008e40: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00008e50: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00008e60: 2253 756e 6461 6e65 7365 2229 0d0a 2020  "Sundanese")..  
-00008e70: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00008e80: 6e61 6d65 732e 6170 7065 6e64 2822 5377  names.append("Sw
-00008e90: 6168 696c 6922 290d 0a20 2020 2020 2020  ahili")..       
-00008ea0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00008eb0: 2e61 7070 656e 6428 2253 7765 6469 7368  .append("Swedish
-00008ec0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00008ed0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00008ee0: 6e64 2822 5461 6a69 6b22 290d 0a20 2020  nd("Tajik")..   
-00008ef0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00008f00: 616d 6573 2e61 7070 656e 6428 2254 616d  ames.append("Tam
-00008f10: 696c 2229 0d0a 2020 2020 2020 2020 7365  il")..        se
-00008f20: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00008f30: 7065 6e64 2822 5461 7461 7222 290d 0a20  pend("Tatar").. 
-00008f40: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00008f50: 5f6e 616d 6573 2e61 7070 656e 6428 2254  _names.append("T
-00008f60: 656c 7567 7522 290d 0a20 2020 2020 2020  elugu")..       
-00008f70: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00008f80: 2e61 7070 656e 6428 2254 6861 6922 290d  .append("Thai").
-00008f90: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00008fa0: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00008fb0: 2254 6967 7269 6e79 6122 290d 0a20 2020  "Tigrinya")..   
-00008fc0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00008fd0: 616d 6573 2e61 7070 656e 6428 2254 736f  ames.append("Tso
-00008fe0: 6e67 6122 290d 0a20 2020 2020 2020 2073  nga")..        s
-00008ff0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00009000: 7070 656e 6428 2254 7572 6b69 7368 2229  ppend("Turkish")
-00009010: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00009020: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00009030: 2822 5475 726b 6d65 6e22 290d 0a20 2020  ("Turkmen")..   
-00009040: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00009050: 616d 6573 2e61 7070 656e 6428 2254 7769  ames.append("Twi
-00009060: 2028 416b 616e 2922 290d 0a20 2020 2020   (Akan)")..     
-00009070: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00009080: 6573 2e61 7070 656e 6428 2255 6b72 6169  es.append("Ukrai
-00009090: 6e69 616e 2229 0d0a 2020 2020 2020 2020  nian")..        
-000090a0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-000090b0: 6170 7065 6e64 2822 5572 6475 2229 0d0a  append("Urdu")..
-000090c0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-000090d0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-000090e0: 5579 6768 7572 2229 0d0a 2020 2020 2020  Uyghur")..      
-000090f0: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00009100: 732e 6170 7065 6e64 2822 557a 6265 6b22  s.append("Uzbek"
-00009110: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00009120: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00009130: 6428 2256 6965 746e 616d 6573 6522 290d  d("Vietnamese").
-00009140: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00009150: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00009160: 2257 656c 7368 2229 0d0a 2020 2020 2020  "Welsh")..      
-00009170: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00009180: 732e 6170 7065 6e64 2822 5868 6f73 6122  s.append("Xhosa"
-00009190: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000091a0: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-000091b0: 6428 2259 6964 6469 7368 2229 0d0a 2020  d("Yiddish")..  
-000091c0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-000091d0: 6e61 6d65 732e 6170 7065 6e64 2822 596f  names.append("Yo
-000091e0: 7275 6261 2229 0d0a 2020 2020 2020 2020  ruba")..        
-000091f0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00009200: 6170 7065 6e64 2822 5a75 6c75 2229 0d0a  append("Zulu")..
-00009210: 0d0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
-00009220: 6f64 655f 6f66 5f6e 616d 6520 3d20 6469  ode_of_name = di
-00009230: 6374 287a 6970 2873 656c 662e 6c69 7374  ct(zip(self.list
-00009240: 5f6e 616d 6573 2c20 7365 6c66 2e6c 6973  _names, self.lis
-00009250: 745f 636f 6465 7329 290d 0a20 2020 2020  t_codes))..     
-00009260: 2020 2073 656c 662e 6e61 6d65 5f6f 665f     self.name_of_
-00009270: 636f 6465 203d 2064 6963 7428 7a69 7028  code = dict(zip(
-00009280: 7365 6c66 2e6c 6973 745f 636f 6465 732c  self.list_codes,
-00009290: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-000092a0: 2929 0d0a 0d0a 2020 2020 2020 2020 7365  ))....        se
-000092b0: 6c66 2e64 6963 7420 3d20 7b0d 0a20 2020  lf.dict = {..   
-000092c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092d0: 2020 2020 2027 6166 273a 2027 4166 7269       'af': 'Afri
-000092e0: 6b61 616e 7327 2c0d 0a20 2020 2020 2020  kaans',..       
-000092f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009300: 2027 7371 273a 2027 416c 6261 6e69 616e   'sq': 'Albanian
-00009310: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00009320: 2020 2020 2020 2020 2020 2020 2761 6d27              'am'
-00009330: 3a20 2741 6d68 6172 6963 272c 0d0a 2020  : 'Amharic',..  
-00009340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009350: 2020 2020 2020 2761 7227 3a20 2741 7261        'ar': 'Ara
-00009360: 6269 6327 2c0d 0a20 2020 2020 2020 2020  bic',..         
-00009370: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00009380: 6879 273a 2027 4172 6d65 6e69 616e 272c  hy': 'Armenian',
-00009390: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000093a0: 2020 2020 2020 2020 2020 2761 7327 3a20            'as': 
-000093b0: 2741 7373 616d 6573 6527 2c0d 0a20 2020  'Assamese',..   
-000093c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000093d0: 2020 2020 2027 6179 273a 2027 4179 6d61       'ay': 'Ayma
-000093e0: 7261 272c 0d0a 2020 2020 2020 2020 2020  ra',..          
-000093f0: 2020 2020 2020 2020 2020 2020 2020 2761                'a
-00009400: 7a27 3a20 2741 7a65 7262 6169 6a61 6e69  z': 'Azerbaijani
-00009410: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00009420: 2020 2020 2020 2020 2020 2020 2762 6d27              'bm'
-00009430: 3a20 2742 616d 6261 7261 272c 0d0a 2020  : 'Bambara',..  
-00009440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009450: 2020 2020 2020 2765 7527 3a20 2742 6173        'eu': 'Bas
-00009460: 7175 6527 2c0d 0a20 2020 2020 2020 2020  que',..         
-00009470: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00009480: 6265 273a 2027 4265 6c61 7275 7369 616e  be': 'Belarusian
-00009490: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-000094a0: 2020 2020 2020 2020 2020 2020 2762 6e27              'bn'
-000094b0: 3a20 2742 656e 6761 6c69 272c 0d0a 2020  : 'Bengali',..  
-000094c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094d0: 2020 2020 2020 2762 686f 273a 2027 4268        'bho': 'Bh
-000094e0: 6f6a 7075 7269 272c 0d0a 2020 2020 2020  ojpuri',..      
-000094f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009500: 2020 2762 7327 3a20 2742 6f73 6e69 616e    'bs': 'Bosnian
-00009510: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00009520: 2020 2020 2020 2020 2020 2020 2762 6727              'bg'
-00009530: 3a20 2742 756c 6761 7269 616e 272c 0d0a  : 'Bulgarian',..
-00009540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009550: 2020 2020 2020 2020 2763 6127 3a20 2743          'ca': 'C
-00009560: 6174 616c 616e 272c 0d0a 2020 2020 2020  atalan',..      
-00009570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009580: 2020 2763 6562 273a 2027 4365 6275 616e    'ceb': 'Cebuan
-00009590: 6f27 2c0d 0a20 2020 2020 2020 2020 2020  o',..           
-000095a0: 2020 2020 2020 2020 2020 2020 2027 6e79               'ny
-000095b0: 273a 2027 4368 6963 6865 7761 272c 0d0a  ': 'Chichewa',..
-000095c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095d0: 2020 2020 2020 2020 277a 682d 434e 273a          'zh-CN':
-000095e0: 2027 4368 696e 6573 6520 2853 696d 706c   'Chinese (Simpl
-000095f0: 6966 6965 6429 272c 0d0a 2020 2020 2020  ified)',..      
-00009600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009610: 2020 277a 682d 5457 273a 2027 4368 696e    'zh-TW': 'Chin
-00009620: 6573 6520 2854 7261 6469 7469 6f6e 616c  ese (Traditional
-00009630: 2927 2c0d 0a20 2020 2020 2020 2020 2020  )',..           
-00009640: 2020 2020 2020 2020 2020 2020 2027 636f               'co
-00009650: 273a 2027 436f 7273 6963 616e 272c 0d0a  ': 'Corsican',..
-00009660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009670: 2020 2020 2020 2020 2768 7227 3a20 2743          'hr': 'C
-00009680: 726f 6174 6961 6e27 2c0d 0a20 2020 2020  roatian',..     
-00009690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096a0: 2020 2027 6373 273a 2027 437a 6563 6827     'cs': 'Czech'
-000096b0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000096c0: 2020 2020 2020 2020 2020 2027 6461 273a             'da':
-000096d0: 2027 4461 6e69 7368 272c 0d0a 2020 2020   'Danish',..    
-000096e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096f0: 2020 2020 2764 7627 3a20 2744 6869 7665      'dv': 'Dhive
-00009700: 6869 272c 0d0a 2020 2020 2020 2020 2020  hi',..          
-00009710: 2020 2020 2020 2020 2020 2020 2020 2764                'd
-00009720: 6f69 273a 2027 446f 6772 6927 2c0d 0a20  oi': 'Dogri',.. 
-00009730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009740: 2020 2020 2020 2027 6e6c 273a 2027 4475         'nl': 'Du
-00009750: 7463 6827 2c0d 0a20 2020 2020 2020 2020  tch',..         
-00009760: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00009770: 656e 273a 2027 456e 676c 6973 6827 2c0d  en': 'English',.
-00009780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009790: 2020 2020 2020 2020 2027 656f 273a 2027           'eo': '
-000097a0: 4573 7065 7261 6e74 6f27 2c0d 0a20 2020  Esperanto',..   
-000097b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097c0: 2020 2020 2027 6574 273a 2027 4573 746f       'et': 'Esto
-000097d0: 6e69 616e 272c 0d0a 2020 2020 2020 2020  nian',..        
-000097e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097f0: 2765 6527 3a20 2745 7765 272c 0d0a 2020  'ee': 'Ewe',..  
-00009800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009810: 2020 2020 2020 2766 696c 273a 2027 4669        'fil': 'Fi
-00009820: 6c69 7069 6e6f 272c 0d0a 2020 2020 2020  lipino',..      
-00009830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009840: 2020 2766 6927 3a20 2746 696e 6e69 7368    'fi': 'Finnish
-00009850: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00009860: 2020 2020 2020 2020 2020 2020 2766 7227              'fr'
-00009870: 3a20 2746 7265 6e63 6827 2c0d 0a20 2020  : 'French',..   
-00009880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009890: 2020 2020 2027 6679 273a 2027 4672 6973       'fy': 'Fris
-000098a0: 6961 6e27 2c0d 0a20 2020 2020 2020 2020  ian',..         
-000098b0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000098c0: 676c 273a 2027 4761 6c69 6369 616e 272c  gl': 'Galician',
-000098d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000098e0: 2020 2020 2020 2020 2020 276b 6127 3a20            'ka': 
-000098f0: 2747 656f 7267 6961 6e27 2c0d 0a20 2020  'Georgian',..   
-00009900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009910: 2020 2020 2027 6465 273a 2027 4765 726d       'de': 'Germ
-00009920: 616e 272c 0d0a 2020 2020 2020 2020 2020  an',..          
-00009930: 2020 2020 2020 2020 2020 2020 2020 2765                'e
-00009940: 6c27 3a20 2747 7265 656b 272c 0d0a 2020  l': 'Greek',..  
-00009950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009960: 2020 2020 2020 2767 6e27 3a20 2747 7561        'gn': 'Gua
-00009970: 7261 6e69 272c 0d0a 2020 2020 2020 2020  rani',..        
-00009980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009990: 2767 7527 3a20 2747 756a 6172 6174 6927  'gu': 'Gujarati'
-000099a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000099b0: 2020 2020 2020 2020 2020 2027 6874 273a             'ht':
-000099c0: 2027 4861 6974 6961 6e20 4372 656f 6c65   'Haitian Creole
-000099d0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-000099e0: 2020 2020 2020 2020 2020 2020 2768 6127              'ha'
-000099f0: 3a20 2748 6175 7361 272c 0d0a 2020 2020  : 'Hausa',..    
-00009a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a10: 2020 2020 2768 6177 273a 2027 4861 7761      'haw': 'Hawa
-00009a20: 6969 616e 272c 0d0a 2020 2020 2020 2020  iian',..        
-00009a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a40: 2768 6527 3a20 2748 6562 7265 7727 2c0d  'he': 'Hebrew',.
-00009a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009a60: 2020 2020 2020 2020 2027 6869 273a 2027           'hi': '
-00009a70: 4869 6e64 6927 2c0d 0a20 2020 2020 2020  Hindi',..       
-00009a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a90: 2027 686d 6e27 3a20 2748 6d6f 6e67 272c   'hmn': 'Hmong',
-00009aa0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009ab0: 2020 2020 2020 2020 2020 2768 7527 3a20            'hu': 
-00009ac0: 2748 756e 6761 7269 616e 272c 0d0a 2020  'Hungarian',..  
-00009ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ae0: 2020 2020 2020 2769 7327 3a20 2749 6365        'is': 'Ice
-00009af0: 6c61 6e64 6963 272c 0d0a 2020 2020 2020  landic',..      
-00009b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b10: 2020 2769 6727 3a20 2749 6762 6f27 2c0d    'ig': 'Igbo',.
-00009b20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009b30: 2020 2020 2020 2020 2027 696c 6f27 3a20           'ilo': 
-00009b40: 2749 6c6f 6361 6e6f 272c 0d0a 2020 2020  'Ilocano',..    
-00009b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b60: 2020 2020 2769 6427 3a20 2749 6e64 6f6e      'id': 'Indon
-00009b70: 6573 6961 6e27 2c0d 0a20 2020 2020 2020  esian',..       
-00009b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b90: 2027 6761 273a 2027 4972 6973 6827 2c0d   'ga': 'Irish',.
-00009ba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009bb0: 2020 2020 2020 2020 2027 6974 273a 2027           'it': '
-00009bc0: 4974 616c 6961 6e27 2c0d 0a20 2020 2020  Italian',..     
-00009bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009be0: 2020 2027 6a61 273a 2027 4a61 7061 6e65     'ja': 'Japane
-00009bf0: 7365 272c 0d0a 2020 2020 2020 2020 2020  se',..          
-00009c00: 2020 2020 2020 2020 2020 2020 2020 276a                'j
-00009c10: 7627 3a20 274a 6176 616e 6573 6527 2c0d  v': 'Javanese',.
-00009c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009c30: 2020 2020 2020 2020 2027 6b6e 273a 2027           'kn': '
-00009c40: 4b61 6e6e 6164 6127 2c0d 0a20 2020 2020  Kannada',..     
-00009c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c60: 2020 2027 6b6b 273a 2027 4b61 7a61 6b68     'kk': 'Kazakh
-00009c70: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00009c80: 2020 2020 2020 2020 2020 2020 276b 6d27              'km'
-00009c90: 3a20 274b 686d 6572 272c 0d0a 2020 2020  : 'Khmer',..    
-00009ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009cb0: 2020 2020 2772 7727 3a20 274b 696e 7961      'rw': 'Kinya
-00009cc0: 7277 616e 6461 272c 0d0a 2020 2020 2020  rwanda',..      
-00009cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ce0: 2020 2767 6f6d 273a 2027 4b6f 6e6b 616e    'gom': 'Konkan
-00009cf0: 6927 2c0d 0a20 2020 2020 2020 2020 2020  i',..           
-00009d00: 2020 2020 2020 2020 2020 2020 2027 6b6f               'ko
-00009d10: 273a 2027 4b6f 7265 616e 272c 0d0a 2020  ': 'Korean',..  
-00009d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d30: 2020 2020 2020 276b 7269 273a 2027 4b72        'kri': 'Kr
-00009d40: 696f 272c 0d0a 2020 2020 2020 2020 2020  io',..          
-00009d50: 2020 2020 2020 2020 2020 2020 2020 276b                'k
-00009d60: 6d72 273a 2027 4b75 7264 6973 6820 284b  mr': 'Kurdish (K
-00009d70: 7572 6d61 6e6a 6929 272c 0d0a 2020 2020  urmanji)',..    
-00009d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d90: 2020 2020 2763 6b62 273a 2027 4b75 7264      'ckb': 'Kurd
-00009da0: 6973 6820 2853 6f72 616e 6929 272c 0d0a  ish (Sorani)',..
-00009db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009dc0: 2020 2020 2020 2020 276b 7927 3a20 274b          'ky': 'K
-00009dd0: 7972 6779 7a27 2c0d 0a20 2020 2020 2020  yrgyz',..       
-00009de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009df0: 2027 6c6f 273a 2027 4c61 6f27 2c0d 0a20   'lo': 'Lao',.. 
-00009e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e10: 2020 2020 2020 2027 6c61 273a 2027 4c61         'la': 'La
-00009e20: 7469 6e27 2c0d 0a20 2020 2020 2020 2020  tin',..         
-00009e30: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00009e40: 6c76 273a 2027 4c61 7476 6961 6e27 2c0d  lv': 'Latvian',.
-00009e50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009e60: 2020 2020 2020 2020 2027 6c6e 273a 2027           'ln': '
-00009e70: 4c69 6e67 616c 6127 2c0d 0a20 2020 2020  Lingala',..     
-00009e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e90: 2020 2027 6c74 273a 2027 4c69 7468 7561     'lt': 'Lithua
-00009ea0: 6e69 616e 272c 0d0a 2020 2020 2020 2020  nian',..        
-00009eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ec0: 276c 6727 3a20 274c 7567 616e 6461 272c  'lg': 'Luganda',
-00009ed0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009ee0: 2020 2020 2020 2020 2020 276c 6227 3a20            'lb': 
-00009ef0: 274c 7578 656d 626f 7572 6769 7368 272c  'Luxembourgish',
-00009f00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009f10: 2020 2020 2020 2020 2020 276d 6b27 3a20            'mk': 
-00009f20: 274d 6163 6564 6f6e 6961 6e27 2c0d 0a20  'Macedonian',.. 
-00009f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f40: 2020 2020 2020 2027 6d67 273a 2027 4d61         'mg': 'Ma
-00009f50: 6c61 6761 7379 272c 0d0a 2020 2020 2020  lagasy',..      
-00009f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f70: 2020 276d 7327 3a20 274d 616c 6179 272c    'ms': 'Malay',
-00009f80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009f90: 2020 2020 2020 2020 2020 276d 6c27 3a20            'ml': 
-00009fa0: 274d 616c 6179 616c 616d 272c 0d0a 2020  'Malayalam',..  
-00009fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009fc0: 2020 2020 2020 276d 7427 3a20 274d 616c        'mt': 'Mal
-00009fd0: 7465 7365 272c 0d0a 2020 2020 2020 2020  tese',..        
-00009fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ff0: 276d 6927 3a20 274d 616f 7269 272c 0d0a  'mi': 'Maori',..
-0000a000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a010: 2020 2020 2020 2020 276d 7227 3a20 274d          'mr': 'M
-0000a020: 6172 6174 6869 272c 0d0a 2020 2020 2020  arathi',..      
-0000a030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a040: 2020 276d 6e69 2d4d 7465 6927 3a20 274d    'mni-Mtei': 'M
-0000a050: 6569 7465 696c 6f6e 2028 4d61 6e69 7075  eiteilon (Manipu
-0000a060: 7269 2927 2c0d 0a20 2020 2020 2020 2020  ri)',..         
-0000a070: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000a080: 6c75 7327 3a20 274d 697a 6f27 2c0d 0a20  lus': 'Mizo',.. 
-0000a090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0a0: 2020 2020 2020 2027 6d6e 273a 2027 4d6f         'mn': 'Mo
-0000a0b0: 6e67 6f6c 6961 6e27 2c0d 0a20 2020 2020  ngolian',..     
-0000a0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0d0: 2020 2027 6d79 273a 2027 4d79 616e 6d61     'my': 'Myanma
-0000a0e0: 7220 2842 7572 6d65 7365 2927 2c0d 0a20  r (Burmese)',.. 
-0000a0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a100: 2020 2020 2020 2027 6e65 273a 2027 4e65         'ne': 'Ne
-0000a110: 7061 6c69 272c 0d0a 2020 2020 2020 2020  pali',..        
-0000a120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a130: 276e 6f27 3a20 274e 6f72 7765 6769 616e  'no': 'Norwegian
-0000a140: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-0000a150: 2020 2020 2020 2020 2020 2020 276f 7227              'or'
-0000a160: 3a20 274f 6469 7961 2028 4f72 6979 6129  : 'Odiya (Oriya)
-0000a170: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-0000a180: 2020 2020 2020 2020 2020 2020 276f 6d27              'om'
-0000a190: 3a20 274f 726f 6d6f 272c 0d0a 2020 2020  : 'Oromo',..    
-0000a1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1b0: 2020 2020 2770 7327 3a20 2750 6173 6874      'ps': 'Pasht
-0000a1c0: 6f27 2c0d 0a20 2020 2020 2020 2020 2020  o',..           
-0000a1d0: 2020 2020 2020 2020 2020 2020 2027 6661               'fa
-0000a1e0: 273a 2027 5065 7273 6961 6e27 2c0d 0a20  ': 'Persian',.. 
-0000a1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a200: 2020 2020 2020 2027 706c 273a 2027 506f         'pl': 'Po
-0000a210: 6c69 7368 272c 0d0a 2020 2020 2020 2020  lish',..        
-0000a220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a230: 2770 7427 3a20 2750 6f72 7475 6775 6573  'pt': 'Portugues
-0000a240: 6527 2c0d 0a20 2020 2020 2020 2020 2020  e',..           
-0000a250: 2020 2020 2020 2020 2020 2020 2027 7061               'pa
-0000a260: 273a 2027 5075 6e6a 6162 6927 2c0d 0a20  ': 'Punjabi',.. 
-0000a270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a280: 2020 2020 2020 2027 7175 273a 2027 5175         'qu': 'Qu
-0000a290: 6563 6875 6127 2c0d 0a20 2020 2020 2020  echua',..       
-0000a2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2b0: 2027 726f 273a 2027 526f 6d61 6e69 616e   'ro': 'Romanian
-0000a2c0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-0000a2d0: 2020 2020 2020 2020 2020 2020 2772 7527              'ru'
-0000a2e0: 3a20 2752 7573 7369 616e 272c 0d0a 2020  : 'Russian',..  
-0000a2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a300: 2020 2020 2020 2773 6d27 3a20 2753 616d        'sm': 'Sam
-0000a310: 6f61 6e27 2c0d 0a20 2020 2020 2020 2020  oan',..         
-0000a320: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000a330: 7361 273a 2027 5361 6e73 6b72 6974 272c  sa': 'Sanskrit',
-0000a340: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a350: 2020 2020 2020 2020 2020 2767 6427 3a20            'gd': 
-0000a360: 2753 636f 7473 2047 6165 6c69 6327 2c0d  'Scots Gaelic',.
-0000a370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a380: 2020 2020 2020 2020 2027 6e73 6f27 3a20           'nso': 
-0000a390: 2753 6570 6564 6927 2c0d 0a20 2020 2020  'Sepedi',..     
-0000a3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3b0: 2020 2027 7372 273a 2027 5365 7262 6961     'sr': 'Serbia
-0000a3c0: 6e27 2c0d 0a20 2020 2020 2020 2020 2020  n',..           
-0000a3d0: 2020 2020 2020 2020 2020 2020 2027 7374               'st
-0000a3e0: 273a 2027 5365 736f 7468 6f27 2c0d 0a20  ': 'Sesotho',.. 
-0000a3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a400: 2020 2020 2020 2027 736e 273a 2027 5368         'sn': 'Sh
-0000a410: 6f6e 6127 2c0d 0a20 2020 2020 2020 2020  ona',..         
-0000a420: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000a430: 7364 273a 2027 5369 6e64 6869 272c 0d0a  sd': 'Sindhi',..
-0000a440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a450: 2020 2020 2020 2020 2773 6927 3a20 2753          'si': 'S
-0000a460: 696e 6861 6c61 272c 0d0a 2020 2020 2020  inhala',..      
-0000a470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a480: 2020 2773 6b27 3a20 2753 6c6f 7661 6b27    'sk': 'Slovak'
-0000a490: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000a4a0: 2020 2020 2020 2020 2020 2027 736c 273a             'sl':
-0000a4b0: 2027 536c 6f76 656e 6961 6e27 2c0d 0a20   'Slovenian',.. 
-0000a4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4d0: 2020 2020 2020 2027 736f 273a 2027 536f         'so': 'So
-0000a4e0: 6d61 6c69 272c 0d0a 2020 2020 2020 2020  mali',..        
-0000a4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a500: 2765 7327 3a20 2753 7061 6e69 7368 272c  'es': 'Spanish',
-0000a510: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a520: 2020 2020 2020 2020 2020 2773 7527 3a20            'su': 
-0000a530: 2753 756e 6461 6e65 7365 272c 0d0a 2020  'Sundanese',..  
-0000a540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a550: 2020 2020 2020 2773 7727 3a20 2753 7761        'sw': 'Swa
-0000a560: 6869 6c69 272c 0d0a 2020 2020 2020 2020  hili',..        
-0000a570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a580: 2773 7627 3a20 2753 7765 6469 7368 272c  'sv': 'Swedish',
-0000a590: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a5a0: 2020 2020 2020 2020 2020 2774 6727 3a20            'tg': 
-0000a5b0: 2754 616a 696b 272c 0d0a 2020 2020 2020  'Tajik',..      
-0000a5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5d0: 2020 2774 6127 3a20 2754 616d 696c 272c    'ta': 'Tamil',
-0000a5e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a5f0: 2020 2020 2020 2020 2020 2774 7427 3a20            'tt': 
-0000a600: 2754 6174 6172 272c 0d0a 2020 2020 2020  'Tatar',..      
-0000a610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a620: 2020 2774 6527 3a20 2754 656c 7567 7527    'te': 'Telugu'
-0000a630: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000a640: 2020 2020 2020 2020 2020 2027 7468 273a             'th':
-0000a650: 2027 5468 6169 272c 0d0a 2020 2020 2020   'Thai',..      
-0000a660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a670: 2020 2774 6927 3a20 2754 6967 7269 6e79    'ti': 'Tigriny
-0000a680: 6127 2c0d 0a20 2020 2020 2020 2020 2020  a',..           
-0000a690: 2020 2020 2020 2020 2020 2020 2027 7473               'ts
-0000a6a0: 273a 2027 5473 6f6e 6761 272c 0d0a 2020  ': 'Tsonga',..  
-0000a6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6c0: 2020 2020 2020 2774 7227 3a20 2754 7572        'tr': 'Tur
-0000a6d0: 6b69 7368 272c 0d0a 2020 2020 2020 2020  kish',..        
-0000a6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6f0: 2774 6b27 3a20 2754 7572 6b6d 656e 272c  'tk': 'Turkmen',
-0000a700: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a710: 2020 2020 2020 2020 2020 2774 7727 3a20            'tw': 
-0000a720: 2754 7769 2028 416b 616e 2927 2c0d 0a20  'Twi (Akan)',.. 
-0000a730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a740: 2020 2020 2020 2027 756b 273a 2027 556b         'uk': 'Uk
-0000a750: 7261 696e 6961 6e27 2c0d 0a20 2020 2020  rainian',..     
-0000a760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a770: 2020 2027 7572 273a 2027 5572 6475 272c     'ur': 'Urdu',
-0000a780: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a790: 2020 2020 2020 2020 2020 2775 6727 3a20            'ug': 
-0000a7a0: 2755 7967 6875 7227 2c0d 0a20 2020 2020  'Uyghur',..     
-0000a7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7c0: 2020 2027 757a 273a 2027 557a 6265 6b27     'uz': 'Uzbek'
-0000a7d0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000a7e0: 2020 2020 2020 2020 2020 2027 7669 273a             'vi':
-0000a7f0: 2027 5669 6574 6e61 6d65 7365 272c 0d0a   'Vietnamese',..
-0000a800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a810: 2020 2020 2020 2020 2763 7927 3a20 2757          'cy': 'W
-0000a820: 656c 7368 272c 0d0a 2020 2020 2020 2020  elsh',..        
-0000a830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a840: 2778 6827 3a20 2758 686f 7361 272c 0d0a  'xh': 'Xhosa',..
-0000a850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a860: 2020 2020 2020 2020 2779 6927 3a20 2759          'yi': 'Y
-0000a870: 6964 6469 7368 272c 0d0a 2020 2020 2020  iddish',..      
-0000a880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a890: 2020 2779 6f27 3a20 2759 6f72 7562 6127    'yo': 'Yoruba'
-0000a8a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000a8b0: 2020 2020 2020 2020 2020 2027 7a75 273a             'zu':
-0000a8c0: 2027 5a75 6c75 272c 0d0a 2020 2020 2020   'Zulu',..      
-0000a8d0: 2020 2020 2020 2020 2020 2020 2020 7d0d                }.
-0000a8e0: 0a0d 0a20 2020 2064 6566 2067 6574 5f6e  ...    def get_n
-0000a8f0: 616d 6528 7365 6c66 2c20 6765 745f 636f  ame(self, get_co
-0000a900: 6465 293a 0d0a 2020 2020 2020 2020 7265  de):..        re
-0000a910: 7475 726e 2073 656c 662e 6469 6374 2e67  turn self.dict.g
-0000a920: 6574 2867 6574 5f63 6f64 652e 6c6f 7765  et(get_code.lowe
-0000a930: 7228 292c 2022 2229 0d0a 0d0a 2020 2020  r(), "")....    
-0000a940: 6465 6620 6765 745f 636f 6465 2873 656c  def get_code(sel
-0000a950: 662c 206c 616e 6775 6167 6529 3a0d 0a20  f, language):.. 
-0000a960: 2020 2020 2020 2066 6f72 2067 6574 5f63         for get_c
-0000a970: 6f64 652c 206c 616e 6720 696e 2073 656c  ode, lang in sel
-0000a980: 662e 6469 6374 2e69 7465 6d73 2829 3a0d  f.dict.items():.
-0000a990: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000a9a0: 6c61 6e67 2e6c 6f77 6572 2829 203d 3d20  lang.lower() == 
-0000a9b0: 6c61 6e67 7561 6765 2e6c 6f77 6572 2829  language.lower()
-0000a9c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000a9d0: 2020 2072 6574 7572 6e20 6765 745f 636f     return get_co
-0000a9e0: 6465 0d0a 2020 2020 2020 2020 7265 7475  de..        retu
-0000a9f0: 726e 2022 220d 0a0d 0a0d 0a63 6c61 7373  rn ""......class
-0000aa00: 2057 6176 436f 6e76 6572 7465 723a 0d0a   WavConverter:..
-0000aa10: 2020 2020 4073 7461 7469 636d 6574 686f      @staticmetho
-0000aa20: 640d 0a20 2020 2064 6566 2077 6869 6368  d..    def which
-0000aa30: 2870 726f 6772 616d 293a 0d0a 2020 2020  (program):..    
-0000aa40: 2020 2020 6465 6620 6973 5f65 7865 2866      def is_exe(f
-0000aa50: 696c 655f 7061 7468 293a 0d0a 2020 2020  ile_path):..    
-0000aa60: 2020 2020 2020 2020 7265 7475 726e 206f          return o
-0000aa70: 732e 7061 7468 2e69 7366 696c 6528 6669  s.path.isfile(fi
-0000aa80: 6c65 5f70 6174 6829 2061 6e64 206f 732e  le_path) and os.
-0000aa90: 6163 6365 7373 2866 696c 655f 7061 7468  access(file_path
-0000aaa0: 2c20 6f73 2e58 5f4f 4b29 0d0a 2020 2020  , os.X_OK)..    
-0000aab0: 2020 2020 6670 6174 682c 205f 203d 206f      fpath, _ = o
-0000aac0: 732e 7061 7468 2e73 706c 6974 2870 726f  s.path.split(pro
-0000aad0: 6772 616d 290d 0a20 2020 2020 2020 2069  gram)..        i
-0000aae0: 6620 6670 6174 683a 0d0a 2020 2020 2020  f fpath:..      
-0000aaf0: 2020 2020 2020 6966 2069 735f 6578 6528        if is_exe(
-0000ab00: 7072 6f67 7261 6d29 3a0d 0a20 2020 2020  program):..     
-0000ab10: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000ab20: 6e20 7072 6f67 7261 6d0d 0a20 2020 2020  n program..     
-0000ab30: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-0000ab40: 2020 2020 2020 666f 7220 7061 7468 2069        for path i
-0000ab50: 6e20 6f73 2e65 6e76 6972 6f6e 5b22 5041  n os.environ["PA
-0000ab60: 5448 225d 2e73 706c 6974 286f 732e 7061  TH"].split(os.pa
-0000ab70: 7468 7365 7029 3a0d 0a20 2020 2020 2020  thsep):..       
-0000ab80: 2020 2020 2020 2020 2070 6174 6820 3d20           path = 
-0000ab90: 7061 7468 2e73 7472 6970 2827 2227 290d  path.strip('"').
-0000aba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000abb0: 2065 7865 5f66 696c 6520 3d20 6f73 2e70   exe_file = os.p
-0000abc0: 6174 682e 6a6f 696e 2870 6174 682c 2070  ath.join(path, p
-0000abd0: 726f 6772 616d 290d 0a20 2020 2020 2020  rogram)..       
-0000abe0: 2020 2020 2020 2020 2069 6620 6973 5f65           if is_e
-0000abf0: 7865 2865 7865 5f66 696c 6529 3a0d 0a20  xe(exe_file):.. 
-0000ac00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac10: 2020 2072 6574 7572 6e20 6578 655f 6669     return exe_fi
-0000ac20: 6c65 0d0a 2020 2020 2020 2020 7265 7475  le..        retu
-0000ac30: 726e 204e 6f6e 650d 0a0d 0a20 2020 2040  rn None....    @
-0000ac40: 7374 6174 6963 6d65 7468 6f64 0d0a 2020  staticmethod..  
-0000ac50: 2020 6465 6620 6666 6d70 6567 5f63 6865    def ffmpeg_che
-0000ac60: 636b 2829 3a0d 0a20 2020 2020 2020 2069  ck():..        i
-0000ac70: 6620 5761 7643 6f6e 7665 7274 6572 2e77  f WavConverter.w
-0000ac80: 6869 6368 2822 6666 6d70 6567 2229 3a0d  hich("ffmpeg"):.
-0000ac90: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000aca0: 7572 6e20 2266 666d 7065 6722 0d0a 2020  urn "ffmpeg"..  
-0000acb0: 2020 2020 2020 6966 2057 6176 436f 6e76        if WavConv
-0000acc0: 6572 7465 722e 7768 6963 6828 2266 666d  erter.which("ffm
-0000acd0: 7065 672e 6578 6522 293a 0d0a 2020 2020  peg.exe"):..    
-0000ace0: 2020 2020 2020 2020 7265 7475 726e 2022          return "
-0000acf0: 6666 6d70 6567 2e65 7865 220d 0a20 2020  ffmpeg.exe"..   
-0000ad00: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
-0000ad10: 0d0a 0d0a 2020 2020 6465 6620 5f5f 696e  ....    def __in
-0000ad20: 6974 5f5f 2873 656c 662c 2063 6861 6e6e  it__(self, chann
-0000ad30: 656c 733d 312c 2072 6174 653d 3438 3030  els=1, rate=4800
-0000ad40: 302c 2070 726f 6772 6573 735f 6361 6c6c  0, progress_call
-0000ad50: 6261 636b 3d4e 6f6e 652c 2065 7272 6f72  back=None, error
-0000ad60: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
-0000ad70: 636b 3d4e 6f6e 6529 3a0d 0a20 2020 2020  ck=None):..     
-0000ad80: 2020 2073 656c 662e 6368 616e 6e65 6c73     self.channels
-0000ad90: 203d 2063 6861 6e6e 656c 730d 0a20 2020   = channels..   
-0000ada0: 2020 2020 2073 656c 662e 7261 7465 203d       self.rate =
-0000adb0: 2072 6174 650d 0a20 2020 2020 2020 2073   rate..        s
-0000adc0: 656c 662e 7072 6f67 7265 7373 5f63 616c  elf.progress_cal
-0000add0: 6c62 6163 6b20 3d20 7072 6f67 7265 7373  lback = progress
-0000ade0: 5f63 616c 6c62 6163 6b0d 0a20 2020 2020  _callback..     
-0000adf0: 2020 2073 656c 662e 6572 726f 725f 6d65     self.error_me
-0000ae00: 7373 6167 6573 5f63 616c 6c62 6163 6b20  ssages_callback 
-0000ae10: 3d20 6572 726f 725f 6d65 7373 6167 6573  = error_messages
-0000ae20: 5f63 616c 6c62 6163 6b0d 0a0d 0a20 2020  _callback....   
-0000ae30: 2064 6566 205f 5f63 616c 6c5f 5f28 7365   def __call__(se
-0000ae40: 6c66 2c20 6d65 6469 615f 6669 6c65 7061  lf, media_filepa
-0000ae50: 7468 293a 0d0a 2020 2020 2020 2020 7465  th):..        te
-0000ae60: 6d70 203d 2074 656d 7066 696c 652e 4e61  mp = tempfile.Na
-0000ae70: 6d65 6454 656d 706f 7261 7279 4669 6c65  medTemporaryFile
-0000ae80: 2873 7566 6669 783d 272e 7761 7627 2c20  (suffix='.wav', 
-0000ae90: 6465 6c65 7465 3d46 616c 7365 290d 0a20  delete=False).. 
-0000aea0: 2020 2020 2020 2069 6620 6e6f 7420 6f73         if not os
-0000aeb0: 2e70 6174 682e 6973 6669 6c65 286d 6564  .path.isfile(med
-0000aec0: 6961 5f66 696c 6570 6174 6829 3a0d 0a20  ia_filepath):.. 
-0000aed0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000aee0: 6c66 2e65 7272 6f72 5f6d 6573 7361 6765  lf.error_message
-0000aef0: 735f 6361 6c6c 6261 636b 3a0d 0a20 2020  s_callback:..   
-0000af00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000af10: 662e 6572 726f 725f 6d65 7373 6167 6573  f.error_messages
-0000af20: 5f63 616c 6c62 6163 6b28 2254 6865 2067  _callback("The g
-0000af30: 6976 656e 2066 696c 6520 646f 6573 206e  iven file does n
-0000af40: 6f74 2065 7869 7374 3a20 7b30 7d22 2e66  ot exist: {0}".f
-0000af50: 6f72 6d61 7428 6d65 6469 615f 6669 6c65  ormat(media_file
-0000af60: 7061 7468 2929 0d0a 2020 2020 2020 2020  path))..        
-0000af70: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-0000af80: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0000af90: 2822 5468 6520 6769 7665 6e20 6669 6c65  ("The given file
-0000afa0: 2064 6f65 7320 6e6f 7420 6578 6973 743a   does not exist:
-0000afb0: 207b 307d 222e 666f 726d 6174 286d 6564   {0}".format(med
-0000afc0: 6961 5f66 696c 6570 6174 6829 290d 0a20  ia_filepath)).. 
-0000afd0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000afe0: 6169 7365 2045 7863 6570 7469 6f6e 2822  aise Exception("
-0000aff0: 496e 7661 6c69 6420 6669 6c65 3a20 7b30  Invalid file: {0
-0000b000: 7d22 2e66 6f72 6d61 7428 6d65 6469 615f  }".format(media_
-0000b010: 6669 6c65 7061 7468 2929 0d0a 2020 2020  filepath))..    
-0000b020: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
-0000b030: 6666 6d70 6567 5f63 6865 636b 2829 3a0d  ffmpeg_check():.
-0000b040: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000b050: 7365 6c66 2e65 7272 6f72 5f6d 6573 7361  self.error_messa
-0000b060: 6765 735f 6361 6c6c 6261 636b 3a0d 0a20  ges_callback:.. 
-0000b070: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000b080: 656c 662e 6572 726f 725f 6d65 7373 6167  elf.error_messag
-0000b090: 6573 5f63 616c 6c62 6163 6b28 2266 666d  es_callback("ffm
-0000b0a0: 7065 673a 2045 7865 6375 7461 626c 6520  peg: Executable 
-0000b0b0: 6e6f 7420 666f 756e 6420 6f6e 206d 6163  not found on mac
-0000b0c0: 6869 6e65 2e22 290d 0a20 2020 2020 2020  hine.")..       
-0000b0d0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-0000b0e0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0000b0f0: 7428 2266 666d 7065 673a 2045 7865 6375  t("ffmpeg: Execu
-0000b100: 7461 626c 6520 6e6f 7420 666f 756e 6420  table not found 
-0000b110: 6f6e 206d 6163 6869 6e65 2e22 290d 0a20  on machine.").. 
-0000b120: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000b130: 6169 7365 2045 7863 6570 7469 6f6e 2822  aise Exception("
-0000b140: 4465 7065 6e64 656e 6379 206e 6f74 2066  Dependency not f
-0000b150: 6f75 6e64 3a20 6666 6d70 6567 2229 0d0a  ound: ffmpeg")..
-0000b160: 0d0a 2020 2020 2020 2020 636f 6d6d 616e  ..        comman
-0000b170: 6420 3d20 5b0d 0a20 2020 2020 2020 2020  d = [..         
-0000b180: 2020 2020 2020 2020 2020 2022 6666 6d70             "ffmp
-0000b190: 6567 222c 0d0a 2020 2020 2020 2020 2020  eg",..          
-0000b1a0: 2020 2020 2020 2020 2020 222d 7922 2c0d            "-y",.
-0000b1b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b1c0: 2020 2020 2022 2d69 222c 206d 6564 6961       "-i", media
-0000b1d0: 5f66 696c 6570 6174 682c 0d0a 2020 2020  _filepath,..    
-0000b1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1f0: 222d 6163 222c 2073 7472 2873 656c 662e  "-ac", str(self.
-0000b200: 6368 616e 6e65 6c73 292c 0d0a 2020 2020  channels),..    
-0000b210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b220: 222d 6172 222c 2073 7472 2873 656c 662e  "-ar", str(self.
-0000b230: 7261 7465 292c 0d0a 2020 2020 2020 2020  rate),..        
-0000b240: 2020 2020 2020 2020 2020 2020 222d 6c6f              "-lo
-0000b250: 676c 6576 656c 222c 2022 6572 726f 7222  glevel", "error"
-0000b260: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000b270: 2020 2020 2020 2022 2d68 6964 655f 6261         "-hide_ba
-0000b280: 6e6e 6572 222c 0d0a 2020 2020 2020 2020  nner",..        
-0000b290: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-0000b2a0: 2e6e 616d 650d 0a20 2020 2020 2020 2020  .name..         
-0000b2b0: 2020 2020 2020 2020 205d 0d0a 0d0a 2020           ]....  
-0000b2c0: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
-0000b2d0: 2020 2020 2020 2020 2320 5255 4e4e 494e          # RUNNIN
-0000b2e0: 4720 6666 6d70 6567 2057 4954 484f 5554  G ffmpeg WITHOUT
-0000b2f0: 2053 484f 5749 4e47 2050 524f 4752 4553   SHOWING PROGRES
-0000b300: 5353 0d0a 2020 2020 2020 2020 2020 2020  SS..            
-0000b310: 2375 7365 5f73 6865 6c6c 203d 2054 7275  #use_shell = Tru
-0000b320: 6520 6966 206f 732e 6e61 6d65 203d 3d20  e if os.name == 
-0000b330: 226e 7422 2065 6c73 6520 4661 6c73 650d  "nt" else False.
-0000b340: 0a20 2020 2020 2020 2020 2020 2023 7375  .            #su
-0000b350: 6270 726f 6365 7373 2e63 6865 636b 5f6f  bprocess.check_o
-0000b360: 7574 7075 7428 636f 6d6d 616e 642c 2073  utput(command, s
-0000b370: 7464 696e 3d6f 7065 6e28 6f73 2e64 6576  tdin=open(os.dev
-0000b380: 6e75 6c6c 292c 2073 6865 6c6c 3d75 7365  null), shell=use
-0000b390: 5f73 6865 6c6c 290d 0a0d 0a20 2020 2020  _shell)....     
-0000b3a0: 2020 2020 2020 2023 2052 554e 4e49 4e47         # RUNNING
-0000b3b0: 2066 666d 7065 6720 5749 5448 2050 524f   ffmpeg WITH PRO
-0000b3c0: 4752 4553 5353 0d0a 2020 2020 2020 2020  GRESSS..        
-0000b3d0: 2020 2020 6666 203d 2046 666d 7065 6750      ff = FfmpegP
-0000b3e0: 726f 6772 6573 7328 636f 6d6d 616e 6429  rogress(command)
-0000b3f0: 0d0a 2020 2020 2020 2020 2020 2020 7065  ..            pe
-0000b400: 7263 656e 7461 6765 203d 2030 0d0a 2020  rcentage = 0..  
-0000b410: 2020 2020 2020 2020 2020 666f 7220 7072            for pr
-0000b420: 6f67 7265 7373 2069 6e20 6666 2e72 756e  ogress in ff.run
-0000b430: 5f63 6f6d 6d61 6e64 5f77 6974 685f 7072  _command_with_pr
-0000b440: 6f67 7265 7373 2829 3a0d 0a20 2020 2020  ogress():..     
-0000b450: 2020 2020 2020 2020 2020 2070 6572 6365             perce
-0000b460: 6e74 6167 6520 3d20 7072 6f67 7265 7373  ntage = progress
-0000b470: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000b480: 2020 6966 2073 656c 662e 7072 6f67 7265    if self.progre
-0000b490: 7373 5f63 616c 6c62 6163 6b3a 0d0a 2020  ss_callback:..  
-0000b4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b4b0: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
-0000b4c0: 6361 6c6c 6261 636b 286d 6564 6961 5f66  callback(media_f
-0000b4d0: 696c 6570 6174 682c 2070 6572 6365 6e74  ilepath, percent
-0000b4e0: 6167 6529 0d0a 2020 2020 2020 2020 2020  age)..          
-0000b4f0: 2020 7465 6d70 2e63 6c6f 7365 2829 0d0a    temp.close()..
-0000b500: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-0000b510: 7475 726e 2074 656d 702e 6e61 6d65 2c20  turn temp.name, 
-0000b520: 7365 6c66 2e72 6174 650d 0a0d 0a20 2020  self.rate....   
-0000b530: 2020 2020 2065 7863 6570 7420 4b65 7962       except Keyb
-0000b540: 6f61 7264 496e 7465 7272 7570 743a 0d0a  oardInterrupt:..
-0000b550: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000b560: 656c 662e 6572 726f 725f 6d65 7373 6167  elf.error_messag
-0000b570: 6573 5f63 616c 6c62 6163 6b3a 0d0a 2020  es_callback:..  
-0000b580: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000b590: 6c66 2e65 7272 6f72 5f6d 6573 7361 6765  lf.error_message
-0000b5a0: 735f 6361 6c6c 6261 636b 2822 4361 6e63  s_callback("Canc
-0000b5b0: 656c 6c69 6e67 2061 6c6c 2074 6173 6b73  elling all tasks
-0000b5c0: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-0000b5d0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-0000b5e0: 2020 2020 2020 2070 7269 6e74 2822 4361         print("Ca
-0000b5f0: 6e63 656c 6c69 6e67 2061 6c6c 2074 6173  ncelling all tas
-0000b600: 6b73 2229 0d0a 2020 2020 2020 2020 2020  ks")..          
-0000b610: 2020 7265 7475 726e 0d0a 0d0a 2020 2020    return....    
-0000b620: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-0000b630: 7469 6f6e 2061 7320 653a 0d0a 2020 2020  tion as e:..    
-0000b640: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000b650: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
-0000b660: 616c 6c62 6163 6b3a 0d0a 2020 2020 2020  allback:..      
-0000b670: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
-0000b680: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
-0000b690: 6c6c 6261 636b 2865 290d 0a20 2020 2020  llback(e)..     
-0000b6a0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-0000b6b0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-0000b6c0: 696e 7428 6529 0d0a 2020 2020 2020 2020  int(e)..        
-0000b6d0: 2020 2020 7265 7475 726e 0d0a 0d0a 0d0a      return......
-0000b6e0: 636c 6173 7320 5370 6565 6368 5265 6769  class SpeechRegi
-0000b6f0: 6f6e 4669 6e64 6572 3a0d 0a20 2020 2040  onFinder:..    @
-0000b700: 7374 6174 6963 6d65 7468 6f64 0d0a 2020  staticmethod..  
-0000b710: 2020 6465 6620 7065 7263 656e 7469 6c65    def percentile
-0000b720: 2861 7272 2c20 7065 7263 656e 7429 3a0d  (arr, percent):.
-0000b730: 0a20 2020 2020 2020 2061 7272 203d 2073  .        arr = s
-0000b740: 6f72 7465 6428 6172 7229 0d0a 2020 2020  orted(arr)..    
-0000b750: 2020 2020 6b20 3d20 286c 656e 2861 7272      k = (len(arr
-0000b760: 2920 2d20 3129 202a 2070 6572 6365 6e74  ) - 1) * percent
-0000b770: 0d0a 2020 2020 2020 2020 6620 3d20 6d61  ..        f = ma
-0000b780: 7468 2e66 6c6f 6f72 286b 290d 0a20 2020  th.floor(k)..   
-0000b790: 2020 2020 2063 203d 206d 6174 682e 6365       c = math.ce
-0000b7a0: 696c 286b 290d 0a20 2020 2020 2020 2069  il(k)..        i
-0000b7b0: 6620 6620 3d3d 2063 3a20 7265 7475 726e  f f == c: return
-0000b7c0: 2061 7272 5b69 6e74 286b 295d 0d0a 2020   arr[int(k)]..  
-0000b7d0: 2020 2020 2020 6430 203d 2061 7272 5b69        d0 = arr[i
-0000b7e0: 6e74 2866 295d 202a 2028 6320 2d20 6b29  nt(f)] * (c - k)
-0000b7f0: 0d0a 2020 2020 2020 2020 6431 203d 2061  ..        d1 = a
-0000b800: 7272 5b69 6e74 2863 295d 202a 2028 6b20  rr[int(c)] * (k 
-0000b810: 2d20 6629 0d0a 2020 2020 2020 2020 7265  - f)..        re
-0000b820: 7475 726e 2064 3020 2b20 6431 0d0a 0d0a  turn d0 + d1....
-0000b830: 2020 2020 2364 6566 205f 5f69 6e69 745f      #def __init_
-0000b840: 5f28 7365 6c66 2c20 6672 616d 655f 7769  _(self, frame_wi
-0000b850: 6474 683d 3430 3936 2c20 6d69 6e5f 7265  dth=4096, min_re
-0000b860: 6769 6f6e 5f73 697a 653d 302e 352c 206d  gion_size=0.5, m
-0000b870: 6178 5f72 6567 696f 6e5f 7369 7a65 3d36  ax_region_size=6
-0000b880: 293a 0d0a 2020 2020 6465 6620 5f5f 696e  ):..    def __in
-0000b890: 6974 5f5f 2873 656c 662c 2066 7261 6d65  it__(self, frame
-0000b8a0: 5f77 6964 7468 3d34 3039 362c 206d 696e  _width=4096, min
-0000b8b0: 5f72 6567 696f 6e5f 7369 7a65 3d30 2e35  _region_size=0.5
-0000b8c0: 2c20 6d61 785f 7265 6769 6f6e 5f73 697a  , max_region_siz
-0000b8d0: 653d 362c 2065 7272 6f72 5f6d 6573 7361  e=6, error_messa
-0000b8e0: 6765 735f 6361 6c6c 6261 636b 3d4e 6f6e  ges_callback=Non
-0000b8f0: 6529 3a0d 0a20 2020 2020 2020 2073 656c  e):..        sel
-0000b900: 662e 6672 616d 655f 7769 6474 6820 3d20  f.frame_width = 
-0000b910: 6672 616d 655f 7769 6474 680d 0a20 2020  frame_width..   
-0000b920: 2020 2020 2073 656c 662e 6d69 6e5f 7265       self.min_re
-0000b930: 6769 6f6e 5f73 697a 6520 3d20 6d69 6e5f  gion_size = min_
-0000b940: 7265 6769 6f6e 5f73 697a 650d 0a20 2020  region_size..   
-0000b950: 2020 2020 2073 656c 662e 6d61 785f 7265       self.max_re
-0000b960: 6769 6f6e 5f73 697a 6520 3d20 6d61 785f  gion_size = max_
-0000b970: 7265 6769 6f6e 5f73 697a 650d 0a20 2020  region_size..   
-0000b980: 2020 2020 2073 656c 662e 6572 726f 725f       self.error_
-0000b990: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
-0000b9a0: 6b20 3d20 6572 726f 725f 6d65 7373 6167  k = error_messag
-0000b9b0: 6573 5f63 616c 6c62 6163 6b0d 0a0d 0a20  es_callback.... 
-0000b9c0: 2020 2023 6465 6620 5f5f 6361 6c6c 5f5f     #def __call__
-0000b9d0: 2873 656c 662c 2077 6176 5f66 696c 6570  (self, wav_filep
-0000b9e0: 6174 682c 2065 7272 6f72 5f6d 6573 7361  ath, error_messa
-0000b9f0: 6765 735f 6361 6c6c 6261 636b 3d4e 6f6e  ges_callback=Non
-0000ba00: 6529 3a0d 0a20 2020 2064 6566 205f 5f63  e):..    def __c
-0000ba10: 616c 6c5f 5f28 7365 6c66 2c20 7761 765f  all__(self, wav_
-0000ba20: 6669 6c65 7061 7468 293a 0d0a 2020 2020  filepath):..    
-0000ba30: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
-0000ba40: 2020 2020 2020 7265 6164 6572 203d 2077        reader = w
-0000ba50: 6176 652e 6f70 656e 2877 6176 5f66 696c  ave.open(wav_fil
-0000ba60: 6570 6174 6829 0d0a 2020 2020 2020 2020  epath)..        
-0000ba70: 2020 2020 7361 6d70 6c65 5f77 6964 7468      sample_width
-0000ba80: 203d 2072 6561 6465 722e 6765 7473 616d   = reader.getsam
-0000ba90: 7077 6964 7468 2829 0d0a 2020 2020 2020  pwidth()..      
-0000baa0: 2020 2020 2020 7261 7465 203d 2072 6561        rate = rea
-0000bab0: 6465 722e 6765 7466 7261 6d65 7261 7465  der.getframerate
-0000bac0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-0000bad0: 6e5f 6368 616e 6e65 6c73 203d 2072 6561  n_channels = rea
-0000bae0: 6465 722e 6765 746e 6368 616e 6e65 6c73  der.getnchannels
-0000baf0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-0000bb00: 746f 7461 6c5f 6475 7261 7469 6f6e 203d  total_duration =
-0000bb10: 2072 6561 6465 722e 6765 746e 6672 616d   reader.getnfram
-0000bb20: 6573 2829 202f 2072 6174 650d 0a20 2020  es() / rate..   
-0000bb30: 2020 2020 2020 2020 2063 6875 6e6b 5f64           chunk_d
-0000bb40: 7572 6174 696f 6e20 3d20 666c 6f61 7428  uration = float(
-0000bb50: 7365 6c66 2e66 7261 6d65 5f77 6964 7468  self.frame_width
-0000bb60: 2920 2f20 7261 7465 0d0a 2020 2020 2020  ) / rate..      
-0000bb70: 2020 2020 2020 6e5f 6368 756e 6b73 203d        n_chunks =
-0000bb80: 2069 6e74 2874 6f74 616c 5f64 7572 6174   int(total_durat
-0000bb90: 696f 6e20 2f20 6368 756e 6b5f 6475 7261  ion / chunk_dura
-0000bba0: 7469 6f6e 290d 0a20 2020 2020 2020 2020  tion)..         
-0000bbb0: 2020 2065 6e65 7267 6965 7320 3d20 5b5d     energies = []
-0000bbc0: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-0000bbd0: 7220 6920 696e 2072 616e 6765 286e 5f63  r i in range(n_c
-0000bbe0: 6875 6e6b 7329 3a0d 0a20 2020 2020 2020  hunks):..       
-0000bbf0: 2020 2020 2020 2020 2063 6875 6e6b 203d           chunk =
-0000bc00: 2072 6561 6465 722e 7265 6164 6672 616d   reader.readfram
-0000bc10: 6573 2873 656c 662e 6672 616d 655f 7769  es(self.frame_wi
-0000bc20: 6474 6829 0d0a 2020 2020 2020 2020 2020  dth)..          
-0000bc30: 2020 2020 2020 656e 6572 6769 6573 2e61        energies.a
-0000bc40: 7070 656e 6428 6175 6469 6f6f 702e 726d  ppend(audioop.rm
-0000bc50: 7328 6368 756e 6b2c 2073 616d 706c 655f  s(chunk, sample_
-0000bc60: 7769 6474 6820 2a20 6e5f 6368 616e 6e65  width * n_channe
-0000bc70: 6c73 2929 0d0a 2020 2020 2020 2020 2020  ls))..          
-0000bc80: 2020 7468 7265 7368 6f6c 6420 3d20 5370    threshold = Sp
-0000bc90: 6565 6368 5265 6769 6f6e 4669 6e64 6572  eechRegionFinder
-0000bca0: 2e70 6572 6365 6e74 696c 6528 656e 6572  .percentile(ener
-0000bcb0: 6769 6573 2c20 302e 3229 0d0a 2020 2020  gies, 0.2)..    
-0000bcc0: 2020 2020 2020 2020 656c 6170 7365 645f          elapsed_
-0000bcd0: 7469 6d65 203d 2030 0d0a 2020 2020 2020  time = 0..      
-0000bce0: 2020 2020 2020 7265 6769 6f6e 7320 3d20        regions = 
-0000bcf0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-0000bd00: 7265 6769 6f6e 5f73 7461 7274 203d 204e  region_start = N
-0000bd10: 6f6e 650d 0a20 2020 2020 2020 2020 2020  one..           
-0000bd20: 2066 6f72 2065 6e65 7267 7920 696e 2065   for energy in e
-0000bd30: 6e65 7267 6965 733a 0d0a 2020 2020 2020  nergies:..      
-0000bd40: 2020 2020 2020 2020 2020 6973 5f73 696c            is_sil
-0000bd50: 656e 6365 203d 2065 6e65 7267 7920 3c3d  ence = energy <=
-0000bd60: 2074 6872 6573 686f 6c64 0d0a 2020 2020   threshold..    
-0000bd70: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
-0000bd80: 6578 6365 6564 6564 203d 2072 6567 696f  exceeded = regio
-0000bd90: 6e5f 7374 6172 7420 616e 6420 656c 6170  n_start and elap
-0000bda0: 7365 645f 7469 6d65 202d 2072 6567 696f  sed_time - regio
-0000bdb0: 6e5f 7374 6172 7420 3e3d 2073 656c 662e  n_start >= self.
-0000bdc0: 6d61 785f 7265 6769 6f6e 5f73 697a 650d  max_region_size.
-0000bdd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bde0: 2069 6620 286d 6178 5f65 7863 6565 6465   if (max_exceede
-0000bdf0: 6420 6f72 2069 735f 7369 6c65 6e63 6529  d or is_silence)
-0000be00: 2061 6e64 2072 6567 696f 6e5f 7374 6172   and region_star
-0000be10: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
-0000be20: 2020 2020 2020 2020 6966 2065 6c61 7073          if elaps
-0000be30: 6564 5f74 696d 6520 2d20 7265 6769 6f6e  ed_time - region
-0000be40: 5f73 7461 7274 203e 3d20 7365 6c66 2e6d  _start >= self.m
-0000be50: 696e 5f72 6567 696f 6e5f 7369 7a65 3a0d  in_region_size:.
-0000be60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000be70: 2020 2020 2020 2020 2072 6567 696f 6e73           regions
-0000be80: 2e61 7070 656e 6428 2872 6567 696f 6e5f  .append((region_
-0000be90: 7374 6172 742c 2065 6c61 7073 6564 5f74  start, elapsed_t
-0000bea0: 696d 6529 290d 0a20 2020 2020 2020 2020  ime))..         
-0000beb0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000bec0: 6567 696f 6e5f 7374 6172 7420 3d20 4e6f  egion_start = No
-0000bed0: 6e65 0d0a 2020 2020 2020 2020 2020 2020  ne..            
-0000bee0: 2020 2020 656c 6966 2028 6e6f 7420 7265      elif (not re
-0000bef0: 6769 6f6e 5f73 7461 7274 2920 616e 6420  gion_start) and 
-0000bf00: 286e 6f74 2069 735f 7369 6c65 6e63 6529  (not is_silence)
-0000bf10: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000bf20: 2020 2020 2020 2072 6567 696f 6e5f 7374         region_st
-0000bf30: 6172 7420 3d20 656c 6170 7365 645f 7469  art = elapsed_ti
-0000bf40: 6d65 0d0a 2020 2020 2020 2020 2020 2020  me..            
-0000bf50: 2020 2020 656c 6170 7365 645f 7469 6d65      elapsed_time
-0000bf60: 202b 3d20 6368 756e 6b5f 6475 7261 7469   += chunk_durati
-0000bf70: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
-0000bf80: 7265 7475 726e 2072 6567 696f 6e73 0d0a  return regions..
-0000bf90: 0d0a 2020 2020 2020 2020 6578 6365 7074  ..        except
-0000bfa0: 204b 6579 626f 6172 6449 6e74 6572 7275   KeyboardInterru
-0000bfb0: 7074 3a0d 0a20 2020 2020 2020 2020 2020  pt:..           
-0000bfc0: 2069 6620 7365 6c66 2e65 7272 6f72 5f6d   if self.error_m
-0000bfd0: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
-0000bfe0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000bff0: 2020 2073 656c 662e 6572 726f 725f 6d65     self.error_me
-0000c000: 7373 6167 6573 5f63 616c 6c62 6163 6b28  ssages_callback(
-0000c010: 2243 616e 6365 6c6c 696e 6720 616c 6c20  "Cancelling all 
-0000c020: 7461 736b 7322 290d 0a20 2020 2020 2020  tasks")..       
-0000c030: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-0000c040: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0000c050: 7428 2243 616e 6365 6c6c 696e 6720 616c  t("Cancelling al
-0000c060: 6c20 7461 736b 7322 290d 0a20 2020 2020  l tasks")..     
-0000c070: 2020 2020 2020 2072 6574 7572 6e0d 0a0d         return...
-0000c080: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-0000c090: 4578 6365 7074 696f 6e20 6173 2065 3a0d  Exception as e:.
-0000c0a0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000c0b0: 7365 6c66 2e65 7272 6f72 5f6d 6573 7361  self.error_messa
-0000c0c0: 6765 735f 6361 6c6c 6261 636b 3a0d 0a20  ges_callback:.. 
-0000c0d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000c0e0: 656c 662e 6572 726f 725f 6d65 7373 6167  elf.error_messag
-0000c0f0: 6573 5f63 616c 6c62 6163 6b28 6529 0d0a  es_callback(e)..
-0000c100: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000c110: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000c120: 2020 2070 7269 6e74 2865 290d 0a20 2020     print(e)..   
-0000c130: 2020 2020 2020 2020 2072 6574 7572 6e0d           return.
-0000c140: 0a0d 0a0d 0a63 6c61 7373 2046 4c41 4343  .....class FLACC
-0000c150: 6f6e 7665 7274 6572 286f 626a 6563 7429  onverter(object)
-0000c160: 3a0d 0a20 2020 2023 6465 6620 5f5f 696e  :..    #def __in
-0000c170: 6974 5f5f 2873 656c 662c 2077 6176 5f66  it__(self, wav_f
-0000c180: 696c 6570 6174 682c 2069 6e63 6c75 6465  ilepath, include
-0000c190: 5f62 6566 6f72 653d 302e 3235 2c20 696e  _before=0.25, in
-0000c1a0: 636c 7564 655f 6166 7465 723d 302e 3235  clude_after=0.25
-0000c1b0: 293a 0d0a 2020 2020 6465 6620 5f5f 696e  ):..    def __in
-0000c1c0: 6974 5f5f 2873 656c 662c 2077 6176 5f66  it__(self, wav_f
-0000c1d0: 696c 6570 6174 682c 2069 6e63 6c75 6465  ilepath, include
-0000c1e0: 5f62 6566 6f72 653d 302e 3235 2c20 696e  _before=0.25, in
-0000c1f0: 636c 7564 655f 6166 7465 723d 302e 3235  clude_after=0.25
-0000c200: 2c20 6572 726f 725f 6d65 7373 6167 6573  , error_messages
-0000c210: 5f63 616c 6c62 6163 6b3d 4e6f 6e65 293a  _callback=None):
-0000c220: 0d0a 2020 2020 2020 2020 7365 6c66 2e77  ..        self.w
-0000c230: 6176 5f66 696c 6570 6174 6820 3d20 7761  av_filepath = wa
-0000c240: 765f 6669 6c65 7061 7468 0d0a 2020 2020  v_filepath..    
-0000c250: 2020 2020 7365 6c66 2e69 6e63 6c75 6465      self.include
-0000c260: 5f62 6566 6f72 6520 3d20 696e 636c 7564  _before = includ
-0000c270: 655f 6265 666f 7265 0d0a 2020 2020 2020  e_before..      
-0000c280: 2020 7365 6c66 2e69 6e63 6c75 6465 5f61    self.include_a
-0000c290: 6674 6572 203d 2069 6e63 6c75 6465 5f61  fter = include_a
-0000c2a0: 6674 6572 0d0a 2020 2020 2020 2020 7365  fter..        se
-0000c2b0: 6c66 2e65 7272 6f72 5f6d 6573 7361 6765  lf.error_message
-0000c2c0: 735f 6361 6c6c 6261 636b 203d 2065 7272  s_callback = err
-0000c2d0: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
-0000c2e0: 6261 636b 0d0a 0d0a 2020 2020 2364 6566  back....    #def
-0000c2f0: 205f 5f63 616c 6c5f 5f28 7365 6c66 2c20   __call__(self, 
-0000c300: 7265 6769 6f6e 2c20 6572 726f 725f 6d65  region, error_me
-0000c310: 7373 6167 6573 5f63 616c 6c62 6163 6b3d  ssages_callback=
-0000c320: 4e6f 6e65 293a 0d0a 2020 2020 6465 6620  None):..    def 
-0000c330: 5f5f 6361 6c6c 5f5f 2873 656c 662c 2072  __call__(self, r
-0000c340: 6567 696f 6e29 3a0d 0a20 2020 2020 2020  egion):..       
-0000c350: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
-0000c360: 2020 2073 7461 7274 2c20 656e 6420 3d20     start, end = 
-0000c370: 7265 6769 6f6e 0d0a 2020 2020 2020 2020  region..        
-0000c380: 2020 2020 7374 6172 7420 3d20 6d61 7828      start = max(
-0000c390: 302c 2073 7461 7274 202d 2073 656c 662e  0, start - self.
-0000c3a0: 696e 636c 7564 655f 6265 666f 7265 290d  include_before).
-0000c3b0: 0a20 2020 2020 2020 2020 2020 2065 6e64  .            end
-0000c3c0: 202b 3d20 7365 6c66 2e69 6e63 6c75 6465   += self.include
-0000c3d0: 5f61 6674 6572 0d0a 2020 2020 2020 2020  _after..        
-0000c3e0: 2020 2020 7465 6d70 203d 2074 656d 7066      temp = tempf
-0000c3f0: 696c 652e 4e61 6d65 6454 656d 706f 7261  ile.NamedTempora
-0000c400: 7279 4669 6c65 2873 7566 6669 783d 272e  ryFile(suffix='.
-0000c410: 666c 6163 272c 2064 656c 6574 653d 4661  flac', delete=Fa
-0000c420: 6c73 6529 0d0a 2020 2020 2020 2020 2020  lse)..          
-0000c430: 2020 636f 6d6d 616e 6420 3d20 5b0d 0a20    command = [.. 
-0000c440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c450: 2020 2020 2020 2022 6666 6d70 6567 222c         "ffmpeg",
-0000c460: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c470: 2020 2020 2020 2020 2020 222d 7373 222c            "-ss",
-0000c480: 2073 7472 2873 7461 7274 292c 0d0a 2020   str(start),..  
-0000c490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4a0: 2020 2020 2020 222d 7422 2c20 7374 7228        "-t", str(
-0000c4b0: 656e 6420 2d20 7374 6172 7429 2c0d 0a20  end - start),.. 
-0000c4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4d0: 2020 2020 2020 2022 2d79 222c 0d0a 2020         "-y",..  
-0000c4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4f0: 2020 2020 2020 222d 6922 2c20 7365 6c66        "-i", self
-0000c500: 2e77 6176 5f66 696c 6570 6174 682c 0d0a  .wav_filepath,..
-0000c510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c520: 2020 2020 2020 2020 222d 6c6f 676c 6576          "-loglev
-0000c530: 656c 222c 2022 6572 726f 7222 2c0d 0a20  el", "error",.. 
-0000c540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c550: 2020 2020 2020 2074 656d 702e 6e61 6d65         temp.name
-0000c560: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c570: 2020 2020 2020 2020 5d0d 0a20 2020 2020          ]..     
-0000c580: 2020 2020 2020 2073 7562 7072 6f63 6573         subproces
-0000c590: 732e 6368 6563 6b5f 6f75 7470 7574 2863  s.check_output(c
-0000c5a0: 6f6d 6d61 6e64 2c20 7374 6469 6e3d 6f70  ommand, stdin=op
-0000c5b0: 656e 286f 732e 6465 766e 756c 6c29 290d  en(os.devnull)).
-0000c5c0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-0000c5d0: 7465 6e74 203d 2074 656d 702e 7265 6164  tent = temp.read
-0000c5e0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-0000c5f0: 7465 6d70 2e63 6c6f 7365 2829 0d0a 2020  temp.close()..  
-0000c600: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000c610: 2063 6f6e 7465 6e74 0d0a 0d0a 2020 2020   content....    
-0000c620: 2020 2020 6578 6365 7074 204b 6579 626f      except Keybo
-0000c630: 6172 6449 6e74 6572 7275 7074 3a0d 0a20  ardInterrupt:.. 
-0000c640: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000c650: 6c66 2e65 7272 6f72 5f6d 6573 7361 6765  lf.error_message
-0000c660: 735f 6361 6c6c 6261 636b 3a0d 0a20 2020  s_callback:..   
-0000c670: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000c680: 662e 6572 726f 725f 6d65 7373 6167 6573  f.error_messages
-0000c690: 5f63 616c 6c62 6163 6b28 2243 616e 6365  _callback("Cance
-0000c6a0: 6c6c 696e 6720 616c 6c20 7461 736b 7322  lling all tasks"
-0000c6b0: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-0000c6c0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-0000c6d0: 2020 2020 2020 7072 696e 7428 2243 616e        print("Can
-0000c6e0: 6365 6c6c 696e 6720 616c 6c20 7461 736b  celling all task
-0000c6f0: 7322 290d 0a20 2020 2020 2020 2020 2020  s")..           
-0000c700: 2072 6574 7572 6e0d 0a0d 0a20 2020 2020   return....     
-0000c710: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-0000c720: 696f 6e20 6173 2065 3a0d 0a20 2020 2020  ion as e:..     
-0000c730: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
-0000c740: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
-0000c750: 6c6c 6261 636b 3a0d 0a20 2020 2020 2020  llback:..       
-0000c760: 2020 2020 2020 2020 2073 656c 662e 6572           self.er
-0000c770: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
-0000c780: 6c62 6163 6b28 6529 0d0a 2020 2020 2020  lback(e)..      
-0000c790: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-0000c7a0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-0000c7b0: 6e74 2865 290d 0a20 2020 2020 2020 2020  nt(e)..         
-0000c7c0: 2020 2072 6574 7572 6e0d 0a0d 0a0d 0a63     return......c
-0000c7d0: 6c61 7373 2053 7065 6563 6852 6563 6f67  lass SpeechRecog
-0000c7e0: 6e69 7a65 7228 6f62 6a65 6374 293a 0d0a  nizer(object):..
-0000c7f0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-0000c800: 2873 656c 662c 206c 616e 6775 6167 653d  (self, language=
-0000c810: 2265 6e22 2c20 7261 7465 3d34 3431 3030  "en", rate=44100
-0000c820: 2c20 7265 7472 6965 733d 332c 2061 7069  , retries=3, api
-0000c830: 5f6b 6579 3d22 4149 7a61 5379 424f 7469  _key="AIzaSyBOti
-0000c840: 346d 4d2d 3678 3957 446e 5a49 6a49 6579  4mM-6x9WDnZIjIey
-0000c850: 4555 3231 4f70 4258 7157 4267 7722 2c20  EU21OpBXqWBgw", 
-0000c860: 7469 6d65 6f75 743d 3330 2c20 6572 726f  timeout=30, erro
-0000c870: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
-0000c880: 6163 6b3d 4e6f 6e65 293a 0d0a 2020 2020  ack=None):..    
-0000c890: 2020 2020 7365 6c66 2e6c 616e 6775 6167      self.languag
-0000c8a0: 6520 3d20 6c61 6e67 7561 6765 0d0a 2020  e = language..  
-0000c8b0: 2020 2020 2020 7365 6c66 2e72 6174 6520        self.rate 
-0000c8c0: 3d20 7261 7465 0d0a 2020 2020 2020 2020  = rate..        
-0000c8d0: 7365 6c66 2e61 7069 5f6b 6579 203d 2061  self.api_key = a
-0000c8e0: 7069 5f6b 6579 0d0a 2020 2020 2020 2020  pi_key..        
-0000c8f0: 7365 6c66 2e72 6574 7269 6573 203d 2072  self.retries = r
-0000c900: 6574 7269 6573 0d0a 2020 2020 2020 2020  etries..        
-0000c910: 7365 6c66 2e74 696d 656f 7574 203d 2074  self.timeout = t
-0000c920: 696d 656f 7574 0d0a 2020 2020 2020 2020  imeout..        
-0000c930: 7365 6c66 2e65 7272 6f72 5f6d 6573 7361  self.error_messa
-0000c940: 6765 735f 6361 6c6c 6261 636b 203d 2065  ges_callback = e
-0000c950: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
-0000c960: 6c6c 6261 636b 0d0a 0d0a 2020 2020 6465  llback....    de
-0000c970: 6620 5f5f 6361 6c6c 5f5f 2873 656c 662c  f __call__(self,
-0000c980: 2064 6174 6129 3a0d 0a20 2020 2020 2020   data):..       
-0000c990: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
-0000c9a0: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-0000c9b0: 6528 7365 6c66 2e72 6574 7269 6573 293a  e(self.retries):
-0000c9c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c9d0: 2020 7572 6c20 3d20 2268 7474 703a 2f2f    url = "http://
-0000c9e0: 7777 772e 676f 6f67 6c65 2e63 6f6d 2f73  www.google.com/s
-0000c9f0: 7065 6563 682d 6170 692f 7632 2f72 6563  peech-api/v2/rec
-0000ca00: 6f67 6e69 7a65 3f63 6c69 656e 743d 6368  ognize?client=ch
-0000ca10: 726f 6d69 756d 266c 616e 673d 7b6c 616e  romium&lang={lan
-0000ca20: 677d 266b 6579 3d7b 6b65 797d 222e 666f  g}&key={key}".fo
-0000ca30: 726d 6174 286c 616e 673d 7365 6c66 2e6c  rmat(lang=self.l
-0000ca40: 616e 6775 6167 652c 206b 6579 3d73 656c  anguage, key=sel
-0000ca50: 662e 6170 695f 6b65 7929 0d0a 2020 2020  f.api_key)..    
-0000ca60: 2020 2020 2020 2020 2020 2020 6865 6164              head
-0000ca70: 6572 7320 3d20 7b22 436f 6e74 656e 742d  ers = {"Content-
-0000ca80: 5479 7065 223a 2022 6175 6469 6f2f 782d  Type": "audio/x-
-0000ca90: 666c 6163 2072 6174 653d 2564 2220 2520  flac rate=%d" % 
-0000caa0: 7365 6c66 2e72 6174 657d 0d0a 0d0a 2020  self.rate}....  
-0000cab0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-0000cac0: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
-0000cad0: 2020 2020 2020 2020 7265 7370 203d 2072          resp = r
-0000cae0: 6571 7565 7374 732e 706f 7374 2875 726c  equests.post(url
-0000caf0: 2c20 6461 7461 3d64 6174 612c 2068 6561  , data=data, hea
-0000cb00: 6465 7273 3d68 6561 6465 7273 2c20 7469  ders=headers, ti
-0000cb10: 6d65 6f75 743d 7365 6c66 2e74 696d 656f  meout=self.timeo
-0000cb20: 7574 290d 0a20 2020 2020 2020 2020 2020  ut)..           
-0000cb30: 2020 2020 2065 7863 6570 7420 7265 7175       except requ
-0000cb40: 6573 7473 2e65 7863 6570 7469 6f6e 732e  ests.exceptions.
-0000cb50: 436f 6e6e 6563 7469 6f6e 4572 726f 723a  ConnectionError:
-0000cb60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000cb70: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
-0000cb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb90: 2020 2020 7265 7370 203d 2068 7474 7078      resp = httpx
-0000cba0: 2e70 6f73 7428 7572 6c2c 2064 6174 613d  .post(url, data=
-0000cbb0: 6461 7461 2c20 6865 6164 6572 733d 6865  data, headers=he
-0000cbc0: 6164 6572 732c 2074 696d 656f 7574 3d73  aders, timeout=s
-0000cbd0: 656c 662e 7469 6d65 6f75 7429 0d0a 2020  elf.timeout)..  
-0000cbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cbf0: 2020 6578 6365 7074 2068 7474 7078 2e65    except httpx.e
-0000cc00: 7863 6570 7469 6f6e 732e 4e65 7477 6f72  xceptions.Networ
-0000cc10: 6b45 7272 6f72 3a0d 0a20 2020 2020 2020  kError:..       
-0000cc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc30: 2063 6f6e 7469 6e75 650d 0a0d 0a20 2020   continue....   
-0000cc40: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000cc50: 206c 696e 6520 696e 2072 6573 702e 636f   line in resp.co
-0000cc60: 6e74 656e 742e 6465 636f 6465 2827 7574  ntent.decode('ut
-0000cc70: 662d 3827 292e 7370 6c69 7428 225c 6e22  f-8').split("\n"
-0000cc80: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0000cc90: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
-0000cca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ccb0: 2020 2020 2020 6c69 6e65 203d 206a 736f        line = jso
-0000ccc0: 6e2e 6c6f 6164 7328 6c69 6e65 290d 0a20  n.loads(line).. 
-0000ccd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cce0: 2020 2020 2020 206c 696e 6520 3d20 6c69         line = li
-0000ccf0: 6e65 5b27 7265 7375 6c74 275d 5b30 5d5b  ne['result'][0][
-0000cd00: 2761 6c74 6572 6e61 7469 7665 275d 5b30  'alternative'][0
-0000cd10: 5d5b 2774 7261 6e73 6372 6970 7427 5d0d  ]['transcript'].
-0000cd20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cd30: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000cd40: 6c69 6e65 5b3a 315d 2e75 7070 6572 2829  line[:1].upper()
-0000cd50: 202b 206c 696e 655b 313a 5d0d 0a20 2020   + line[1:]..   
-0000cd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd70: 2065 7863 6570 743a 0d0a 2020 2020 2020   except:..      
-0000cd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd90: 2020 2320 6e6f 2072 6573 756c 740d 0a20    # no result.. 
-0000cda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cdb0: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
-0000cdc0: 0a0d 0a20 2020 2020 2020 2065 7863 6570  ...        excep
-0000cdd0: 7420 4b65 7962 6f61 7264 496e 7465 7272  t KeyboardInterr
-0000cde0: 7570 743a 0d0a 2020 2020 2020 2020 2020  upt:..          
-0000cdf0: 2020 6966 2073 656c 662e 6572 726f 725f    if self.error_
-0000ce00: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
-0000ce10: 6b3a 0d0a 2020 2020 2020 2020 2020 2020  k:..            
-0000ce20: 2020 2020 7365 6c66 2e65 7272 6f72 5f6d      self.error_m
-0000ce30: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
-0000ce40: 2822 4361 6e63 656c 6c69 6e67 2061 6c6c  ("Cancelling all
-0000ce50: 2074 6173 6b73 2229 0d0a 2020 2020 2020   tasks")..      
-0000ce60: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-0000ce70: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-0000ce80: 6e74 2822 4361 6e63 656c 6c69 6e67 2061  nt("Cancelling a
-0000ce90: 6c6c 2074 6173 6b73 2229 0d0a 2020 2020  ll tasks")..    
-0000cea0: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
-0000ceb0: 0d0a 2020 2020 2020 2020 6578 6365 7074  ..        except
-0000cec0: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
-0000ced0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-0000cee0: 2073 656c 662e 6572 726f 725f 6d65 7373   self.error_mess
-0000cef0: 6167 6573 5f63 616c 6c62 6163 6b3a 0d0a  ages_callback:..
-0000cf00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf10: 7365 6c66 2e65 7272 6f72 5f6d 6573 7361  self.error_messa
-0000cf20: 6765 735f 6361 6c6c 6261 636b 2865 290d  ges_callback(e).
-0000cf30: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0000cf40: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0000cf50: 2020 2020 7072 696e 7428 6529 0d0a 2020      print(e)..  
-0000cf60: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000cf70: 0d0a 0d0a 0d0a 636c 6173 7320 5768 6973  ......class Whis
-0000cf80: 7065 7252 6563 6f67 6e69 7a65 7228 6f62  perRecognizer(ob
-0000cf90: 6a65 6374 293a 0d0a 2020 2020 6465 6620  ject):..    def 
-0000cfa0: 5f5f 696e 6974 5f5f 2873 656c 662c 206d  __init__(self, m
-0000cfb0: 6f64 656c 3d22 736d 616c 6c22 2c20 6c61  odel="small", la
-0000cfc0: 6e67 7561 6765 3d22 656e 222c 2066 7031  nguage="en", fp1
-0000cfd0: 363d 4661 6c73 652c 2074 6173 6b3d 2274  6=False, task="t
-0000cfe0: 7261 6e73 6372 6962 6522 2c20 7665 7262  ranscribe", verb
-0000cff0: 6f73 653d 4661 6c73 652c 2065 7272 6f72  ose=False, error
-0000d000: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
-0000d010: 636b 3d4e 6f6e 6529 3a0d 0a20 2020 2020  ck=None):..     
-0000d020: 2020 2073 656c 662e 6d6f 6465 6c20 3d20     self.model = 
-0000d030: 6d6f 6465 6c0d 0a20 2020 2020 2020 2073  model..        s
-0000d040: 656c 662e 6c61 6e67 7561 6765 203d 206c  elf.language = l
-0000d050: 616e 6775 6167 650d 0a20 2020 2020 2020  anguage..       
-0000d060: 2073 656c 662e 6670 3136 203d 2066 7031   self.fp16 = fp1
-0000d070: 360d 0a20 2020 2020 2020 2073 656c 662e  6..        self.
-0000d080: 7461 736b 203d 2074 6173 6b0d 0a20 2020  task = task..   
-0000d090: 2020 2020 2073 656c 662e 7665 7262 6f73       self.verbos
-0000d0a0: 6520 3d20 7665 7262 6f73 650d 0a20 2020  e = verbose..   
-0000d0b0: 2020 2020 2073 656c 662e 6572 726f 725f       self.error_
-0000d0c0: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
-0000d0d0: 6b20 3d20 6572 726f 725f 6d65 7373 6167  k = error_messag
-0000d0e0: 6573 5f63 616c 6c62 6163 6b0d 0a0d 0a20  es_callback.... 
-0000d0f0: 2020 2064 6566 205f 5f63 616c 6c5f 5f28     def __call__(
-0000d100: 7365 6c66 2c20 6175 6469 6f5f 7061 7468  self, audio_path
-0000d110: 293a 0d0a 2020 2020 2020 2020 7472 793a  ):..        try:
-0000d120: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-0000d130: 7375 6c74 203d 2073 656c 662e 6d6f 6465  sult = self.mode
-0000d140: 6c2e 7472 616e 7363 7269 6265 2861 7564  l.transcribe(aud
-0000d150: 696f 5f70 6174 682c 206c 616e 6775 6167  io_path, languag
-0000d160: 653d 7365 6c66 2e6c 616e 6775 6167 652c  e=self.language,
-0000d170: 2066 7031 363d 7365 6c66 2e66 7031 362c   fp16=self.fp16,
-0000d180: 2074 6173 6b3d 7365 6c66 2e74 6173 6b2c   task=self.task,
-0000d190: 2076 6572 626f 7365 3d73 656c 662e 7665   verbose=self.ve
-0000d1a0: 7262 6f73 6529 0d0a 2020 2020 2020 2020  rbose)..        
-0000d1b0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-0000d1c0: 740d 0a0d 0a20 2020 2020 2020 2065 7863  t....        exc
-0000d1d0: 6570 7420 4b65 7962 6f61 7264 496e 7465  ept KeyboardInte
-0000d1e0: 7272 7570 743a 0d0a 2020 2020 2020 2020  rrupt:..        
-0000d1f0: 2020 2020 6966 2073 656c 662e 6572 726f      if self.erro
-0000d200: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
-0000d210: 6163 6b3a 0d0a 2020 2020 2020 2020 2020  ack:..          
-0000d220: 2020 2020 2020 7365 6c66 2e65 7272 6f72        self.error
-0000d230: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
-0000d240: 636b 2822 4361 6e63 656c 6c69 6e67 2061  ck("Cancelling a
-0000d250: 6c6c 2074 6173 6b73 2229 0d0a 2020 2020  ll tasks")..    
-0000d260: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-0000d270: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000d280: 7269 6e74 2822 4361 6e63 656c 6c69 6e67  rint("Cancelling
-0000d290: 2061 6c6c 2074 6173 6b73 2229 0d0a 2020   all tasks")..  
-0000d2a0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000d2b0: 0d0a 0d0a 2020 2020 2020 2020 6578 6365  ....        exce
-0000d2c0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-0000d2d0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0000d2e0: 6966 2073 656c 662e 6572 726f 725f 6d65  if self.error_me
-0000d2f0: 7373 6167 6573 5f63 616c 6c62 6163 6b3a  ssages_callback:
-0000d300: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d310: 2020 7365 6c66 2e65 7272 6f72 5f6d 6573    self.error_mes
-0000d320: 7361 6765 735f 6361 6c6c 6261 636b 2865  sages_callback(e
-0000d330: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-0000d340: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-0000d350: 2020 2020 2020 7072 696e 7428 6529 0d0a        print(e)..
-0000d360: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000d370: 726e 0d0a 0d0a 0d0a 636c 6173 7320 5365  rn......class Se
-0000d380: 6e74 656e 6365 5472 616e 736c 6174 6f72  ntenceTranslator
-0000d390: 286f 626a 6563 7429 3a0d 0a20 2020 2064  (object):..    d
-0000d3a0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-0000d3b0: 2c20 7372 632c 2064 7374 2c20 7061 7469  , src, dst, pati
-0000d3c0: 656e 6365 3d2d 312c 2074 696d 656f 7574  ence=-1, timeout
-0000d3d0: 3d33 302c 2065 7272 6f72 5f6d 6573 7361  =30, error_messa
-0000d3e0: 6765 735f 6361 6c6c 6261 636b 3d4e 6f6e  ges_callback=Non
-0000d3f0: 6529 3a0d 0a20 2020 2020 2020 2073 656c  e):..        sel
-0000d400: 662e 7372 6320 3d20 7372 630d 0a20 2020  f.src = src..   
-0000d410: 2020 2020 2073 656c 662e 6473 7420 3d20       self.dst = 
-0000d420: 6473 740d 0a20 2020 2020 2020 2073 656c  dst..        sel
-0000d430: 662e 7061 7469 656e 6365 203d 2070 6174  f.patience = pat
-0000d440: 6965 6e63 650d 0a20 2020 2020 2020 2073  ience..        s
-0000d450: 656c 662e 7469 6d65 6f75 7420 3d20 7469  elf.timeout = ti
-0000d460: 6d65 6f75 740d 0a20 2020 2020 2020 2073  meout..        s
-0000d470: 656c 662e 6572 726f 725f 6d65 7373 6167  elf.error_messag
-0000d480: 6573 5f63 616c 6c62 6163 6b20 3d20 6572  es_callback = er
-0000d490: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
-0000d4a0: 6c62 6163 6b0d 0a0d 0a20 2020 2064 6566  lback....    def
-0000d4b0: 205f 5f63 616c 6c5f 5f28 7365 6c66 2c20   __call__(self, 
-0000d4c0: 7365 6e74 656e 6365 293a 0d0a 2020 2020  sentence):..    
-0000d4d0: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
-0000d4e0: 2020 2020 2020 7472 616e 736c 6174 6564        translated
-0000d4f0: 5f73 656e 7465 6e63 6520 3d20 5b5d 0d0a  _sentence = []..
-0000d500: 2020 2020 2020 2020 2020 2020 2320 6861              # ha
-0000d510: 6e64 6c65 2074 6865 2073 7065 6369 616c  ndle the special
-0000d520: 2063 6173 653a 2065 6d70 7479 2073 7472   case: empty str
-0000d530: 696e 672e 0d0a 2020 2020 2020 2020 2020  ing...          
-0000d540: 2020 6966 206e 6f74 2073 656e 7465 6e63    if not sentenc
-0000d550: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0000d560: 2020 2020 7265 7475 726e 204e 6f6e 650d      return None.
-0000d570: 0a20 2020 2020 2020 2020 2020 2074 7261  .            tra
-0000d580: 6e73 6c61 7465 645f 7365 6e74 656e 6365  nslated_sentence
-0000d590: 203d 2073 656c 662e 476f 6f67 6c65 5472   = self.GoogleTr
-0000d5a0: 616e 736c 6174 6528 7365 6e74 656e 6365  anslate(sentence
-0000d5b0: 2c20 7372 633d 7365 6c66 2e73 7263 2c20  , src=self.src, 
-0000d5c0: 6473 743d 7365 6c66 2e64 7374 2c20 7469  dst=self.dst, ti
-0000d5d0: 6d65 6f75 743d 7365 6c66 2e74 696d 656f  meout=self.timeo
-0000d5e0: 7574 290d 0a20 2020 2020 2020 2020 2020  ut)..           
-0000d5f0: 2066 6169 6c5f 746f 5f74 7261 6e73 6c61   fail_to_transla
-0000d600: 7465 203d 2074 7261 6e73 6c61 7465 645f  te = translated_
-0000d610: 7365 6e74 656e 6365 5b2d 315d 203d 3d20  sentence[-1] == 
-0000d620: 275c 6e27 0d0a 2020 2020 2020 2020 2020  '\n'..          
-0000d630: 2020 7768 696c 6520 6661 696c 5f74 6f5f    while fail_to_
-0000d640: 7472 616e 736c 6174 6520 616e 6420 7061  translate and pa
-0000d650: 7469 656e 6365 3a0d 0a20 2020 2020 2020  tience:..       
-0000d660: 2020 2020 2020 2020 2074 7261 6e73 6c61           transla
-0000d670: 7465 645f 7365 6e74 656e 6365 203d 2073  ted_sentence = s
-0000d680: 656c 662e 476f 6f67 6c65 5472 616e 736c  elf.GoogleTransl
-0000d690: 6174 6528 7472 616e 736c 6174 6564 5f73  ate(translated_s
-0000d6a0: 656e 7465 6e63 652c 2073 7263 3d73 656c  entence, src=sel
-0000d6b0: 662e 7372 632c 2064 7374 3d73 656c 662e  f.src, dst=self.
-0000d6c0: 6473 742c 2074 696d 656f 7574 3d73 656c  dst, timeout=sel
-0000d6d0: 662e 7469 6d65 6f75 7429 2e74 6578 740d  f.timeout).text.
-0000d6e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d6f0: 2069 6620 7472 616e 736c 6174 6564 5f73   if translated_s
-0000d700: 656e 7465 6e63 655b 2d31 5d20 3d3d 2027  entence[-1] == '
-0000d710: 5c6e 273a 0d0a 2020 2020 2020 2020 2020  \n':..          
-0000d720: 2020 2020 2020 2020 2020 6966 2070 6174            if pat
-0000d730: 6965 6e63 6520 3d3d 202d 313a 0d0a 2020  ience == -1:..  
-0000d740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d750: 2020 2020 2020 636f 6e74 696e 7565 0d0a        continue..
-0000d760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d770: 2020 2020 7061 7469 656e 6365 202d 3d20      patience -= 
-0000d780: 310d 0a20 2020 2020 2020 2020 2020 2020  1..             
-0000d790: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-0000d7a0: 2020 2020 2020 2020 2020 2020 2020 6661                fa
-0000d7b0: 696c 5f74 6f5f 7472 616e 736c 6174 6520  il_to_translate 
-0000d7c0: 3d20 4661 6c73 650d 0a0d 0a20 2020 2020  = False....     
-0000d7d0: 2020 2020 2020 2072 6574 7572 6e20 7472         return tr
-0000d7e0: 616e 736c 6174 6564 5f73 656e 7465 6e63  anslated_sentenc
-0000d7f0: 650d 0a0d 0a20 2020 2020 2020 2065 7863  e....        exc
-0000d800: 6570 7420 4b65 7962 6f61 7264 496e 7465  ept KeyboardInte
-0000d810: 7272 7570 743a 0d0a 2020 2020 2020 2020  rrupt:..        
-0000d820: 2020 2020 6966 2073 656c 662e 6572 726f      if self.erro
-0000d830: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
-0000d840: 6163 6b3a 0d0a 2020 2020 2020 2020 2020  ack:..          
-0000d850: 2020 2020 2020 7365 6c66 2e65 7272 6f72        self.error
-0000d860: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
-0000d870: 636b 2822 4361 6e63 656c 6c69 6e67 2061  ck("Cancelling a
-0000d880: 6c6c 2074 6173 6b73 2229 0d0a 2020 2020  ll tasks")..    
-0000d890: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-0000d8a0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000d8b0: 7269 6e74 2822 4361 6e63 656c 6c69 6e67  rint("Cancelling
-0000d8c0: 2061 6c6c 2074 6173 6b73 2229 0d0a 2020   all tasks")..  
-0000d8d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000d8e0: 0d0a 0d0a 2020 2020 2020 2020 6578 6365  ....        exce
-0000d8f0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-0000d900: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0000d910: 6966 2073 656c 662e 6572 726f 725f 6d65  if self.error_me
-0000d920: 7373 6167 6573 5f63 616c 6c62 6163 6b3a  ssages_callback:
-0000d930: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d940: 2020 7365 6c66 2e65 7272 6f72 5f6d 6573    self.error_mes
-0000d950: 7361 6765 735f 6361 6c6c 6261 636b 2865  sages_callback(e
-0000d960: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-0000d970: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-0000d980: 2020 2020 2020 7072 696e 7428 6529 0d0a        print(e)..
-0000d990: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000d9a0: 726e 0d0a 0d0a 2020 2020 6465 6620 476f  rn....    def Go
-0000d9b0: 6f67 6c65 5472 616e 736c 6174 6528 7365  ogleTranslate(se
-0000d9c0: 6c66 2c20 7465 7874 2c20 7372 632c 2064  lf, text, src, d
-0000d9d0: 7374 2c20 7469 6d65 6f75 743d 3330 293a  st, timeout=30):
-0000d9e0: 0d0a 2020 2020 2020 2020 7572 6c20 3d20  ..        url = 
-0000d9f0: 2768 7474 7073 3a2f 2f74 7261 6e73 6c61  'https://transla
-0000da00: 7465 2e67 6f6f 676c 6561 7069 732e 636f  te.googleapis.co
-0000da10: 6d2f 7472 616e 736c 6174 655f 612f 270d  m/translate_a/'.
-0000da20: 0a20 2020 2020 2020 2070 6172 616d 7320  .        params 
-0000da30: 3d20 2773 696e 676c 653f 636c 6965 6e74  = 'single?client
-0000da40: 3d67 7478 2673 6c3d 272b 7372 632b 2726  =gtx&sl='+src+'&
-0000da50: 746c 3d27 2b64 7374 2b27 2664 743d 7426  tl='+dst+'&dt=t&
-0000da60: 713d 272b 7465 7874 3b0d 0a20 2020 2020  q='+text;..     
-0000da70: 2020 2068 6561 6465 7273 203d 207b 2755     headers = {'U
-0000da80: 7365 722d 4167 656e 7427 3a20 274d 6f7a  ser-Agent': 'Moz
-0000da90: 696c 6c61 2f35 2e30 2028 5769 6e64 6f77  illa/5.0 (Window
-0000daa0: 7320 4e54 2031 302e 303b 2057 696e 3634  s NT 10.0; Win64
-0000dab0: 3b20 7836 3429 272c 2027 5265 6665 7265  ; x64)', 'Refere
-0000dac0: 7227 3a20 2768 7474 7073 3a2f 2f74 7261  r': 'https://tra
-0000dad0: 6e73 6c61 7465 2e67 6f6f 676c 652e 636f  nslate.google.co
-0000dae0: 6d27 2c7d 0d0a 0d0a 2020 2020 2020 2020  m',}....        
-0000daf0: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-0000db00: 2020 7265 7370 6f6e 7365 203d 2072 6571    response = req
-0000db10: 7565 7374 732e 6765 7428 7572 6c2b 7061  uests.get(url+pa
-0000db20: 7261 6d73 2c20 6865 6164 6572 733d 6865  rams, headers=he
-0000db30: 6164 6572 732c 2074 696d 656f 7574 3d73  aders, timeout=s
-0000db40: 656c 662e 7469 6d65 6f75 7429 0d0a 2020  elf.timeout)..  
-0000db50: 2020 2020 2020 2020 2020 6966 2072 6573            if res
-0000db60: 706f 6e73 652e 7374 6174 7573 5f63 6f64  ponse.status_cod
-0000db70: 6520 3d3d 2032 3030 3a0d 0a20 2020 2020  e == 200:..     
-0000db80: 2020 2020 2020 2020 2020 2072 6573 706f             respo
-0000db90: 6e73 655f 6a73 6f6e 203d 2072 6573 706f  nse_json = respo
-0000dba0: 6e73 652e 6a73 6f6e 2829 5b30 5d0d 0a20  nse.json()[0].. 
-0000dbb0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0000dbc0: 656e 6774 6820 3d20 6c65 6e28 7265 7370  ength = len(resp
-0000dbd0: 6f6e 7365 5f6a 736f 6e29 0d0a 2020 2020  onse_json)..    
-0000dbe0: 2020 2020 2020 2020 2020 2020 7472 616e              tran
-0000dbf0: 736c 6174 696f 6e20 3d20 2222 0d0a 2020  slation = ""..  
-0000dc00: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0000dc10: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
-0000dc20: 6774 6829 3a0d 0a20 2020 2020 2020 2020  gth):..         
-0000dc30: 2020 2020 2020 2020 2020 2074 7261 6e73             trans
-0000dc40: 6c61 7469 6f6e 203d 2074 7261 6e73 6c61  lation = transla
-0000dc50: 7469 6f6e 202b 2072 6573 706f 6e73 655f  tion + response_
-0000dc60: 6a73 6f6e 5b69 5d5b 305d 0d0a 2020 2020  json[i][0]..    
-0000dc70: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000dc80: 726e 2074 7261 6e73 6c61 7469 6f6e 0d0a  rn translation..
-0000dc90: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000dca0: 726e 0d0a 0d0a 2020 2020 2020 2020 6578  rn....        ex
-0000dcb0: 6365 7074 2072 6571 7565 7374 732e 6578  cept requests.ex
-0000dcc0: 6365 7074 696f 6e73 2e43 6f6e 6e65 6374  ceptions.Connect
-0000dcd0: 696f 6e45 7272 6f72 3a0d 0a20 2020 2020  ionError:..     
-0000dce0: 2020 2020 2020 2077 6974 6820 6874 7470         with http
-0000dcf0: 782e 436c 6965 6e74 2829 2061 7320 636c  x.Client() as cl
-0000dd00: 6965 6e74 3a0d 0a20 2020 2020 2020 2020  ient:..         
-0000dd10: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
-0000dd20: 3d20 636c 6965 6e74 2e67 6574 2875 726c  = client.get(url
-0000dd30: 2b70 6172 616d 732c 2068 6561 6465 7273  +params, headers
-0000dd40: 3d68 6561 6465 7273 2c20 7469 6d65 6f75  =headers, timeou
-0000dd50: 743d 7365 6c66 2e74 696d 656f 7574 290d  t=self.timeout).
-0000dd60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dd70: 2069 6620 7265 7370 6f6e 7365 2e73 7461   if response.sta
-0000dd80: 7475 735f 636f 6465 203d 3d20 3230 303a  tus_code == 200:
-0000dd90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000dda0: 2020 2020 2020 7265 7370 6f6e 7365 5f6a        response_j
-0000ddb0: 736f 6e20 3d20 7265 7370 6f6e 7365 2e6a  son = response.j
-0000ddc0: 736f 6e28 295b 305d 0d0a 2020 2020 2020  son()[0]..      
-0000ddd0: 2020 2020 2020 2020 2020 2020 2020 6c65                le
-0000dde0: 6e67 7468 203d 206c 656e 2872 6573 706f  ngth = len(respo
-0000ddf0: 6e73 655f 6a73 6f6e 290d 0a20 2020 2020  nse_json)..     
-0000de00: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000de10: 7261 6e73 6c61 7469 6f6e 203d 2022 220d  ranslation = "".
-0000de20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000de30: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-0000de40: 6e67 6528 6c65 6e67 7468 293a 0d0a 2020  nge(length):..  
-0000de50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de60: 2020 2020 2020 7472 616e 736c 6174 696f        translatio
-0000de70: 6e20 3d20 7472 616e 736c 6174 696f 6e20  n = translation 
-0000de80: 2b20 7265 7370 6f6e 7365 5f6a 736f 6e5b  + response_json[
-0000de90: 695d 5b30 5d0d 0a20 2020 2020 2020 2020  i][0]..         
-0000dea0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000deb0: 6e20 7472 616e 736c 6174 696f 6e0d 0a20  n translation.. 
-0000dec0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000ded0: 6574 7572 6e0d 0a0d 0a20 2020 2020 2020  eturn....       
-0000dee0: 2065 7863 6570 7420 4b65 7962 6f61 7264   except Keyboard
-0000def0: 496e 7465 7272 7570 743a 0d0a 2020 2020  Interrupt:..    
-0000df00: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000df10: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
-0000df20: 616c 6c62 6163 6b3a 0d0a 2020 2020 2020  allback:..      
-0000df30: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
-0000df40: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
-0000df50: 6c6c 6261 636b 2822 4361 6e63 656c 6c69  llback("Cancelli
-0000df60: 6e67 2061 6c6c 2074 6173 6b73 2229 0d0a  ng all tasks")..
-0000df70: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000df80: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000df90: 2020 2070 7269 6e74 2822 4361 6e63 656c     print("Cancel
-0000dfa0: 6c69 6e67 2061 6c6c 2074 6173 6b73 2229  ling all tasks")
-0000dfb0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-0000dfc0: 7475 726e 0d0a 0d0a 2020 2020 2020 2020  turn....        
-0000dfd0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-0000dfe0: 2061 7320 653a 0d0a 2020 2020 2020 2020   as e:..        
-0000dff0: 2020 2020 6966 2073 656c 662e 6572 726f      if self.erro
-0000e000: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
-0000e010: 6163 6b3a 0d0a 2020 2020 2020 2020 2020  ack:..          
-0000e020: 2020 2020 2020 7365 6c66 2e65 7272 6f72        self.error
-0000e030: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
-0000e040: 636b 2865 290d 0a20 2020 2020 2020 2020  ck(e)..         
-0000e050: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-0000e060: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-0000e070: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-0000e080: 7265 7475 726e 0d0a 0d0a 0d0a 636c 6173  return......clas
-0000e090: 7320 5375 6274 6974 6c65 466f 726d 6174  s SubtitleFormat
-0000e0a0: 7465 723a 0d0a 2020 2020 7375 7070 6f72  ter:..    suppor
-0000e0b0: 7465 645f 666f 726d 6174 7320 3d20 5b27  ted_formats = ['
-0000e0c0: 7372 7427 2c20 2776 7474 272c 2027 6a73  srt', 'vtt', 'js
-0000e0d0: 6f6e 272c 2027 7261 7727 5d0d 0a0d 0a20  on', 'raw'].... 
-0000e0e0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-0000e0f0: 7365 6c66 2c20 666f 726d 6174 5f74 7970  self, format_typ
-0000e100: 652c 2065 7272 6f72 5f6d 6573 7361 6765  e, error_message
-0000e110: 735f 6361 6c6c 6261 636b 3d4e 6f6e 6529  s_callback=None)
-0000e120: 3a0d 0a20 2020 2020 2020 2073 656c 662e  :..        self.
-0000e130: 666f 726d 6174 5f74 7970 6520 3d20 666f  format_type = fo
-0000e140: 726d 6174 5f74 7970 652e 6c6f 7765 7228  rmat_type.lower(
-0000e150: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-0000e160: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
-0000e170: 616c 6c62 6163 6b20 3d20 6572 726f 725f  allback = error_
-0000e180: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
-0000e190: 6b0d 0a20 2020 2020 2020 200d 0a20 2020  k..        ..   
-0000e1a0: 2064 6566 205f 5f63 616c 6c5f 5f28 7365   def __call__(se
-0000e1b0: 6c66 2c20 7375 6274 6974 6c65 732c 2070  lf, subtitles, p
-0000e1c0: 6164 6469 6e67 5f62 6566 6f72 653d 302c  adding_before=0,
-0000e1d0: 2070 6164 6469 6e67 5f61 6674 6572 3d30   padding_after=0
-0000e1e0: 293a 0d0a 2020 2020 2020 2020 7472 793a  ):..        try:
-0000e1f0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-0000e200: 2073 656c 662e 666f 726d 6174 5f74 7970   self.format_typ
-0000e210: 6520 3d3d 2027 7372 7427 3a0d 0a20 2020  e == 'srt':..   
-0000e220: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-0000e230: 7572 6e20 7365 6c66 2e73 7274 5f66 6f72  urn self.srt_for
-0000e240: 6d61 7474 6572 2873 7562 7469 746c 6573  matter(subtitles
-0000e250: 2c20 7061 6464 696e 675f 6265 666f 7265  , padding_before
-0000e260: 2c20 7061 6464 696e 675f 6166 7465 7229  , padding_after)
-0000e270: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-0000e280: 6966 2073 656c 662e 666f 726d 6174 5f74  if self.format_t
-0000e290: 7970 6520 3d3d 2027 7674 7427 3a0d 0a20  ype == 'vtt':.. 
-0000e2a0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000e2b0: 6574 7572 6e20 7365 6c66 2e76 7474 5f66  eturn self.vtt_f
-0000e2c0: 6f72 6d61 7474 6572 2873 7562 7469 746c  ormatter(subtitl
-0000e2d0: 6573 2c20 7061 6464 696e 675f 6265 666f  es, padding_befo
-0000e2e0: 7265 2c20 7061 6464 696e 675f 6166 7465  re, padding_afte
-0000e2f0: 7229 0d0a 2020 2020 2020 2020 2020 2020  r)..            
-0000e300: 656c 6966 2073 656c 662e 666f 726d 6174  elif self.format
-0000e310: 5f74 7970 6520 3d3d 2027 6a73 6f6e 273a  _type == 'json':
-0000e320: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e330: 2020 7265 7475 726e 2073 656c 662e 6a73    return self.js
-0000e340: 6f6e 5f66 6f72 6d61 7474 6572 2873 7562  on_formatter(sub
-0000e350: 7469 746c 6573 290d 0a20 2020 2020 2020  titles)..       
-0000e360: 2020 2020 2065 6c69 6620 7365 6c66 2e66       elif self.f
-0000e370: 6f72 6d61 745f 7479 7065 203d 3d20 2772  ormat_type == 'r
-0000e380: 6177 273a 0d0a 2020 2020 2020 2020 2020  aw':..          
-0000e390: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000e3a0: 662e 7261 775f 666f 726d 6174 7465 7228  f.raw_formatter(
-0000e3b0: 7375 6274 6974 6c65 7329 0d0a 2020 2020  subtitles)..    
-0000e3c0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-0000e3d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000e3e0: 6620 6572 726f 725f 6d65 7373 6167 6573  f error_messages
-0000e3f0: 5f63 616c 6c62 6163 6b3a 0d0a 2020 2020  _callback:..    
-0000e400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e410: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
-0000e420: 616c 6c62 6163 6b28 6627 556e 7375 7070  allback(f'Unsupp
-0000e430: 6f72 7465 6420 666f 726d 6174 2074 7970  orted format typ
-0000e440: 653a 207b 7365 6c66 2e66 6f72 6d61 745f  e: {self.format_
-0000e450: 7479 7065 7d27 290d 0a20 2020 2020 2020  type}')..       
-0000e460: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-0000e470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e480: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-0000e490: 7272 6f72 2866 2755 6e73 7570 706f 7274  rror(f'Unsupport
-0000e4a0: 6564 2066 6f72 6d61 7420 7479 7065 3a20  ed format type: 
-0000e4b0: 7b73 656c 662e 666f 726d 6174 5f74 7970  {self.format_typ
-0000e4c0: 657d 2729 0d0a 0d0a 2020 2020 2020 2020  e}')....        
-0000e4d0: 6578 6365 7074 204b 6579 626f 6172 6449  except KeyboardI
-0000e4e0: 6e74 6572 7275 7074 3a0d 0a20 2020 2020  nterrupt:..     
-0000e4f0: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
-0000e500: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
-0000e510: 6c6c 6261 636b 3a0d 0a20 2020 2020 2020  llback:..       
-0000e520: 2020 2020 2020 2020 2073 656c 662e 6572           self.er
-0000e530: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
-0000e540: 6c62 6163 6b28 2243 616e 6365 6c6c 696e  lback("Cancellin
-0000e550: 6720 616c 6c20 7461 736b 7322 290d 0a20  g all tasks").. 
-0000e560: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000e570: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e580: 2020 7072 696e 7428 2243 616e 6365 6c6c    print("Cancell
-0000e590: 696e 6720 616c 6c20 7461 736b 7322 290d  ing all tasks").
-0000e5a0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000e5b0: 7572 6e0d 0a0d 0a20 2020 2020 2020 2065  urn....        e
-0000e5c0: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
-0000e5d0: 6173 2065 3a0d 0a20 2020 2020 2020 2020  as e:..         
-0000e5e0: 2020 2069 6620 7365 6c66 2e65 7272 6f72     if self.error
-0000e5f0: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
-0000e600: 636b 3a0d 0a20 2020 2020 2020 2020 2020  ck:..           
-0000e610: 2020 2020 2073 656c 662e 6572 726f 725f       self.error_
-0000e620: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
-0000e630: 6b28 6529 0d0a 2020 2020 2020 2020 2020  k(e)..          
-0000e640: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-0000e650: 2020 2020 2020 2020 2070 7269 6e74 2865           print(e
-0000e660: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
-0000e670: 6574 7572 6e0d 0a0d 0a20 2020 2064 6566  eturn....    def
-0000e680: 2073 7274 5f66 6f72 6d61 7474 6572 2873   srt_formatter(s
-0000e690: 656c 662c 2073 7562 7469 746c 6573 2c20  elf, subtitles, 
-0000e6a0: 7061 6464 696e 675f 6265 666f 7265 3d30  padding_before=0
-0000e6b0: 2c20 7061 6464 696e 675f 6166 7465 723d  , padding_after=
-0000e6c0: 3029 3a0d 0a20 2020 2020 2020 2022 2222  0):..        """
-0000e6d0: 0d0a 2020 2020 2020 2020 5365 7269 616c  ..        Serial
-0000e6e0: 697a 6520 6120 6c69 7374 206f 6620 7375  ize a list of su
-0000e6f0: 6274 6974 6c65 7320 6163 636f 7264 696e  btitles accordin
-0000e700: 6720 746f 2074 6865 2053 5254 2066 6f72  g to the SRT for
-0000e710: 6d61 742c 2077 6974 6820 6f70 7469 6f6e  mat, with option
-0000e720: 616c 2074 696d 6520 7061 6464 696e 672e  al time padding.
-0000e730: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-0000e740: 2020 2020 2020 2073 7562 5f72 6970 5f66         sub_rip_f
-0000e750: 696c 6520 3d20 7079 7372 742e 5375 6252  ile = pysrt.SubR
-0000e760: 6970 4669 6c65 2829 0d0a 2020 2020 2020  ipFile()..      
-0000e770: 2020 666f 7220 692c 2028 2873 7461 7274    for i, ((start
-0000e780: 2c20 656e 6429 2c20 7465 7874 2920 696e  , end), text) in
-0000e790: 2065 6e75 6d65 7261 7465 2873 7562 7469   enumerate(subti
-0000e7a0: 746c 6573 2c20 7374 6172 743d 3129 3a0d  tles, start=1):.
-0000e7b0: 0a20 2020 2020 2020 2020 2020 2069 7465  .            ite
-0000e7c0: 6d20 3d20 7079 7372 742e 5375 6252 6970  m = pysrt.SubRip
-0000e7d0: 4974 656d 2829 0d0a 2020 2020 2020 2020  Item()..        
-0000e7e0: 2020 2020 6974 656d 2e69 6e64 6578 203d      item.index =
-0000e7f0: 2069 0d0a 2020 2020 2020 2020 2020 2020   i..            
-0000e800: 6974 656d 2e74 6578 7420 3d20 7369 782e  item.text = six.
-0000e810: 7465 7874 5f74 7970 6528 7465 7874 290d  text_type(text).
-0000e820: 0a20 2020 2020 2020 2020 2020 2069 7465  .            ite
-0000e830: 6d2e 7374 6172 742e 7365 636f 6e64 7320  m.start.seconds 
-0000e840: 3d20 6d61 7828 302c 2073 7461 7274 202d  = max(0, start -
-0000e850: 2070 6164 6469 6e67 5f62 6566 6f72 6529   padding_before)
-0000e860: 0d0a 2020 2020 2020 2020 2020 2020 6974  ..            it
-0000e870: 656d 2e65 6e64 2e73 6563 6f6e 6473 203d  em.end.seconds =
-0000e880: 2065 6e64 202b 2070 6164 6469 6e67 5f61   end + padding_a
-0000e890: 6674 6572 0d0a 2020 2020 2020 2020 2020  fter..          
-0000e8a0: 2020 7375 625f 7269 705f 6669 6c65 2e61    sub_rip_file.a
-0000e8b0: 7070 656e 6428 6974 656d 290d 0a20 2020  ppend(item)..   
-0000e8c0: 2020 2020 2072 6574 7572 6e20 275c 6e27       return '\n'
-0000e8d0: 2e6a 6f69 6e28 7369 782e 7465 7874 5f74  .join(six.text_t
-0000e8e0: 7970 6528 6974 656d 2920 666f 7220 6974  ype(item) for it
-0000e8f0: 656d 2069 6e20 7375 625f 7269 705f 6669  em in sub_rip_fi
-0000e900: 6c65 290d 0a0d 0a20 2020 2064 6566 2076  le)....    def v
-0000e910: 7474 5f66 6f72 6d61 7474 6572 2873 656c  tt_formatter(sel
-0000e920: 662c 2073 7562 7469 746c 6573 2c20 7061  f, subtitles, pa
-0000e930: 6464 696e 675f 6265 666f 7265 3d30 2c20  dding_before=0, 
-0000e940: 7061 6464 696e 675f 6166 7465 723d 3029  padding_after=0)
-0000e950: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-0000e960: 2020 2020 2020 2020 5365 7269 616c 697a          Serializ
-0000e970: 6520 6120 6c69 7374 206f 6620 7375 6274  e a list of subt
-0000e980: 6974 6c65 7320 6163 636f 7264 696e 6720  itles according 
-0000e990: 746f 2074 6865 2056 5454 2066 6f72 6d61  to the VTT forma
-0000e9a0: 742c 2077 6974 6820 6f70 7469 6f6e 616c  t, with optional
-0000e9b0: 2074 696d 6520 7061 6464 696e 672e 0d0a   time padding...
-0000e9c0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-0000e9d0: 2020 2020 2074 6578 7420 3d20 7365 6c66       text = self
-0000e9e0: 2e73 7274 5f66 6f72 6d61 7474 6572 2873  .srt_formatter(s
-0000e9f0: 7562 7469 746c 6573 2c20 7061 6464 696e  ubtitles, paddin
-0000ea00: 675f 6265 666f 7265 2c20 7061 6464 696e  g_before, paddin
-0000ea10: 675f 6166 7465 7229 0d0a 2020 2020 2020  g_after)..      
-0000ea20: 2020 7465 7874 203d 2027 5745 4256 5454    text = 'WEBVTT
-0000ea30: 5c6e 5c6e 2720 2b20 7465 7874 2e72 6570  \n\n' + text.rep
-0000ea40: 6c61 6365 2827 2c27 2c20 272e 2729 0d0a  lace(',', '.')..
-0000ea50: 2020 2020 2020 2020 7265 7475 726e 2074          return t
-0000ea60: 6578 740d 0a0d 0a20 2020 2064 6566 206a  ext....    def j
-0000ea70: 736f 6e5f 666f 726d 6174 7465 7228 7365  son_formatter(se
-0000ea80: 6c66 2c20 7375 6274 6974 6c65 7329 3a0d  lf, subtitles):.
-0000ea90: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-0000eaa0: 2020 2020 2020 5365 7269 616c 697a 6520        Serialize 
-0000eab0: 6120 6c69 7374 206f 6620 7375 6274 6974  a list of subtit
-0000eac0: 6c65 7320 6173 2061 204a 534f 4e20 626c  les as a JSON bl
-0000ead0: 6f62 2e0d 0a20 2020 2020 2020 2022 2222  ob...        """
-0000eae0: 0d0a 2020 2020 2020 2020 7375 6274 6974  ..        subtit
-0000eaf0: 6c65 5f64 6963 7473 203d 205b 0d0a 2020  le_dicts = [..  
-0000eb00: 2020 2020 2020 2020 2020 7b0d 0a20 2020            {..   
-0000eb10: 2020 2020 2020 2020 2020 2020 2027 7374               'st
-0000eb20: 6172 7427 3a20 7374 6172 742c 0d0a 2020  art': start,..  
-0000eb30: 2020 2020 2020 2020 2020 2020 2020 2765                'e
-0000eb40: 6e64 273a 2065 6e64 2c0d 0a20 2020 2020  nd': end,..     
-0000eb50: 2020 2020 2020 2020 2020 2027 636f 6e74             'cont
-0000eb60: 656e 7427 3a20 7465 7874 2c0d 0a20 2020  ent': text,..   
-0000eb70: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
-0000eb80: 2020 2020 2020 2020 666f 7220 2828 7374          for ((st
-0000eb90: 6172 742c 2065 6e64 292c 2074 6578 7429  art, end), text)
-0000eba0: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
-0000ebb0: 2073 7562 7469 746c 6573 0d0a 2020 2020   subtitles..    
-0000ebc0: 2020 2020 5d0d 0a20 2020 2020 2020 2072      ]..        r
-0000ebd0: 6574 7572 6e20 6a73 6f6e 2e64 756d 7073  eturn json.dumps
-0000ebe0: 2873 7562 7469 746c 655f 6469 6374 7329  (subtitle_dicts)
-0000ebf0: 0d0a 0d0a 2020 2020 6465 6620 7261 775f  ....    def raw_
-0000ec00: 666f 726d 6174 7465 7228 7365 6c66 2c20  formatter(self, 
-0000ec10: 7375 6274 6974 6c65 7329 3a0d 0a20 2020  subtitles):..   
-0000ec20: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-0000ec30: 2020 5365 7269 616c 697a 6520 6120 6c69    Serialize a li
-0000ec40: 7374 206f 6620 7375 6274 6974 6c65 7320  st of subtitles 
-0000ec50: 6173 2061 206e 6577 6c69 6e65 2d64 656c  as a newline-del
-0000ec60: 696d 6974 6564 2073 7472 696e 672e 0d0a  imited string...
-0000ec70: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-0000ec80: 2020 2020 2072 6574 7572 6e20 2720 272e       return ' '.
-0000ec90: 6a6f 696e 2874 6578 7420 666f 7220 285f  join(text for (_
-0000eca0: 726e 672c 2074 6578 7429 2069 6e20 7375  rng, text) in su
-0000ecb0: 6274 6974 6c65 7329 0d0a 0d0a 0d0a 636c  btitles)......cl
-0000ecc0: 6173 7320 5375 6274 6974 6c65 5772 6974  ass SubtitleWrit
-0000ecd0: 6572 3a0d 0a20 2020 2064 6566 205f 5f69  er:..    def __i
-0000ece0: 6e69 745f 5f28 7365 6c66 2c20 7265 6769  nit__(self, regi
-0000ecf0: 6f6e 732c 2074 7261 6e73 6372 6970 7473  ons, transcripts
-0000ed00: 2c20 666f 726d 6174 2c20 6572 726f 725f  , format, error_
-0000ed10: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
-0000ed20: 6b3d 4e6f 6e65 293a 0d0a 2020 2020 2020  k=None):..      
-0000ed30: 2020 7365 6c66 2e72 6567 696f 6e73 203d    self.regions =
-0000ed40: 2072 6567 696f 6e73 0d0a 2020 2020 2020   regions..      
-0000ed50: 2020 7365 6c66 2e74 7261 6e73 6372 6970    self.transcrip
-0000ed60: 7473 203d 2074 7261 6e73 6372 6970 7473  ts = transcripts
-0000ed70: 0d0a 2020 2020 2020 2020 7365 6c66 2e66  ..        self.f
-0000ed80: 6f72 6d61 7420 3d20 666f 726d 6174 0d0a  ormat = format..
-0000ed90: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
-0000eda0: 6564 5f73 7562 7469 746c 6573 203d 205b  ed_subtitles = [
-0000edb0: 2872 2c20 7429 2066 6f72 2072 2c20 7420  (r, t) for r, t 
-0000edc0: 696e 207a 6970 2873 656c 662e 7265 6769  in zip(self.regi
-0000edd0: 6f6e 732c 2073 656c 662e 7472 616e 7363  ons, self.transc
-0000ede0: 7269 7074 7329 2069 6620 745d 0d0a 2020  ripts) if t]..  
-0000edf0: 2020 2020 2020 7365 6c66 2e65 7272 6f72        self.error
-0000ee00: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
-0000ee10: 636b 203d 2065 7272 6f72 5f6d 6573 7361  ck = error_messa
-0000ee20: 6765 735f 6361 6c6c 6261 636b 0d0a 0d0a  ges_callback....
-0000ee30: 2020 2020 6465 6620 6765 745f 7469 6d65      def get_time
-0000ee40: 645f 7375 6274 6974 6c65 7328 7365 6c66  d_subtitles(self
-0000ee50: 293a 0d0a 2020 2020 2020 2020 7265 7475  ):..        retu
-0000ee60: 726e 2073 656c 662e 7469 6d65 645f 7375  rn self.timed_su
-0000ee70: 6274 6974 6c65 730d 0a0d 0a20 2020 2064  btitles....    d
-0000ee80: 6566 2077 7269 7465 2873 656c 662c 2064  ef write(self, d
-0000ee90: 6563 6c61 7265 645f 7375 6274 6974 6c65  eclared_subtitle
-0000eea0: 5f66 696c 6570 6174 6829 3a0d 0a20 2020  _filepath):..   
-0000eeb0: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
-0000eec0: 2020 2020 2020 2066 6f72 6d61 7474 6572         formatter
-0000eed0: 203d 2053 7562 7469 746c 6546 6f72 6d61   = SubtitleForma
-0000eee0: 7474 6572 2873 656c 662e 666f 726d 6174  tter(self.format
-0000eef0: 290d 0a20 2020 2020 2020 2020 2020 2066  )..            f
-0000ef00: 6f72 6d61 7474 6564 5f73 7562 7469 746c  ormatted_subtitl
-0000ef10: 6573 203d 2066 6f72 6d61 7474 6572 2873  es = formatter(s
-0000ef20: 656c 662e 7469 6d65 645f 7375 6274 6974  elf.timed_subtit
-0000ef30: 6c65 7329 0d0a 2020 2020 2020 2020 2020  les)..          
-0000ef40: 2020 7361 7665 645f 7375 6274 6974 6c65    saved_subtitle
-0000ef50: 5f66 696c 6570 6174 6820 3d20 6465 636c  _filepath = decl
-0000ef60: 6172 6564 5f73 7562 7469 746c 655f 6669  ared_subtitle_fi
-0000ef70: 6c65 7061 7468 0d0a 2020 2020 2020 2020  lepath..        
-0000ef80: 2020 2020 6966 2073 6176 6564 5f73 7562      if saved_sub
-0000ef90: 7469 746c 655f 6669 6c65 7061 7468 3a0d  title_filepath:.
-0000efa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000efb0: 2073 7562 7469 746c 655f 6669 6c65 5f62   subtitle_file_b
-0000efc0: 6173 652c 2073 7562 7469 746c 655f 6669  ase, subtitle_fi
-0000efd0: 6c65 5f65 7874 203d 206f 732e 7061 7468  le_ext = os.path
-0000efe0: 2e73 706c 6974 6578 7428 7361 7665 645f  .splitext(saved_
-0000eff0: 7375 6274 6974 6c65 5f66 696c 6570 6174  subtitle_filepat
-0000f000: 6829 0d0a 2020 2020 2020 2020 2020 2020  h)..            
-0000f010: 2020 2020 6966 206e 6f74 2073 7562 7469      if not subti
-0000f020: 746c 655f 6669 6c65 5f65 7874 3a0d 0a20  tle_file_ext:.. 
-0000f030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f040: 2020 2073 6176 6564 5f73 7562 7469 746c     saved_subtitl
-0000f050: 655f 6669 6c65 7061 7468 203d 2022 7b62  e_filepath = "{b
-0000f060: 6173 657d 2e7b 666f 726d 6174 7d22 2e66  ase}.{format}".f
-0000f070: 6f72 6d61 7428 6261 7365 3d73 7562 7469  ormat(base=subti
-0000f080: 746c 655f 6669 6c65 5f62 6173 652c 2066  tle_file_base, f
-0000f090: 6f72 6d61 743d 7365 6c66 2e66 6f72 6d61  ormat=self.forma
-0000f0a0: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
-0000f0b0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-0000f0c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f0d0: 6176 6564 5f73 7562 7469 746c 655f 6669  aved_subtitle_fi
-0000f0e0: 6c65 7061 7468 203d 2064 6563 6c61 7265  lepath = declare
-0000f0f0: 645f 7375 6274 6974 6c65 5f66 696c 6570  d_subtitle_filep
-0000f100: 6174 680d 0a20 2020 2020 2020 2020 2020  ath..           
-0000f110: 2077 6974 6820 6f70 656e 2873 6176 6564   with open(saved
-0000f120: 5f73 7562 7469 746c 655f 6669 6c65 7061  _subtitle_filepa
-0000f130: 7468 2c20 2777 6227 2920 6173 2066 3a0d  th, 'wb') as f:.
-0000f140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f150: 2066 2e77 7269 7465 2866 6f72 6d61 7474   f.write(formatt
-0000f160: 6564 5f73 7562 7469 746c 6573 2e65 6e63  ed_subtitles.enc
-0000f170: 6f64 6528 2275 7466 2d38 2229 290d 0a20  ode("utf-8")).. 
-0000f180: 2020 2020 2020 2020 2020 2023 7769 7468             #with
-0000f190: 206f 7065 6e28 7361 7665 645f 7375 6274   open(saved_subt
-0000f1a0: 6974 6c65 5f66 696c 6570 6174 682c 2027  itle_filepath, '
-0000f1b0: 6127 2920 6173 2066 3a0d 0a20 2020 2020  a') as f:..     
-0000f1c0: 2020 2020 2020 2023 2020 2020 662e 7772         #    f.wr
-0000f1d0: 6974 6528 225c 6e22 290d 0a0d 0a20 2020  ite("\n")....   
-0000f1e0: 2020 2020 2065 7863 6570 7420 4b65 7962       except Keyb
-0000f1f0: 6f61 7264 496e 7465 7272 7570 743a 0d0a  oardInterrupt:..
-0000f200: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000f210: 656c 662e 6572 726f 725f 6d65 7373 6167  elf.error_messag
-0000f220: 6573 5f63 616c 6c62 6163 6b3a 0d0a 2020  es_callback:..  
-0000f230: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f240: 6c66 2e65 7272 6f72 5f6d 6573 7361 6765  lf.error_message
-0000f250: 735f 6361 6c6c 6261 636b 2822 4361 6e63  s_callback("Canc
-0000f260: 656c 6c69 6e67 2061 6c6c 2074 6173 6b73  elling all tasks
-0000f270: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-0000f280: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-0000f290: 2020 2020 2020 2070 7269 6e74 2822 4361         print("Ca
-0000f2a0: 6e63 656c 6c69 6e67 2061 6c6c 2074 6173  ncelling all tas
-0000f2b0: 6b73 2229 0d0a 2020 2020 2020 2020 2020  ks")..          
-0000f2c0: 2020 7265 7475 726e 0d0a 0d0a 2020 2020    return....    
-0000f2d0: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-0000f2e0: 7469 6f6e 2061 7320 653a 0d0a 2020 2020  tion as e:..    
-0000f2f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000f300: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
-0000f310: 616c 6c62 6163 6b3a 0d0a 2020 2020 2020  allback:..      
-0000f320: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
-0000f330: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
-0000f340: 6c6c 6261 636b 2865 290d 0a20 2020 2020  llback(e)..     
-0000f350: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-0000f360: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-0000f370: 696e 7428 6529 0d0a 2020 2020 2020 2020  int(e)..        
-0000f380: 2020 2020 7265 7475 726e 0d0a 0d0a 0d0a      return......
-0000f390: 636c 6173 7320 5352 5446 696c 6552 6561  class SRTFileRea
-0000f3a0: 6465 723a 0d0a 2020 2020 6465 6620 5f5f  der:..    def __
-0000f3b0: 696e 6974 5f5f 2873 656c 662c 2073 7274  init__(self, srt
-0000f3c0: 5f66 696c 655f 7061 7468 2c20 6572 726f  _file_path, erro
-0000f3d0: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
-0000f3e0: 6163 6b3d 4e6f 6e65 293a 0d0a 2020 2020  ack=None):..    
-0000f3f0: 2020 2020 7365 6c66 2e74 696d 6564 5f73      self.timed_s
-0000f400: 7562 7469 746c 6573 203d 2073 656c 6628  ubtitles = self(
-0000f410: 7372 745f 6669 6c65 5f70 6174 6829 0d0a  srt_file_path)..
-0000f420: 2020 2020 2020 2020 7365 6c66 2e65 7272          self.err
-0000f430: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
-0000f440: 6261 636b 203d 2065 7272 6f72 5f6d 6573  back = error_mes
-0000f450: 7361 6765 735f 6361 6c6c 6261 636b 0d0a  sages_callback..
-0000f460: 0d0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
-0000f470: 686f 640d 0a20 2020 2064 6566 205f 5f63  hod..    def __c
-0000f480: 616c 6c5f 5f28 7372 745f 6669 6c65 5f70  all__(srt_file_p
-0000f490: 6174 6829 3a0d 0a20 2020 2020 2020 2074  ath):..        t
-0000f4a0: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
-0000f4b0: 2022 2222 0d0a 2020 2020 2020 2020 2020   """..          
-0000f4c0: 2020 5265 6164 2053 5254 2066 6f72 6d61    Read SRT forma
-0000f4d0: 7474 6564 2073 7562 7469 746c 6520 6669  tted subtitle fi
-0000f4e0: 6c65 2061 6e64 2072 6574 7572 6e20 7375  le and return su
-0000f4f0: 6274 6974 6c65 7320 6173 206c 6973 7420  btitles as list 
-0000f500: 6f66 2074 7570 6c65 730d 0a20 2020 2020  of tuples..     
-0000f510: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-0000f520: 2020 2020 2020 2020 7469 6d65 645f 7375          timed_su
-0000f530: 6274 6974 6c65 7320 3d20 5b5d 0d0a 2020  btitles = []..  
-0000f540: 2020 2020 2020 2020 2020 7769 7468 206f            with o
-0000f550: 7065 6e28 7372 745f 6669 6c65 5f70 6174  pen(srt_file_pat
-0000f560: 682c 2027 7227 2920 6173 2073 7274 5f66  h, 'r') as srt_f
-0000f570: 696c 653a 0d0a 2020 2020 2020 2020 2020  ile:..          
-0000f580: 2020 2020 2020 6c69 6e65 7320 3d20 7372        lines = sr
-0000f590: 745f 6669 6c65 2e72 6561 646c 696e 6573  t_file.readlines
-0000f5a0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-0000f5b0: 2020 2020 2320 5370 6c69 7420 7468 6520      # Split the 
-0000f5c0: 7375 6274 6974 6c65 2066 696c 6520 696e  subtitle file in
-0000f5d0: 746f 2073 7562 7469 746c 6520 626c 6f63  to subtitle bloc
-0000f5e0: 6b73 0d0a 2020 2020 2020 2020 2020 2020  ks..            
-0000f5f0: 2020 2020 7375 6274 6974 6c65 5f62 6c6f      subtitle_blo
-0000f600: 636b 7320 3d20 5b5d 0d0a 2020 2020 2020  cks = []..      
-0000f610: 2020 2020 2020 2020 2020 626c 6f63 6b20            block 
-0000f620: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-0000f630: 2020 2020 2020 666f 7220 6c69 6e65 2069        for line i
-0000f640: 6e20 6c69 6e65 733a 0d0a 2020 2020 2020  n lines:..      
-0000f650: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000f660: 206c 696e 652e 7374 7269 7028 2920 3d3d   line.strip() ==
-0000f670: 2027 273a 0d0a 2020 2020 2020 2020 2020   '':..          
-0000f680: 2020 2020 2020 2020 2020 2020 2020 7375                su
-0000f690: 6274 6974 6c65 5f62 6c6f 636b 732e 6170  btitle_blocks.ap
-0000f6a0: 7065 6e64 2862 6c6f 636b 290d 0a20 2020  pend(block)..   
-0000f6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6c0: 2020 2020 2062 6c6f 636b 203d 205b 5d0d       block = [].
-0000f6d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f6e0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-0000f6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f700: 2020 2020 626c 6f63 6b2e 6170 7065 6e64      block.append
-0000f710: 286c 696e 652e 7374 7269 7028 2929 0d0a  (line.strip())..
-0000f720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f730: 7375 6274 6974 6c65 5f62 6c6f 636b 732e  subtitle_blocks.
-0000f740: 6170 7065 6e64 2862 6c6f 636b 290d 0a0d  append(block)...
-0000f750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f760: 2023 2050 6172 7365 2065 6163 6820 7375   # Parse each su
-0000f770: 6274 6974 6c65 2062 6c6f 636b 2061 6e64  btitle block and
-0000f780: 2073 746f 7265 2061 7320 7475 706c 6520   store as tuple 
-0000f790: 696e 2074 696d 6564 5f73 7562 7469 746c  in timed_subtitl
-0000f7a0: 6573 206c 6973 740d 0a20 2020 2020 2020  es list..       
-0000f7b0: 2020 2020 2020 2020 2066 6f72 2062 6c6f           for blo
-0000f7c0: 636b 2069 6e20 7375 6274 6974 6c65 5f62  ck in subtitle_b
-0000f7d0: 6c6f 636b 733a 0d0a 2020 2020 2020 2020  locks:..        
-0000f7e0: 2020 2020 2020 2020 2020 2020 6966 2062              if b
-0000f7f0: 6c6f 636b 3a0d 0a20 2020 2020 2020 2020  lock:..         
-0000f800: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000f810: 2045 7874 7261 6374 2073 7461 7274 2061   Extract start a
-0000f820: 6e64 2065 6e64 2074 696d 6573 2066 726f  nd end times fro
-0000f830: 6d20 7375 6274 6974 6c65 2062 6c6f 636b  m subtitle block
-0000f840: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f850: 2020 2020 2020 2020 2020 7374 6172 745f            start_
-0000f860: 7469 6d65 5f73 7472 2c20 656e 645f 7469  time_str, end_ti
-0000f870: 6d65 5f73 7472 203d 2062 6c6f 636b 5b31  me_str = block[1
-0000f880: 5d2e 7370 6c69 7428 2720 2d2d 3e20 2729  ].split(' --> ')
-0000f890: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f8a0: 2020 2020 2020 2020 2020 7469 6d65 5f66            time_f
-0000f8b0: 6f72 6d61 7420 3d20 2725 483a 254d 3a25  ormat = '%H:%M:%
-0000f8c0: 532c 2566 270d 0a20 2020 2020 2020 2020  S,%f'..         
-0000f8d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f8e0: 7461 7274 5f74 696d 655f 7469 6d65 5f64  tart_time_time_d
-0000f8f0: 656c 7461 203d 2064 6174 6574 696d 652e  elta = datetime.
-0000f900: 7374 7270 7469 6d65 2873 7461 7274 5f74  strptime(start_t
-0000f910: 696d 655f 7374 722c 2074 696d 655f 666f  ime_str, time_fo
-0000f920: 726d 6174 2920 2d20 6461 7465 7469 6d65  rmat) - datetime
-0000f930: 2e73 7472 7074 696d 6528 2730 303a 3030  .strptime('00:00
-0000f940: 3a30 302c 3030 3027 2c20 7469 6d65 5f66  :00,000', time_f
-0000f950: 6f72 6d61 7429 0d0a 2020 2020 2020 2020  ormat)..        
-0000f960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f970: 7374 6172 745f 7469 6d65 5f74 6f74 616c  start_time_total
-0000f980: 5f73 6563 6f6e 6473 203d 2073 7461 7274  _seconds = start
-0000f990: 5f74 696d 655f 7469 6d65 5f64 656c 7461  _time_time_delta
-0000f9a0: 2e74 6f74 616c 5f73 6563 6f6e 6473 2829  .total_seconds()
-0000f9b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f9c0: 2020 2020 2020 2020 2020 656e 645f 7469            end_ti
-0000f9d0: 6d65 5f74 696d 655f 6465 6c74 6120 3d20  me_time_delta = 
-0000f9e0: 6461 7465 7469 6d65 2e73 7472 7074 696d  datetime.strptim
-0000f9f0: 6528 656e 645f 7469 6d65 5f73 7472 2c20  e(end_time_str, 
-0000fa00: 7469 6d65 5f66 6f72 6d61 7429 202d 2064  time_format) - d
-0000fa10: 6174 6574 696d 652e 7374 7270 7469 6d65  atetime.strptime
-0000fa20: 2827 3030 3a30 303a 3030 2c30 3030 272c  ('00:00:00,000',
-0000fa30: 2074 696d 655f 666f 726d 6174 290d 0a20   time_format).. 
-0000fa40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa50: 2020 2020 2020 2065 6e64 5f74 696d 655f         end_time_
-0000fa60: 746f 7461 6c5f 7365 636f 6e64 7320 3d20  total_seconds = 
-0000fa70: 656e 645f 7469 6d65 5f74 696d 655f 6465  end_time_time_de
-0000fa80: 6c74 612e 746f 7461 6c5f 7365 636f 6e64  lta.total_second
-0000fa90: 7328 290d 0a20 2020 2020 2020 2020 2020  s()..           
-0000faa0: 2020 2020 2020 2020 2020 2020 2023 2045               # E
-0000fab0: 7874 7261 6374 2073 7562 7469 746c 6520  xtract subtitle 
-0000fac0: 7465 7874 2066 726f 6d20 7375 6274 6974  text from subtit
-0000fad0: 6c65 2062 6c6f 636b 0d0a 2020 2020 2020  le block..      
-0000fae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000faf0: 2020 7375 6274 6974 6c65 203d 2027 2027    subtitle = ' '
-0000fb00: 2e6a 6f69 6e28 626c 6f63 6b5b 323a 5d29  .join(block[2:])
-0000fb10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fb20: 2020 2020 2020 2020 2020 7469 6d65 645f            timed_
-0000fb30: 7375 6274 6974 6c65 732e 6170 7065 6e64  subtitles.append
-0000fb40: 2828 2873 7461 7274 5f74 696d 655f 746f  (((start_time_to
-0000fb50: 7461 6c5f 7365 636f 6e64 732c 2065 6e64  tal_seconds, end
-0000fb60: 5f74 696d 655f 746f 7461 6c5f 7365 636f  _time_total_seco
-0000fb70: 6e64 7329 2c20 7375 6274 6974 6c65 2929  nds), subtitle))
-0000fb80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fb90: 2020 7265 7475 726e 2074 696d 6564 5f73    return timed_s
-0000fba0: 7562 7469 746c 6573 0d0a 0d0a 2020 2020  ubtitles....    
-0000fbb0: 2020 2020 6578 6365 7074 204b 6579 626f      except Keybo
-0000fbc0: 6172 6449 6e74 6572 7275 7074 3a0d 0a20  ardInterrupt:.. 
-0000fbd0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000fbe0: 6c66 2e65 7272 6f72 5f6d 6573 7361 6765  lf.error_message
-0000fbf0: 735f 6361 6c6c 6261 636b 3a0d 0a20 2020  s_callback:..   
-0000fc00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000fc10: 662e 6572 726f 725f 6d65 7373 6167 6573  f.error_messages
-0000fc20: 5f63 616c 6c62 6163 6b28 2243 616e 6365  _callback("Cance
-0000fc30: 6c6c 696e 6720 616c 6c20 7461 736b 7322  lling all tasks"
-0000fc40: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-0000fc50: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-0000fc60: 2020 2020 2020 7072 696e 7428 2243 616e        print("Can
-0000fc70: 6365 6c6c 696e 6720 616c 6c20 7461 736b  celling all task
-0000fc80: 7322 290d 0a20 2020 2020 2020 2020 2020  s")..           
-0000fc90: 2072 6574 7572 6e0d 0a0d 0a20 2020 2020   return....     
-0000fca0: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-0000fcb0: 696f 6e20 6173 2065 3a0d 0a20 2020 2020  ion as e:..     
-0000fcc0: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
-0000fcd0: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
-0000fce0: 6c6c 6261 636b 3a0d 0a20 2020 2020 2020  llback:..       
-0000fcf0: 2020 2020 2020 2020 2073 656c 662e 6572           self.er
-0000fd00: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
-0000fd10: 6c62 6163 6b28 6529 0d0a 2020 2020 2020  lback(e)..      
-0000fd20: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-0000fd30: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-0000fd40: 6e74 2865 290d 0a20 2020 2020 2020 2020  nt(e)..         
-0000fd50: 2020 2072 6574 7572 6e0d 0a0d 0a0d 0a64     return......d
-0000fd60: 6566 2073 686f 775f 7072 6f67 7265 7373  ef show_progress
-0000fd70: 286d 6564 6961 5f66 696c 6570 6174 682c  (media_filepath,
-0000fd80: 2070 726f 6772 6573 7329 3a0d 0a20 2020   progress):..   
-0000fd90: 2067 6c6f 6261 6c20 7062 6172 0d0a 2020   global pbar..  
-0000fda0: 2020 7062 6172 2e75 7064 6174 6528 7072    pbar.update(pr
-0000fdb0: 6f67 7265 7373 290d 0a0d 0a0d 0a64 6566  ogress)......def
-0000fdc0: 2073 686f 775f 6572 726f 725f 6d65 7373   show_error_mess
-0000fdd0: 6167 6573 286d 6573 7361 6765 7329 3a0d  ages(messages):.
-0000fde0: 0a20 2020 2070 7269 6e74 286d 6573 7361  .    print(messa
-0000fdf0: 6765 7329 0d0a 0d0a 0d0a 6465 6620 6d61  ges)......def ma
-0000fe00: 696e 2829 3a0d 0a20 2020 2067 6c6f 6261  in():..    globa
-0000fe10: 6c20 7062 6172 0d0a 0d0a 2020 2020 6966  l pbar....    if
-0000fe20: 2073 7973 2e70 6c61 7466 6f72 6d20 3d3d   sys.platform ==
-0000fe30: 2022 7769 6e33 3222 3a0d 0a20 2020 2020   "win32":..     
-0000fe40: 2020 2073 746f 705f 6666 6d70 6567 5f77     stop_ffmpeg_w
-0000fe50: 696e 646f 7773 2865 7272 6f72 5f6d 6573  indows(error_mes
-0000fe60: 7361 6765 735f 6361 6c6c 6261 636b 3d73  sages_callback=s
-0000fe70: 686f 775f 6572 726f 725f 6d65 7373 6167  how_error_messag
-0000fe80: 6573 290d 0a20 2020 2065 6c73 653a 0d0a  es)..    else:..
-0000fe90: 2020 2020 2020 2020 7374 6f70 5f66 666d          stop_ffm
-0000fea0: 7065 675f 6c69 6e75 7828 6572 726f 725f  peg_linux(error_
-0000feb0: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
-0000fec0: 6b3d 7368 6f77 5f65 7272 6f72 5f6d 6573  k=show_error_mes
-0000fed0: 7361 6765 7329 0d0a 0d0a 2020 2020 7265  sages)....    re
-0000fee0: 6d6f 7665 5f74 656d 705f 6669 6c65 7328  move_temp_files(
-0000fef0: 2266 6c61 6322 2c20 6572 726f 725f 6d65  "flac", error_me
-0000ff00: 7373 6167 6573 5f63 616c 6c62 6163 6b3d  ssages_callback=
-0000ff10: 7368 6f77 5f65 7272 6f72 5f6d 6573 7361  show_error_messa
-0000ff20: 6765 7329 0d0a 2020 2020 7265 6d6f 7665  ges)..    remove
-0000ff30: 5f74 656d 705f 6669 6c65 7328 2277 6176  _temp_files("wav
-0000ff40: 222c 2065 7272 6f72 5f6d 6573 7361 6765  ", error_message
-0000ff50: 735f 6361 6c6c 6261 636b 3d73 686f 775f  s_callback=show_
-0000ff60: 6572 726f 725f 6d65 7373 6167 6573 290d  error_messages).
-0000ff70: 0a0d 0a20 2020 2070 6172 7365 7220 3d20  ...    parser = 
-0000ff80: 6172 6770 6172 7365 2e41 7267 756d 656e  argparse.Argumen
-0000ff90: 7450 6172 7365 7228 290d 0a20 2020 2070  tParser()..    p
-0000ffa0: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
-0000ffb0: 6e74 2827 736f 7572 6365 5f70 6174 6827  nt('source_path'
-0000ffc0: 2c20 6865 6c70 3d22 5061 7468 2074 6f20  , help="Path to 
-0000ffd0: 7468 6520 7669 6465 6f20 6f72 2061 7564  the video or aud
-0000ffe0: 696f 2066 696c 6573 2074 6f20 6765 6e65  io files to gene
-0000fff0: 7261 7465 2073 7562 7469 746c 6573 2066  rate subtitles f
-00010000: 696c 6573 2028 7573 6520 7769 6c64 6361  iles (use wildca
-00010010: 7264 2066 6f72 206d 756c 7469 706c 6520  rd for multiple 
-00010020: 6669 6c65 7320 6f72 2073 6570 6172 6174  files or separat
-00010030: 6520 7468 656d 2077 6974 6820 6120 7370  e them with a sp
-00010040: 6163 6520 6368 6172 6163 7465 7220 652e  ace character e.
-00010050: 672e 205c 2266 696c 6520 312e 6d70 345c  g. \"file 1.mp4\
-00010060: 2220 5c22 6669 6c65 2032 2e6d 7034 5c22  " \"file 2.mp4\"
-00010070: 2922 2c20 6e61 7267 733d 272a 2729 0d0a  )", nargs='*')..
-00010080: 2020 2020 7061 7273 6572 2e61 6464 5f61      parser.add_a
-00010090: 7267 756d 656e 7428 272d 6d27 2c20 272d  rgument('-m', '-
-000100a0: 2d6d 6f64 656c 2d6e 616d 6527 2c20 6465  -model-name', de
-000100b0: 6661 756c 743d 2273 6d61 6c6c 222c 2068  fault="small", h
-000100c0: 656c 703d 226e 616d 6520 6f66 2074 6865  elp="name of the
-000100d0: 2057 6869 7370 6572 206d 6f64 656c 2074   Whisper model t
-000100e0: 6f20 7573 6522 290d 0a20 2020 2070 6172  o use")..    par
-000100f0: 7365 722e 6164 645f 6172 6775 6d65 6e74  ser.add_argument
-00010100: 2827 2d6c 6d27 2c20 272d 2d6c 6973 742d  ('-lm', '--list-
-00010110: 6d6f 6465 6c73 272c 2068 656c 703d 224c  models', help="L
-00010120: 6973 7420 6f66 2057 6869 7370 6572 206d  ist of Whisper m
-00010130: 6f64 656c 7320 6e61 6d65 222c 2061 6374  odels name", act
-00010140: 696f 6e3d 2773 746f 7265 5f74 7275 6527  ion='store_true'
-00010150: 290d 0a20 2020 2070 6172 7365 722e 6164  )..    parser.ad
-00010160: 645f 6172 6775 6d65 6e74 2827 2d53 272c  d_argument('-S',
-00010170: 2027 2d2d 7372 632d 6c61 6e67 7561 6765   '--src-language
-00010180: 272c 2068 656c 703d 224c 616e 6775 6167  ', help="Languag
-00010190: 6520 636f 6465 206f 6620 7468 6520 6175  e code of the au
-000101a0: 6469 6f20 6c61 6e67 7561 6765 2073 706f  dio language spo
-000101b0: 6b65 6e20 696e 2076 6964 656f 2f61 7564  ken in video/aud
-000101c0: 696f 2073 6f75 7263 655f 7061 7468 222c  io source_path",
-000101d0: 2064 6566 6175 6c74 3d22 656e 2229 0d0a   default="en")..
-000101e0: 2020 2020 7061 7273 6572 2e61 6464 5f61      parser.add_a
-000101f0: 7267 756d 656e 7428 272d 4427 2c20 272d  rgument('-D', '-
-00010200: 2d64 7374 2d6c 616e 6775 6167 6527 2c20  -dst-language', 
-00010210: 6865 6c70 3d22 4465 7369 7265 6420 7472  help="Desired tr
-00010220: 616e 736c 6174 696f 6e20 6c61 6e67 7561  anslation langua
-00010230: 6765 2063 6f64 6520 666f 7220 7468 6520  ge code for the 
-00010240: 7375 6274 6974 6c65 7322 2c20 6465 6661  subtitles", defa
-00010250: 756c 743d 4e6f 6e65 290d 0a20 2020 2070  ult=None)..    p
-00010260: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
-00010270: 6e74 2827 2d6c 776c 272c 2027 2d2d 6c69  nt('-lwl', '--li
-00010280: 7374 2d77 6869 7370 6572 2d6c 616e 6775  st-whisper-langu
-00010290: 6167 6573 272c 2068 656c 703d 224c 6973  ages', help="Lis
-000102a0: 7420 616c 6c20 7768 6973 7065 7220 7375  t all whisper su
-000102b0: 7070 6f72 7465 6420 6c61 6e67 7561 6765  pported language
-000102c0: 7322 2c20 6163 7469 6f6e 3d27 7374 6f72  s", action='stor
-000102d0: 655f 7472 7565 2729 0d0a 2020 2020 7061  e_true')..    pa
-000102e0: 7273 6572 2e61 6464 5f61 7267 756d 656e  rser.add_argumen
-000102f0: 7428 272d 6c67 6c27 2c20 272d 2d6c 6973  t('-lgl', '--lis
-00010300: 742d 676f 6f67 6c65 2d6c 616e 6775 6167  t-google-languag
-00010310: 6573 272c 2068 656c 703d 224c 6973 7420  es', help="List 
-00010320: 616c 6c20 676f 6f67 6c65 2074 7261 6e73  all google trans
-00010330: 6c61 7465 2073 7570 706f 7274 6564 206c  late supported l
-00010340: 616e 6775 6167 6573 222c 2061 6374 696f  anguages", actio
-00010350: 6e3d 2773 746f 7265 5f74 7275 6527 290d  n='store_true').
-00010360: 0a20 2020 2070 6172 7365 722e 6164 645f  .    parser.add_
-00010370: 6172 6775 6d65 6e74 2827 2d46 272c 2027  argument('-F', '
-00010380: 2d2d 666f 726d 6174 272c 2068 656c 703d  --format', help=
-00010390: 2244 6573 6972 6564 2073 7562 7469 746c  "Desired subtitl
-000103a0: 6520 666f 726d 6174 222c 2064 6566 6175  e format", defau
-000103b0: 6c74 3d22 7372 7422 290d 0a20 2020 2070  lt="srt")..    p
-000103c0: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
-000103d0: 6e74 2827 2d6c 6627 2c20 272d 2d6c 6973  nt('-lf', '--lis
-000103e0: 742d 666f 726d 6174 7327 2c20 6865 6c70  t-formats', help
-000103f0: 3d22 4c69 7374 2061 6c6c 2073 7570 706f  ="List all suppo
-00010400: 7274 6564 2073 7562 7469 746c 6520 666f  rted subtitle fo
-00010410: 726d 6174 7322 2c20 6163 7469 6f6e 3d27  rmats", action='
-00010420: 7374 6f72 655f 7472 7565 2729 0d0a 2020  store_true')..  
-00010430: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
-00010440: 756d 656e 7428 272d 4327 2c20 272d 2d63  ument('-C', '--c
-00010450: 6f6e 6375 7272 656e 6379 272c 2068 656c  oncurrency', hel
-00010460: 703d 224e 756d 6265 7220 6f66 2063 6f6e  p="Number of con
-00010470: 6375 7272 656e 7420 4150 4920 7265 7175  current API requ
-00010480: 6573 7473 2074 6f20 6d61 6b65 222c 2074  ests to make", t
-00010490: 7970 653d 696e 742c 2064 6566 6175 6c74  ype=int, default
-000104a0: 3d31 3029 0d0a 2020 2020 7061 7273 6572  =10)..    parser
-000104b0: 2e61 6464 5f61 7267 756d 656e 7428 272d  .add_argument('-
-000104c0: 7627 2c20 272d 2d76 6572 7369 6f6e 272c  v', '--version',
-000104d0: 2061 6374 696f 6e3d 2776 6572 7369 6f6e   action='version
-000104e0: 272c 2076 6572 7369 6f6e 3d56 4552 5349  ', version=VERSI
-000104f0: 4f4e 290d 0a0d 0a20 2020 2061 7267 7320  ON)....    args 
-00010500: 3d20 7061 7273 6572 2e70 6172 7365 5f61  = parser.parse_a
-00010510: 7267 7328 290d 0a0d 0a20 2020 2073 7263  rgs()....    src
-00010520: 5f6c 616e 6775 6167 6520 3d20 6172 6773  _language = args
-00010530: 2e73 7263 5f6c 616e 6775 6167 650d 0a20  .src_language.. 
-00010540: 2020 2064 7374 5f6c 616e 6775 6167 6520     dst_language 
-00010550: 3d20 6172 6773 2e64 7374 5f6c 616e 6775  = args.dst_langu
-00010560: 6167 650d 0a0d 0a20 2020 206d 6f64 656c  age....    model
-00010570: 5f6e 616d 6520 3d20 6172 6773 2e6d 6f64  _name = args.mod
-00010580: 656c 5f6e 616d 650d 0a20 2020 2069 6620  el_name..    if 
-00010590: 6d6f 6465 6c5f 6e61 6d65 2e65 6e64 7377  model_name.endsw
-000105a0: 6974 6828 222e 656e 2229 3a0d 0a20 2020  ith(".en"):..   
-000105b0: 2020 2020 2070 7269 6e74 2866 227b 6d6f       print(f"{mo
-000105c0: 6465 6c5f 6e61 6d65 7d20 6973 2061 6e20  del_name} is an 
-000105d0: 456e 676c 6973 682d 6f6e 6c79 206d 6f64  English-only mod
-000105e0: 656c 2c20 666f 7263 696e 6720 456e 676c  el, forcing Engl
-000105f0: 6973 6820 6465 7465 6374 696f 6e2e 2229  ish detection.")
-00010600: 0d0a 2020 2020 2020 2020 6172 6773 2e73  ..        args.s
-00010610: 7263 5f6c 616e 6775 6167 6520 3d20 2265  rc_language = "e
-00010620: 6e22 0d0a 2020 2020 656c 6966 2061 7267  n"..    elif arg
-00010630: 732e 7372 635f 6c61 6e67 7561 6765 2021  s.src_language !
-00010640: 3d20 2261 7574 6f22 3a0d 0a20 2020 2020  = "auto":..     
-00010650: 2020 2061 7267 732e 7372 635f 6c61 6e67     args.src_lang
-00010660: 7561 6765 203d 2073 7263 5f6c 616e 6775  uage = src_langu
-00010670: 6167 650d 0a0d 0a20 2020 206d 6f64 656c  age....    model
-00010680: 203d 2077 6869 7370 6572 2e6c 6f61 645f   = whisper.load_
-00010690: 6d6f 6465 6c28 6d6f 6465 6c5f 6e61 6d65  model(model_name
-000106a0: 290d 0a0d 0a20 2020 2069 6620 6172 6773  )....    if args
-000106b0: 2e6c 6973 745f 6d6f 6465 6c73 3a0d 0a20  .list_models:.. 
-000106c0: 2020 2020 2020 2070 7269 6e74 2822 4c69         print("Li
-000106d0: 7374 206f 6620 7768 6973 7065 7220 6d6f  st of whisper mo
-000106e0: 6465 6c73 3a22 290d 0a20 2020 2020 2020  dels:")..       
-000106f0: 2066 6f72 206d 6f64 656c 5f6e 616d 6520   for model_name 
-00010700: 696e 2077 6869 7370 6572 2e61 7661 696c  in whisper.avail
-00010710: 6162 6c65 5f6d 6f64 656c 7328 293a 0d0a  able_models():..
-00010720: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00010730: 7428 6d6f 6465 6c5f 6e61 6d65 290d 0a20  t(model_name).. 
-00010740: 2020 2020 2020 2072 6574 7572 6e20 300d         return 0.
-00010750: 0a0d 0a20 2020 2077 6869 7370 6572 5f6c  ...    whisper_l
-00010760: 616e 6775 6167 6520 3d20 5768 6973 7065  anguage = Whispe
-00010770: 724c 616e 6775 6167 6528 290d 0a20 2020  rLanguage()..   
-00010780: 2067 6f6f 676c 655f 6c61 6e67 7561 6765   google_language
-00010790: 203d 2047 6f6f 676c 654c 616e 6775 6167   = GoogleLanguag
-000107a0: 6528 290d 0a0d 0a20 2020 2069 6620 6172  e()....    if ar
-000107b0: 6773 2e6c 6973 745f 7768 6973 7065 725f  gs.list_whisper_
-000107c0: 6c61 6e67 7561 6765 733a 0d0a 2020 2020  languages:..    
-000107d0: 2020 2020 7072 696e 7428 224c 6973 7420      print("List 
-000107e0: 6f66 2077 6869 7370 6572 2073 7570 706f  of whisper suppo
-000107f0: 7274 6564 206c 616e 6775 6167 6573 3a22  rted languages:"
-00010800: 290d 0a20 2020 2020 2020 2066 6f72 2077  )..        for w
-00010810: 6869 7370 6572 5f63 6f64 652c 2077 6869  hisper_code, whi
-00010820: 7370 6572 5f6c 616e 6775 6167 6520 696e  sper_language in
-00010830: 2073 6f72 7465 6428 7768 6973 7065 725f   sorted(whisper_
-00010840: 6c61 6e67 7561 6765 2e6e 616d 655f 6f66  language.name_of
-00010850: 5f63 6f64 652e 6974 656d 7328 2929 3a0d  _code.items()):.
-00010860: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00010870: 6e74 2822 252d 3873 203a 2025 7322 2025  nt("%-8s : %s" %
-00010880: 2877 6869 7370 6572 5f63 6f64 652c 2077  (whisper_code, w
-00010890: 6869 7370 6572 5f6c 616e 6775 6167 6529  hisper_language)
-000108a0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-000108b0: 6e20 300d 0a0d 0a20 2020 2069 6620 6172  n 0....    if ar
-000108c0: 6773 2e6c 6973 745f 676f 6f67 6c65 5f6c  gs.list_google_l
-000108d0: 616e 6775 6167 6573 3a0d 0a20 2020 2020  anguages:..     
-000108e0: 2020 2070 7269 6e74 2822 4c69 7374 206f     print("List o
-000108f0: 6620 676f 6f67 6c65 2074 7261 6e73 6c61  f google transla
-00010900: 7465 2073 7570 706f 7274 6564 206c 616e  te supported lan
-00010910: 6775 6167 6573 3a22 290d 0a20 2020 2020  guages:")..     
-00010920: 2020 2066 6f72 2067 6f6f 676c 655f 636f     for google_co
-00010930: 6465 2c20 676f 6f67 6c65 5f6c 616e 6775  de, google_langu
-00010940: 6167 6520 696e 2073 6f72 7465 6428 676f  age in sorted(go
-00010950: 6f67 6c65 5f6c 616e 6775 6167 652e 6e61  ogle_language.na
-00010960: 6d65 5f6f 665f 636f 6465 2e69 7465 6d73  me_of_code.items
-00010970: 2829 293a 0d0a 2020 2020 2020 2020 2020  ()):..          
-00010980: 2020 7072 696e 7428 2225 2d38 7320 3a20    print("%-8s : 
-00010990: 2573 2220 2528 676f 6f67 6c65 5f63 6f64  %s" %(google_cod
-000109a0: 652c 2067 6f6f 676c 655f 6c61 6e67 7561  e, google_langua
-000109b0: 6765 2929 0d0a 2020 2020 2020 2020 7265  ge))..        re
-000109c0: 7475 726e 2030 0d0a 0d0a 2020 2020 6966  turn 0....    if
-000109d0: 2061 7267 732e 7372 635f 6c61 6e67 7561   args.src_langua
-000109e0: 6765 206e 6f74 2069 6e20 7768 6973 7065  ge not in whispe
-000109f0: 725f 6c61 6e67 7561 6765 2e6e 616d 655f  r_language.name_
-00010a00: 6f66 5f63 6f64 652e 6b65 7973 2829 3a0d  of_code.keys():.
-00010a10: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
-00010a20: 536f 7572 6365 206c 616e 6775 6167 6520  Source language 
-00010a30: 6973 206e 6f74 2073 7570 706f 7274 6564  is not supported
-00010a40: 2e20 5275 6e20 7769 7468 202d 2d6c 6973  . Run with --lis
-00010a50: 742d 7768 6973 7065 722d 6c61 6e67 7561  t-whisper-langua
-00010a60: 6765 7320 746f 2073 6565 2061 6c6c 2077  ges to see all w
-00010a70: 6869 7370 6572 2073 7570 706f 7274 6564  hisper supported
-00010a80: 206c 616e 6775 6167 6573 2e22 290d 0a20   languages.").. 
-00010a90: 2020 2020 2020 2072 6574 7572 6e20 310d         return 1.
-00010aa0: 0a0d 0a20 2020 2069 6620 6172 6773 2e64  ...    if args.d
-00010ab0: 7374 5f6c 616e 6775 6167 653a 0d0a 2020  st_language:..  
-00010ac0: 2020 2020 2020 6966 206e 6f74 2061 7267        if not arg
-00010ad0: 732e 6473 745f 6c61 6e67 7561 6765 2069  s.dst_language i
-00010ae0: 6e20 676f 6f67 6c65 5f6c 616e 6775 6167  n google_languag
-00010af0: 652e 6e61 6d65 5f6f 665f 636f 6465 2e6b  e.name_of_code.k
-00010b00: 6579 7328 293a 0d0a 2020 2020 2020 2020  eys():..        
-00010b10: 2020 2020 7072 696e 7428 2244 6573 7469      print("Desti
-00010b20: 6e61 7469 6f6e 206c 616e 6775 6167 6520  nation language 
-00010b30: 6973 206e 6f74 2073 7570 706f 7274 6564  is not supported
-00010b40: 2e20 5275 6e20 7769 7468 202d 2d6c 6973  . Run with --lis
-00010b50: 742d 676f 6f67 6c65 2d6c 616e 6775 6167  t-google-languag
-00010b60: 6573 2074 6f20 7365 6520 616c 6c20 676f  es to see all go
-00010b70: 6f67 6c65 2074 7261 6e73 6c61 7465 2073  ogle translate s
-00010b80: 7570 706f 7274 6564 206c 616e 6775 6167  upported languag
-00010b90: 6573 2e22 290d 0a20 2020 2020 2020 2020  es.")..         
-00010ba0: 2020 2072 6574 7572 6e20 310d 0a20 2020     return 1..   
-00010bb0: 2020 2020 2069 6620 6e6f 7420 6973 5f73       if not is_s
-00010bc0: 616d 655f 6c61 6e67 7561 6765 2861 7267  ame_language(arg
-00010bd0: 732e 7372 635f 6c61 6e67 7561 6765 2c20  s.src_language, 
-00010be0: 6172 6773 2e64 7374 5f6c 616e 6775 6167  args.dst_languag
-00010bf0: 652c 2065 7272 6f72 5f6d 6573 7361 6765  e, error_message
-00010c00: 735f 6361 6c6c 6261 636b 3d73 686f 775f  s_callback=show_
-00010c10: 6572 726f 725f 6d65 7373 6167 6573 293a  error_messages):
-00010c20: 0d0a 2020 2020 2020 2020 2020 2020 646f  ..            do
-00010c30: 5f74 7261 6e73 6c61 7465 203d 2054 7275  _translate = Tru
-00010c40: 650d 0a20 2020 2020 2020 2065 6c73 653a  e..        else:
-00010c50: 0d0a 2020 2020 2020 2020 2020 2020 646f  ..            do
-00010c60: 5f74 7261 6e73 6c61 7465 203d 2046 616c  _translate = Fal
-00010c70: 7365 0d0a 2020 2020 656c 7365 3a0d 0a20  se..    else:.. 
-00010c80: 2020 2020 2020 2064 6f5f 7472 616e 736c         do_transl
-00010c90: 6174 6520 3d20 4661 6c73 650d 0a0d 0a20  ate = False.... 
-00010ca0: 2020 2069 6620 6172 6773 2e6c 6973 745f     if args.list_
-00010cb0: 666f 726d 6174 733a 0d0a 2020 2020 2020  formats:..      
-00010cc0: 2020 7072 696e 7428 224c 6973 7420 6f66    print("List of
-00010cd0: 2073 7570 706f 7274 6564 2073 7562 7469   supported subti
-00010ce0: 746c 6520 666f 726d 6174 733a 2229 0d0a  tle formats:")..
-00010cf0: 2020 2020 2020 2020 666f 7220 7375 6274          for subt
-00010d00: 6974 6c65 5f66 6f72 6d61 7420 696e 2053  itle_format in S
-00010d10: 7562 7469 746c 6546 6f72 6d61 7474 6572  ubtitleFormatter
-00010d20: 2e73 7570 706f 7274 6564 5f66 6f72 6d61  .supported_forma
-00010d30: 7473 3a0d 0a20 2020 2020 2020 2020 2020  ts:..           
-00010d40: 2070 7269 6e74 2822 7b66 6f72 6d61 747d   print("{format}
-00010d50: 222e 666f 726d 6174 2866 6f72 6d61 743d  ".format(format=
-00010d60: 7375 6274 6974 6c65 5f66 6f72 6d61 7429  subtitle_format)
-00010d70: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00010d80: 6e20 300d 0a0d 0a20 2020 2069 6620 6172  n 0....    if ar
-00010d90: 6773 2e66 6f72 6d61 7420 6e6f 7420 696e  gs.format not in
-00010da0: 2053 7562 7469 746c 6546 6f72 6d61 7474   SubtitleFormatt
-00010db0: 6572 2e73 7570 706f 7274 6564 5f66 6f72  er.supported_for
-00010dc0: 6d61 7473 3a0d 0a20 2020 2020 2020 2070  mats:..        p
-00010dd0: 7269 6e74 2822 5375 6274 6974 6c65 2066  rint("Subtitle f
-00010de0: 6f72 6d61 7420 6973 206e 6f74 2073 7570  ormat is not sup
-00010df0: 706f 7274 6564 2e20 5275 6e20 7769 7468  ported. Run with
-00010e00: 202d 2d6c 6973 742d 666f 726d 6174 7320   --list-formats 
-00010e10: 746f 2073 6565 2061 6c6c 2073 7570 706f  to see all suppo
-00010e20: 7274 6564 2066 6f72 6d61 7473 2e22 290d  rted formats.").
-00010e30: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00010e40: 310d 0a0d 0a20 2020 2069 6620 6e6f 7420  1....    if not 
-00010e50: 6172 6773 2e73 6f75 7263 655f 7061 7468  args.source_path
-00010e60: 3a0d 0a20 2020 2020 2020 2070 6172 7365  :..        parse
-00010e70: 722e 7072 696e 745f 6865 6c70 2873 7973  r.print_help(sys
-00010e80: 2e73 7464 6572 7229 0d0a 2020 2020 2020  .stderr)..      
-00010e90: 2020 7265 7475 726e 2031 0d0a 0d0a 2020    return 1....  
-00010ea0: 2020 636f 6d70 6c65 7465 645f 7461 736b    completed_task
-00010eb0: 7320 3d20 300d 0a20 2020 206d 6564 6961  s = 0..    media
+00002650: 3d3d 3d3d 3d3d 3d3d 3d3d 3d23 0d0a 0d0a  ===========#....
+00002660: 0d0a 6465 6620 7374 6f70 5f66 666d 7065  ..def stop_ffmpe
+00002670: 675f 7769 6e64 6f77 7328 6572 726f 725f  g_windows(error_
+00002680: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
+00002690: 6b3d 4e6f 6e65 293a 0d0a 2020 2020 7472  k=None):..    tr
+000026a0: 793a 0d0a 2020 2020 2020 2020 7461 736b  y:..        task
+000026b0: 6c69 7374 5f6f 7574 7075 7420 3d20 7375  list_output = su
+000026c0: 6270 726f 6365 7373 2e63 6865 636b 5f6f  bprocess.check_o
+000026d0: 7574 7075 7428 5b27 7461 736b 6c69 7374  utput(['tasklist
+000026e0: 275d 2c20 6372 6561 7469 6f6e 666c 6167  '], creationflag
+000026f0: 733d 7375 6270 726f 6365 7373 2e43 5245  s=subprocess.CRE
+00002700: 4154 455f 4e4f 5f57 494e 444f 5729 2e64  ATE_NO_WINDOW).d
+00002710: 6563 6f64 6528 2775 7466 2d38 2729 0d0a  ecode('utf-8')..
+00002720: 2020 2020 2020 2020 6666 6d70 6567 5f70          ffmpeg_p
+00002730: 6964 203d 204e 6f6e 650d 0a20 2020 2020  id = None..     
+00002740: 2020 2066 6f72 206c 696e 6520 696e 2074     for line in t
+00002750: 6173 6b6c 6973 745f 6f75 7470 7574 2e73  asklist_output.s
+00002760: 706c 6974 2827 5c6e 2729 3a0d 0a20 2020  plit('\n'):..   
+00002770: 2020 2020 2020 2020 2069 6620 2266 666d           if "ffm
+00002780: 7065 6722 2069 6e20 6c69 6e65 3a0d 0a20  peg" in line:.. 
+00002790: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000027a0: 666d 7065 675f 7069 6420 3d20 6c69 6e65  fmpeg_pid = line
+000027b0: 2e73 706c 6974 2829 5b31 5d0d 0a20 2020  .split()[1]..   
+000027c0: 2020 2020 2020 2020 2020 2020 2062 7265               bre
+000027d0: 616b 0d0a 2020 2020 2020 2020 6966 2066  ak..        if f
+000027e0: 666d 7065 675f 7069 643a 0d0a 2020 2020  fmpeg_pid:..    
+000027f0: 2020 2020 2020 2020 6465 766e 756c 6c20          devnull 
+00002800: 3d20 6f70 656e 286f 732e 6465 766e 756c  = open(os.devnul
+00002810: 6c2c 2027 7727 290d 0a20 2020 2020 2020  l, 'w')..       
+00002820: 2020 2020 2073 7562 7072 6f63 6573 732e       subprocess.
+00002830: 506f 7065 6e28 5b27 7461 736b 6b69 6c6c  Popen(['taskkill
+00002840: 272c 2027 2f46 272c 2027 2f54 272c 2027  ', '/F', '/T', '
+00002850: 2f50 4944 272c 2066 666d 7065 675f 7069  /PID', ffmpeg_pi
+00002860: 645d 2c20 7374 646f 7574 3d73 7562 7072  d], stdout=subpr
+00002870: 6f63 6573 732e 5049 5045 2c20 7374 6465  ocess.PIPE, stde
+00002880: 7272 3d73 7562 7072 6f63 6573 732e 5354  rr=subprocess.ST
+00002890: 444f 5554 2c20 7368 656c 6c3d 5472 7565  DOUT, shell=True
+000028a0: 2c20 6372 6561 7469 6f6e 666c 6167 733d  , creationflags=
+000028b0: 7375 6270 726f 6365 7373 2e43 5245 4154  subprocess.CREAT
+000028c0: 455f 4e4f 5f57 494e 444f 5729 0d0a 0d0a  E_NO_WINDOW)....
+000028d0: 2020 2020 6578 6365 7074 204b 6579 626f      except Keybo
+000028e0: 6172 6449 6e74 6572 7275 7074 3a0d 0a20  ardInterrupt:.. 
+000028f0: 2020 2020 2020 2069 6620 6572 726f 725f         if error_
+00002900: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
+00002910: 6b3a 0d0a 2020 2020 2020 2020 2020 2020  k:..            
+00002920: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
+00002930: 616c 6c62 6163 6b28 2243 616e 6365 6c6c  allback("Cancell
+00002940: 696e 6720 616c 6c20 7461 736b 7322 290d  ing all tasks").
+00002950: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
+00002960: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00002970: 7428 2243 616e 6365 6c6c 696e 6720 616c  t("Cancelling al
+00002980: 6c20 7461 736b 7322 290d 0a20 2020 2020  l tasks")..     
+00002990: 2020 2072 6574 7572 6e0d 0a0d 0a20 2020     return....   
+000029a0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+000029b0: 6e20 6173 2065 3a0d 0a20 2020 2020 2020  n as e:..       
+000029c0: 2069 6620 6572 726f 725f 6d65 7373 6167   if error_messag
+000029d0: 6573 5f63 616c 6c62 6163 6b3a 0d0a 2020  es_callback:..  
+000029e0: 2020 2020 2020 2020 2020 6572 726f 725f            error_
+000029f0: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
+00002a00: 6b28 6529 0d0a 2020 2020 2020 2020 656c  k(e)..        el
+00002a10: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00002a20: 2070 7269 6e74 2865 290d 0a20 2020 2020   print(e)..     
+00002a30: 2020 2072 6574 7572 6e0d 0a0d 0a0d 0a64     return......d
+00002a40: 6566 2073 746f 705f 6666 6d70 6567 5f6c  ef stop_ffmpeg_l
+00002a50: 696e 7578 2865 7272 6f72 5f6d 6573 7361  inux(error_messa
+00002a60: 6765 735f 6361 6c6c 6261 636b 3d4e 6f6e  ges_callback=Non
+00002a70: 6529 3a0d 0a20 2020 2070 726f 6365 7373  e):..    process
+00002a80: 5f6e 616d 6520 3d20 2766 666d 7065 6727  _name = 'ffmpeg'
+00002a90: 0d0a 2020 2020 7472 793a 0d0a 2020 2020  ..    try:..    
+00002aa0: 2020 2020 6f75 7470 7574 203d 2073 7562      output = sub
+00002ab0: 7072 6f63 6573 732e 6368 6563 6b5f 6f75  process.check_ou
+00002ac0: 7470 7574 285b 2770 7327 2c20 272d 6566  tput(['ps', '-ef
+00002ad0: 275d 290d 0a20 2020 2020 2020 2070 6964  '])..        pid
+00002ae0: 203d 205b 6c69 6e65 2e73 706c 6974 2829   = [line.split()
+00002af0: 5b31 5d20 666f 7220 6c69 6e65 2069 6e20  [1] for line in 
+00002b00: 6f75 7470 7574 2e64 6563 6f64 6528 2775  output.decode('u
+00002b10: 7466 2d38 2729 2e73 706c 6974 2827 5c6e  tf-8').split('\n
+00002b20: 2729 2069 6620 7072 6f63 6573 735f 6e61  ') if process_na
+00002b30: 6d65 2069 6e20 6c69 6e65 5d5b 305d 0d0a  me in line][0]..
+00002b40: 2020 2020 2020 2020 7375 6270 726f 6365          subproce
+00002b50: 7373 2e63 616c 6c28 5b27 6b69 6c6c 272c  ss.call(['kill',
+00002b60: 2027 2d39 272c 2073 7472 2870 6964 295d   '-9', str(pid)]
+00002b70: 290d 0a20 2020 2020 2020 2023 7072 696e  )..        #prin
+00002b80: 7428 6622 7b70 726f 6365 7373 5f6e 616d  t(f"{process_nam
+00002b90: 657d 2068 6173 2062 6565 6e20 6b69 6c6c  e} has been kill
+00002ba0: 6564 2229 0d0a 2020 2020 6578 6365 7074  ed")..    except
+00002bb0: 2049 6e64 6578 4572 726f 723a 0d0a 2020   IndexError:..  
+00002bc0: 2020 2020 2020 2370 7269 6e74 2866 227b        #print(f"{
+00002bd0: 7072 6f63 6573 735f 6e61 6d65 7d20 6973  process_name} is
+00002be0: 206e 6f74 2072 756e 6e69 6e67 2229 0d0a   not running")..
+00002bf0: 2020 2020 2020 2020 7061 7373 0d0a 0d0a          pass....
+00002c00: 2020 2020 6578 6365 7074 204b 6579 626f      except Keybo
+00002c10: 6172 6449 6e74 6572 7275 7074 3a0d 0a20  ardInterrupt:.. 
+00002c20: 2020 2020 2020 2069 6620 6572 726f 725f         if error_
+00002c30: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
+00002c40: 6b3a 0d0a 2020 2020 2020 2020 2020 2020  k:..            
+00002c50: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
+00002c60: 616c 6c62 6163 6b28 2243 616e 6365 6c6c  allback("Cancell
+00002c70: 696e 6720 616c 6c20 7461 736b 7322 290d  ing all tasks").
+00002c80: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
+00002c90: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00002ca0: 7428 2243 616e 6365 6c6c 696e 6720 616c  t("Cancelling al
+00002cb0: 6c20 7461 736b 7322 290d 0a20 2020 2020  l tasks")..     
+00002cc0: 2020 2072 6574 7572 6e0d 0a0d 0a20 2020     return....   
+00002cd0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+00002ce0: 6e20 6173 2065 3a0d 0a20 2020 2020 2020  n as e:..       
+00002cf0: 2069 6620 6572 726f 725f 6d65 7373 6167   if error_messag
+00002d00: 6573 5f63 616c 6c62 6163 6b3a 0d0a 2020  es_callback:..  
+00002d10: 2020 2020 2020 2020 2020 6572 726f 725f            error_
+00002d20: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
+00002d30: 6b28 6529 0d0a 2020 2020 2020 2020 656c  k(e)..        el
+00002d40: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00002d50: 2070 7269 6e74 2865 290d 0a20 2020 2020   print(e)..     
+00002d60: 2020 2072 6574 7572 6e0d 0a0d 0a0d 0a64     return......d
+00002d70: 6566 2072 656d 6f76 655f 7465 6d70 5f66  ef remove_temp_f
+00002d80: 696c 6573 2865 7874 656e 7369 6f6e 2c20  iles(extension, 
+00002d90: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
+00002da0: 616c 6c62 6163 6b3d 4e6f 6e65 293a 0d0a  allback=None):..
+00002db0: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+00002dc0: 2020 7465 6d70 5f64 6972 203d 2074 656d    temp_dir = tem
+00002dd0: 7066 696c 652e 6765 7474 656d 7064 6972  pfile.gettempdir
+00002de0: 2829 0d0a 2020 2020 2020 2020 666f 7220  ()..        for 
+00002df0: 726f 6f74 2c20 6469 7273 2c20 6669 6c65  root, dirs, file
+00002e00: 7320 696e 206f 732e 7761 6c6b 2874 656d  s in os.walk(tem
+00002e10: 705f 6469 7229 3a0d 0a20 2020 2020 2020  p_dir):..       
+00002e20: 2020 2020 2066 6f72 2066 696c 6520 696e       for file in
+00002e30: 2066 696c 6573 3a0d 0a20 2020 2020 2020   files:..       
+00002e40: 2020 2020 2020 2020 2069 6620 6669 6c65           if file
+00002e50: 2e65 6e64 7377 6974 6828 222e 2220 2b20  .endswith("." + 
+00002e60: 6578 7465 6e73 696f 6e29 3a0d 0a20 2020  extension):..   
+00002e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e80: 206f 732e 7265 6d6f 7665 286f 732e 7061   os.remove(os.pa
+00002e90: 7468 2e6a 6f69 6e28 726f 6f74 2c20 6669  th.join(root, fi
+00002ea0: 6c65 2929 0d0a 2020 2020 6578 6365 7074  le))..    except
+00002eb0: 204b 6579 626f 6172 6449 6e74 6572 7275   KeyboardInterru
+00002ec0: 7074 3a0d 0a20 2020 2020 2020 2069 6620  pt:..        if 
+00002ed0: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
+00002ee0: 616c 6c62 6163 6b3a 0d0a 2020 2020 2020  allback:..      
+00002ef0: 2020 2020 2020 6572 726f 725f 6d65 7373        error_mess
+00002f00: 6167 6573 5f63 616c 6c62 6163 6b28 2243  ages_callback("C
+00002f10: 616e 6365 6c6c 696e 6720 616c 6c20 7461  ancelling all ta
+00002f20: 736b 7322 290d 0a20 2020 2020 2020 2065  sks")..        e
+00002f30: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00002f40: 2020 7072 696e 7428 2243 616e 6365 6c6c    print("Cancell
+00002f50: 696e 6720 616c 6c20 7461 736b 7322 290d  ing all tasks").
+00002f60: 0a20 2020 2020 2020 2072 6574 7572 6e0d  .        return.
+00002f70: 0a0d 0a20 2020 2065 7863 6570 7420 4578  ...    except Ex
+00002f80: 6365 7074 696f 6e20 6173 2065 3a0d 0a20  ception as e:.. 
+00002f90: 2020 2020 2020 2069 6620 6572 726f 725f         if error_
+00002fa0: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
+00002fb0: 6b3a 0d0a 2020 2020 2020 2020 2020 2020  k:..            
+00002fc0: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
+00002fd0: 616c 6c62 6163 6b28 6529 0d0a 2020 2020  allback(e)..    
+00002fe0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00002ff0: 2020 2020 2020 2070 7269 6e74 2865 290d         print(e).
+00003000: 0a20 2020 2020 2020 2072 6574 7572 6e0d  .        return.
+00003010: 0a0d 0a0d 0a64 6566 2069 735f 7361 6d65  .....def is_same
+00003020: 5f6c 616e 6775 6167 6528 7372 632c 2064  _language(src, d
+00003030: 7374 2c20 6572 726f 725f 6d65 7373 6167  st, error_messag
+00003040: 6573 5f63 616c 6c62 6163 6b3d 4e6f 6e65  es_callback=None
+00003050: 293a 0d0a 2020 2020 7472 793a 0d0a 2020  ):..    try:..  
+00003060: 2020 2020 2020 7265 7475 726e 2073 7263        return src
+00003070: 2e73 706c 6974 2822 2d22 295b 305d 203d  .split("-")[0] =
+00003080: 3d20 6473 742e 7370 6c69 7428 222d 2229  = dst.split("-")
+00003090: 5b30 5d0d 0a20 2020 2065 7863 6570 7420  [0]..    except 
+000030a0: 4578 6365 7074 696f 6e20 6173 2065 3a0d  Exception as e:.
+000030b0: 0a20 2020 2020 2020 2069 6620 6572 726f  .        if erro
+000030c0: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
+000030d0: 6163 6b3a 0d0a 2020 2020 2020 2020 2020  ack:..          
+000030e0: 2020 6572 726f 725f 6d65 7373 6167 6573    error_messages
+000030f0: 5f63 616c 6c62 6163 6b28 6529 0d0a 2020  _callback(e)..  
+00003100: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00003110: 2020 2020 2020 2020 2070 7269 6e74 2865           print(e
+00003120: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00003130: 6e0d 0a0d 0a0d 0a64 6566 2063 6865 636b  n......def check
+00003140: 5f66 696c 655f 7479 7065 2866 696c 655f  _file_type(file_
+00003150: 7061 7468 2c20 6572 726f 725f 6d65 7373  path, error_mess
+00003160: 6167 6573 5f63 616c 6c62 6163 6b3d 4e6f  ages_callback=No
+00003170: 6e65 293a 0d0a 2020 2020 7472 793a 0d0a  ne):..    try:..
+00003180: 2020 2020 2020 2020 6666 7072 6f62 655f          ffprobe_
+00003190: 636d 6420 3d20 5b27 6666 7072 6f62 6527  cmd = ['ffprobe'
+000031a0: 2c20 272d 7627 2c20 2765 7272 6f72 272c  , '-v', 'error',
+000031b0: 2027 2d73 686f 775f 666f 726d 6174 272c   '-show_format',
+000031c0: 2027 2d73 686f 775f 7374 7265 616d 7327   '-show_streams'
+000031d0: 2c20 272d 7072 696e 745f 666f 726d 6174  , '-print_format
+000031e0: 272c 2027 6a73 6f6e 272c 2066 696c 655f  ', 'json', file_
+000031f0: 7061 7468 5d0d 0a20 2020 2020 2020 206f  path]..        o
+00003200: 7574 7075 7420 3d20 4e6f 6e65 0d0a 2020  utput = None..  
+00003210: 2020 2020 2020 6966 2073 7973 2e70 6c61        if sys.pla
+00003220: 7466 6f72 6d20 3d3d 2022 7769 6e33 3222  tform == "win32"
+00003230: 3a0d 0a20 2020 2020 2020 2020 2020 206f  :..            o
+00003240: 7574 7075 7420 3d20 7375 6270 726f 6365  utput = subproce
+00003250: 7373 2e63 6865 636b 5f6f 7574 7075 7428  ss.check_output(
+00003260: 6666 7072 6f62 655f 636d 642c 2063 7265  ffprobe_cmd, cre
+00003270: 6174 696f 6e66 6c61 6773 3d73 7562 7072  ationflags=subpr
+00003280: 6f63 6573 732e 4352 4541 5445 5f4e 4f5f  ocess.CREATE_NO_
+00003290: 5749 4e44 4f57 292e 6465 636f 6465 2827  WINDOW).decode('
+000032a0: 7574 662d 3827 290d 0a20 2020 2020 2020  utf-8')..       
+000032b0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+000032c0: 2020 2020 6f75 7470 7574 203d 2073 7562      output = sub
+000032d0: 7072 6f63 6573 732e 6368 6563 6b5f 6f75  process.check_ou
+000032e0: 7470 7574 2866 6670 726f 6265 5f63 6d64  tput(ffprobe_cmd
+000032f0: 292e 6465 636f 6465 2827 7574 662d 3827  ).decode('utf-8'
+00003300: 290d 0a20 2020 2020 2020 2064 6174 6120  )..        data 
+00003310: 3d20 6a73 6f6e 2e6c 6f61 6473 286f 7574  = json.loads(out
+00003320: 7075 7429 0d0a 0d0a 2020 2020 2020 2020  put)....        
+00003330: 6966 2027 7374 7265 616d 7327 2069 6e20  if 'streams' in 
+00003340: 6461 7461 3a0d 0a20 2020 2020 2020 2020  data:..         
+00003350: 2020 2066 6f72 2073 7472 6561 6d20 696e     for stream in
+00003360: 2064 6174 615b 2773 7472 6561 6d73 275d   data['streams']
+00003370: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00003380: 2020 2069 6620 2763 6f64 6563 5f74 7970     if 'codec_typ
+00003390: 6527 2069 6e20 7374 7265 616d 2061 6e64  e' in stream and
+000033a0: 2073 7472 6561 6d5b 2763 6f64 6563 5f74   stream['codec_t
+000033b0: 7970 6527 5d20 3d3d 2027 6175 6469 6f27  ype'] == 'audio'
+000033c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000033d0: 2020 2020 2020 2072 6574 7572 6e20 2761         return 'a
+000033e0: 7564 696f 270d 0a20 2020 2020 2020 2020  udio'..         
+000033f0: 2020 2020 2020 2065 6c69 6620 2763 6f64         elif 'cod
+00003400: 6563 5f74 7970 6527 2069 6e20 7374 7265  ec_type' in stre
+00003410: 616d 2061 6e64 2073 7472 6561 6d5b 2763  am and stream['c
+00003420: 6f64 6563 5f74 7970 6527 5d20 3d3d 2027  odec_type'] == '
+00003430: 7669 6465 6f27 3a0d 0a20 2020 2020 2020  video':..       
+00003440: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00003450: 7572 6e20 2776 6964 656f 270d 0a20 2020  urn 'video'..   
+00003460: 2065 7863 6570 7420 2873 7562 7072 6f63   except (subproc
+00003470: 6573 732e 4361 6c6c 6564 5072 6f63 6573  ess.CalledProces
+00003480: 7345 7272 6f72 2c20 6a73 6f6e 2e4a 534f  sError, json.JSO
+00003490: 4e44 6563 6f64 6545 7272 6f72 293a 0d0a  NDecodeError):..
+000034a0: 2020 2020 2020 2020 7061 7373 0d0a 0d0a          pass....
+000034b0: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
+000034c0: 7469 6f6e 2061 7320 653a 0d0a 2020 2020  tion as e:..    
+000034d0: 2020 2020 6966 2065 7272 6f72 5f6d 6573      if error_mes
+000034e0: 7361 6765 735f 6361 6c6c 6261 636b 3a0d  sages_callback:.
+000034f0: 0a20 2020 2020 2020 2020 2020 2065 7272  .            err
+00003500: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
+00003510: 6261 636b 2865 290d 0a20 2020 2020 2020  back(e)..       
+00003520: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00003530: 2020 2020 7072 696e 7428 6529 0d0a 0d0a      print(e)....
+00003540: 2020 2020 7265 7475 726e 204e 6f6e 650d      return None.
+00003550: 0a0d 0a0d 0a63 6c61 7373 2057 6869 7370  .....class Whisp
+00003560: 6572 4c61 6e67 7561 6765 3a0d 0a20 2020  erLanguage:..   
+00003570: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00003580: 6c66 293a 0d0a 2020 2020 2020 2020 7365  lf):..        se
+00003590: 6c66 2e6c 6973 745f 636f 6465 7320 3d20  lf.list_codes = 
+000035a0: 5b5d 0d0a 2020 2020 2020 2020 7365 6c66  []..        self
+000035b0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+000035c0: 6e64 2822 6166 2229 0d0a 2020 2020 2020  nd("af")..      
+000035d0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+000035e0: 732e 6170 7065 6e64 2822 7371 2229 0d0a  s.append("sq")..
+000035f0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00003600: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00003610: 616d 2229 0d0a 2020 2020 2020 2020 7365  am")..        se
+00003620: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00003630: 7065 6e64 2822 6172 2229 0d0a 2020 2020  pend("ar")..    
+00003640: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+00003650: 6465 732e 6170 7065 6e64 2822 6879 2229  des.append("hy")
+00003660: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00003670: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+00003680: 2822 6173 2229 0d0a 2020 2020 2020 2020  ("as")..        
+00003690: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+000036a0: 6170 7065 6e64 2822 617a 2229 0d0a 2020  append("az")..  
+000036b0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+000036c0: 636f 6465 732e 6170 7065 6e64 2822 6261  codes.append("ba
+000036d0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+000036e0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+000036f0: 6e64 2822 6575 2229 0d0a 2020 2020 2020  nd("eu")..      
+00003700: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00003710: 732e 6170 7065 6e64 2822 6265 2229 0d0a  s.append("be")..
+00003720: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00003730: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00003740: 626e 2229 0d0a 2020 2020 2020 2020 7365  bn")..        se
+00003750: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00003760: 7065 6e64 2822 6273 2229 0d0a 2020 2020  pend("bs")..    
+00003770: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+00003780: 6465 732e 6170 7065 6e64 2822 6272 2229  des.append("br")
+00003790: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+000037a0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+000037b0: 2822 6267 2229 0d0a 2020 2020 2020 2020  ("bg")..        
+000037c0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+000037d0: 6170 7065 6e64 2822 6361 2229 0d0a 2020  append("ca")..  
+000037e0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+000037f0: 636f 6465 732e 6170 7065 6e64 2822 7a68  codes.append("zh
+00003800: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00003810: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00003820: 6e64 2822 6872 2229 0d0a 2020 2020 2020  nd("hr")..      
+00003830: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00003840: 732e 6170 7065 6e64 2822 6373 2229 0d0a  s.append("cs")..
+00003850: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00003860: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00003870: 6461 2229 0d0a 2020 2020 2020 2020 7365  da")..        se
+00003880: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00003890: 7065 6e64 2822 6e6c 2229 0d0a 2020 2020  pend("nl")..    
+000038a0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+000038b0: 6465 732e 6170 7065 6e64 2822 656e 2229  des.append("en")
+000038c0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+000038d0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+000038e0: 2822 6574 2229 0d0a 2020 2020 2020 2020  ("et")..        
+000038f0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00003900: 6170 7065 6e64 2822 666f 2229 0d0a 2020  append("fo")..  
+00003910: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00003920: 636f 6465 732e 6170 7065 6e64 2822 6669  codes.append("fi
+00003930: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00003940: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00003950: 6e64 2822 6672 2229 0d0a 2020 2020 2020  nd("fr")..      
+00003960: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00003970: 732e 6170 7065 6e64 2822 676c 2229 0d0a  s.append("gl")..
+00003980: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00003990: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+000039a0: 6b61 2229 0d0a 2020 2020 2020 2020 7365  ka")..        se
+000039b0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+000039c0: 7065 6e64 2822 6465 2229 0d0a 2020 2020  pend("de")..    
+000039d0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+000039e0: 6465 732e 6170 7065 6e64 2822 656c 2229  des.append("el")
+000039f0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00003a00: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+00003a10: 2822 6775 2229 0d0a 2020 2020 2020 2020  ("gu")..        
+00003a20: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00003a30: 6170 7065 6e64 2822 6874 2229 0d0a 2020  append("ht")..  
+00003a40: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00003a50: 636f 6465 732e 6170 7065 6e64 2822 6861  codes.append("ha
+00003a60: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00003a70: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00003a80: 6e64 2822 6861 7722 290d 0a20 2020 2020  nd("haw")..     
+00003a90: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00003aa0: 6573 2e61 7070 656e 6428 2268 6522 290d  es.append("he").
+00003ab0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00003ac0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00003ad0: 2268 6922 290d 0a20 2020 2020 2020 2073  "hi")..        s
+00003ae0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00003af0: 7070 656e 6428 2268 7522 290d 0a20 2020  ppend("hu")..   
+00003b00: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00003b10: 6f64 6573 2e61 7070 656e 6428 2269 7322  odes.append("is"
+00003b20: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00003b30: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00003b40: 6428 2269 6422 290d 0a20 2020 2020 2020  d("id")..       
+00003b50: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00003b60: 2e61 7070 656e 6428 2269 7422 290d 0a20  .append("it").. 
+00003b70: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00003b80: 5f63 6f64 6573 2e61 7070 656e 6428 226a  _codes.append("j
+00003b90: 6122 290d 0a20 2020 2020 2020 2073 656c  a")..        sel
+00003ba0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+00003bb0: 656e 6428 226a 7622 290d 0a20 2020 2020  end("jv")..     
+00003bc0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00003bd0: 6573 2e61 7070 656e 6428 226b 6e22 290d  es.append("kn").
+00003be0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00003bf0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00003c00: 226b 6b22 290d 0a20 2020 2020 2020 2073  "kk")..        s
+00003c10: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00003c20: 7070 656e 6428 226b 6d22 290d 0a20 2020  ppend("km")..   
+00003c30: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00003c40: 6f64 6573 2e61 7070 656e 6428 226b 6f22  odes.append("ko"
+00003c50: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00003c60: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00003c70: 6428 226c 6f22 290d 0a20 2020 2020 2020  d("lo")..       
+00003c80: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00003c90: 2e61 7070 656e 6428 226c 6122 290d 0a20  .append("la").. 
+00003ca0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00003cb0: 5f63 6f64 6573 2e61 7070 656e 6428 226c  _codes.append("l
+00003cc0: 7622 290d 0a20 2020 2020 2020 2073 656c  v")..        sel
+00003cd0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+00003ce0: 656e 6428 226c 6e22 290d 0a20 2020 2020  end("ln")..     
+00003cf0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00003d00: 6573 2e61 7070 656e 6428 226c 7422 290d  es.append("lt").
+00003d10: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00003d20: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00003d30: 226c 6222 290d 0a20 2020 2020 2020 2073  "lb")..        s
+00003d40: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00003d50: 7070 656e 6428 226d 6b22 290d 0a20 2020  ppend("mk")..   
+00003d60: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00003d70: 6f64 6573 2e61 7070 656e 6428 226d 6722  odes.append("mg"
+00003d80: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00003d90: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00003da0: 6428 226d 7322 290d 0a20 2020 2020 2020  d("ms")..       
+00003db0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00003dc0: 2e61 7070 656e 6428 226d 6c22 290d 0a20  .append("ml").. 
+00003dd0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00003de0: 5f63 6f64 6573 2e61 7070 656e 6428 226d  _codes.append("m
+00003df0: 7422 290d 0a20 2020 2020 2020 2073 656c  t")..        sel
+00003e00: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+00003e10: 656e 6428 226d 6922 290d 0a20 2020 2020  end("mi")..     
+00003e20: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00003e30: 6573 2e61 7070 656e 6428 226d 7222 290d  es.append("mr").
+00003e40: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00003e50: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00003e60: 226d 6e22 290d 0a20 2020 2020 2020 2073  "mn")..        s
+00003e70: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00003e80: 7070 656e 6428 226d 7922 290d 0a20 2020  ppend("my")..   
+00003e90: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00003ea0: 6f64 6573 2e61 7070 656e 6428 226e 6522  odes.append("ne"
+00003eb0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00003ec0: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00003ed0: 6428 226e 6f22 290d 0a20 2020 2020 2020  d("no")..       
+00003ee0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00003ef0: 2e61 7070 656e 6428 226e 6e22 290d 0a20  .append("nn").. 
+00003f00: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00003f10: 5f63 6f64 6573 2e61 7070 656e 6428 226f  _codes.append("o
+00003f20: 6322 290d 0a20 2020 2020 2020 2073 656c  c")..        sel
+00003f30: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+00003f40: 656e 6428 2270 7322 290d 0a20 2020 2020  end("ps")..     
+00003f50: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00003f60: 6573 2e61 7070 656e 6428 2266 6122 290d  es.append("fa").
+00003f70: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00003f80: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00003f90: 2270 6c22 290d 0a20 2020 2020 2020 2073  "pl")..        s
+00003fa0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00003fb0: 7070 656e 6428 2270 7422 290d 0a20 2020  ppend("pt")..   
+00003fc0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00003fd0: 6f64 6573 2e61 7070 656e 6428 2270 6122  odes.append("pa"
+00003fe0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00003ff0: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00004000: 6428 2272 6f22 290d 0a20 2020 2020 2020  d("ro")..       
+00004010: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00004020: 2e61 7070 656e 6428 2272 7522 290d 0a20  .append("ru").. 
+00004030: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00004040: 5f63 6f64 6573 2e61 7070 656e 6428 2273  _codes.append("s
+00004050: 6122 290d 0a20 2020 2020 2020 2073 656c  a")..        sel
+00004060: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+00004070: 656e 6428 2273 7222 290d 0a20 2020 2020  end("sr")..     
+00004080: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00004090: 6573 2e61 7070 656e 6428 2273 6e22 290d  es.append("sn").
+000040a0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+000040b0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+000040c0: 2273 6422 290d 0a20 2020 2020 2020 2073  "sd")..        s
+000040d0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+000040e0: 7070 656e 6428 2273 6922 290d 0a20 2020  ppend("si")..   
+000040f0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00004100: 6f64 6573 2e61 7070 656e 6428 2273 6b22  odes.append("sk"
+00004110: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00004120: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00004130: 6428 2273 6c22 290d 0a20 2020 2020 2020  d("sl")..       
+00004140: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00004150: 2e61 7070 656e 6428 2273 6f22 290d 0a20  .append("so").. 
+00004160: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00004170: 5f63 6f64 6573 2e61 7070 656e 6428 2265  _codes.append("e
+00004180: 7322 290d 0a20 2020 2020 2020 2073 656c  s")..        sel
+00004190: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+000041a0: 656e 6428 2273 7522 290d 0a20 2020 2020  end("su")..     
+000041b0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+000041c0: 6573 2e61 7070 656e 6428 2273 7722 290d  es.append("sw").
+000041d0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+000041e0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+000041f0: 2273 7622 290d 0a20 2020 2020 2020 2073  "sv")..        s
+00004200: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00004210: 7070 656e 6428 2274 6c22 290d 0a20 2020  ppend("tl")..   
+00004220: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00004230: 6f64 6573 2e61 7070 656e 6428 2274 6722  odes.append("tg"
+00004240: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00004250: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00004260: 6428 2274 6122 290d 0a20 2020 2020 2020  d("ta")..       
+00004270: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00004280: 2e61 7070 656e 6428 2274 7422 290d 0a20  .append("tt").. 
+00004290: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+000042a0: 5f63 6f64 6573 2e61 7070 656e 6428 2274  _codes.append("t
+000042b0: 6522 290d 0a20 2020 2020 2020 2073 656c  e")..        sel
+000042c0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+000042d0: 656e 6428 2274 6822 290d 0a20 2020 2020  end("th")..     
+000042e0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+000042f0: 6573 2e61 7070 656e 6428 2262 6f22 290d  es.append("bo").
+00004300: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00004310: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00004320: 2274 7222 290d 0a20 2020 2020 2020 2073  "tr")..        s
+00004330: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00004340: 7070 656e 6428 2274 6b22 290d 0a20 2020  ppend("tk")..   
+00004350: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00004360: 6f64 6573 2e61 7070 656e 6428 2275 6b22  odes.append("uk"
+00004370: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00004380: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00004390: 6428 2275 7222 290d 0a20 2020 2020 2020  d("ur")..       
+000043a0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+000043b0: 2e61 7070 656e 6428 2275 7a22 290d 0a20  .append("uz").. 
+000043c0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+000043d0: 5f63 6f64 6573 2e61 7070 656e 6428 2276  _codes.append("v
+000043e0: 6922 290d 0a20 2020 2020 2020 2073 656c  i")..        sel
+000043f0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+00004400: 656e 6428 2263 7922 290d 0a20 2020 2020  end("cy")..     
+00004410: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00004420: 6573 2e61 7070 656e 6428 2279 6922 290d  es.append("yi").
+00004430: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00004440: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00004450: 2279 6f22 290d 0a0d 0a20 2020 2020 2020  "yo")....       
+00004460: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00004470: 203d 205b 5d0d 0a20 2020 2020 2020 2073   = []..        s
+00004480: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00004490: 7070 656e 6428 2241 6672 696b 6161 6e73  ppend("Afrikaans
+000044a0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+000044b0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+000044c0: 6e64 2822 416c 6261 6e69 616e 2229 0d0a  nd("Albanian")..
+000044d0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+000044e0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+000044f0: 416d 6861 7269 6322 290d 0a20 2020 2020  Amharic")..     
+00004500: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00004510: 6573 2e61 7070 656e 6428 2241 7261 6269  es.append("Arabi
+00004520: 6322 290d 0a20 2020 2020 2020 2073 656c  c")..        sel
+00004530: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00004540: 656e 6428 2241 726d 656e 6961 6e22 290d  end("Armenian").
+00004550: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00004560: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00004570: 2241 7373 616d 6573 6522 290d 0a20 2020  "Assamese")..   
+00004580: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00004590: 616d 6573 2e61 7070 656e 6428 2241 7a65  ames.append("Aze
+000045a0: 7262 6169 6a61 6e69 2229 0d0a 2020 2020  rbaijani")..    
+000045b0: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+000045c0: 6d65 732e 6170 7065 6e64 2822 4261 7368  mes.append("Bash
+000045d0: 6b69 7222 290d 0a20 2020 2020 2020 2073  kir")..        s
+000045e0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+000045f0: 7070 656e 6428 2242 6173 7175 6522 290d  ppend("Basque").
+00004600: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00004610: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00004620: 2242 656c 6172 7573 6961 6e22 290d 0a20  "Belarusian").. 
+00004630: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00004640: 5f6e 616d 6573 2e61 7070 656e 6428 2242  _names.append("B
+00004650: 656e 6761 6c69 2229 0d0a 2020 2020 2020  engali")..      
+00004660: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00004670: 732e 6170 7065 6e64 2822 426f 736e 6961  s.append("Bosnia
+00004680: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
+00004690: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+000046a0: 656e 6428 2242 7265 746f 6e22 290d 0a20  end("Breton").. 
+000046b0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+000046c0: 5f6e 616d 6573 2e61 7070 656e 6428 2242  _names.append("B
+000046d0: 756c 6761 7269 616e 2229 0d0a 2020 2020  ulgarian")..    
+000046e0: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+000046f0: 6d65 732e 6170 7065 6e64 2822 4361 7461  mes.append("Cata
+00004700: 6c61 6e22 290d 0a20 2020 2020 2020 2073  lan")..        s
+00004710: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00004720: 7070 656e 6428 2243 6869 6e65 7365 2229  ppend("Chinese")
+00004730: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00004740: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00004750: 2822 4372 6f61 7469 616e 2229 0d0a 2020  ("Croatian")..  
+00004760: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00004770: 6e61 6d65 732e 6170 7065 6e64 2822 437a  names.append("Cz
+00004780: 6563 6822 290d 0a20 2020 2020 2020 2073  ech")..        s
+00004790: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+000047a0: 7070 656e 6428 2244 616e 6973 6822 290d  ppend("Danish").
+000047b0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+000047c0: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+000047d0: 2244 7574 6368 2229 0d0a 2020 2020 2020  "Dutch")..      
+000047e0: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+000047f0: 732e 6170 7065 6e64 2822 456e 676c 6973  s.append("Englis
+00004800: 6822 290d 0a20 2020 2020 2020 2073 656c  h")..        sel
+00004810: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00004820: 656e 6428 2245 7374 6f6e 6961 6e22 290d  end("Estonian").
+00004830: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00004840: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00004850: 2246 6172 6f65 7365 2229 0d0a 2020 2020  "Faroese")..    
+00004860: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00004870: 6d65 732e 6170 7065 6e64 2822 4669 6e6e  mes.append("Finn
+00004880: 6973 6822 290d 0a20 2020 2020 2020 2073  ish")..        s
+00004890: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+000048a0: 7070 656e 6428 2246 7265 6e63 6822 290d  ppend("French").
+000048b0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+000048c0: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+000048d0: 2247 616c 6963 6961 6e22 290d 0a20 2020  "Galician")..   
+000048e0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+000048f0: 616d 6573 2e61 7070 656e 6428 2247 656f  ames.append("Geo
+00004900: 7267 6961 6e22 290d 0a20 2020 2020 2020  rgian")..       
+00004910: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00004920: 2e61 7070 656e 6428 2247 6572 6d61 6e22  .append("German"
+00004930: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00004940: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00004950: 6428 2247 7265 656b 2229 0d0a 2020 2020  d("Greek")..    
+00004960: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00004970: 6d65 732e 6170 7065 6e64 2822 4775 6a61  mes.append("Guja
+00004980: 7261 7469 2229 0d0a 2020 2020 2020 2020  rati")..        
+00004990: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+000049a0: 6170 7065 6e64 2822 4861 6974 6961 6e20  append("Haitian 
+000049b0: 4372 656f 6c65 2229 0d0a 2020 2020 2020  Creole")..      
+000049c0: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+000049d0: 732e 6170 7065 6e64 2822 4861 7573 6122  s.append("Hausa"
+000049e0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000049f0: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00004a00: 6428 2248 6177 6169 6961 6e22 290d 0a20  d("Hawaiian").. 
+00004a10: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00004a20: 5f6e 616d 6573 2e61 7070 656e 6428 2248  _names.append("H
+00004a30: 6562 7265 7722 290d 0a20 2020 2020 2020  ebrew")..       
+00004a40: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00004a50: 2e61 7070 656e 6428 2248 696e 6469 2229  .append("Hindi")
+00004a60: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00004a70: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00004a80: 2822 4875 6e67 6172 6961 6e22 290d 0a20  ("Hungarian").. 
+00004a90: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00004aa0: 5f6e 616d 6573 2e61 7070 656e 6428 2249  _names.append("I
+00004ab0: 6365 6c61 6e64 6963 2229 0d0a 2020 2020  celandic")..    
+00004ac0: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00004ad0: 6d65 732e 6170 7065 6e64 2822 496e 646f  mes.append("Indo
+00004ae0: 6e65 7369 616e 2229 0d0a 2020 2020 2020  nesian")..      
+00004af0: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00004b00: 732e 6170 7065 6e64 2822 4974 616c 6961  s.append("Italia
+00004b10: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
+00004b20: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00004b30: 656e 6428 224a 6170 616e 6573 6522 290d  end("Japanese").
+00004b40: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00004b50: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00004b60: 224a 6176 616e 6573 6522 290d 0a20 2020  "Javanese")..   
+00004b70: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00004b80: 616d 6573 2e61 7070 656e 6428 224b 616e  ames.append("Kan
+00004b90: 6e61 6461 2229 0d0a 2020 2020 2020 2020  nada")..        
+00004ba0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00004bb0: 6170 7065 6e64 2822 4b61 7a61 6b68 2229  append("Kazakh")
+00004bc0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00004bd0: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00004be0: 2822 4b68 6d65 7222 290d 0a20 2020 2020  ("Khmer")..     
+00004bf0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00004c00: 6573 2e61 7070 656e 6428 224b 6f72 6561  es.append("Korea
+00004c10: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
+00004c20: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00004c30: 656e 6428 224c 616f 2229 0d0a 2020 2020  end("Lao")..    
+00004c40: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00004c50: 6d65 732e 6170 7065 6e64 2822 4c61 7469  mes.append("Lati
+00004c60: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
+00004c70: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00004c80: 656e 6428 224c 6174 7669 616e 2229 0d0a  end("Latvian")..
+00004c90: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00004ca0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+00004cb0: 4c69 6e67 616c 6122 290d 0a20 2020 2020  Lingala")..     
+00004cc0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00004cd0: 6573 2e61 7070 656e 6428 224c 6974 6875  es.append("Lithu
+00004ce0: 616e 6961 6e22 290d 0a20 2020 2020 2020  anian")..       
+00004cf0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00004d00: 2e61 7070 656e 6428 224c 7578 656d 626f  .append("Luxembo
+00004d10: 7572 6769 7368 2229 0d0a 2020 2020 2020  urgish")..      
+00004d20: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00004d30: 732e 6170 7065 6e64 2822 4d61 6365 646f  s.append("Macedo
+00004d40: 6e69 616e 2229 0d0a 2020 2020 2020 2020  nian")..        
+00004d50: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00004d60: 6170 7065 6e64 2822 4d61 6c61 6761 7379  append("Malagasy
+00004d70: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00004d80: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00004d90: 6e64 2822 4d61 6c61 7922 290d 0a20 2020  nd("Malay")..   
+00004da0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00004db0: 616d 6573 2e61 7070 656e 6428 224d 616c  ames.append("Mal
+00004dc0: 6179 616c 616d 2229 0d0a 2020 2020 2020  ayalam")..      
+00004dd0: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00004de0: 732e 6170 7065 6e64 2822 4d61 6c74 6573  s.append("Maltes
+00004df0: 6522 290d 0a20 2020 2020 2020 2073 656c  e")..        sel
+00004e00: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00004e10: 656e 6428 224d 616f 7269 2229 0d0a 2020  end("Maori")..  
+00004e20: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00004e30: 6e61 6d65 732e 6170 7065 6e64 2822 4d61  names.append("Ma
+00004e40: 7261 7468 6922 290d 0a20 2020 2020 2020  rathi")..       
+00004e50: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00004e60: 2e61 7070 656e 6428 224d 6f6e 676f 6c69  .append("Mongoli
+00004e70: 616e 2229 0d0a 2020 2020 2020 2020 7365  an")..        se
+00004e80: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00004e90: 7065 6e64 2822 4d79 616e 6d61 7220 2842  pend("Myanmar (B
+00004ea0: 7572 6d65 7365 2922 290d 0a20 2020 2020  urmese)")..     
+00004eb0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00004ec0: 6573 2e61 7070 656e 6428 224e 6570 616c  es.append("Nepal
+00004ed0: 6922 290d 0a20 2020 2020 2020 2073 656c  i")..        sel
+00004ee0: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00004ef0: 656e 6428 224e 6f72 7765 6769 616e 2229  end("Norwegian")
+00004f00: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00004f10: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00004f20: 2822 4e79 6e6f 7273 6b22 290d 0a20 2020  ("Nynorsk")..   
+00004f30: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00004f40: 616d 6573 2e61 7070 656e 6428 224f 6363  ames.append("Occ
+00004f50: 6974 616e 2229 0d0a 2020 2020 2020 2020  itan")..        
+00004f60: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00004f70: 6170 7065 6e64 2822 5061 7368 746f 2229  append("Pashto")
+00004f80: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00004f90: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00004fa0: 2822 5065 7273 6961 6e22 290d 0a20 2020  ("Persian")..   
+00004fb0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00004fc0: 616d 6573 2e61 7070 656e 6428 2250 6f6c  ames.append("Pol
+00004fd0: 6973 6822 290d 0a20 2020 2020 2020 2073  ish")..        s
+00004fe0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00004ff0: 7070 656e 6428 2250 6f72 7475 6775 6573  ppend("Portugues
+00005000: 6522 290d 0a20 2020 2020 2020 2073 656c  e")..        sel
+00005010: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00005020: 656e 6428 2250 756e 6a61 6269 2229 0d0a  end("Punjabi")..
+00005030: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00005040: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+00005050: 526f 6d61 6e69 616e 2229 0d0a 2020 2020  Romanian")..    
+00005060: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00005070: 6d65 732e 6170 7065 6e64 2822 5275 7373  mes.append("Russ
+00005080: 6961 6e22 290d 0a20 2020 2020 2020 2073  ian")..        s
+00005090: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+000050a0: 7070 656e 6428 2253 616e 736b 7269 7422  ppend("Sanskrit"
+000050b0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000050c0: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+000050d0: 6428 2253 6572 6269 616e 2229 0d0a 2020  d("Serbian")..  
+000050e0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+000050f0: 6e61 6d65 732e 6170 7065 6e64 2822 5368  names.append("Sh
+00005100: 6f6e 6122 290d 0a20 2020 2020 2020 2073  ona")..        s
+00005110: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00005120: 7070 656e 6428 2253 696e 6468 6922 290d  ppend("Sindhi").
+00005130: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00005140: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00005150: 2253 696e 6861 6c61 2229 0d0a 2020 2020  "Sinhala")..    
+00005160: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00005170: 6d65 732e 6170 7065 6e64 2822 536c 6f76  mes.append("Slov
+00005180: 616b 2229 0d0a 2020 2020 2020 2020 7365  ak")..        se
+00005190: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+000051a0: 7065 6e64 2822 536c 6f76 656e 6961 6e22  pend("Slovenian"
+000051b0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000051c0: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+000051d0: 6428 2253 6f6d 616c 6922 290d 0a20 2020  d("Somali")..   
+000051e0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+000051f0: 616d 6573 2e61 7070 656e 6428 2253 7061  ames.append("Spa
+00005200: 6e69 7368 2229 0d0a 2020 2020 2020 2020  nish")..        
+00005210: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00005220: 6170 7065 6e64 2822 5375 6e64 616e 6573  append("Sundanes
+00005230: 6522 290d 0a20 2020 2020 2020 2073 656c  e")..        sel
+00005240: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00005250: 656e 6428 2253 7761 6869 6c69 2229 0d0a  end("Swahili")..
+00005260: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00005270: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+00005280: 5377 6564 6973 6822 290d 0a20 2020 2020  Swedish")..     
+00005290: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+000052a0: 6573 2e61 7070 656e 6428 2254 6167 616c  es.append("Tagal
+000052b0: 6f67 2229 0d0a 2020 2020 2020 2020 7365  og")..        se
+000052c0: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+000052d0: 7065 6e64 2822 5461 6a69 6b22 290d 0a20  pend("Tajik").. 
+000052e0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+000052f0: 5f6e 616d 6573 2e61 7070 656e 6428 2254  _names.append("T
+00005300: 616d 696c 2229 0d0a 2020 2020 2020 2020  amil")..        
+00005310: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00005320: 6170 7065 6e64 2822 5461 7461 7222 290d  append("Tatar").
+00005330: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00005340: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00005350: 2254 656c 7567 7522 290d 0a20 2020 2020  "Telugu")..     
+00005360: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00005370: 6573 2e61 7070 656e 6428 2254 6861 6922  es.append("Thai"
+00005380: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00005390: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+000053a0: 6428 2254 6962 6574 616e 2229 0d0a 2020  d("Tibetan")..  
+000053b0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+000053c0: 6e61 6d65 732e 6170 7065 6e64 2822 5475  names.append("Tu
+000053d0: 726b 6973 6822 290d 0a20 2020 2020 2020  rkish")..       
+000053e0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+000053f0: 2e61 7070 656e 6428 2254 7572 6b6d 656e  .append("Turkmen
+00005400: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00005410: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00005420: 6e64 2822 556b 7261 696e 6961 6e22 290d  nd("Ukrainian").
+00005430: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00005440: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00005450: 2255 7264 7522 290d 0a20 2020 2020 2020  "Urdu")..       
+00005460: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00005470: 2e61 7070 656e 6428 2255 7a62 656b 2229  .append("Uzbek")
+00005480: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00005490: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+000054a0: 2822 5669 6574 6e61 6d65 7365 2229 0d0a  ("Vietnamese")..
+000054b0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+000054c0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+000054d0: 5765 6c73 6822 290d 0a20 2020 2020 2020  Welsh")..       
+000054e0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+000054f0: 2e61 7070 656e 6428 2259 6964 6469 7368  .append("Yiddish
+00005500: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00005510: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00005520: 6e64 2822 596f 7275 6261 2229 0d0a 0d0a  nd("Yoruba")....
+00005530: 2020 2020 2020 2020 7365 6c66 2e63 6f64          self.cod
+00005540: 655f 6f66 5f6e 616d 6520 3d20 6469 6374  e_of_name = dict
+00005550: 287a 6970 2873 656c 662e 6c69 7374 5f6e  (zip(self.list_n
+00005560: 616d 6573 2c20 7365 6c66 2e6c 6973 745f  ames, self.list_
+00005570: 636f 6465 7329 290d 0a20 2020 2020 2020  codes))..       
+00005580: 2073 656c 662e 6e61 6d65 5f6f 665f 636f   self.name_of_co
+00005590: 6465 203d 2064 6963 7428 7a69 7028 7365  de = dict(zip(se
+000055a0: 6c66 2e6c 6973 745f 636f 6465 732c 2073  lf.list_codes, s
+000055b0: 656c 662e 6c69 7374 5f6e 616d 6573 2929  elf.list_names))
+000055c0: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
+000055d0: 2e64 6963 7420 3d20 7b0d 0a20 2020 2020  .dict = {..     
+000055e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055f0: 2020 2027 6166 273a 2027 4166 7269 6b61     'af': 'Afrika
+00005600: 616e 7327 2c0d 0a20 2020 2020 2020 2020  ans',..         
+00005610: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00005620: 7371 273a 2027 416c 6261 6e69 616e 272c  sq': 'Albanian',
+00005630: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005640: 2020 2020 2020 2020 2020 2761 6d27 3a20            'am': 
+00005650: 2741 6d68 6172 6963 272c 0d0a 2020 2020  'Amharic',..    
+00005660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005670: 2020 2020 2761 7227 3a20 2741 7261 6269      'ar': 'Arabi
+00005680: 6327 2c0d 0a20 2020 2020 2020 2020 2020  c',..           
+00005690: 2020 2020 2020 2020 2020 2020 2027 6879               'hy
+000056a0: 273a 2027 4172 6d65 6e69 616e 272c 0d0a  ': 'Armenian',..
+000056b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056c0: 2020 2020 2020 2020 2761 7327 3a20 2741          'as': 'A
+000056d0: 7373 616d 6573 6527 2c0d 0a20 2020 2020  ssamese',..     
+000056e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056f0: 2020 2027 617a 273a 2027 417a 6572 6261     'az': 'Azerba
+00005700: 696a 616e 6927 2c0d 0a20 2020 2020 2020  ijani',..       
+00005710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005720: 2027 6261 273a 2027 4261 7368 6b69 7227   'ba': 'Bashkir'
+00005730: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00005740: 2020 2020 2020 2020 2020 2027 6575 273a             'eu':
+00005750: 2027 4261 7371 7565 272c 0d0a 2020 2020   'Basque',..    
+00005760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005770: 2020 2020 2762 6527 3a20 2742 656c 6172      'be': 'Belar
+00005780: 7573 6961 6e27 2c0d 0a20 2020 2020 2020  usian',..       
+00005790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057a0: 2027 626e 273a 2027 4265 6e67 616c 6927   'bn': 'Bengali'
+000057b0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000057c0: 2020 2020 2020 2020 2020 2027 6273 273a             'bs':
+000057d0: 2027 426f 736e 6961 6e27 2c0d 0a20 2020   'Bosnian',..   
+000057e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057f0: 2020 2020 2027 6272 273a 2027 4272 6574       'br': 'Bret
+00005800: 6f6e 272c 0d0a 2020 2020 2020 2020 2020  on',..          
+00005810: 2020 2020 2020 2020 2020 2020 2020 2762                'b
+00005820: 6727 3a20 2742 756c 6761 7269 616e 272c  g': 'Bulgarian',
+00005830: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005840: 2020 2020 2020 2020 2020 2763 6127 3a20            'ca': 
+00005850: 2743 6174 616c 616e 272c 0d0a 2020 2020  'Catalan',..    
+00005860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005870: 2020 2020 277a 6827 3a20 2743 6869 6e65      'zh': 'Chine
+00005880: 7365 272c 0d0a 2020 2020 2020 2020 2020  se',..          
+00005890: 2020 2020 2020 2020 2020 2020 2020 2768                'h
+000058a0: 7227 3a20 2743 726f 6174 6961 6e27 2c0d  r': 'Croatian',.
+000058b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000058c0: 2020 2020 2020 2020 2027 6373 273a 2027           'cs': '
+000058d0: 437a 6563 6827 2c0d 0a20 2020 2020 2020  Czech',..       
+000058e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058f0: 2027 6461 273a 2027 4461 6e69 7368 272c   'da': 'Danish',
+00005900: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005910: 2020 2020 2020 2020 2020 276e 6c27 3a20            'nl': 
+00005920: 2744 7574 6368 272c 0d0a 2020 2020 2020  'Dutch',..      
+00005930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005940: 2020 2765 6e27 3a20 2745 6e67 6c69 7368    'en': 'English
+00005950: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00005960: 2020 2020 2020 2020 2020 2020 2765 7427              'et'
+00005970: 3a20 2745 7374 6f6e 6961 6e27 2c0d 0a20  : 'Estonian',.. 
+00005980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005990: 2020 2020 2020 2027 666f 273a 2027 4661         'fo': 'Fa
+000059a0: 726f 6573 6527 2c0d 0a20 2020 2020 2020  roese',..       
+000059b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059c0: 2027 6669 273a 2027 4669 6e6e 6973 6827   'fi': 'Finnish'
+000059d0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000059e0: 2020 2020 2020 2020 2020 2027 6672 273a             'fr':
+000059f0: 2027 4672 656e 6368 272c 0d0a 2020 2020   'French',..    
+00005a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a10: 2020 2020 2767 6c27 3a20 2747 616c 6963      'gl': 'Galic
+00005a20: 6961 6e27 2c0d 0a20 2020 2020 2020 2020  ian',..         
+00005a30: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00005a40: 6b61 273a 2027 4765 6f72 6769 616e 272c  ka': 'Georgian',
+00005a50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005a60: 2020 2020 2020 2020 2020 2764 6527 3a20            'de': 
+00005a70: 2747 6572 6d61 6e27 2c0d 0a20 2020 2020  'German',..     
+00005a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a90: 2020 2027 656c 273a 2027 4772 6565 6b27     'el': 'Greek'
+00005aa0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00005ab0: 2020 2020 2020 2020 2020 2027 6775 273a             'gu':
+00005ac0: 2027 4775 6a61 7261 7469 272c 0d0a 2020   'Gujarati',..  
+00005ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ae0: 2020 2020 2020 2768 7427 3a20 2748 6169        'ht': 'Hai
+00005af0: 7469 616e 2043 7265 6f6c 6527 2c0d 0a20  tian Creole',.. 
+00005b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b10: 2020 2020 2020 2027 6861 273a 2027 4861         'ha': 'Ha
+00005b20: 7573 6127 2c0d 0a20 2020 2020 2020 2020  usa',..         
+00005b30: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00005b40: 6861 7727 3a20 2748 6177 6169 6961 6e27  haw': 'Hawaiian'
+00005b50: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00005b60: 2020 2020 2020 2020 2020 2027 6865 273a             'he':
+00005b70: 2027 4865 6272 6577 272c 0d0a 2020 2020   'Hebrew',..    
+00005b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b90: 2020 2020 2768 6927 3a20 2748 696e 6469      'hi': 'Hindi
+00005ba0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00005bb0: 2020 2020 2020 2020 2020 2020 2768 7527              'hu'
+00005bc0: 3a20 2748 756e 6761 7269 616e 272c 0d0a  : 'Hungarian',..
+00005bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005be0: 2020 2020 2020 2020 2769 7327 3a20 2749          'is': 'I
+00005bf0: 6365 6c61 6e64 6963 272c 0d0a 2020 2020  celandic',..    
+00005c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c10: 2020 2020 2769 6427 3a20 2749 6e64 6f6e      'id': 'Indon
+00005c20: 6573 6961 6e27 2c0d 0a20 2020 2020 2020  esian',..       
+00005c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c40: 2027 6974 273a 2027 4974 616c 6961 6e27   'it': 'Italian'
+00005c50: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00005c60: 2020 2020 2020 2020 2020 2027 6a61 273a             'ja':
+00005c70: 2027 4a61 7061 6e65 7365 272c 0d0a 2020   'Japanese',..  
+00005c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c90: 2020 2020 2020 276a 7627 3a20 274a 6176        'jv': 'Jav
+00005ca0: 616e 6573 6527 2c0d 0a20 2020 2020 2020  anese',..       
+00005cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005cc0: 2027 6b6e 273a 2027 4b61 6e6e 6164 6127   'kn': 'Kannada'
+00005cd0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00005ce0: 2020 2020 2020 2020 2020 2027 6b6b 273a             'kk':
+00005cf0: 2027 4b61 7a61 6b68 272c 0d0a 2020 2020   'Kazakh',..    
+00005d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d10: 2020 2020 276b 6d27 3a20 274b 686d 6572      'km': 'Khmer
+00005d20: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00005d30: 2020 2020 2020 2020 2020 2020 276b 6f27              'ko'
+00005d40: 3a20 274b 6f72 6561 6e27 2c0d 0a20 2020  : 'Korean',..   
+00005d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d60: 2020 2020 2027 6c6f 273a 2027 4c61 6f27       'lo': 'Lao'
+00005d70: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00005d80: 2020 2020 2020 2020 2020 2027 6c61 273a             'la':
+00005d90: 2027 4c61 7469 6e27 2c0d 0a20 2020 2020   'Latin',..     
+00005da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005db0: 2020 2027 6c76 273a 2027 4c61 7476 6961     'lv': 'Latvia
+00005dc0: 6e27 2c0d 0a20 2020 2020 2020 2020 2020  n',..           
+00005dd0: 2020 2020 2020 2020 2020 2020 2027 6c6e               'ln
+00005de0: 273a 2027 4c69 6e67 616c 6127 2c0d 0a20  ': 'Lingala',.. 
+00005df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e00: 2020 2020 2020 2027 6c74 273a 2027 4c69         'lt': 'Li
+00005e10: 7468 7561 6e69 616e 272c 0d0a 2020 2020  thuanian',..    
+00005e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e30: 2020 2020 276c 6227 3a20 274c 7578 656d      'lb': 'Luxem
+00005e40: 626f 7572 6769 7368 272c 0d0a 2020 2020  bourgish',..    
+00005e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e60: 2020 2020 276d 6b27 3a20 274d 6163 6564      'mk': 'Maced
+00005e70: 6f6e 6961 6e27 2c0d 0a20 2020 2020 2020  onian',..       
+00005e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e90: 2027 6d67 273a 2027 4d61 6c61 6761 7379   'mg': 'Malagasy
+00005ea0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00005eb0: 2020 2020 2020 2020 2020 2020 276d 7327              'ms'
+00005ec0: 3a20 274d 616c 6179 272c 0d0a 2020 2020  : 'Malay',..    
+00005ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ee0: 2020 2020 276d 6c27 3a20 274d 616c 6179      'ml': 'Malay
+00005ef0: 616c 616d 272c 0d0a 2020 2020 2020 2020  alam',..        
+00005f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f10: 276d 7427 3a20 274d 616c 7465 7365 272c  'mt': 'Maltese',
+00005f20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005f30: 2020 2020 2020 2020 2020 276d 6927 3a20            'mi': 
+00005f40: 274d 616f 7269 272c 0d0a 2020 2020 2020  'Maori',..      
+00005f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f60: 2020 276d 7227 3a20 274d 6172 6174 6869    'mr': 'Marathi
+00005f70: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00005f80: 2020 2020 2020 2020 2020 2020 276d 6e27              'mn'
+00005f90: 3a20 274d 6f6e 676f 6c69 616e 272c 0d0a  : 'Mongolian',..
+00005fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fb0: 2020 2020 2020 2020 276d 7927 3a20 274d          'my': 'M
+00005fc0: 7961 6e6d 6172 2028 4275 726d 6573 6529  yanmar (Burmese)
+00005fd0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00005fe0: 2020 2020 2020 2020 2020 2020 276e 6527              'ne'
+00005ff0: 3a20 274e 6570 616c 6927 2c0d 0a20 2020  : 'Nepali',..   
+00006000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006010: 2020 2020 2027 6e6f 273a 2027 4e6f 7277       'no': 'Norw
+00006020: 6567 6961 6e27 2c0d 0a20 2020 2020 2020  egian',..       
+00006030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006040: 2027 6e6e 273a 2027 4e79 6e6f 7273 6b27   'nn': 'Nynorsk'
+00006050: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00006060: 2020 2020 2020 2020 2020 2027 6f63 273a             'oc':
+00006070: 2027 4f63 6369 7461 6e27 2c0d 0a20 2020   'Occitan',..   
+00006080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006090: 2020 2020 2027 7073 273a 2027 5061 7368       'ps': 'Pash
+000060a0: 746f 272c 0d0a 2020 2020 2020 2020 2020  to',..          
+000060b0: 2020 2020 2020 2020 2020 2020 2020 2766                'f
+000060c0: 6127 3a20 2750 6572 7369 616e 272c 0d0a  a': 'Persian',..
+000060d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060e0: 2020 2020 2020 2020 2770 6c27 3a20 2750          'pl': 'P
+000060f0: 6f6c 6973 6827 2c0d 0a20 2020 2020 2020  olish',..       
+00006100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006110: 2027 7074 273a 2027 506f 7274 7567 7565   'pt': 'Portugue
+00006120: 7365 272c 0d0a 2020 2020 2020 2020 2020  se',..          
+00006130: 2020 2020 2020 2020 2020 2020 2020 2770                'p
+00006140: 6127 3a20 2750 756e 6a61 6269 272c 0d0a  a': 'Punjabi',..
+00006150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006160: 2020 2020 2020 2020 2772 6f27 3a20 2752          'ro': 'R
+00006170: 6f6d 616e 6961 6e27 2c0d 0a20 2020 2020  omanian',..     
+00006180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006190: 2020 2027 7275 273a 2027 5275 7373 6961     'ru': 'Russia
+000061a0: 6e27 2c0d 0a20 2020 2020 2020 2020 2020  n',..           
+000061b0: 2020 2020 2020 2020 2020 2020 2027 7361               'sa
+000061c0: 273a 2027 5361 6e73 6b72 6974 272c 0d0a  ': 'Sanskrit',..
+000061d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061e0: 2020 2020 2020 2020 2773 7227 3a20 2753          'sr': 'S
+000061f0: 6572 6269 616e 272c 0d0a 2020 2020 2020  erbian',..      
+00006200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006210: 2020 2773 6e27 3a20 2753 686f 6e61 272c    'sn': 'Shona',
+00006220: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006230: 2020 2020 2020 2020 2020 2773 6427 3a20            'sd': 
+00006240: 2753 696e 6468 6927 2c0d 0a20 2020 2020  'Sindhi',..     
+00006250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006260: 2020 2027 7369 273a 2027 5369 6e68 616c     'si': 'Sinhal
+00006270: 6127 2c0d 0a20 2020 2020 2020 2020 2020  a',..           
+00006280: 2020 2020 2020 2020 2020 2020 2027 736b               'sk
+00006290: 273a 2027 536c 6f76 616b 272c 0d0a 2020  ': 'Slovak',..  
+000062a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062b0: 2020 2020 2020 2773 6c27 3a20 2753 6c6f        'sl': 'Slo
+000062c0: 7665 6e69 616e 272c 0d0a 2020 2020 2020  venian',..      
+000062d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062e0: 2020 2773 6f27 3a20 2753 6f6d 616c 6927    'so': 'Somali'
+000062f0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00006300: 2020 2020 2020 2020 2020 2027 6573 273a             'es':
+00006310: 2027 5370 616e 6973 6827 2c0d 0a20 2020   'Spanish',..   
+00006320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006330: 2020 2020 2027 7375 273a 2027 5375 6e64       'su': 'Sund
+00006340: 616e 6573 6527 2c0d 0a20 2020 2020 2020  anese',..       
+00006350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006360: 2027 7377 273a 2027 5377 6168 696c 6927   'sw': 'Swahili'
+00006370: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00006380: 2020 2020 2020 2020 2020 2027 7376 273a             'sv':
+00006390: 2027 5377 6564 6973 6827 2c0d 0a20 2020   'Swedish',..   
+000063a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063b0: 2020 2020 2027 746c 273a 2027 5461 6761       'tl': 'Taga
+000063c0: 6c6f 6727 2c0d 0a20 2020 2020 2020 2020  log',..         
+000063d0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000063e0: 7467 273a 2027 5461 6a69 6b27 2c0d 0a20  tg': 'Tajik',.. 
+000063f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006400: 2020 2020 2020 2027 7461 273a 2027 5461         'ta': 'Ta
+00006410: 6d69 6c27 2c0d 0a20 2020 2020 2020 2020  mil',..         
+00006420: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00006430: 7474 273a 2027 5461 7461 7227 2c0d 0a20  tt': 'Tatar',.. 
+00006440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006450: 2020 2020 2020 2027 7465 273a 2027 5465         'te': 'Te
+00006460: 6c75 6775 272c 0d0a 2020 2020 2020 2020  lugu',..        
+00006470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006480: 2774 6827 3a20 2754 6861 6927 2c0d 0a20  'th': 'Thai',.. 
+00006490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000064a0: 2020 2020 2020 2027 626f 273a 2027 5469         'bo': 'Ti
+000064b0: 6265 7461 6e27 2c0d 0a20 2020 2020 2020  betan',..       
+000064c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000064d0: 2027 7472 273a 2027 5475 726b 6973 6827   'tr': 'Turkish'
+000064e0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000064f0: 2020 2020 2020 2020 2020 2027 746b 273a             'tk':
+00006500: 2027 5475 726b 6d65 6e27 2c0d 0a20 2020   'Turkmen',..   
+00006510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006520: 2020 2020 2027 756b 273a 2027 556b 7261       'uk': 'Ukra
+00006530: 696e 6961 6e27 2c0d 0a20 2020 2020 2020  inian',..       
+00006540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006550: 2027 7572 273a 2027 5572 6475 272c 0d0a   'ur': 'Urdu',..
+00006560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006570: 2020 2020 2020 2020 2775 7a27 3a20 2755          'uz': 'U
+00006580: 7a62 656b 272c 0d0a 2020 2020 2020 2020  zbek',..        
+00006590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065a0: 2776 6927 3a20 2756 6965 746e 616d 6573  'vi': 'Vietnames
+000065b0: 6527 2c0d 0a20 2020 2020 2020 2020 2020  e',..           
+000065c0: 2020 2020 2020 2020 2020 2020 2027 6379               'cy
+000065d0: 273a 2027 5765 6c73 6827 2c0d 0a20 2020  ': 'Welsh',..   
+000065e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065f0: 2020 2020 2027 7969 273a 2027 5969 6464       'yi': 'Yidd
+00006600: 6973 6827 2c0d 0a20 2020 2020 2020 2020  ish',..         
+00006610: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00006620: 796f 273a 2027 596f 7275 6261 272c 0d0a  yo': 'Yoruba',..
+00006630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006640: 2020 2020 7d0d 0a0d 0a20 2020 2064 6566      }....    def
+00006650: 2067 6574 5f6e 616d 6528 7365 6c66 2c20   get_name(self, 
+00006660: 6765 745f 636f 6465 293a 0d0a 2020 2020  get_code):..    
+00006670: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00006680: 6469 6374 2e67 6574 2867 6574 5f63 6f64  dict.get(get_cod
+00006690: 652e 6c6f 7765 7228 292c 2022 2229 0d0a  e.lower(), "")..
+000066a0: 0d0a 2020 2020 6465 6620 6765 745f 636f  ..    def get_co
+000066b0: 6465 2873 656c 662c 206c 616e 6775 6167  de(self, languag
+000066c0: 6529 3a0d 0a20 2020 2020 2020 2066 6f72  e):..        for
+000066d0: 2067 6574 5f63 6f64 652c 206c 616e 6720   get_code, lang 
+000066e0: 696e 2073 656c 662e 6469 6374 2e69 7465  in self.dict.ite
+000066f0: 6d73 2829 3a0d 0a20 2020 2020 2020 2020  ms():..         
+00006700: 2020 2069 6620 6c61 6e67 2e6c 6f77 6572     if lang.lower
+00006710: 2829 203d 3d20 6c61 6e67 7561 6765 2e6c  () == language.l
+00006720: 6f77 6572 2829 3a0d 0a20 2020 2020 2020  ower():..       
+00006730: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00006740: 6765 745f 636f 6465 0d0a 2020 2020 2020  get_code..      
+00006750: 2020 7265 7475 726e 2022 220d 0a0d 0a0d    return "".....
+00006760: 0a63 6c61 7373 2047 6f6f 676c 654c 616e  .class GoogleLan
+00006770: 6775 6167 653a 0d0a 2020 2020 6465 6620  guage:..    def 
+00006780: 5f5f 696e 6974 5f5f 2873 656c 6629 3a0d  __init__(self):.
+00006790: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+000067a0: 7374 5f63 6f64 6573 203d 205b 5d0d 0a20  st_codes = [].. 
+000067b0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+000067c0: 5f63 6f64 6573 2e61 7070 656e 6428 2261  _codes.append("a
+000067d0: 6622 290d 0a20 2020 2020 2020 2073 656c  f")..        sel
+000067e0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+000067f0: 656e 6428 2273 7122 290d 0a20 2020 2020  end("sq")..     
+00006800: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00006810: 6573 2e61 7070 656e 6428 2261 6d22 290d  es.append("am").
+00006820: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00006830: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00006840: 2261 7222 290d 0a20 2020 2020 2020 2073  "ar")..        s
+00006850: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00006860: 7070 656e 6428 2268 7922 290d 0a20 2020  ppend("hy")..   
+00006870: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00006880: 6f64 6573 2e61 7070 656e 6428 2261 7322  odes.append("as"
+00006890: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000068a0: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+000068b0: 6428 2261 7922 290d 0a20 2020 2020 2020  d("ay")..       
+000068c0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+000068d0: 2e61 7070 656e 6428 2261 7a22 290d 0a20  .append("az").. 
+000068e0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+000068f0: 5f63 6f64 6573 2e61 7070 656e 6428 2262  _codes.append("b
+00006900: 6d22 290d 0a20 2020 2020 2020 2073 656c  m")..        sel
+00006910: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+00006920: 656e 6428 2265 7522 290d 0a20 2020 2020  end("eu")..     
+00006930: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00006940: 6573 2e61 7070 656e 6428 2262 6522 290d  es.append("be").
+00006950: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00006960: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00006970: 2262 6e22 290d 0a20 2020 2020 2020 2073  "bn")..        s
+00006980: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00006990: 7070 656e 6428 2262 686f 2229 0d0a 2020  ppend("bho")..  
+000069a0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+000069b0: 636f 6465 732e 6170 7065 6e64 2822 6273  codes.append("bs
+000069c0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+000069d0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+000069e0: 6e64 2822 6267 2229 0d0a 2020 2020 2020  nd("bg")..      
+000069f0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00006a00: 732e 6170 7065 6e64 2822 6361 2229 0d0a  s.append("ca")..
+00006a10: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00006a20: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00006a30: 6365 6222 290d 0a20 2020 2020 2020 2073  ceb")..        s
+00006a40: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00006a50: 7070 656e 6428 226e 7922 290d 0a20 2020  ppend("ny")..   
+00006a60: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00006a70: 6f64 6573 2e61 7070 656e 6428 227a 682d  odes.append("zh-
+00006a80: 434e 2229 0d0a 2020 2020 2020 2020 7365  CN")..        se
+00006a90: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00006aa0: 7065 6e64 2822 7a68 2d54 5722 290d 0a20  pend("zh-TW").. 
+00006ab0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00006ac0: 5f63 6f64 6573 2e61 7070 656e 6428 2263  _codes.append("c
+00006ad0: 6f22 290d 0a20 2020 2020 2020 2073 656c  o")..        sel
+00006ae0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+00006af0: 656e 6428 2268 7222 290d 0a20 2020 2020  end("hr")..     
+00006b00: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00006b10: 6573 2e61 7070 656e 6428 2263 7322 290d  es.append("cs").
+00006b20: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00006b30: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00006b40: 2264 6122 290d 0a20 2020 2020 2020 2073  "da")..        s
+00006b50: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00006b60: 7070 656e 6428 2264 7622 290d 0a20 2020  ppend("dv")..   
+00006b70: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00006b80: 6f64 6573 2e61 7070 656e 6428 2264 6f69  odes.append("doi
+00006b90: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00006ba0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00006bb0: 6e64 2822 6e6c 2229 0d0a 2020 2020 2020  nd("nl")..      
+00006bc0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00006bd0: 732e 6170 7065 6e64 2822 656e 2229 0d0a  s.append("en")..
+00006be0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00006bf0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00006c00: 656f 2229 0d0a 2020 2020 2020 2020 7365  eo")..        se
+00006c10: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00006c20: 7065 6e64 2822 6574 2229 0d0a 2020 2020  pend("et")..    
+00006c30: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+00006c40: 6465 732e 6170 7065 6e64 2822 6565 2229  des.append("ee")
+00006c50: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00006c60: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+00006c70: 2822 6669 6c22 290d 0a20 2020 2020 2020  ("fil")..       
+00006c80: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00006c90: 2e61 7070 656e 6428 2266 6922 290d 0a20  .append("fi").. 
+00006ca0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00006cb0: 5f63 6f64 6573 2e61 7070 656e 6428 2266  _codes.append("f
+00006cc0: 7222 290d 0a20 2020 2020 2020 2073 656c  r")..        sel
+00006cd0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+00006ce0: 656e 6428 2266 7922 290d 0a20 2020 2020  end("fy")..     
+00006cf0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00006d00: 6573 2e61 7070 656e 6428 2267 6c22 290d  es.append("gl").
+00006d10: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00006d20: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00006d30: 226b 6122 290d 0a20 2020 2020 2020 2073  "ka")..        s
+00006d40: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00006d50: 7070 656e 6428 2264 6522 290d 0a20 2020  ppend("de")..   
+00006d60: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00006d70: 6f64 6573 2e61 7070 656e 6428 2265 6c22  odes.append("el"
+00006d80: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00006d90: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00006da0: 6428 2267 6e22 290d 0a20 2020 2020 2020  d("gn")..       
+00006db0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00006dc0: 2e61 7070 656e 6428 2267 7522 290d 0a20  .append("gu").. 
+00006dd0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00006de0: 5f63 6f64 6573 2e61 7070 656e 6428 2268  _codes.append("h
+00006df0: 7422 290d 0a20 2020 2020 2020 2073 656c  t")..        sel
+00006e00: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+00006e10: 656e 6428 2268 6122 290d 0a20 2020 2020  end("ha")..     
+00006e20: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00006e30: 6573 2e61 7070 656e 6428 2268 6177 2229  es.append("haw")
+00006e40: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00006e50: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+00006e60: 2822 6865 2229 0d0a 2020 2020 2020 2020  ("he")..        
+00006e70: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00006e80: 6170 7065 6e64 2822 6869 2229 0d0a 2020  append("hi")..  
+00006e90: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00006ea0: 636f 6465 732e 6170 7065 6e64 2822 686d  codes.append("hm
+00006eb0: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
+00006ec0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+00006ed0: 656e 6428 2268 7522 290d 0a20 2020 2020  end("hu")..     
+00006ee0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00006ef0: 6573 2e61 7070 656e 6428 2269 7322 290d  es.append("is").
+00006f00: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00006f10: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00006f20: 2269 6722 290d 0a20 2020 2020 2020 2073  "ig")..        s
+00006f30: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00006f40: 7070 656e 6428 2269 6c6f 2229 0d0a 2020  ppend("ilo")..  
+00006f50: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00006f60: 636f 6465 732e 6170 7065 6e64 2822 6964  codes.append("id
+00006f70: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00006f80: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00006f90: 6e64 2822 6761 2229 0d0a 2020 2020 2020  nd("ga")..      
+00006fa0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00006fb0: 732e 6170 7065 6e64 2822 6974 2229 0d0a  s.append("it")..
+00006fc0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00006fd0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00006fe0: 6a61 2229 0d0a 2020 2020 2020 2020 7365  ja")..        se
+00006ff0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00007000: 7065 6e64 2822 6a76 2229 0d0a 2020 2020  pend("jv")..    
+00007010: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+00007020: 6465 732e 6170 7065 6e64 2822 6b6e 2229  des.append("kn")
+00007030: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00007040: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+00007050: 2822 6b6b 2229 0d0a 2020 2020 2020 2020  ("kk")..        
+00007060: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00007070: 6170 7065 6e64 2822 6b6d 2229 0d0a 2020  append("km")..  
+00007080: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00007090: 636f 6465 732e 6170 7065 6e64 2822 7277  codes.append("rw
+000070a0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+000070b0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+000070c0: 6e64 2822 676f 6d22 290d 0a20 2020 2020  nd("gom")..     
+000070d0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+000070e0: 6573 2e61 7070 656e 6428 226b 6f22 290d  es.append("ko").
+000070f0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00007100: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00007110: 226b 7269 2229 0d0a 2020 2020 2020 2020  "kri")..        
+00007120: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00007130: 6170 7065 6e64 2822 6b6d 7222 290d 0a20  append("kmr").. 
+00007140: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00007150: 5f63 6f64 6573 2e61 7070 656e 6428 2263  _codes.append("c
+00007160: 6b62 2229 0d0a 2020 2020 2020 2020 7365  kb")..        se
+00007170: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00007180: 7065 6e64 2822 6b79 2229 0d0a 2020 2020  pend("ky")..    
+00007190: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+000071a0: 6465 732e 6170 7065 6e64 2822 6c6f 2229  des.append("lo")
+000071b0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+000071c0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+000071d0: 2822 6c61 2229 0d0a 2020 2020 2020 2020  ("la")..        
+000071e0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+000071f0: 6170 7065 6e64 2822 6c76 2229 0d0a 2020  append("lv")..  
+00007200: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00007210: 636f 6465 732e 6170 7065 6e64 2822 6c6e  codes.append("ln
+00007220: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00007230: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00007240: 6e64 2822 6c74 2229 0d0a 2020 2020 2020  nd("lt")..      
+00007250: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00007260: 732e 6170 7065 6e64 2822 6c67 2229 0d0a  s.append("lg")..
+00007270: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00007280: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00007290: 6c62 2229 0d0a 2020 2020 2020 2020 7365  lb")..        se
+000072a0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+000072b0: 7065 6e64 2822 6d6b 2229 0d0a 2020 2020  pend("mk")..    
+000072c0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+000072d0: 6465 732e 6170 7065 6e64 2822 6d67 2229  des.append("mg")
+000072e0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+000072f0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+00007300: 2822 6d73 2229 0d0a 2020 2020 2020 2020  ("ms")..        
+00007310: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00007320: 6170 7065 6e64 2822 6d6c 2229 0d0a 2020  append("ml")..  
+00007330: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00007340: 636f 6465 732e 6170 7065 6e64 2822 6d74  codes.append("mt
+00007350: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00007360: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00007370: 6e64 2822 6d69 2229 0d0a 2020 2020 2020  nd("mi")..      
+00007380: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00007390: 732e 6170 7065 6e64 2822 6d72 2229 0d0a  s.append("mr")..
+000073a0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+000073b0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+000073c0: 6d6e 692d 4d74 6569 2229 0d0a 2020 2020  mni-Mtei")..    
+000073d0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+000073e0: 6465 732e 6170 7065 6e64 2822 6c75 7322  des.append("lus"
+000073f0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00007400: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00007410: 6428 226d 6e22 290d 0a20 2020 2020 2020  d("mn")..       
+00007420: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00007430: 2e61 7070 656e 6428 226d 7922 290d 0a20  .append("my").. 
+00007440: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00007450: 5f63 6f64 6573 2e61 7070 656e 6428 226e  _codes.append("n
+00007460: 6522 290d 0a20 2020 2020 2020 2073 656c  e")..        sel
+00007470: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+00007480: 656e 6428 226e 6f22 290d 0a20 2020 2020  end("no")..     
+00007490: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+000074a0: 6573 2e61 7070 656e 6428 226f 7222 290d  es.append("or").
+000074b0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+000074c0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+000074d0: 226f 6d22 290d 0a20 2020 2020 2020 2073  "om")..        s
+000074e0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+000074f0: 7070 656e 6428 2270 7322 290d 0a20 2020  ppend("ps")..   
+00007500: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00007510: 6f64 6573 2e61 7070 656e 6428 2266 6122  odes.append("fa"
+00007520: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00007530: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00007540: 6428 2270 6c22 290d 0a20 2020 2020 2020  d("pl")..       
+00007550: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00007560: 2e61 7070 656e 6428 2270 7422 290d 0a20  .append("pt").. 
+00007570: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00007580: 5f63 6f64 6573 2e61 7070 656e 6428 2270  _codes.append("p
+00007590: 6122 290d 0a20 2020 2020 2020 2073 656c  a")..        sel
+000075a0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+000075b0: 656e 6428 2271 7522 290d 0a20 2020 2020  end("qu")..     
+000075c0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+000075d0: 6573 2e61 7070 656e 6428 2272 6f22 290d  es.append("ro").
+000075e0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+000075f0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00007600: 2272 7522 290d 0a20 2020 2020 2020 2073  "ru")..        s
+00007610: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00007620: 7070 656e 6428 2273 6d22 290d 0a20 2020  ppend("sm")..   
+00007630: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00007640: 6f64 6573 2e61 7070 656e 6428 2273 6122  odes.append("sa"
+00007650: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00007660: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00007670: 6428 2267 6422 290d 0a20 2020 2020 2020  d("gd")..       
+00007680: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00007690: 2e61 7070 656e 6428 226e 736f 2229 0d0a  .append("nso")..
+000076a0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+000076b0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+000076c0: 7372 2229 0d0a 2020 2020 2020 2020 7365  sr")..        se
+000076d0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+000076e0: 7065 6e64 2822 7374 2229 0d0a 2020 2020  pend("st")..    
+000076f0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+00007700: 6465 732e 6170 7065 6e64 2822 736e 2229  des.append("sn")
+00007710: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00007720: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+00007730: 2822 7364 2229 0d0a 2020 2020 2020 2020  ("sd")..        
+00007740: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00007750: 6170 7065 6e64 2822 7369 2229 0d0a 2020  append("si")..  
+00007760: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00007770: 636f 6465 732e 6170 7065 6e64 2822 736b  codes.append("sk
+00007780: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00007790: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+000077a0: 6e64 2822 736c 2229 0d0a 2020 2020 2020  nd("sl")..      
+000077b0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+000077c0: 732e 6170 7065 6e64 2822 736f 2229 0d0a  s.append("so")..
+000077d0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+000077e0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+000077f0: 6573 2229 0d0a 2020 2020 2020 2020 7365  es")..        se
+00007800: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00007810: 7065 6e64 2822 7375 2229 0d0a 2020 2020  pend("su")..    
+00007820: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+00007830: 6465 732e 6170 7065 6e64 2822 7377 2229  des.append("sw")
+00007840: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00007850: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+00007860: 2822 7376 2229 0d0a 2020 2020 2020 2020  ("sv")..        
+00007870: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00007880: 6170 7065 6e64 2822 7467 2229 0d0a 2020  append("tg")..  
+00007890: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+000078a0: 636f 6465 732e 6170 7065 6e64 2822 7461  codes.append("ta
+000078b0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+000078c0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+000078d0: 6e64 2822 7474 2229 0d0a 2020 2020 2020  nd("tt")..      
+000078e0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+000078f0: 732e 6170 7065 6e64 2822 7465 2229 0d0a  s.append("te")..
+00007900: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00007910: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00007920: 7468 2229 0d0a 2020 2020 2020 2020 7365  th")..        se
+00007930: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00007940: 7065 6e64 2822 7469 2229 0d0a 2020 2020  pend("ti")..    
+00007950: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+00007960: 6465 732e 6170 7065 6e64 2822 7473 2229  des.append("ts")
+00007970: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00007980: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+00007990: 2822 7472 2229 0d0a 2020 2020 2020 2020  ("tr")..        
+000079a0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+000079b0: 6170 7065 6e64 2822 746b 2229 0d0a 2020  append("tk")..  
+000079c0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+000079d0: 636f 6465 732e 6170 7065 6e64 2822 7477  codes.append("tw
+000079e0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+000079f0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00007a00: 6e64 2822 756b 2229 0d0a 2020 2020 2020  nd("uk")..      
+00007a10: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00007a20: 732e 6170 7065 6e64 2822 7572 2229 0d0a  s.append("ur")..
+00007a30: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00007a40: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00007a50: 7567 2229 0d0a 2020 2020 2020 2020 7365  ug")..        se
+00007a60: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00007a70: 7065 6e64 2822 757a 2229 0d0a 2020 2020  pend("uz")..    
+00007a80: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+00007a90: 6465 732e 6170 7065 6e64 2822 7669 2229  des.append("vi")
+00007aa0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00007ab0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+00007ac0: 2822 6379 2229 0d0a 2020 2020 2020 2020  ("cy")..        
+00007ad0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00007ae0: 6170 7065 6e64 2822 7868 2229 0d0a 2020  append("xh")..  
+00007af0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00007b00: 636f 6465 732e 6170 7065 6e64 2822 7969  codes.append("yi
+00007b10: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00007b20: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00007b30: 6e64 2822 796f 2229 0d0a 2020 2020 2020  nd("yo")..      
+00007b40: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00007b50: 732e 6170 7065 6e64 2822 7a75 2229 0d0a  s.append("zu")..
+00007b60: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00007b70: 6973 745f 6e61 6d65 7320 3d20 5b5d 0d0a  ist_names = []..
+00007b80: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00007b90: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+00007ba0: 4166 7269 6b61 616e 7322 290d 0a20 2020  Afrikaans")..   
+00007bb0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00007bc0: 616d 6573 2e61 7070 656e 6428 2241 6c62  ames.append("Alb
+00007bd0: 616e 6961 6e22 290d 0a20 2020 2020 2020  anian")..       
+00007be0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00007bf0: 2e61 7070 656e 6428 2241 6d68 6172 6963  .append("Amharic
+00007c00: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00007c10: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00007c20: 6e64 2822 4172 6162 6963 2229 0d0a 2020  nd("Arabic")..  
+00007c30: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00007c40: 6e61 6d65 732e 6170 7065 6e64 2822 4172  names.append("Ar
+00007c50: 6d65 6e69 616e 2229 0d0a 2020 2020 2020  menian")..      
+00007c60: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00007c70: 732e 6170 7065 6e64 2822 4173 7361 6d65  s.append("Assame
+00007c80: 7365 2229 0d0a 2020 2020 2020 2020 7365  se")..        se
+00007c90: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00007ca0: 7065 6e64 2822 4179 6d61 7261 2229 0d0a  pend("Aymara")..
+00007cb0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00007cc0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+00007cd0: 417a 6572 6261 696a 616e 6922 290d 0a20  Azerbaijani").. 
+00007ce0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00007cf0: 5f6e 616d 6573 2e61 7070 656e 6428 2242  _names.append("B
+00007d00: 616d 6261 7261 2229 0d0a 2020 2020 2020  ambara")..      
+00007d10: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00007d20: 732e 6170 7065 6e64 2822 4261 7371 7565  s.append("Basque
+00007d30: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00007d40: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00007d50: 6e64 2822 4265 6c61 7275 7369 616e 2229  nd("Belarusian")
+00007d60: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00007d70: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00007d80: 2822 4265 6e67 616c 6922 290d 0a20 2020  ("Bengali")..   
+00007d90: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00007da0: 616d 6573 2e61 7070 656e 6428 2242 686f  ames.append("Bho
+00007db0: 6a70 7572 6922 290d 0a20 2020 2020 2020  jpuri")..       
+00007dc0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00007dd0: 2e61 7070 656e 6428 2242 6f73 6e69 616e  .append("Bosnian
+00007de0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00007df0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00007e00: 6e64 2822 4275 6c67 6172 6961 6e22 290d  nd("Bulgarian").
+00007e10: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00007e20: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00007e30: 2243 6174 616c 616e 2229 0d0a 2020 2020  "Catalan")..    
+00007e40: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00007e50: 6d65 732e 6170 7065 6e64 2822 4365 6275  mes.append("Cebu
+00007e60: 616e 6f22 290d 0a20 2020 2020 2020 2073  ano")..        s
+00007e70: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00007e80: 7070 656e 6428 2243 6869 6368 6577 6122  ppend("Chichewa"
+00007e90: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00007ea0: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00007eb0: 6428 2243 6869 6e65 7365 2028 5369 6d70  d("Chinese (Simp
+00007ec0: 6c69 6669 6564 2922 290d 0a20 2020 2020  lified)")..     
+00007ed0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00007ee0: 6573 2e61 7070 656e 6428 2243 6869 6e65  es.append("Chine
+00007ef0: 7365 2028 5472 6164 6974 696f 6e61 6c29  se (Traditional)
+00007f00: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00007f10: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00007f20: 6e64 2822 436f 7273 6963 616e 2229 0d0a  nd("Corsican")..
+00007f30: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00007f40: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+00007f50: 4372 6f61 7469 616e 2229 0d0a 2020 2020  Croatian")..    
+00007f60: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00007f70: 6d65 732e 6170 7065 6e64 2822 437a 6563  mes.append("Czec
+00007f80: 6822 290d 0a20 2020 2020 2020 2073 656c  h")..        sel
+00007f90: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00007fa0: 656e 6428 2244 616e 6973 6822 290d 0a20  end("Danish").. 
+00007fb0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00007fc0: 5f6e 616d 6573 2e61 7070 656e 6428 2244  _names.append("D
+00007fd0: 6869 7665 6869 2229 0d0a 2020 2020 2020  hivehi")..      
+00007fe0: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00007ff0: 732e 6170 7065 6e64 2822 446f 6772 6922  s.append("Dogri"
+00008000: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00008010: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00008020: 6428 2244 7574 6368 2229 0d0a 2020 2020  d("Dutch")..    
+00008030: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00008040: 6d65 732e 6170 7065 6e64 2822 456e 676c  mes.append("Engl
+00008050: 6973 6822 290d 0a20 2020 2020 2020 2073  ish")..        s
+00008060: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00008070: 7070 656e 6428 2245 7370 6572 616e 746f  ppend("Esperanto
+00008080: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00008090: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+000080a0: 6e64 2822 4573 746f 6e69 616e 2229 0d0a  nd("Estonian")..
+000080b0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+000080c0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+000080d0: 4577 6522 290d 0a20 2020 2020 2020 2073  Ewe")..        s
+000080e0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+000080f0: 7070 656e 6428 2246 696c 6970 696e 6f22  ppend("Filipino"
+00008100: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00008110: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00008120: 6428 2246 696e 6e69 7368 2229 0d0a 2020  d("Finnish")..  
+00008130: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00008140: 6e61 6d65 732e 6170 7065 6e64 2822 4672  names.append("Fr
+00008150: 656e 6368 2229 0d0a 2020 2020 2020 2020  ench")..        
+00008160: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00008170: 6170 7065 6e64 2822 4672 6973 6961 6e22  append("Frisian"
+00008180: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00008190: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+000081a0: 6428 2247 616c 6963 6961 6e22 290d 0a20  d("Galician").. 
+000081b0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+000081c0: 5f6e 616d 6573 2e61 7070 656e 6428 2247  _names.append("G
+000081d0: 656f 7267 6961 6e22 290d 0a20 2020 2020  eorgian")..     
+000081e0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+000081f0: 6573 2e61 7070 656e 6428 2247 6572 6d61  es.append("Germa
+00008200: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
+00008210: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00008220: 656e 6428 2247 7265 656b 2229 0d0a 2020  end("Greek")..  
+00008230: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00008240: 6e61 6d65 732e 6170 7065 6e64 2822 4775  names.append("Gu
+00008250: 6172 616e 6922 290d 0a20 2020 2020 2020  arani")..       
+00008260: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00008270: 2e61 7070 656e 6428 2247 756a 6172 6174  .append("Gujarat
+00008280: 6922 290d 0a20 2020 2020 2020 2073 656c  i")..        sel
+00008290: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+000082a0: 656e 6428 2248 6169 7469 616e 2043 7265  end("Haitian Cre
+000082b0: 6f6c 6522 290d 0a20 2020 2020 2020 2073  ole")..        s
+000082c0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+000082d0: 7070 656e 6428 2248 6175 7361 2229 0d0a  ppend("Hausa")..
+000082e0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+000082f0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+00008300: 4861 7761 6969 616e 2229 0d0a 2020 2020  Hawaiian")..    
+00008310: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00008320: 6d65 732e 6170 7065 6e64 2822 4865 6272  mes.append("Hebr
+00008330: 6577 2229 0d0a 2020 2020 2020 2020 7365  ew")..        se
+00008340: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00008350: 7065 6e64 2822 4869 6e64 6922 290d 0a20  pend("Hindi").. 
+00008360: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00008370: 5f6e 616d 6573 2e61 7070 656e 6428 2248  _names.append("H
+00008380: 6d6f 6e67 2229 0d0a 2020 2020 2020 2020  mong")..        
+00008390: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+000083a0: 6170 7065 6e64 2822 4875 6e67 6172 6961  append("Hungaria
+000083b0: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
+000083c0: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+000083d0: 656e 6428 2249 6365 6c61 6e64 6963 2229  end("Icelandic")
+000083e0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+000083f0: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00008400: 2822 4967 626f 2229 0d0a 2020 2020 2020  ("Igbo")..      
+00008410: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00008420: 732e 6170 7065 6e64 2822 496c 6f63 616e  s.append("Ilocan
+00008430: 6f22 290d 0a20 2020 2020 2020 2073 656c  o")..        sel
+00008440: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00008450: 656e 6428 2249 6e64 6f6e 6573 6961 6e22  end("Indonesian"
+00008460: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00008470: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00008480: 6428 2249 7269 7368 2229 0d0a 2020 2020  d("Irish")..    
+00008490: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+000084a0: 6d65 732e 6170 7065 6e64 2822 4974 616c  mes.append("Ital
+000084b0: 6961 6e22 290d 0a20 2020 2020 2020 2073  ian")..        s
+000084c0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+000084d0: 7070 656e 6428 224a 6170 616e 6573 6522  ppend("Japanese"
+000084e0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000084f0: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00008500: 6428 224a 6176 616e 6573 6522 290d 0a20  d("Javanese").. 
+00008510: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00008520: 5f6e 616d 6573 2e61 7070 656e 6428 224b  _names.append("K
+00008530: 616e 6e61 6461 2229 0d0a 2020 2020 2020  annada")..      
+00008540: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00008550: 732e 6170 7065 6e64 2822 4b61 7a61 6b68  s.append("Kazakh
+00008560: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00008570: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00008580: 6e64 2822 4b68 6d65 7222 290d 0a20 2020  nd("Khmer")..   
+00008590: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+000085a0: 616d 6573 2e61 7070 656e 6428 224b 696e  ames.append("Kin
+000085b0: 7961 7277 616e 6461 2229 0d0a 2020 2020  yarwanda")..    
+000085c0: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+000085d0: 6d65 732e 6170 7065 6e64 2822 4b6f 6e6b  mes.append("Konk
+000085e0: 616e 6922 290d 0a20 2020 2020 2020 2073  ani")..        s
+000085f0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00008600: 7070 656e 6428 224b 6f72 6561 6e22 290d  ppend("Korean").
+00008610: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00008620: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00008630: 224b 7269 6f22 290d 0a20 2020 2020 2020  "Krio")..       
+00008640: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00008650: 2e61 7070 656e 6428 224b 7572 6469 7368  .append("Kurdish
+00008660: 2028 4b75 726d 616e 6a69 2922 290d 0a20   (Kurmanji)").. 
+00008670: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00008680: 5f6e 616d 6573 2e61 7070 656e 6428 224b  _names.append("K
+00008690: 7572 6469 7368 2028 536f 7261 6e69 2922  urdish (Sorani)"
+000086a0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000086b0: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+000086c0: 6428 224b 7972 6779 7a22 290d 0a20 2020  d("Kyrgyz")..   
+000086d0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+000086e0: 616d 6573 2e61 7070 656e 6428 224c 616f  ames.append("Lao
+000086f0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00008700: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00008710: 6e64 2822 4c61 7469 6e22 290d 0a20 2020  nd("Latin")..   
+00008720: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00008730: 616d 6573 2e61 7070 656e 6428 224c 6174  ames.append("Lat
+00008740: 7669 616e 2229 0d0a 2020 2020 2020 2020  vian")..        
+00008750: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00008760: 6170 7065 6e64 2822 4c69 6e67 616c 6122  append("Lingala"
+00008770: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00008780: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00008790: 6428 224c 6974 6875 616e 6961 6e22 290d  d("Lithuanian").
+000087a0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+000087b0: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+000087c0: 224c 7567 616e 6461 2229 0d0a 2020 2020  "Luganda")..    
+000087d0: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+000087e0: 6d65 732e 6170 7065 6e64 2822 4c75 7865  mes.append("Luxe
+000087f0: 6d62 6f75 7267 6973 6822 290d 0a20 2020  mbourgish")..   
+00008800: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00008810: 616d 6573 2e61 7070 656e 6428 224d 6163  ames.append("Mac
+00008820: 6564 6f6e 6961 6e22 290d 0a20 2020 2020  edonian")..     
+00008830: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00008840: 6573 2e61 7070 656e 6428 224d 616c 6167  es.append("Malag
+00008850: 6173 7922 290d 0a20 2020 2020 2020 2073  asy")..        s
+00008860: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00008870: 7070 656e 6428 224d 616c 6179 2229 0d0a  ppend("Malay")..
+00008880: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00008890: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+000088a0: 4d61 6c61 7961 6c61 6d22 290d 0a20 2020  Malayalam")..   
+000088b0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+000088c0: 616d 6573 2e61 7070 656e 6428 224d 616c  ames.append("Mal
+000088d0: 7465 7365 2229 0d0a 2020 2020 2020 2020  tese")..        
+000088e0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+000088f0: 6170 7065 6e64 2822 4d61 6f72 6922 290d  append("Maori").
+00008900: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00008910: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00008920: 224d 6172 6174 6869 2229 0d0a 2020 2020  "Marathi")..    
+00008930: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00008940: 6d65 732e 6170 7065 6e64 2822 4d65 6974  mes.append("Meit
+00008950: 6569 6c6f 6e20 284d 616e 6970 7572 6929  eilon (Manipuri)
+00008960: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00008970: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00008980: 6e64 2822 4d69 7a6f 2229 0d0a 2020 2020  nd("Mizo")..    
+00008990: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+000089a0: 6d65 732e 6170 7065 6e64 2822 4d6f 6e67  mes.append("Mong
+000089b0: 6f6c 6961 6e22 290d 0a20 2020 2020 2020  olian")..       
+000089c0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+000089d0: 2e61 7070 656e 6428 224d 7961 6e6d 6172  .append("Myanmar
+000089e0: 2028 4275 726d 6573 6529 2229 0d0a 2020   (Burmese)")..  
+000089f0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00008a00: 6e61 6d65 732e 6170 7065 6e64 2822 4e65  names.append("Ne
+00008a10: 7061 6c69 2229 0d0a 2020 2020 2020 2020  pali")..        
+00008a20: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00008a30: 6170 7065 6e64 2822 4e6f 7277 6567 6961  append("Norwegia
+00008a40: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
+00008a50: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00008a60: 656e 6428 224f 6469 7961 2028 4f72 6979  end("Odiya (Oriy
+00008a70: 6129 2229 0d0a 2020 2020 2020 2020 7365  a)")..        se
+00008a80: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00008a90: 7065 6e64 2822 4f72 6f6d 6f22 290d 0a20  pend("Oromo").. 
+00008aa0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00008ab0: 5f6e 616d 6573 2e61 7070 656e 6428 2250  _names.append("P
+00008ac0: 6173 6874 6f22 290d 0a20 2020 2020 2020  ashto")..       
+00008ad0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00008ae0: 2e61 7070 656e 6428 2250 6572 7369 616e  .append("Persian
+00008af0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00008b00: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00008b10: 6e64 2822 506f 6c69 7368 2229 0d0a 2020  nd("Polish")..  
+00008b20: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00008b30: 6e61 6d65 732e 6170 7065 6e64 2822 506f  names.append("Po
+00008b40: 7274 7567 7565 7365 2229 0d0a 2020 2020  rtuguese")..    
+00008b50: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00008b60: 6d65 732e 6170 7065 6e64 2822 5075 6e6a  mes.append("Punj
+00008b70: 6162 6922 290d 0a20 2020 2020 2020 2073  abi")..        s
+00008b80: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00008b90: 7070 656e 6428 2251 7565 6368 7561 2229  ppend("Quechua")
+00008ba0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00008bb0: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00008bc0: 2822 526f 6d61 6e69 616e 2229 0d0a 2020  ("Romanian")..  
+00008bd0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00008be0: 6e61 6d65 732e 6170 7065 6e64 2822 5275  names.append("Ru
+00008bf0: 7373 6961 6e22 290d 0a20 2020 2020 2020  ssian")..       
+00008c00: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00008c10: 2e61 7070 656e 6428 2253 616d 6f61 6e22  .append("Samoan"
+00008c20: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00008c30: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00008c40: 6428 2253 616e 736b 7269 7422 290d 0a20  d("Sanskrit").. 
+00008c50: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00008c60: 5f6e 616d 6573 2e61 7070 656e 6428 2253  _names.append("S
+00008c70: 636f 7473 2047 6165 6c69 6322 290d 0a20  cots Gaelic").. 
+00008c80: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00008c90: 5f6e 616d 6573 2e61 7070 656e 6428 2253  _names.append("S
+00008ca0: 6570 6564 6922 290d 0a20 2020 2020 2020  epedi")..       
+00008cb0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00008cc0: 2e61 7070 656e 6428 2253 6572 6269 616e  .append("Serbian
+00008cd0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00008ce0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00008cf0: 6e64 2822 5365 736f 7468 6f22 290d 0a20  nd("Sesotho").. 
+00008d00: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00008d10: 5f6e 616d 6573 2e61 7070 656e 6428 2253  _names.append("S
+00008d20: 686f 6e61 2229 0d0a 2020 2020 2020 2020  hona")..        
+00008d30: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00008d40: 6170 7065 6e64 2822 5369 6e64 6869 2229  append("Sindhi")
+00008d50: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00008d60: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00008d70: 2822 5369 6e68 616c 6122 290d 0a20 2020  ("Sinhala")..   
+00008d80: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00008d90: 616d 6573 2e61 7070 656e 6428 2253 6c6f  ames.append("Slo
+00008da0: 7661 6b22 290d 0a20 2020 2020 2020 2073  vak")..        s
+00008db0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00008dc0: 7070 656e 6428 2253 6c6f 7665 6e69 616e  ppend("Slovenian
+00008dd0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00008de0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00008df0: 6e64 2822 536f 6d61 6c69 2229 0d0a 2020  nd("Somali")..  
+00008e00: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00008e10: 6e61 6d65 732e 6170 7065 6e64 2822 5370  names.append("Sp
+00008e20: 616e 6973 6822 290d 0a20 2020 2020 2020  anish")..       
+00008e30: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00008e40: 2e61 7070 656e 6428 2253 756e 6461 6e65  .append("Sundane
+00008e50: 7365 2229 0d0a 2020 2020 2020 2020 7365  se")..        se
+00008e60: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00008e70: 7065 6e64 2822 5377 6168 696c 6922 290d  pend("Swahili").
+00008e80: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00008e90: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00008ea0: 2253 7765 6469 7368 2229 0d0a 2020 2020  "Swedish")..    
+00008eb0: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00008ec0: 6d65 732e 6170 7065 6e64 2822 5461 6a69  mes.append("Taji
+00008ed0: 6b22 290d 0a20 2020 2020 2020 2073 656c  k")..        sel
+00008ee0: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00008ef0: 656e 6428 2254 616d 696c 2229 0d0a 2020  end("Tamil")..  
+00008f00: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00008f10: 6e61 6d65 732e 6170 7065 6e64 2822 5461  names.append("Ta
+00008f20: 7461 7222 290d 0a20 2020 2020 2020 2073  tar")..        s
+00008f30: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00008f40: 7070 656e 6428 2254 656c 7567 7522 290d  ppend("Telugu").
+00008f50: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00008f60: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00008f70: 2254 6861 6922 290d 0a20 2020 2020 2020  "Thai")..       
+00008f80: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00008f90: 2e61 7070 656e 6428 2254 6967 7269 6e79  .append("Tigriny
+00008fa0: 6122 290d 0a20 2020 2020 2020 2073 656c  a")..        sel
+00008fb0: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00008fc0: 656e 6428 2254 736f 6e67 6122 290d 0a20  end("Tsonga").. 
+00008fd0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00008fe0: 5f6e 616d 6573 2e61 7070 656e 6428 2254  _names.append("T
+00008ff0: 7572 6b69 7368 2229 0d0a 2020 2020 2020  urkish")..      
+00009000: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00009010: 732e 6170 7065 6e64 2822 5475 726b 6d65  s.append("Turkme
+00009020: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
+00009030: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00009040: 656e 6428 2254 7769 2028 416b 616e 2922  end("Twi (Akan)"
+00009050: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00009060: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00009070: 6428 2255 6b72 6169 6e69 616e 2229 0d0a  d("Ukrainian")..
+00009080: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00009090: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+000090a0: 5572 6475 2229 0d0a 2020 2020 2020 2020  Urdu")..        
+000090b0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+000090c0: 6170 7065 6e64 2822 5579 6768 7572 2229  append("Uyghur")
+000090d0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+000090e0: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+000090f0: 2822 557a 6265 6b22 290d 0a20 2020 2020  ("Uzbek")..     
+00009100: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00009110: 6573 2e61 7070 656e 6428 2256 6965 746e  es.append("Vietn
+00009120: 616d 6573 6522 290d 0a20 2020 2020 2020  amese")..       
+00009130: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00009140: 2e61 7070 656e 6428 2257 656c 7368 2229  .append("Welsh")
+00009150: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00009160: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00009170: 2822 5868 6f73 6122 290d 0a20 2020 2020  ("Xhosa")..     
+00009180: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00009190: 6573 2e61 7070 656e 6428 2259 6964 6469  es.append("Yiddi
+000091a0: 7368 2229 0d0a 2020 2020 2020 2020 7365  sh")..        se
+000091b0: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+000091c0: 7065 6e64 2822 596f 7275 6261 2229 0d0a  pend("Yoruba")..
+000091d0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+000091e0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+000091f0: 5a75 6c75 2229 0d0a 0d0a 2020 2020 2020  Zulu")....      
+00009200: 2020 7365 6c66 2e63 6f64 655f 6f66 5f6e    self.code_of_n
+00009210: 616d 6520 3d20 6469 6374 287a 6970 2873  ame = dict(zip(s
+00009220: 656c 662e 6c69 7374 5f6e 616d 6573 2c20  elf.list_names, 
+00009230: 7365 6c66 2e6c 6973 745f 636f 6465 7329  self.list_codes)
+00009240: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00009250: 6e61 6d65 5f6f 665f 636f 6465 203d 2064  name_of_code = d
+00009260: 6963 7428 7a69 7028 7365 6c66 2e6c 6973  ict(zip(self.lis
+00009270: 745f 636f 6465 732c 2073 656c 662e 6c69  t_codes, self.li
+00009280: 7374 5f6e 616d 6573 2929 0d0a 0d0a 2020  st_names))....  
+00009290: 2020 2020 2020 7365 6c66 2e64 6963 7420        self.dict 
+000092a0: 3d20 7b0d 0a20 2020 2020 2020 2020 2020  = {..           
+000092b0: 2020 2020 2020 2020 2020 2020 2027 6166               'af
+000092c0: 273a 2027 4166 7269 6b61 616e 7327 2c0d  ': 'Afrikaans',.
+000092d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000092e0: 2020 2020 2020 2020 2027 7371 273a 2027           'sq': '
+000092f0: 416c 6261 6e69 616e 272c 0d0a 2020 2020  Albanian',..    
+00009300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009310: 2020 2020 2761 6d27 3a20 2741 6d68 6172      'am': 'Amhar
+00009320: 6963 272c 0d0a 2020 2020 2020 2020 2020  ic',..          
+00009330: 2020 2020 2020 2020 2020 2020 2020 2761                'a
+00009340: 7227 3a20 2741 7261 6269 6327 2c0d 0a20  r': 'Arabic',.. 
+00009350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009360: 2020 2020 2020 2027 6879 273a 2027 4172         'hy': 'Ar
+00009370: 6d65 6e69 616e 272c 0d0a 2020 2020 2020  menian',..      
+00009380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009390: 2020 2761 7327 3a20 2741 7373 616d 6573    'as': 'Assames
+000093a0: 6527 2c0d 0a20 2020 2020 2020 2020 2020  e',..           
+000093b0: 2020 2020 2020 2020 2020 2020 2027 6179               'ay
+000093c0: 273a 2027 4179 6d61 7261 272c 0d0a 2020  ': 'Aymara',..  
+000093d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000093e0: 2020 2020 2020 2761 7a27 3a20 2741 7a65        'az': 'Aze
+000093f0: 7262 6169 6a61 6e69 272c 0d0a 2020 2020  rbaijani',..    
+00009400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009410: 2020 2020 2762 6d27 3a20 2742 616d 6261      'bm': 'Bamba
+00009420: 7261 272c 0d0a 2020 2020 2020 2020 2020  ra',..          
+00009430: 2020 2020 2020 2020 2020 2020 2020 2765                'e
+00009440: 7527 3a20 2742 6173 7175 6527 2c0d 0a20  u': 'Basque',.. 
+00009450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009460: 2020 2020 2020 2027 6265 273a 2027 4265         'be': 'Be
+00009470: 6c61 7275 7369 616e 272c 0d0a 2020 2020  larusian',..    
+00009480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009490: 2020 2020 2762 6e27 3a20 2742 656e 6761      'bn': 'Benga
+000094a0: 6c69 272c 0d0a 2020 2020 2020 2020 2020  li',..          
+000094b0: 2020 2020 2020 2020 2020 2020 2020 2762                'b
+000094c0: 686f 273a 2027 4268 6f6a 7075 7269 272c  ho': 'Bhojpuri',
+000094d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000094e0: 2020 2020 2020 2020 2020 2762 7327 3a20            'bs': 
+000094f0: 2742 6f73 6e69 616e 272c 0d0a 2020 2020  'Bosnian',..    
+00009500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009510: 2020 2020 2762 6727 3a20 2742 756c 6761      'bg': 'Bulga
+00009520: 7269 616e 272c 0d0a 2020 2020 2020 2020  rian',..        
+00009530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009540: 2763 6127 3a20 2743 6174 616c 616e 272c  'ca': 'Catalan',
+00009550: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009560: 2020 2020 2020 2020 2020 2763 6562 273a            'ceb':
+00009570: 2027 4365 6275 616e 6f27 2c0d 0a20 2020   'Cebuano',..   
+00009580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009590: 2020 2020 2027 6e79 273a 2027 4368 6963       'ny': 'Chic
+000095a0: 6865 7761 272c 0d0a 2020 2020 2020 2020  hewa',..        
+000095b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095c0: 277a 682d 434e 273a 2027 4368 696e 6573  'zh-CN': 'Chines
+000095d0: 6520 2853 696d 706c 6966 6965 6429 272c  e (Simplified)',
+000095e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000095f0: 2020 2020 2020 2020 2020 277a 682d 5457            'zh-TW
+00009600: 273a 2027 4368 696e 6573 6520 2854 7261  ': 'Chinese (Tra
+00009610: 6469 7469 6f6e 616c 2927 2c0d 0a20 2020  ditional)',..   
+00009620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009630: 2020 2020 2027 636f 273a 2027 436f 7273       'co': 'Cors
+00009640: 6963 616e 272c 0d0a 2020 2020 2020 2020  ican',..        
+00009650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009660: 2768 7227 3a20 2743 726f 6174 6961 6e27  'hr': 'Croatian'
+00009670: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00009680: 2020 2020 2020 2020 2020 2027 6373 273a             'cs':
+00009690: 2027 437a 6563 6827 2c0d 0a20 2020 2020   'Czech',..     
+000096a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096b0: 2020 2027 6461 273a 2027 4461 6e69 7368     'da': 'Danish
+000096c0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+000096d0: 2020 2020 2020 2020 2020 2020 2764 7627              'dv'
+000096e0: 3a20 2744 6869 7665 6869 272c 0d0a 2020  : 'Dhivehi',..  
+000096f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009700: 2020 2020 2020 2764 6f69 273a 2027 446f        'doi': 'Do
+00009710: 6772 6927 2c0d 0a20 2020 2020 2020 2020  gri',..         
+00009720: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00009730: 6e6c 273a 2027 4475 7463 6827 2c0d 0a20  nl': 'Dutch',.. 
+00009740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009750: 2020 2020 2020 2027 656e 273a 2027 456e         'en': 'En
+00009760: 676c 6973 6827 2c0d 0a20 2020 2020 2020  glish',..       
+00009770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009780: 2027 656f 273a 2027 4573 7065 7261 6e74   'eo': 'Esperant
+00009790: 6f27 2c0d 0a20 2020 2020 2020 2020 2020  o',..           
+000097a0: 2020 2020 2020 2020 2020 2020 2027 6574               'et
+000097b0: 273a 2027 4573 746f 6e69 616e 272c 0d0a  ': 'Estonian',..
+000097c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097d0: 2020 2020 2020 2020 2765 6527 3a20 2745          'ee': 'E
+000097e0: 7765 272c 0d0a 2020 2020 2020 2020 2020  we',..          
+000097f0: 2020 2020 2020 2020 2020 2020 2020 2766                'f
+00009800: 696c 273a 2027 4669 6c69 7069 6e6f 272c  il': 'Filipino',
+00009810: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009820: 2020 2020 2020 2020 2020 2766 6927 3a20            'fi': 
+00009830: 2746 696e 6e69 7368 272c 0d0a 2020 2020  'Finnish',..    
+00009840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009850: 2020 2020 2766 7227 3a20 2746 7265 6e63      'fr': 'Frenc
+00009860: 6827 2c0d 0a20 2020 2020 2020 2020 2020  h',..           
+00009870: 2020 2020 2020 2020 2020 2020 2027 6679               'fy
+00009880: 273a 2027 4672 6973 6961 6e27 2c0d 0a20  ': 'Frisian',.. 
+00009890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098a0: 2020 2020 2020 2027 676c 273a 2027 4761         'gl': 'Ga
+000098b0: 6c69 6369 616e 272c 0d0a 2020 2020 2020  lician',..      
+000098c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098d0: 2020 276b 6127 3a20 2747 656f 7267 6961    'ka': 'Georgia
+000098e0: 6e27 2c0d 0a20 2020 2020 2020 2020 2020  n',..           
+000098f0: 2020 2020 2020 2020 2020 2020 2027 6465               'de
+00009900: 273a 2027 4765 726d 616e 272c 0d0a 2020  ': 'German',..  
+00009910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009920: 2020 2020 2020 2765 6c27 3a20 2747 7265        'el': 'Gre
+00009930: 656b 272c 0d0a 2020 2020 2020 2020 2020  ek',..          
+00009940: 2020 2020 2020 2020 2020 2020 2020 2767                'g
+00009950: 6e27 3a20 2747 7561 7261 6e69 272c 0d0a  n': 'Guarani',..
+00009960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009970: 2020 2020 2020 2020 2767 7527 3a20 2747          'gu': 'G
+00009980: 756a 6172 6174 6927 2c0d 0a20 2020 2020  ujarati',..     
+00009990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099a0: 2020 2027 6874 273a 2027 4861 6974 6961     'ht': 'Haitia
+000099b0: 6e20 4372 656f 6c65 272c 0d0a 2020 2020  n Creole',..    
+000099c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099d0: 2020 2020 2768 6127 3a20 2748 6175 7361      'ha': 'Hausa
+000099e0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+000099f0: 2020 2020 2020 2020 2020 2020 2768 6177              'haw
+00009a00: 273a 2027 4861 7761 6969 616e 272c 0d0a  ': 'Hawaiian',..
+00009a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a20: 2020 2020 2020 2020 2768 6527 3a20 2748          'he': 'H
+00009a30: 6562 7265 7727 2c0d 0a20 2020 2020 2020  ebrew',..       
+00009a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a50: 2027 6869 273a 2027 4869 6e64 6927 2c0d   'hi': 'Hindi',.
+00009a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009a70: 2020 2020 2020 2020 2027 686d 6e27 3a20           'hmn': 
+00009a80: 2748 6d6f 6e67 272c 0d0a 2020 2020 2020  'Hmong',..      
+00009a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009aa0: 2020 2768 7527 3a20 2748 756e 6761 7269    'hu': 'Hungari
+00009ab0: 616e 272c 0d0a 2020 2020 2020 2020 2020  an',..          
+00009ac0: 2020 2020 2020 2020 2020 2020 2020 2769                'i
+00009ad0: 7327 3a20 2749 6365 6c61 6e64 6963 272c  s': 'Icelandic',
+00009ae0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009af0: 2020 2020 2020 2020 2020 2769 6727 3a20            'ig': 
+00009b00: 2749 6762 6f27 2c0d 0a20 2020 2020 2020  'Igbo',..       
+00009b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b20: 2027 696c 6f27 3a20 2749 6c6f 6361 6e6f   'ilo': 'Ilocano
+00009b30: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00009b40: 2020 2020 2020 2020 2020 2020 2769 6427              'id'
+00009b50: 3a20 2749 6e64 6f6e 6573 6961 6e27 2c0d  : 'Indonesian',.
+00009b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009b70: 2020 2020 2020 2020 2027 6761 273a 2027           'ga': '
+00009b80: 4972 6973 6827 2c0d 0a20 2020 2020 2020  Irish',..       
+00009b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ba0: 2027 6974 273a 2027 4974 616c 6961 6e27   'it': 'Italian'
+00009bb0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00009bc0: 2020 2020 2020 2020 2020 2027 6a61 273a             'ja':
+00009bd0: 2027 4a61 7061 6e65 7365 272c 0d0a 2020   'Japanese',..  
+00009be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009bf0: 2020 2020 2020 276a 7627 3a20 274a 6176        'jv': 'Jav
+00009c00: 616e 6573 6527 2c0d 0a20 2020 2020 2020  anese',..       
+00009c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c20: 2027 6b6e 273a 2027 4b61 6e6e 6164 6127   'kn': 'Kannada'
+00009c30: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00009c40: 2020 2020 2020 2020 2020 2027 6b6b 273a             'kk':
+00009c50: 2027 4b61 7a61 6b68 272c 0d0a 2020 2020   'Kazakh',..    
+00009c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c70: 2020 2020 276b 6d27 3a20 274b 686d 6572      'km': 'Khmer
+00009c80: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00009c90: 2020 2020 2020 2020 2020 2020 2772 7727              'rw'
+00009ca0: 3a20 274b 696e 7961 7277 616e 6461 272c  : 'Kinyarwanda',
+00009cb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009cc0: 2020 2020 2020 2020 2020 2767 6f6d 273a            'gom':
+00009cd0: 2027 4b6f 6e6b 616e 6927 2c0d 0a20 2020   'Konkani',..   
+00009ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009cf0: 2020 2020 2027 6b6f 273a 2027 4b6f 7265       'ko': 'Kore
+00009d00: 616e 272c 0d0a 2020 2020 2020 2020 2020  an',..          
+00009d10: 2020 2020 2020 2020 2020 2020 2020 276b                'k
+00009d20: 7269 273a 2027 4b72 696f 272c 0d0a 2020  ri': 'Krio',..  
+00009d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d40: 2020 2020 2020 276b 6d72 273a 2027 4b75        'kmr': 'Ku
+00009d50: 7264 6973 6820 284b 7572 6d61 6e6a 6929  rdish (Kurmanji)
+00009d60: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00009d70: 2020 2020 2020 2020 2020 2020 2763 6b62              'ckb
+00009d80: 273a 2027 4b75 7264 6973 6820 2853 6f72  ': 'Kurdish (Sor
+00009d90: 616e 6929 272c 0d0a 2020 2020 2020 2020  ani)',..        
+00009da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009db0: 276b 7927 3a20 274b 7972 6779 7a27 2c0d  'ky': 'Kyrgyz',.
+00009dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009dd0: 2020 2020 2020 2020 2027 6c6f 273a 2027           'lo': '
+00009de0: 4c61 6f27 2c0d 0a20 2020 2020 2020 2020  Lao',..         
+00009df0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00009e00: 6c61 273a 2027 4c61 7469 6e27 2c0d 0a20  la': 'Latin',.. 
+00009e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e20: 2020 2020 2020 2027 6c76 273a 2027 4c61         'lv': 'La
+00009e30: 7476 6961 6e27 2c0d 0a20 2020 2020 2020  tvian',..       
+00009e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e50: 2027 6c6e 273a 2027 4c69 6e67 616c 6127   'ln': 'Lingala'
+00009e60: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00009e70: 2020 2020 2020 2020 2020 2027 6c74 273a             'lt':
+00009e80: 2027 4c69 7468 7561 6e69 616e 272c 0d0a   'Lithuanian',..
+00009e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ea0: 2020 2020 2020 2020 276c 6727 3a20 274c          'lg': 'L
+00009eb0: 7567 616e 6461 272c 0d0a 2020 2020 2020  uganda',..      
+00009ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ed0: 2020 276c 6227 3a20 274c 7578 656d 626f    'lb': 'Luxembo
+00009ee0: 7572 6769 7368 272c 0d0a 2020 2020 2020  urgish',..      
+00009ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f00: 2020 276d 6b27 3a20 274d 6163 6564 6f6e    'mk': 'Macedon
+00009f10: 6961 6e27 2c0d 0a20 2020 2020 2020 2020  ian',..         
+00009f20: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00009f30: 6d67 273a 2027 4d61 6c61 6761 7379 272c  mg': 'Malagasy',
+00009f40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009f50: 2020 2020 2020 2020 2020 276d 7327 3a20            'ms': 
+00009f60: 274d 616c 6179 272c 0d0a 2020 2020 2020  'Malay',..      
+00009f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f80: 2020 276d 6c27 3a20 274d 616c 6179 616c    'ml': 'Malayal
+00009f90: 616d 272c 0d0a 2020 2020 2020 2020 2020  am',..          
+00009fa0: 2020 2020 2020 2020 2020 2020 2020 276d                'm
+00009fb0: 7427 3a20 274d 616c 7465 7365 272c 0d0a  t': 'Maltese',..
+00009fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009fd0: 2020 2020 2020 2020 276d 6927 3a20 274d          'mi': 'M
+00009fe0: 616f 7269 272c 0d0a 2020 2020 2020 2020  aori',..        
+00009ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a000: 276d 7227 3a20 274d 6172 6174 6869 272c  'mr': 'Marathi',
+0000a010: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a020: 2020 2020 2020 2020 2020 276d 6e69 2d4d            'mni-M
+0000a030: 7465 6927 3a20 274d 6569 7465 696c 6f6e  tei': 'Meiteilon
+0000a040: 2028 4d61 6e69 7075 7269 2927 2c0d 0a20   (Manipuri)',.. 
+0000a050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a060: 2020 2020 2020 2027 6c75 7327 3a20 274d         'lus': 'M
+0000a070: 697a 6f27 2c0d 0a20 2020 2020 2020 2020  izo',..         
+0000a080: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0000a090: 6d6e 273a 2027 4d6f 6e67 6f6c 6961 6e27  mn': 'Mongolian'
+0000a0a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000a0b0: 2020 2020 2020 2020 2020 2027 6d79 273a             'my':
+0000a0c0: 2027 4d79 616e 6d61 7220 2842 7572 6d65   'Myanmar (Burme
+0000a0d0: 7365 2927 2c0d 0a20 2020 2020 2020 2020  se)',..         
+0000a0e0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0000a0f0: 6e65 273a 2027 4e65 7061 6c69 272c 0d0a  ne': 'Nepali',..
+0000a100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a110: 2020 2020 2020 2020 276e 6f27 3a20 274e          'no': 'N
+0000a120: 6f72 7765 6769 616e 272c 0d0a 2020 2020  orwegian',..    
+0000a130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a140: 2020 2020 276f 7227 3a20 274f 6469 7961      'or': 'Odiya
+0000a150: 2028 4f72 6979 6129 272c 0d0a 2020 2020   (Oriya)',..    
+0000a160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a170: 2020 2020 276f 6d27 3a20 274f 726f 6d6f      'om': 'Oromo
+0000a180: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+0000a190: 2020 2020 2020 2020 2020 2020 2770 7327              'ps'
+0000a1a0: 3a20 2750 6173 6874 6f27 2c0d 0a20 2020  : 'Pashto',..   
+0000a1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a1c0: 2020 2020 2027 6661 273a 2027 5065 7273       'fa': 'Pers
+0000a1d0: 6961 6e27 2c0d 0a20 2020 2020 2020 2020  ian',..         
+0000a1e0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0000a1f0: 706c 273a 2027 506f 6c69 7368 272c 0d0a  pl': 'Polish',..
+0000a200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a210: 2020 2020 2020 2020 2770 7427 3a20 2750          'pt': 'P
+0000a220: 6f72 7475 6775 6573 6527 2c0d 0a20 2020  ortuguese',..   
+0000a230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a240: 2020 2020 2027 7061 273a 2027 5075 6e6a       'pa': 'Punj
+0000a250: 6162 6927 2c0d 0a20 2020 2020 2020 2020  abi',..         
+0000a260: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0000a270: 7175 273a 2027 5175 6563 6875 6127 2c0d  qu': 'Quechua',.
+0000a280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a290: 2020 2020 2020 2020 2027 726f 273a 2027           'ro': '
+0000a2a0: 526f 6d61 6e69 616e 272c 0d0a 2020 2020  Romanian',..    
+0000a2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2c0: 2020 2020 2772 7527 3a20 2752 7573 7369      'ru': 'Russi
+0000a2d0: 616e 272c 0d0a 2020 2020 2020 2020 2020  an',..          
+0000a2e0: 2020 2020 2020 2020 2020 2020 2020 2773                's
+0000a2f0: 6d27 3a20 2753 616d 6f61 6e27 2c0d 0a20  m': 'Samoan',.. 
+0000a300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a310: 2020 2020 2020 2027 7361 273a 2027 5361         'sa': 'Sa
+0000a320: 6e73 6b72 6974 272c 0d0a 2020 2020 2020  nskrit',..      
+0000a330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a340: 2020 2767 6427 3a20 2753 636f 7473 2047    'gd': 'Scots G
+0000a350: 6165 6c69 6327 2c0d 0a20 2020 2020 2020  aelic',..       
+0000a360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a370: 2027 6e73 6f27 3a20 2753 6570 6564 6927   'nso': 'Sepedi'
+0000a380: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000a390: 2020 2020 2020 2020 2020 2027 7372 273a             'sr':
+0000a3a0: 2027 5365 7262 6961 6e27 2c0d 0a20 2020   'Serbian',..   
+0000a3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3c0: 2020 2020 2027 7374 273a 2027 5365 736f       'st': 'Seso
+0000a3d0: 7468 6f27 2c0d 0a20 2020 2020 2020 2020  tho',..         
+0000a3e0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0000a3f0: 736e 273a 2027 5368 6f6e 6127 2c0d 0a20  sn': 'Shona',.. 
+0000a400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a410: 2020 2020 2020 2027 7364 273a 2027 5369         'sd': 'Si
+0000a420: 6e64 6869 272c 0d0a 2020 2020 2020 2020  ndhi',..        
+0000a430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a440: 2773 6927 3a20 2753 696e 6861 6c61 272c  'si': 'Sinhala',
+0000a450: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a460: 2020 2020 2020 2020 2020 2773 6b27 3a20            'sk': 
+0000a470: 2753 6c6f 7661 6b27 2c0d 0a20 2020 2020  'Slovak',..     
+0000a480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a490: 2020 2027 736c 273a 2027 536c 6f76 656e     'sl': 'Sloven
+0000a4a0: 6961 6e27 2c0d 0a20 2020 2020 2020 2020  ian',..         
+0000a4b0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0000a4c0: 736f 273a 2027 536f 6d61 6c69 272c 0d0a  so': 'Somali',..
+0000a4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4e0: 2020 2020 2020 2020 2765 7327 3a20 2753          'es': 'S
+0000a4f0: 7061 6e69 7368 272c 0d0a 2020 2020 2020  panish',..      
+0000a500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a510: 2020 2773 7527 3a20 2753 756e 6461 6e65    'su': 'Sundane
+0000a520: 7365 272c 0d0a 2020 2020 2020 2020 2020  se',..          
+0000a530: 2020 2020 2020 2020 2020 2020 2020 2773                's
+0000a540: 7727 3a20 2753 7761 6869 6c69 272c 0d0a  w': 'Swahili',..
+0000a550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a560: 2020 2020 2020 2020 2773 7627 3a20 2753          'sv': 'S
+0000a570: 7765 6469 7368 272c 0d0a 2020 2020 2020  wedish',..      
+0000a580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a590: 2020 2774 6727 3a20 2754 616a 696b 272c    'tg': 'Tajik',
+0000a5a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a5b0: 2020 2020 2020 2020 2020 2774 6127 3a20            'ta': 
+0000a5c0: 2754 616d 696c 272c 0d0a 2020 2020 2020  'Tamil',..      
+0000a5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5e0: 2020 2774 7427 3a20 2754 6174 6172 272c    'tt': 'Tatar',
+0000a5f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a600: 2020 2020 2020 2020 2020 2774 6527 3a20            'te': 
+0000a610: 2754 656c 7567 7527 2c0d 0a20 2020 2020  'Telugu',..     
+0000a620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a630: 2020 2027 7468 273a 2027 5468 6169 272c     'th': 'Thai',
+0000a640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a650: 2020 2020 2020 2020 2020 2774 6927 3a20            'ti': 
+0000a660: 2754 6967 7269 6e79 6127 2c0d 0a20 2020  'Tigrinya',..   
+0000a670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a680: 2020 2020 2027 7473 273a 2027 5473 6f6e       'ts': 'Tson
+0000a690: 6761 272c 0d0a 2020 2020 2020 2020 2020  ga',..          
+0000a6a0: 2020 2020 2020 2020 2020 2020 2020 2774                't
+0000a6b0: 7227 3a20 2754 7572 6b69 7368 272c 0d0a  r': 'Turkish',..
+0000a6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6d0: 2020 2020 2020 2020 2774 6b27 3a20 2754          'tk': 'T
+0000a6e0: 7572 6b6d 656e 272c 0d0a 2020 2020 2020  urkmen',..      
+0000a6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a700: 2020 2774 7727 3a20 2754 7769 2028 416b    'tw': 'Twi (Ak
+0000a710: 616e 2927 2c0d 0a20 2020 2020 2020 2020  an)',..         
+0000a720: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0000a730: 756b 273a 2027 556b 7261 696e 6961 6e27  uk': 'Ukrainian'
+0000a740: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000a750: 2020 2020 2020 2020 2020 2027 7572 273a             'ur':
+0000a760: 2027 5572 6475 272c 0d0a 2020 2020 2020   'Urdu',..      
+0000a770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a780: 2020 2775 6727 3a20 2755 7967 6875 7227    'ug': 'Uyghur'
+0000a790: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000a7a0: 2020 2020 2020 2020 2020 2027 757a 273a             'uz':
+0000a7b0: 2027 557a 6265 6b27 2c0d 0a20 2020 2020   'Uzbek',..     
+0000a7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7d0: 2020 2027 7669 273a 2027 5669 6574 6e61     'vi': 'Vietna
+0000a7e0: 6d65 7365 272c 0d0a 2020 2020 2020 2020  mese',..        
+0000a7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a800: 2763 7927 3a20 2757 656c 7368 272c 0d0a  'cy': 'Welsh',..
+0000a810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a820: 2020 2020 2020 2020 2778 6827 3a20 2758          'xh': 'X
+0000a830: 686f 7361 272c 0d0a 2020 2020 2020 2020  hosa',..        
+0000a840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a850: 2779 6927 3a20 2759 6964 6469 7368 272c  'yi': 'Yiddish',
+0000a860: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a870: 2020 2020 2020 2020 2020 2779 6f27 3a20            'yo': 
+0000a880: 2759 6f72 7562 6127 2c0d 0a20 2020 2020  'Yoruba',..     
+0000a890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8a0: 2020 2027 7a75 273a 2027 5a75 6c75 272c     'zu': 'Zulu',
+0000a8b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a8c0: 2020 2020 2020 7d0d 0a0d 0a20 2020 2064        }....    d
+0000a8d0: 6566 2067 6574 5f6e 616d 6528 7365 6c66  ef get_name(self
+0000a8e0: 2c20 6765 745f 636f 6465 293a 0d0a 2020  , get_code):..  
+0000a8f0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000a900: 662e 6469 6374 2e67 6574 2867 6574 5f63  f.dict.get(get_c
+0000a910: 6f64 652e 6c6f 7765 7228 292c 2022 2229  ode.lower(), "")
+0000a920: 0d0a 0d0a 2020 2020 6465 6620 6765 745f  ....    def get_
+0000a930: 636f 6465 2873 656c 662c 206c 616e 6775  code(self, langu
+0000a940: 6167 6529 3a0d 0a20 2020 2020 2020 2066  age):..        f
+0000a950: 6f72 2067 6574 5f63 6f64 652c 206c 616e  or get_code, lan
+0000a960: 6720 696e 2073 656c 662e 6469 6374 2e69  g in self.dict.i
+0000a970: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
+0000a980: 2020 2020 2069 6620 6c61 6e67 2e6c 6f77       if lang.low
+0000a990: 6572 2829 203d 3d20 6c61 6e67 7561 6765  er() == language
+0000a9a0: 2e6c 6f77 6572 2829 3a0d 0a20 2020 2020  .lower():..     
+0000a9b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000a9c0: 6e20 6765 745f 636f 6465 0d0a 2020 2020  n get_code..    
+0000a9d0: 2020 2020 7265 7475 726e 2022 220d 0a0d      return ""...
+0000a9e0: 0a0d 0a63 6c61 7373 2057 6176 436f 6e76  ...class WavConv
+0000a9f0: 6572 7465 723a 0d0a 2020 2020 4073 7461  erter:..    @sta
+0000aa00: 7469 636d 6574 686f 640d 0a20 2020 2064  ticmethod..    d
+0000aa10: 6566 2077 6869 6368 2870 726f 6772 616d  ef which(program
+0000aa20: 293a 0d0a 2020 2020 2020 2020 6465 6620  ):..        def 
+0000aa30: 6973 5f65 7865 2866 696c 655f 7061 7468  is_exe(file_path
+0000aa40: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000aa50: 7265 7475 726e 206f 732e 7061 7468 2e69  return os.path.i
+0000aa60: 7366 696c 6528 6669 6c65 5f70 6174 6829  sfile(file_path)
+0000aa70: 2061 6e64 206f 732e 6163 6365 7373 2866   and os.access(f
+0000aa80: 696c 655f 7061 7468 2c20 6f73 2e58 5f4f  ile_path, os.X_O
+0000aa90: 4b29 0d0a 2020 2020 2020 2020 6670 6174  K)..        fpat
+0000aaa0: 682c 205f 203d 206f 732e 7061 7468 2e73  h, _ = os.path.s
+0000aab0: 706c 6974 2870 726f 6772 616d 290d 0a20  plit(program).. 
+0000aac0: 2020 2020 2020 2069 6620 6670 6174 683a         if fpath:
+0000aad0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0000aae0: 2069 735f 6578 6528 7072 6f67 7261 6d29   is_exe(program)
+0000aaf0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000ab00: 2020 2072 6574 7572 6e20 7072 6f67 7261     return progra
+0000ab10: 6d0d 0a20 2020 2020 2020 2065 6c73 653a  m..        else:
+0000ab20: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
+0000ab30: 7220 7061 7468 2069 6e20 6f73 2e65 6e76  r path in os.env
+0000ab40: 6972 6f6e 5b22 5041 5448 225d 2e73 706c  iron["PATH"].spl
+0000ab50: 6974 286f 732e 7061 7468 7365 7029 3a0d  it(os.pathsep):.
+0000ab60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ab70: 2070 6174 6820 3d20 7061 7468 2e73 7472   path = path.str
+0000ab80: 6970 2827 2227 290d 0a20 2020 2020 2020  ip('"')..       
+0000ab90: 2020 2020 2020 2020 2065 7865 5f66 696c           exe_fil
+0000aba0: 6520 3d20 6f73 2e70 6174 682e 6a6f 696e  e = os.path.join
+0000abb0: 2870 6174 682c 2070 726f 6772 616d 290d  (path, program).
+0000abc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000abd0: 2069 6620 6973 5f65 7865 2865 7865 5f66   if is_exe(exe_f
+0000abe0: 696c 6529 3a0d 0a20 2020 2020 2020 2020  ile):..         
+0000abf0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000ac00: 6e20 6578 655f 6669 6c65 0d0a 2020 2020  n exe_file..    
+0000ac10: 2020 2020 7265 7475 726e 204e 6f6e 650d      return None.
+0000ac20: 0a0d 0a20 2020 2040 7374 6174 6963 6d65  ...    @staticme
+0000ac30: 7468 6f64 0d0a 2020 2020 6465 6620 6666  thod..    def ff
+0000ac40: 6d70 6567 5f63 6865 636b 2829 3a0d 0a20  mpeg_check():.. 
+0000ac50: 2020 2020 2020 2069 6620 5761 7643 6f6e         if WavCon
+0000ac60: 7665 7274 6572 2e77 6869 6368 2822 6666  verter.which("ff
+0000ac70: 6d70 6567 2229 3a0d 0a20 2020 2020 2020  mpeg"):..       
+0000ac80: 2020 2020 2072 6574 7572 6e20 2266 666d       return "ffm
+0000ac90: 7065 6722 0d0a 2020 2020 2020 2020 6966  peg"..        if
+0000aca0: 2057 6176 436f 6e76 6572 7465 722e 7768   WavConverter.wh
+0000acb0: 6963 6828 2266 666d 7065 672e 6578 6522  ich("ffmpeg.exe"
+0000acc0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000acd0: 7265 7475 726e 2022 6666 6d70 6567 2e65  return "ffmpeg.e
+0000ace0: 7865 220d 0a20 2020 2020 2020 2072 6574  xe"..        ret
+0000acf0: 7572 6e20 4e6f 6e65 0d0a 0d0a 2020 2020  urn None....    
+0000ad00: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+0000ad10: 662c 2063 6861 6e6e 656c 733d 312c 2072  f, channels=1, r
+0000ad20: 6174 653d 3438 3030 302c 2070 726f 6772  ate=48000, progr
+0000ad30: 6573 735f 6361 6c6c 6261 636b 3d4e 6f6e  ess_callback=Non
+0000ad40: 652c 2065 7272 6f72 5f6d 6573 7361 6765  e, error_message
+0000ad50: 735f 6361 6c6c 6261 636b 3d4e 6f6e 6529  s_callback=None)
+0000ad60: 3a0d 0a20 2020 2020 2020 2073 656c 662e  :..        self.
+0000ad70: 6368 616e 6e65 6c73 203d 2063 6861 6e6e  channels = chann
+0000ad80: 656c 730d 0a20 2020 2020 2020 2073 656c  els..        sel
+0000ad90: 662e 7261 7465 203d 2072 6174 650d 0a20  f.rate = rate.. 
+0000ada0: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
+0000adb0: 7265 7373 5f63 616c 6c62 6163 6b20 3d20  ress_callback = 
+0000adc0: 7072 6f67 7265 7373 5f63 616c 6c62 6163  progress_callbac
+0000add0: 6b0d 0a20 2020 2020 2020 2073 656c 662e  k..        self.
+0000ade0: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
+0000adf0: 616c 6c62 6163 6b20 3d20 6572 726f 725f  allback = error_
+0000ae00: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
+0000ae10: 6b0d 0a0d 0a20 2020 2064 6566 205f 5f63  k....    def __c
+0000ae20: 616c 6c5f 5f28 7365 6c66 2c20 6d65 6469  all__(self, medi
+0000ae30: 615f 6669 6c65 7061 7468 293a 0d0a 2020  a_filepath):..  
+0000ae40: 2020 2020 2020 7465 6d70 203d 2074 656d        temp = tem
+0000ae50: 7066 696c 652e 4e61 6d65 6454 656d 706f  pfile.NamedTempo
+0000ae60: 7261 7279 4669 6c65 2873 7566 6669 783d  raryFile(suffix=
+0000ae70: 272e 7761 7627 2c20 6465 6c65 7465 3d46  '.wav', delete=F
+0000ae80: 616c 7365 290d 0a20 2020 2020 2020 2069  alse)..        i
+0000ae90: 6620 6e6f 7420 6f73 2e70 6174 682e 6973  f not os.path.is
+0000aea0: 6669 6c65 286d 6564 6961 5f66 696c 6570  file(media_filep
+0000aeb0: 6174 6829 3a0d 0a20 2020 2020 2020 2020  ath):..         
+0000aec0: 2020 2069 6620 7365 6c66 2e65 7272 6f72     if self.error
+0000aed0: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
+0000aee0: 636b 3a0d 0a20 2020 2020 2020 2020 2020  ck:..           
+0000aef0: 2020 2020 2073 656c 662e 6572 726f 725f       self.error_
+0000af00: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
+0000af10: 6b28 2254 6865 2067 6976 656e 2066 696c  k("The given fil
+0000af20: 6520 646f 6573 206e 6f74 2065 7869 7374  e does not exist
+0000af30: 3a20 7b30 7d22 2e66 6f72 6d61 7428 6d65  : {0}".format(me
+0000af40: 6469 615f 6669 6c65 7061 7468 2929 0d0a  dia_filepath))..
+0000af50: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0000af60: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000af70: 2020 2070 7269 6e74 2822 5468 6520 6769     print("The gi
+0000af80: 7665 6e20 6669 6c65 2064 6f65 7320 6e6f  ven file does no
+0000af90: 7420 6578 6973 743a 207b 307d 222e 666f  t exist: {0}".fo
+0000afa0: 726d 6174 286d 6564 6961 5f66 696c 6570  rmat(media_filep
+0000afb0: 6174 6829 290d 0a20 2020 2020 2020 2020  ath))..         
+0000afc0: 2020 2020 2020 2072 6169 7365 2045 7863         raise Exc
+0000afd0: 6570 7469 6f6e 2822 496e 7661 6c69 6420  eption("Invalid 
+0000afe0: 6669 6c65 3a20 7b30 7d22 2e66 6f72 6d61  file: {0}".forma
+0000aff0: 7428 6d65 6469 615f 6669 6c65 7061 7468  t(media_filepath
+0000b000: 2929 0d0a 2020 2020 2020 2020 6966 206e  ))..        if n
+0000b010: 6f74 2073 656c 662e 6666 6d70 6567 5f63  ot self.ffmpeg_c
+0000b020: 6865 636b 2829 3a0d 0a20 2020 2020 2020  heck():..       
+0000b030: 2020 2020 2069 6620 7365 6c66 2e65 7272       if self.err
+0000b040: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
+0000b050: 6261 636b 3a0d 0a20 2020 2020 2020 2020  back:..         
+0000b060: 2020 2020 2020 2073 656c 662e 6572 726f         self.erro
+0000b070: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
+0000b080: 6163 6b28 2266 666d 7065 673a 2045 7865  ack("ffmpeg: Exe
+0000b090: 6375 7461 626c 6520 6e6f 7420 666f 756e  cutable not foun
+0000b0a0: 6420 6f6e 206d 6163 6869 6e65 2e22 290d  d on machine.").
+0000b0b0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+0000b0c0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000b0d0: 2020 2020 7072 696e 7428 2266 666d 7065      print("ffmpe
+0000b0e0: 673a 2045 7865 6375 7461 626c 6520 6e6f  g: Executable no
+0000b0f0: 7420 666f 756e 6420 6f6e 206d 6163 6869  t found on machi
+0000b100: 6e65 2e22 290d 0a20 2020 2020 2020 2020  ne.")..         
+0000b110: 2020 2020 2020 2072 6169 7365 2045 7863         raise Exc
+0000b120: 6570 7469 6f6e 2822 4465 7065 6e64 656e  eption("Dependen
+0000b130: 6379 206e 6f74 2066 6f75 6e64 3a20 6666  cy not found: ff
+0000b140: 6d70 6567 2229 0d0a 0d0a 2020 2020 2020  mpeg")....      
+0000b150: 2020 636f 6d6d 616e 6420 3d20 5b0d 0a20    command = [.. 
+0000b160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b170: 2020 2022 6666 6d70 6567 222c 0d0a 2020     "ffmpeg",..  
+0000b180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b190: 2020 222d 7922 2c0d 0a20 2020 2020 2020    "-y",..       
+0000b1a0: 2020 2020 2020 2020 2020 2020 2022 2d69               "-i
+0000b1b0: 222c 206d 6564 6961 5f66 696c 6570 6174  ", media_filepat
+0000b1c0: 682c 0d0a 2020 2020 2020 2020 2020 2020  h,..            
+0000b1d0: 2020 2020 2020 2020 222d 6163 222c 2073          "-ac", s
+0000b1e0: 7472 2873 656c 662e 6368 616e 6e65 6c73  tr(self.channels
+0000b1f0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+0000b200: 2020 2020 2020 2020 222d 6172 222c 2073          "-ar", s
+0000b210: 7472 2873 656c 662e 7261 7465 292c 0d0a  tr(self.rate),..
+0000b220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b230: 2020 2020 222d 6c6f 676c 6576 656c 222c      "-loglevel",
+0000b240: 2022 6572 726f 7222 2c0d 0a20 2020 2020   "error",..     
+0000b250: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000b260: 2d68 6964 655f 6261 6e6e 6572 222c 0d0a  -hide_banner",..
+0000b270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b280: 2020 2020 7465 6d70 2e6e 616d 650d 0a20      temp.name.. 
+0000b290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2a0: 205d 0d0a 0d0a 2020 2020 2020 2020 7472   ]....        tr
+0000b2b0: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+0000b2c0: 2320 5255 4e4e 494e 4720 6666 6d70 6567  # RUNNING ffmpeg
+0000b2d0: 2057 4954 484f 5554 2053 484f 5749 4e47   WITHOUT SHOWING
+0000b2e0: 2050 524f 4752 4553 5353 0d0a 2020 2020   PROGRESSS..    
+0000b2f0: 2020 2020 2020 2020 2375 7365 5f73 6865          #use_she
+0000b300: 6c6c 203d 2054 7275 6520 6966 206f 732e  ll = True if os.
+0000b310: 6e61 6d65 203d 3d20 226e 7422 2065 6c73  name == "nt" els
+0000b320: 6520 4661 6c73 650d 0a20 2020 2020 2020  e False..       
+0000b330: 2020 2020 2023 7375 6270 726f 6365 7373       #subprocess
+0000b340: 2e63 6865 636b 5f6f 7574 7075 7428 636f  .check_output(co
+0000b350: 6d6d 616e 642c 2073 7464 696e 3d6f 7065  mmand, stdin=ope
+0000b360: 6e28 6f73 2e64 6576 6e75 6c6c 292c 2073  n(os.devnull), s
+0000b370: 6865 6c6c 3d75 7365 5f73 6865 6c6c 290d  hell=use_shell).
+0000b380: 0a0d 0a20 2020 2020 2020 2020 2020 2023  ...            #
+0000b390: 2052 554e 4e49 4e47 2066 666d 7065 6720   RUNNING ffmpeg 
+0000b3a0: 5749 5448 2050 524f 4752 4553 5353 0d0a  WITH PROGRESSS..
+0000b3b0: 2020 2020 2020 2020 2020 2020 6666 203d              ff =
+0000b3c0: 2046 666d 7065 6750 726f 6772 6573 7328   FfmpegProgress(
+0000b3d0: 636f 6d6d 616e 6429 0d0a 2020 2020 2020  command)..      
+0000b3e0: 2020 2020 2020 7065 7263 656e 7461 6765        percentage
+0000b3f0: 203d 2030 0d0a 2020 2020 2020 2020 2020   = 0..          
+0000b400: 2020 666f 7220 7072 6f67 7265 7373 2069    for progress i
+0000b410: 6e20 6666 2e72 756e 5f63 6f6d 6d61 6e64  n ff.run_command
+0000b420: 5f77 6974 685f 7072 6f67 7265 7373 2829  _with_progress()
+0000b430: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000b440: 2020 2070 6572 6365 6e74 6167 6520 3d20     percentage = 
+0000b450: 7072 6f67 7265 7373 0d0a 2020 2020 2020  progress..      
+0000b460: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000b470: 662e 7072 6f67 7265 7373 5f63 616c 6c62  f.progress_callb
+0000b480: 6163 6b3a 0d0a 2020 2020 2020 2020 2020  ack:..          
+0000b490: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+0000b4a0: 726f 6772 6573 735f 6361 6c6c 6261 636b  rogress_callback
+0000b4b0: 286d 6564 6961 5f66 696c 6570 6174 682c  (media_filepath,
+0000b4c0: 2070 6572 6365 6e74 6167 6529 0d0a 2020   percentage)..  
+0000b4d0: 2020 2020 2020 2020 2020 7465 6d70 2e63            temp.c
+0000b4e0: 6c6f 7365 2829 0d0a 0d0a 2020 2020 2020  lose()....      
+0000b4f0: 2020 2020 2020 7265 7475 726e 2074 656d        return tem
+0000b500: 702e 6e61 6d65 2c20 7365 6c66 2e72 6174  p.name, self.rat
+0000b510: 650d 0a0d 0a20 2020 2020 2020 2065 7863  e....        exc
+0000b520: 6570 7420 4b65 7962 6f61 7264 496e 7465  ept KeyboardInte
+0000b530: 7272 7570 743a 0d0a 2020 2020 2020 2020  rrupt:..        
+0000b540: 2020 2020 6966 2073 656c 662e 6572 726f      if self.erro
+0000b550: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
+0000b560: 6163 6b3a 0d0a 2020 2020 2020 2020 2020  ack:..          
+0000b570: 2020 2020 2020 7365 6c66 2e65 7272 6f72        self.error
+0000b580: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
+0000b590: 636b 2822 4361 6e63 656c 6c69 6e67 2061  ck("Cancelling a
+0000b5a0: 6c6c 2074 6173 6b73 2229 0d0a 2020 2020  ll tasks")..    
+0000b5b0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+0000b5c0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000b5d0: 7269 6e74 2822 4361 6e63 656c 6c69 6e67  rint("Cancelling
+0000b5e0: 2061 6c6c 2074 6173 6b73 2229 0d0a 2020   all tasks")..  
+0000b5f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000b600: 0d0a 0d0a 2020 2020 2020 2020 6578 6365  ....        exce
+0000b610: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+0000b620: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000b630: 6966 2073 656c 662e 6572 726f 725f 6d65  if self.error_me
+0000b640: 7373 6167 6573 5f63 616c 6c62 6163 6b3a  ssages_callback:
+0000b650: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000b660: 2020 7365 6c66 2e65 7272 6f72 5f6d 6573    self.error_mes
+0000b670: 7361 6765 735f 6361 6c6c 6261 636b 2865  sages_callback(e
+0000b680: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+0000b690: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+0000b6a0: 2020 2020 2020 7072 696e 7428 6529 0d0a        print(e)..
+0000b6b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000b6c0: 726e 0d0a 0d0a 0d0a 636c 6173 7320 5370  rn......class Sp
+0000b6d0: 6565 6368 5265 6769 6f6e 4669 6e64 6572  eechRegionFinder
+0000b6e0: 3a0d 0a20 2020 2040 7374 6174 6963 6d65  :..    @staticme
+0000b6f0: 7468 6f64 0d0a 2020 2020 6465 6620 7065  thod..    def pe
+0000b700: 7263 656e 7469 6c65 2861 7272 2c20 7065  rcentile(arr, pe
+0000b710: 7263 656e 7429 3a0d 0a20 2020 2020 2020  rcent):..       
+0000b720: 2061 7272 203d 2073 6f72 7465 6428 6172   arr = sorted(ar
+0000b730: 7229 0d0a 2020 2020 2020 2020 6b20 3d20  r)..        k = 
+0000b740: 286c 656e 2861 7272 2920 2d20 3129 202a  (len(arr) - 1) *
+0000b750: 2070 6572 6365 6e74 0d0a 2020 2020 2020   percent..      
+0000b760: 2020 6620 3d20 6d61 7468 2e66 6c6f 6f72    f = math.floor
+0000b770: 286b 290d 0a20 2020 2020 2020 2063 203d  (k)..        c =
+0000b780: 206d 6174 682e 6365 696c 286b 290d 0a20   math.ceil(k).. 
+0000b790: 2020 2020 2020 2069 6620 6620 3d3d 2063         if f == c
+0000b7a0: 3a20 7265 7475 726e 2061 7272 5b69 6e74  : return arr[int
+0000b7b0: 286b 295d 0d0a 2020 2020 2020 2020 6430  (k)]..        d0
+0000b7c0: 203d 2061 7272 5b69 6e74 2866 295d 202a   = arr[int(f)] *
+0000b7d0: 2028 6320 2d20 6b29 0d0a 2020 2020 2020   (c - k)..      
+0000b7e0: 2020 6431 203d 2061 7272 5b69 6e74 2863    d1 = arr[int(c
+0000b7f0: 295d 202a 2028 6b20 2d20 6629 0d0a 2020  )] * (k - f)..  
+0000b800: 2020 2020 2020 7265 7475 726e 2064 3020        return d0 
+0000b810: 2b20 6431 0d0a 0d0a 2020 2020 2364 6566  + d1....    #def
+0000b820: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+0000b830: 6672 616d 655f 7769 6474 683d 3430 3936  frame_width=4096
+0000b840: 2c20 6d69 6e5f 7265 6769 6f6e 5f73 697a  , min_region_siz
+0000b850: 653d 302e 352c 206d 6178 5f72 6567 696f  e=0.5, max_regio
+0000b860: 6e5f 7369 7a65 3d36 293a 0d0a 2020 2020  n_size=6):..    
+0000b870: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+0000b880: 662c 2066 7261 6d65 5f77 6964 7468 3d34  f, frame_width=4
+0000b890: 3039 362c 206d 696e 5f72 6567 696f 6e5f  096, min_region_
+0000b8a0: 7369 7a65 3d30 2e35 2c20 6d61 785f 7265  size=0.5, max_re
+0000b8b0: 6769 6f6e 5f73 697a 653d 362c 2065 7272  gion_size=6, err
+0000b8c0: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
+0000b8d0: 6261 636b 3d4e 6f6e 6529 3a0d 0a20 2020  back=None):..   
+0000b8e0: 2020 2020 2073 656c 662e 6672 616d 655f       self.frame_
+0000b8f0: 7769 6474 6820 3d20 6672 616d 655f 7769  width = frame_wi
+0000b900: 6474 680d 0a20 2020 2020 2020 2073 656c  dth..        sel
+0000b910: 662e 6d69 6e5f 7265 6769 6f6e 5f73 697a  f.min_region_siz
+0000b920: 6520 3d20 6d69 6e5f 7265 6769 6f6e 5f73  e = min_region_s
+0000b930: 697a 650d 0a20 2020 2020 2020 2073 656c  ize..        sel
+0000b940: 662e 6d61 785f 7265 6769 6f6e 5f73 697a  f.max_region_siz
+0000b950: 6520 3d20 6d61 785f 7265 6769 6f6e 5f73  e = max_region_s
+0000b960: 697a 650d 0a20 2020 2020 2020 2073 656c  ize..        sel
+0000b970: 662e 6572 726f 725f 6d65 7373 6167 6573  f.error_messages
+0000b980: 5f63 616c 6c62 6163 6b20 3d20 6572 726f  _callback = erro
+0000b990: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
+0000b9a0: 6163 6b0d 0a0d 0a20 2020 2023 6465 6620  ack....    #def 
+0000b9b0: 5f5f 6361 6c6c 5f5f 2873 656c 662c 2077  __call__(self, w
+0000b9c0: 6176 5f66 696c 6570 6174 682c 2065 7272  av_filepath, err
+0000b9d0: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
+0000b9e0: 6261 636b 3d4e 6f6e 6529 3a0d 0a20 2020  back=None):..   
+0000b9f0: 2064 6566 205f 5f63 616c 6c5f 5f28 7365   def __call__(se
+0000ba00: 6c66 2c20 7761 765f 6669 6c65 7061 7468  lf, wav_filepath
+0000ba10: 293a 0d0a 2020 2020 2020 2020 7472 793a  ):..        try:
+0000ba20: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+0000ba30: 6164 6572 203d 2077 6176 652e 6f70 656e  ader = wave.open
+0000ba40: 2877 6176 5f66 696c 6570 6174 6829 0d0a  (wav_filepath)..
+0000ba50: 2020 2020 2020 2020 2020 2020 7361 6d70              samp
+0000ba60: 6c65 5f77 6964 7468 203d 2072 6561 6465  le_width = reade
+0000ba70: 722e 6765 7473 616d 7077 6964 7468 2829  r.getsampwidth()
+0000ba80: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
+0000ba90: 7465 203d 2072 6561 6465 722e 6765 7466  te = reader.getf
+0000baa0: 7261 6d65 7261 7465 2829 0d0a 2020 2020  ramerate()..    
+0000bab0: 2020 2020 2020 2020 6e5f 6368 616e 6e65          n_channe
+0000bac0: 6c73 203d 2072 6561 6465 722e 6765 746e  ls = reader.getn
+0000bad0: 6368 616e 6e65 6c73 2829 0d0a 2020 2020  channels()..    
+0000bae0: 2020 2020 2020 2020 746f 7461 6c5f 6475          total_du
+0000baf0: 7261 7469 6f6e 203d 2072 6561 6465 722e  ration = reader.
+0000bb00: 6765 746e 6672 616d 6573 2829 202f 2072  getnframes() / r
+0000bb10: 6174 650d 0a20 2020 2020 2020 2020 2020  ate..           
+0000bb20: 2063 6875 6e6b 5f64 7572 6174 696f 6e20   chunk_duration 
+0000bb30: 3d20 666c 6f61 7428 7365 6c66 2e66 7261  = float(self.fra
+0000bb40: 6d65 5f77 6964 7468 2920 2f20 7261 7465  me_width) / rate
+0000bb50: 0d0a 2020 2020 2020 2020 2020 2020 6e5f  ..            n_
+0000bb60: 6368 756e 6b73 203d 2069 6e74 2874 6f74  chunks = int(tot
+0000bb70: 616c 5f64 7572 6174 696f 6e20 2f20 6368  al_duration / ch
+0000bb80: 756e 6b5f 6475 7261 7469 6f6e 290d 0a20  unk_duration).. 
+0000bb90: 2020 2020 2020 2020 2020 2065 6e65 7267             energ
+0000bba0: 6965 7320 3d20 5b5d 0d0a 2020 2020 2020  ies = []..      
+0000bbb0: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+0000bbc0: 616e 6765 286e 5f63 6875 6e6b 7329 3a0d  ange(n_chunks):.
+0000bbd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bbe0: 2063 6875 6e6b 203d 2072 6561 6465 722e   chunk = reader.
+0000bbf0: 7265 6164 6672 616d 6573 2873 656c 662e  readframes(self.
+0000bc00: 6672 616d 655f 7769 6474 6829 0d0a 2020  frame_width)..  
+0000bc10: 2020 2020 2020 2020 2020 2020 2020 656e                en
+0000bc20: 6572 6769 6573 2e61 7070 656e 6428 6175  ergies.append(au
+0000bc30: 6469 6f6f 702e 726d 7328 6368 756e 6b2c  dioop.rms(chunk,
+0000bc40: 2073 616d 706c 655f 7769 6474 6820 2a20   sample_width * 
+0000bc50: 6e5f 6368 616e 6e65 6c73 2929 0d0a 2020  n_channels))..  
+0000bc60: 2020 2020 2020 2020 2020 7468 7265 7368            thresh
+0000bc70: 6f6c 6420 3d20 5370 6565 6368 5265 6769  old = SpeechRegi
+0000bc80: 6f6e 4669 6e64 6572 2e70 6572 6365 6e74  onFinder.percent
+0000bc90: 696c 6528 656e 6572 6769 6573 2c20 302e  ile(energies, 0.
+0000bca0: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
+0000bcb0: 656c 6170 7365 645f 7469 6d65 203d 2030  elapsed_time = 0
+0000bcc0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+0000bcd0: 6769 6f6e 7320 3d20 5b5d 0d0a 2020 2020  gions = []..    
+0000bce0: 2020 2020 2020 2020 7265 6769 6f6e 5f73          region_s
+0000bcf0: 7461 7274 203d 204e 6f6e 650d 0a20 2020  tart = None..   
+0000bd00: 2020 2020 2020 2020 2066 6f72 2065 6e65           for ene
+0000bd10: 7267 7920 696e 2065 6e65 7267 6965 733a  rgy in energies:
+0000bd20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000bd30: 2020 6973 5f73 696c 656e 6365 203d 2065    is_silence = e
+0000bd40: 6e65 7267 7920 3c3d 2074 6872 6573 686f  nergy <= thresho
+0000bd50: 6c64 0d0a 2020 2020 2020 2020 2020 2020  ld..            
+0000bd60: 2020 2020 6d61 785f 6578 6365 6564 6564      max_exceeded
+0000bd70: 203d 2072 6567 696f 6e5f 7374 6172 7420   = region_start 
+0000bd80: 616e 6420 656c 6170 7365 645f 7469 6d65  and elapsed_time
+0000bd90: 202d 2072 6567 696f 6e5f 7374 6172 7420   - region_start 
+0000bda0: 3e3d 2073 656c 662e 6d61 785f 7265 6769  >= self.max_regi
+0000bdb0: 6f6e 5f73 697a 650d 0a20 2020 2020 2020  on_size..       
+0000bdc0: 2020 2020 2020 2020 2069 6620 286d 6178           if (max
+0000bdd0: 5f65 7863 6565 6465 6420 6f72 2069 735f  _exceeded or is_
+0000bde0: 7369 6c65 6e63 6529 2061 6e64 2072 6567  silence) and reg
+0000bdf0: 696f 6e5f 7374 6172 743a 0d0a 2020 2020  ion_start:..    
+0000be00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be10: 6966 2065 6c61 7073 6564 5f74 696d 6520  if elapsed_time 
+0000be20: 2d20 7265 6769 6f6e 5f73 7461 7274 203e  - region_start >
+0000be30: 3d20 7365 6c66 2e6d 696e 5f72 6567 696f  = self.min_regio
+0000be40: 6e5f 7369 7a65 3a0d 0a20 2020 2020 2020  n_size:..       
+0000be50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be60: 2072 6567 696f 6e73 2e61 7070 656e 6428   regions.append(
+0000be70: 2872 6567 696f 6e5f 7374 6172 742c 2065  (region_start, e
+0000be80: 6c61 7073 6564 5f74 696d 6529 290d 0a20  lapsed_time)).. 
+0000be90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bea0: 2020 2020 2020 2072 6567 696f 6e5f 7374         region_st
+0000beb0: 6172 7420 3d20 4e6f 6e65 0d0a 2020 2020  art = None..    
+0000bec0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+0000bed0: 2028 6e6f 7420 7265 6769 6f6e 5f73 7461   (not region_sta
+0000bee0: 7274 2920 616e 6420 286e 6f74 2069 735f  rt) and (not is_
+0000bef0: 7369 6c65 6e63 6529 3a0d 0a20 2020 2020  silence):..     
+0000bf00: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000bf10: 6567 696f 6e5f 7374 6172 7420 3d20 656c  egion_start = el
+0000bf20: 6170 7365 645f 7469 6d65 0d0a 2020 2020  apsed_time..    
+0000bf30: 2020 2020 2020 2020 2020 2020 656c 6170              elap
+0000bf40: 7365 645f 7469 6d65 202b 3d20 6368 756e  sed_time += chun
+0000bf50: 6b5f 6475 7261 7469 6f6e 0d0a 2020 2020  k_duration..    
+0000bf60: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0000bf70: 6567 696f 6e73 0d0a 0d0a 2020 2020 2020  egions....      
+0000bf80: 2020 6578 6365 7074 204b 6579 626f 6172    except Keyboar
+0000bf90: 6449 6e74 6572 7275 7074 3a0d 0a20 2020  dInterrupt:..   
+0000bfa0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0000bfb0: 2e65 7272 6f72 5f6d 6573 7361 6765 735f  .error_messages_
+0000bfc0: 6361 6c6c 6261 636b 3a0d 0a20 2020 2020  callback:..     
+0000bfd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000bfe0: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
+0000bff0: 616c 6c62 6163 6b28 2243 616e 6365 6c6c  allback("Cancell
+0000c000: 696e 6720 616c 6c20 7461 736b 7322 290d  ing all tasks").
+0000c010: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+0000c020: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000c030: 2020 2020 7072 696e 7428 2243 616e 6365      print("Cance
+0000c040: 6c6c 696e 6720 616c 6c20 7461 736b 7322  lling all tasks"
+0000c050: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
+0000c060: 6574 7572 6e0d 0a0d 0a20 2020 2020 2020  eturn....       
+0000c070: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+0000c080: 6e20 6173 2065 3a0d 0a20 2020 2020 2020  n as e:..       
+0000c090: 2020 2020 2069 6620 7365 6c66 2e65 7272       if self.err
+0000c0a0: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
+0000c0b0: 6261 636b 3a0d 0a20 2020 2020 2020 2020  back:..         
+0000c0c0: 2020 2020 2020 2073 656c 662e 6572 726f         self.erro
+0000c0d0: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
+0000c0e0: 6163 6b28 6529 0d0a 2020 2020 2020 2020  ack(e)..        
+0000c0f0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+0000c100: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0000c110: 2865 290d 0a20 2020 2020 2020 2020 2020  (e)..           
+0000c120: 2072 6574 7572 6e0d 0a0d 0a0d 0a63 6c61   return......cla
+0000c130: 7373 2046 4c41 4343 6f6e 7665 7274 6572  ss FLACConverter
+0000c140: 286f 626a 6563 7429 3a0d 0a20 2020 2023  (object):..    #
+0000c150: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+0000c160: 662c 2077 6176 5f66 696c 6570 6174 682c  f, wav_filepath,
+0000c170: 2069 6e63 6c75 6465 5f62 6566 6f72 653d   include_before=
+0000c180: 302e 3235 2c20 696e 636c 7564 655f 6166  0.25, include_af
+0000c190: 7465 723d 302e 3235 293a 0d0a 2020 2020  ter=0.25):..    
+0000c1a0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+0000c1b0: 662c 2077 6176 5f66 696c 6570 6174 682c  f, wav_filepath,
+0000c1c0: 2069 6e63 6c75 6465 5f62 6566 6f72 653d   include_before=
+0000c1d0: 302e 3235 2c20 696e 636c 7564 655f 6166  0.25, include_af
+0000c1e0: 7465 723d 302e 3235 2c20 6572 726f 725f  ter=0.25, error_
+0000c1f0: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
+0000c200: 6b3d 4e6f 6e65 293a 0d0a 2020 2020 2020  k=None):..      
+0000c210: 2020 7365 6c66 2e77 6176 5f66 696c 6570    self.wav_filep
+0000c220: 6174 6820 3d20 7761 765f 6669 6c65 7061  ath = wav_filepa
+0000c230: 7468 0d0a 2020 2020 2020 2020 7365 6c66  th..        self
+0000c240: 2e69 6e63 6c75 6465 5f62 6566 6f72 6520  .include_before 
+0000c250: 3d20 696e 636c 7564 655f 6265 666f 7265  = include_before
+0000c260: 0d0a 2020 2020 2020 2020 7365 6c66 2e69  ..        self.i
+0000c270: 6e63 6c75 6465 5f61 6674 6572 203d 2069  nclude_after = i
+0000c280: 6e63 6c75 6465 5f61 6674 6572 0d0a 2020  nclude_after..  
+0000c290: 2020 2020 2020 7365 6c66 2e65 7272 6f72        self.error
+0000c2a0: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
+0000c2b0: 636b 203d 2065 7272 6f72 5f6d 6573 7361  ck = error_messa
+0000c2c0: 6765 735f 6361 6c6c 6261 636b 0d0a 0d0a  ges_callback....
+0000c2d0: 2020 2020 2364 6566 205f 5f63 616c 6c5f      #def __call_
+0000c2e0: 5f28 7365 6c66 2c20 7265 6769 6f6e 2c20  _(self, region, 
+0000c2f0: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
+0000c300: 616c 6c62 6163 6b3d 4e6f 6e65 293a 0d0a  allback=None):..
+0000c310: 2020 2020 6465 6620 5f5f 6361 6c6c 5f5f      def __call__
+0000c320: 2873 656c 662c 2072 6567 696f 6e29 3a0d  (self, region):.
+0000c330: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
+0000c340: 2020 2020 2020 2020 2020 2073 7461 7274             start
+0000c350: 2c20 656e 6420 3d20 7265 6769 6f6e 0d0a  , end = region..
+0000c360: 2020 2020 2020 2020 2020 2020 7374 6172              star
+0000c370: 7420 3d20 6d61 7828 302c 2073 7461 7274  t = max(0, start
+0000c380: 202d 2073 656c 662e 696e 636c 7564 655f   - self.include_
+0000c390: 6265 666f 7265 290d 0a20 2020 2020 2020  before)..       
+0000c3a0: 2020 2020 2065 6e64 202b 3d20 7365 6c66       end += self
+0000c3b0: 2e69 6e63 6c75 6465 5f61 6674 6572 0d0a  .include_after..
+0000c3c0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+0000c3d0: 203d 2074 656d 7066 696c 652e 4e61 6d65   = tempfile.Name
+0000c3e0: 6454 656d 706f 7261 7279 4669 6c65 2873  dTemporaryFile(s
+0000c3f0: 7566 6669 783d 272e 666c 6163 272c 2064  uffix='.flac', d
+0000c400: 656c 6574 653d 4661 6c73 6529 0d0a 2020  elete=False)..  
+0000c410: 2020 2020 2020 2020 2020 636f 6d6d 616e            comman
+0000c420: 6420 3d20 5b0d 0a20 2020 2020 2020 2020  d = [..         
+0000c430: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000c440: 6666 6d70 6567 222c 0d0a 2020 2020 2020  ffmpeg",..      
+0000c450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c460: 2020 222d 7373 222c 2073 7472 2873 7461    "-ss", str(sta
+0000c470: 7274 292c 0d0a 2020 2020 2020 2020 2020  rt),..          
+0000c480: 2020 2020 2020 2020 2020 2020 2020 222d                "-
+0000c490: 7422 2c20 7374 7228 656e 6420 2d20 7374  t", str(end - st
+0000c4a0: 6172 7429 2c0d 0a20 2020 2020 2020 2020  art),..         
+0000c4b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000c4c0: 2d79 222c 0d0a 2020 2020 2020 2020 2020  -y",..          
+0000c4d0: 2020 2020 2020 2020 2020 2020 2020 222d                "-
+0000c4e0: 6922 2c20 7365 6c66 2e77 6176 5f66 696c  i", self.wav_fil
+0000c4f0: 6570 6174 682c 0d0a 2020 2020 2020 2020  epath,..        
+0000c500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c510: 222d 6c6f 676c 6576 656c 222c 2022 6572  "-loglevel", "er
+0000c520: 726f 7222 2c0d 0a20 2020 2020 2020 2020  ror",..         
+0000c530: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000c540: 656d 702e 6e61 6d65 0d0a 2020 2020 2020  emp.name..      
+0000c550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c560: 5d0d 0a20 2020 2020 2020 2020 2020 2073  ]..            s
+0000c570: 7562 7072 6f63 6573 732e 6368 6563 6b5f  ubprocess.check_
+0000c580: 6f75 7470 7574 2863 6f6d 6d61 6e64 2c20  output(command, 
+0000c590: 7374 6469 6e3d 6f70 656e 286f 732e 6465  stdin=open(os.de
+0000c5a0: 766e 756c 6c29 290d 0a20 2020 2020 2020  vnull))..       
+0000c5b0: 2020 2020 2063 6f6e 7465 6e74 203d 2074       content = t
+0000c5c0: 656d 702e 7265 6164 2829 0d0a 2020 2020  emp.read()..    
+0000c5d0: 2020 2020 2020 2020 7465 6d70 2e63 6c6f          temp.clo
+0000c5e0: 7365 2829 0d0a 2020 2020 2020 2020 2020  se()..          
+0000c5f0: 2020 7265 7475 726e 2063 6f6e 7465 6e74    return content
+0000c600: 0d0a 0d0a 2020 2020 2020 2020 6578 6365  ....        exce
+0000c610: 7074 204b 6579 626f 6172 6449 6e74 6572  pt KeyboardInter
+0000c620: 7275 7074 3a0d 0a20 2020 2020 2020 2020  rupt:..         
+0000c630: 2020 2069 6620 7365 6c66 2e65 7272 6f72     if self.error
+0000c640: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
+0000c650: 636b 3a0d 0a20 2020 2020 2020 2020 2020  ck:..           
+0000c660: 2020 2020 2073 656c 662e 6572 726f 725f       self.error_
+0000c670: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
+0000c680: 6b28 2243 616e 6365 6c6c 696e 6720 616c  k("Cancelling al
+0000c690: 6c20 7461 736b 7322 290d 0a20 2020 2020  l tasks")..     
+0000c6a0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+0000c6b0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+0000c6c0: 696e 7428 2243 616e 6365 6c6c 696e 6720  int("Cancelling 
+0000c6d0: 616c 6c20 7461 736b 7322 290d 0a20 2020  all tasks")..   
+0000c6e0: 2020 2020 2020 2020 2072 6574 7572 6e0d           return.
+0000c6f0: 0a0d 0a20 2020 2020 2020 2065 7863 6570  ...        excep
+0000c700: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+0000c710: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
+0000c720: 6620 7365 6c66 2e65 7272 6f72 5f6d 6573  f self.error_mes
+0000c730: 7361 6765 735f 6361 6c6c 6261 636b 3a0d  sages_callback:.
+0000c740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c750: 2073 656c 662e 6572 726f 725f 6d65 7373   self.error_mess
+0000c760: 6167 6573 5f63 616c 6c62 6163 6b28 6529  ages_callback(e)
+0000c770: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+0000c780: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+0000c790: 2020 2020 2070 7269 6e74 2865 290d 0a20       print(e).. 
+0000c7a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000c7b0: 6e0d 0a0d 0a0d 0a63 6c61 7373 2053 7065  n......class Spe
+0000c7c0: 6563 6852 6563 6f67 6e69 7a65 7228 6f62  echRecognizer(ob
+0000c7d0: 6a65 6374 293a 0d0a 2020 2020 6465 6620  ject):..    def 
+0000c7e0: 5f5f 696e 6974 5f5f 2873 656c 662c 206c  __init__(self, l
+0000c7f0: 616e 6775 6167 653d 2265 6e22 2c20 7261  anguage="en", ra
+0000c800: 7465 3d34 3431 3030 2c20 7265 7472 6965  te=44100, retrie
+0000c810: 733d 332c 2061 7069 5f6b 6579 3d22 4149  s=3, api_key="AI
+0000c820: 7a61 5379 424f 7469 346d 4d2d 3678 3957  zaSyBOti4mM-6x9W
+0000c830: 446e 5a49 6a49 6579 4555 3231 4f70 4258  DnZIjIeyEU21OpBX
+0000c840: 7157 4267 7722 2c20 7469 6d65 6f75 743d  qWBgw", timeout=
+0000c850: 3330 2c20 6572 726f 725f 6d65 7373 6167  30, error_messag
+0000c860: 6573 5f63 616c 6c62 6163 6b3d 4e6f 6e65  es_callback=None
+0000c870: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
+0000c880: 2e6c 616e 6775 6167 6520 3d20 6c61 6e67  .language = lang
+0000c890: 7561 6765 0d0a 2020 2020 2020 2020 7365  uage..        se
+0000c8a0: 6c66 2e72 6174 6520 3d20 7261 7465 0d0a  lf.rate = rate..
+0000c8b0: 2020 2020 2020 2020 7365 6c66 2e61 7069          self.api
+0000c8c0: 5f6b 6579 203d 2061 7069 5f6b 6579 0d0a  _key = api_key..
+0000c8d0: 2020 2020 2020 2020 7365 6c66 2e72 6574          self.ret
+0000c8e0: 7269 6573 203d 2072 6574 7269 6573 0d0a  ries = retries..
+0000c8f0: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
+0000c900: 656f 7574 203d 2074 696d 656f 7574 0d0a  eout = timeout..
+0000c910: 2020 2020 2020 2020 7365 6c66 2e65 7272          self.err
+0000c920: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
+0000c930: 6261 636b 203d 2065 7272 6f72 5f6d 6573  back = error_mes
+0000c940: 7361 6765 735f 6361 6c6c 6261 636b 0d0a  sages_callback..
+0000c950: 0d0a 2020 2020 6465 6620 5f5f 6361 6c6c  ..    def __call
+0000c960: 5f5f 2873 656c 662c 2064 6174 6129 3a0d  __(self, data):.
+0000c970: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
+0000c980: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+0000c990: 2069 6e20 7261 6e67 6528 7365 6c66 2e72   in range(self.r
+0000c9a0: 6574 7269 6573 293a 0d0a 2020 2020 2020  etries):..      
+0000c9b0: 2020 2020 2020 2020 2020 7572 6c20 3d20            url = 
+0000c9c0: 2268 7474 703a 2f2f 7777 772e 676f 6f67  "http://www.goog
+0000c9d0: 6c65 2e63 6f6d 2f73 7065 6563 682d 6170  le.com/speech-ap
+0000c9e0: 692f 7632 2f72 6563 6f67 6e69 7a65 3f63  i/v2/recognize?c
+0000c9f0: 6c69 656e 743d 6368 726f 6d69 756d 266c  lient=chromium&l
+0000ca00: 616e 673d 7b6c 616e 677d 266b 6579 3d7b  ang={lang}&key={
+0000ca10: 6b65 797d 222e 666f 726d 6174 286c 616e  key}".format(lan
+0000ca20: 673d 7365 6c66 2e6c 616e 6775 6167 652c  g=self.language,
+0000ca30: 206b 6579 3d73 656c 662e 6170 695f 6b65   key=self.api_ke
+0000ca40: 7929 0d0a 2020 2020 2020 2020 2020 2020  y)..            
+0000ca50: 2020 2020 6865 6164 6572 7320 3d20 7b22      headers = {"
+0000ca60: 436f 6e74 656e 742d 5479 7065 223a 2022  Content-Type": "
+0000ca70: 6175 6469 6f2f 782d 666c 6163 2072 6174  audio/x-flac rat
+0000ca80: 653d 2564 2220 2520 7365 6c66 2e72 6174  e=%d" % self.rat
+0000ca90: 657d 0d0a 0d0a 2020 2020 2020 2020 2020  e}....          
+0000caa0: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
+0000cab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cac0: 7265 7370 203d 2072 6571 7565 7374 732e  resp = requests.
+0000cad0: 706f 7374 2875 726c 2c20 6461 7461 3d64  post(url, data=d
+0000cae0: 6174 612c 2068 6561 6465 7273 3d68 6561  ata, headers=hea
+0000caf0: 6465 7273 2c20 7469 6d65 6f75 743d 7365  ders, timeout=se
+0000cb00: 6c66 2e74 696d 656f 7574 290d 0a20 2020  lf.timeout)..   
+0000cb10: 2020 2020 2020 2020 2020 2020 2065 7863               exc
+0000cb20: 6570 7420 7265 7175 6573 7473 2e65 7863  ept requests.exc
+0000cb30: 6570 7469 6f6e 732e 436f 6e6e 6563 7469  eptions.Connecti
+0000cb40: 6f6e 4572 726f 723a 0d0a 2020 2020 2020  onError:..      
+0000cb50: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+0000cb60: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+0000cb70: 2020 2020 2020 2020 2020 2020 7265 7370              resp
+0000cb80: 203d 2068 7474 7078 2e70 6f73 7428 7572   = httpx.post(ur
+0000cb90: 6c2c 2064 6174 613d 6461 7461 2c20 6865  l, data=data, he
+0000cba0: 6164 6572 733d 6865 6164 6572 732c 2074  aders=headers, t
+0000cbb0: 696d 656f 7574 3d73 656c 662e 7469 6d65  imeout=self.time
+0000cbc0: 6f75 7429 0d0a 2020 2020 2020 2020 2020  out)..          
+0000cbd0: 2020 2020 2020 2020 2020 6578 6365 7074            except
+0000cbe0: 2068 7474 7078 2e65 7863 6570 7469 6f6e   httpx.exception
+0000cbf0: 732e 4e65 7477 6f72 6b45 7272 6f72 3a0d  s.NetworkError:.
+0000cc00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cc10: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+0000cc20: 650d 0a0d 0a20 2020 2020 2020 2020 2020  e....           
+0000cc30: 2020 2020 2066 6f72 206c 696e 6520 696e       for line in
+0000cc40: 2072 6573 702e 636f 6e74 656e 742e 6465   resp.content.de
+0000cc50: 636f 6465 2827 7574 662d 3827 292e 7370  code('utf-8').sp
+0000cc60: 6c69 7428 225c 6e22 293a 0d0a 2020 2020  lit("\n"):..    
+0000cc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc80: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
+0000cc90: 2020 2020 2020 2020 2020 2020 2020 6c69                li
+0000cca0: 6e65 203d 206a 736f 6e2e 6c6f 6164 7328  ne = json.loads(
+0000ccb0: 6c69 6e65 290d 0a20 2020 2020 2020 2020  line)..         
+0000ccc0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000ccd0: 696e 6520 3d20 6c69 6e65 5b27 7265 7375  ine = line['resu
+0000cce0: 6c74 275d 5b30 5d5b 2761 6c74 6572 6e61  lt'][0]['alterna
+0000ccf0: 7469 7665 275d 5b30 5d5b 2774 7261 6e73  tive'][0]['trans
+0000cd00: 6372 6970 7427 5d0d 0a20 2020 2020 2020  cript']..       
+0000cd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd20: 2072 6574 7572 6e20 6c69 6e65 5b3a 315d   return line[:1]
+0000cd30: 2e75 7070 6572 2829 202b 206c 696e 655b  .upper() + line[
+0000cd40: 313a 5d0d 0a20 2020 2020 2020 2020 2020  1:]..           
+0000cd50: 2020 2020 2020 2020 2065 7863 6570 743a           except:
+0000cd60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000cd70: 2020 2020 2020 2020 2020 2320 6e6f 2072            # no r
+0000cd80: 6573 756c 740d 0a20 2020 2020 2020 2020  esult..         
+0000cd90: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000cda0: 6f6e 7469 6e75 650d 0a0d 0a20 2020 2020  ontinue....     
+0000cdb0: 2020 2065 7863 6570 7420 4b65 7962 6f61     except Keyboa
+0000cdc0: 7264 496e 7465 7272 7570 743a 0d0a 2020  rdInterrupt:..  
+0000cdd0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000cde0: 662e 6572 726f 725f 6d65 7373 6167 6573  f.error_messages
+0000cdf0: 5f63 616c 6c62 6163 6b3a 0d0a 2020 2020  _callback:..    
+0000ce00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ce10: 2e65 7272 6f72 5f6d 6573 7361 6765 735f  .error_messages_
+0000ce20: 6361 6c6c 6261 636b 2822 4361 6e63 656c  callback("Cancel
+0000ce30: 6c69 6e67 2061 6c6c 2074 6173 6b73 2229  ling all tasks")
+0000ce40: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+0000ce50: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+0000ce60: 2020 2020 2070 7269 6e74 2822 4361 6e63       print("Canc
+0000ce70: 656c 6c69 6e67 2061 6c6c 2074 6173 6b73  elling all tasks
+0000ce80: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+0000ce90: 7265 7475 726e 0d0a 0d0a 2020 2020 2020  return....      
+0000cea0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+0000ceb0: 6f6e 2061 7320 653a 0d0a 2020 2020 2020  on as e:..      
+0000cec0: 2020 2020 2020 6966 2073 656c 662e 6572        if self.er
+0000ced0: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
+0000cee0: 6c62 6163 6b3a 0d0a 2020 2020 2020 2020  lback:..        
+0000cef0: 2020 2020 2020 2020 7365 6c66 2e65 7272          self.err
+0000cf00: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
+0000cf10: 6261 636b 2865 290d 0a20 2020 2020 2020  back(e)..       
+0000cf20: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+0000cf30: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0000cf40: 7428 6529 0d0a 2020 2020 2020 2020 2020  t(e)..          
+0000cf50: 2020 7265 7475 726e 0d0a 0d0a 0d0a 636c    return......cl
+0000cf60: 6173 7320 5768 6973 7065 7252 6563 6f67  ass WhisperRecog
+0000cf70: 6e69 7a65 7228 6f62 6a65 6374 293a 0d0a  nizer(object):..
+0000cf80: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0000cf90: 2873 656c 662c 206d 6f64 656c 3d22 736d  (self, model="sm
+0000cfa0: 616c 6c22 2c20 6c61 6e67 7561 6765 3d22  all", language="
+0000cfb0: 656e 222c 2066 7031 363d 4661 6c73 652c  en", fp16=False,
+0000cfc0: 2074 6173 6b3d 2274 7261 6e73 6372 6962   task="transcrib
+0000cfd0: 6522 2c20 7665 7262 6f73 653d 4661 6c73  e", verbose=Fals
+0000cfe0: 652c 2065 7272 6f72 5f6d 6573 7361 6765  e, error_message
+0000cff0: 735f 6361 6c6c 6261 636b 3d4e 6f6e 6529  s_callback=None)
+0000d000: 3a0d 0a20 2020 2020 2020 2073 656c 662e  :..        self.
+0000d010: 6d6f 6465 6c20 3d20 6d6f 6465 6c0d 0a20  model = model.. 
+0000d020: 2020 2020 2020 2073 656c 662e 6c61 6e67         self.lang
+0000d030: 7561 6765 203d 206c 616e 6775 6167 650d  uage = language.
+0000d040: 0a20 2020 2020 2020 2073 656c 662e 6670  .        self.fp
+0000d050: 3136 203d 2066 7031 360d 0a20 2020 2020  16 = fp16..     
+0000d060: 2020 2073 656c 662e 7461 736b 203d 2074     self.task = t
+0000d070: 6173 6b0d 0a20 2020 2020 2020 2073 656c  ask..        sel
+0000d080: 662e 7665 7262 6f73 6520 3d20 7665 7262  f.verbose = verb
+0000d090: 6f73 650d 0a20 2020 2020 2020 2073 656c  ose..        sel
+0000d0a0: 662e 6572 726f 725f 6d65 7373 6167 6573  f.error_messages
+0000d0b0: 5f63 616c 6c62 6163 6b20 3d20 6572 726f  _callback = erro
+0000d0c0: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
+0000d0d0: 6163 6b0d 0a0d 0a20 2020 2064 6566 205f  ack....    def _
+0000d0e0: 5f63 616c 6c5f 5f28 7365 6c66 2c20 6175  _call__(self, au
+0000d0f0: 6469 6f5f 7061 7468 293a 0d0a 2020 2020  dio_path):..    
+0000d100: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+0000d110: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
+0000d120: 656c 662e 6d6f 6465 6c2e 7472 616e 7363  elf.model.transc
+0000d130: 7269 6265 2861 7564 696f 5f70 6174 682c  ribe(audio_path,
+0000d140: 206c 616e 6775 6167 653d 7365 6c66 2e6c   language=self.l
+0000d150: 616e 6775 6167 652c 2066 7031 363d 7365  anguage, fp16=se
+0000d160: 6c66 2e66 7031 362c 2074 6173 6b3d 7365  lf.fp16, task=se
+0000d170: 6c66 2e74 6173 6b2c 2076 6572 626f 7365  lf.task, verbose
+0000d180: 3d73 656c 662e 7665 7262 6f73 6529 0d0a  =self.verbose)..
+0000d190: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000d1a0: 726e 2072 6573 756c 740d 0a0d 0a20 2020  rn result....   
+0000d1b0: 2020 2020 2065 7863 6570 7420 4b65 7962       except Keyb
+0000d1c0: 6f61 7264 496e 7465 7272 7570 743a 0d0a  oardInterrupt:..
+0000d1d0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000d1e0: 656c 662e 6572 726f 725f 6d65 7373 6167  elf.error_messag
+0000d1f0: 6573 5f63 616c 6c62 6163 6b3a 0d0a 2020  es_callback:..  
+0000d200: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000d210: 6c66 2e65 7272 6f72 5f6d 6573 7361 6765  lf.error_message
+0000d220: 735f 6361 6c6c 6261 636b 2822 4361 6e63  s_callback("Canc
+0000d230: 656c 6c69 6e67 2061 6c6c 2074 6173 6b73  elling all tasks
+0000d240: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+0000d250: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+0000d260: 2020 2020 2020 2070 7269 6e74 2822 4361         print("Ca
+0000d270: 6e63 656c 6c69 6e67 2061 6c6c 2074 6173  ncelling all tas
+0000d280: 6b73 2229 0d0a 2020 2020 2020 2020 2020  ks")..          
+0000d290: 2020 7265 7475 726e 0d0a 0d0a 2020 2020    return....    
+0000d2a0: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
+0000d2b0: 7469 6f6e 2061 7320 653a 0d0a 2020 2020  tion as e:..    
+0000d2c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000d2d0: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
+0000d2e0: 616c 6c62 6163 6b3a 0d0a 2020 2020 2020  allback:..      
+0000d2f0: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
+0000d300: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
+0000d310: 6c6c 6261 636b 2865 290d 0a20 2020 2020  llback(e)..     
+0000d320: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+0000d330: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+0000d340: 696e 7428 6529 0d0a 2020 2020 2020 2020  int(e)..        
+0000d350: 2020 2020 7265 7475 726e 0d0a 0d0a 0d0a      return......
+0000d360: 636c 6173 7320 5365 6e74 656e 6365 5472  class SentenceTr
+0000d370: 616e 736c 6174 6f72 286f 626a 6563 7429  anslator(object)
+0000d380: 3a0d 0a20 2020 2064 6566 205f 5f69 6e69  :..    def __ini
+0000d390: 745f 5f28 7365 6c66 2c20 7372 632c 2064  t__(self, src, d
+0000d3a0: 7374 2c20 7061 7469 656e 6365 3d2d 312c  st, patience=-1,
+0000d3b0: 2074 696d 656f 7574 3d33 302c 2065 7272   timeout=30, err
+0000d3c0: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
+0000d3d0: 6261 636b 3d4e 6f6e 6529 3a0d 0a20 2020  back=None):..   
+0000d3e0: 2020 2020 2073 656c 662e 7372 6320 3d20       self.src = 
+0000d3f0: 7372 630d 0a20 2020 2020 2020 2073 656c  src..        sel
+0000d400: 662e 6473 7420 3d20 6473 740d 0a20 2020  f.dst = dst..   
+0000d410: 2020 2020 2073 656c 662e 7061 7469 656e       self.patien
+0000d420: 6365 203d 2070 6174 6965 6e63 650d 0a20  ce = patience.. 
+0000d430: 2020 2020 2020 2073 656c 662e 7469 6d65         self.time
+0000d440: 6f75 7420 3d20 7469 6d65 6f75 740d 0a20  out = timeout.. 
+0000d450: 2020 2020 2020 2073 656c 662e 6572 726f         self.erro
+0000d460: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
+0000d470: 6163 6b20 3d20 6572 726f 725f 6d65 7373  ack = error_mess
+0000d480: 6167 6573 5f63 616c 6c62 6163 6b0d 0a0d  ages_callback...
+0000d490: 0a20 2020 2064 6566 205f 5f63 616c 6c5f  .    def __call_
+0000d4a0: 5f28 7365 6c66 2c20 7365 6e74 656e 6365  _(self, sentence
+0000d4b0: 293a 0d0a 2020 2020 2020 2020 7472 793a  ):..        try:
+0000d4c0: 0d0a 2020 2020 2020 2020 2020 2020 7472  ..            tr
+0000d4d0: 616e 736c 6174 6564 5f73 656e 7465 6e63  anslated_sentenc
+0000d4e0: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
+0000d4f0: 2020 2020 2320 6861 6e64 6c65 2074 6865      # handle the
+0000d500: 2073 7065 6369 616c 2063 6173 653a 2065   special case: e
+0000d510: 6d70 7479 2073 7472 696e 672e 0d0a 2020  mpty string...  
+0000d520: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+0000d530: 2073 656e 7465 6e63 653a 0d0a 2020 2020   sentence:..    
+0000d540: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000d550: 726e 204e 6f6e 650d 0a20 2020 2020 2020  rn None..       
+0000d560: 2020 2020 2074 7261 6e73 6c61 7465 645f       translated_
+0000d570: 7365 6e74 656e 6365 203d 2073 656c 662e  sentence = self.
+0000d580: 476f 6f67 6c65 5472 616e 736c 6174 6528  GoogleTranslate(
+0000d590: 7365 6e74 656e 6365 2c20 7372 633d 7365  sentence, src=se
+0000d5a0: 6c66 2e73 7263 2c20 6473 743d 7365 6c66  lf.src, dst=self
+0000d5b0: 2e64 7374 2c20 7469 6d65 6f75 743d 7365  .dst, timeout=se
+0000d5c0: 6c66 2e74 696d 656f 7574 290d 0a20 2020  lf.timeout)..   
+0000d5d0: 2020 2020 2020 2020 2066 6169 6c5f 746f           fail_to
+0000d5e0: 5f74 7261 6e73 6c61 7465 203d 2074 7261  _translate = tra
+0000d5f0: 6e73 6c61 7465 645f 7365 6e74 656e 6365  nslated_sentence
+0000d600: 5b2d 315d 203d 3d20 275c 6e27 0d0a 2020  [-1] == '\n'..  
+0000d610: 2020 2020 2020 2020 2020 7768 696c 6520            while 
+0000d620: 6661 696c 5f74 6f5f 7472 616e 736c 6174  fail_to_translat
+0000d630: 6520 616e 6420 7061 7469 656e 6365 3a0d  e and patience:.
+0000d640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d650: 2074 7261 6e73 6c61 7465 645f 7365 6e74   translated_sent
+0000d660: 656e 6365 203d 2073 656c 662e 476f 6f67  ence = self.Goog
+0000d670: 6c65 5472 616e 736c 6174 6528 7472 616e  leTranslate(tran
+0000d680: 736c 6174 6564 5f73 656e 7465 6e63 652c  slated_sentence,
+0000d690: 2073 7263 3d73 656c 662e 7372 632c 2064   src=self.src, d
+0000d6a0: 7374 3d73 656c 662e 6473 742c 2074 696d  st=self.dst, tim
+0000d6b0: 656f 7574 3d73 656c 662e 7469 6d65 6f75  eout=self.timeou
+0000d6c0: 7429 2e74 6578 740d 0a20 2020 2020 2020  t).text..       
+0000d6d0: 2020 2020 2020 2020 2069 6620 7472 616e           if tran
+0000d6e0: 736c 6174 6564 5f73 656e 7465 6e63 655b  slated_sentence[
+0000d6f0: 2d31 5d20 3d3d 2027 5c6e 273a 0d0a 2020  -1] == '\n':..  
+0000d700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d710: 2020 6966 2070 6174 6965 6e63 6520 3d3d    if patience ==
+0000d720: 202d 313a 0d0a 2020 2020 2020 2020 2020   -1:..          
+0000d730: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0000d740: 6e74 696e 7565 0d0a 2020 2020 2020 2020  ntinue..        
+0000d750: 2020 2020 2020 2020 2020 2020 7061 7469              pati
+0000d760: 656e 6365 202d 3d20 310d 0a20 2020 2020  ence -= 1..     
+0000d770: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000d780: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000d790: 2020 2020 2020 6661 696c 5f74 6f5f 7472        fail_to_tr
+0000d7a0: 616e 736c 6174 6520 3d20 4661 6c73 650d  anslate = False.
+0000d7b0: 0a0d 0a20 2020 2020 2020 2020 2020 2072  ...            r
+0000d7c0: 6574 7572 6e20 7472 616e 736c 6174 6564  eturn translated
+0000d7d0: 5f73 656e 7465 6e63 650d 0a0d 0a20 2020  _sentence....   
+0000d7e0: 2020 2020 2065 7863 6570 7420 4b65 7962       except Keyb
+0000d7f0: 6f61 7264 496e 7465 7272 7570 743a 0d0a  oardInterrupt:..
+0000d800: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000d810: 656c 662e 6572 726f 725f 6d65 7373 6167  elf.error_messag
+0000d820: 6573 5f63 616c 6c62 6163 6b3a 0d0a 2020  es_callback:..  
+0000d830: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000d840: 6c66 2e65 7272 6f72 5f6d 6573 7361 6765  lf.error_message
+0000d850: 735f 6361 6c6c 6261 636b 2822 4361 6e63  s_callback("Canc
+0000d860: 656c 6c69 6e67 2061 6c6c 2074 6173 6b73  elling all tasks
+0000d870: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+0000d880: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+0000d890: 2020 2020 2020 2070 7269 6e74 2822 4361         print("Ca
+0000d8a0: 6e63 656c 6c69 6e67 2061 6c6c 2074 6173  ncelling all tas
+0000d8b0: 6b73 2229 0d0a 2020 2020 2020 2020 2020  ks")..          
+0000d8c0: 2020 7265 7475 726e 0d0a 0d0a 2020 2020    return....    
+0000d8d0: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
+0000d8e0: 7469 6f6e 2061 7320 653a 0d0a 2020 2020  tion as e:..    
+0000d8f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000d900: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
+0000d910: 616c 6c62 6163 6b3a 0d0a 2020 2020 2020  allback:..      
+0000d920: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
+0000d930: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
+0000d940: 6c6c 6261 636b 2865 290d 0a20 2020 2020  llback(e)..     
+0000d950: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+0000d960: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+0000d970: 696e 7428 6529 0d0a 2020 2020 2020 2020  int(e)..        
+0000d980: 2020 2020 7265 7475 726e 0d0a 0d0a 2020      return....  
+0000d990: 2020 6465 6620 476f 6f67 6c65 5472 616e    def GoogleTran
+0000d9a0: 736c 6174 6528 7365 6c66 2c20 7465 7874  slate(self, text
+0000d9b0: 2c20 7372 632c 2064 7374 2c20 7469 6d65  , src, dst, time
+0000d9c0: 6f75 743d 3330 293a 0d0a 2020 2020 2020  out=30):..      
+0000d9d0: 2020 7572 6c20 3d20 2768 7474 7073 3a2f    url = 'https:/
+0000d9e0: 2f74 7261 6e73 6c61 7465 2e67 6f6f 676c  /translate.googl
+0000d9f0: 6561 7069 732e 636f 6d2f 7472 616e 736c  eapis.com/transl
+0000da00: 6174 655f 612f 270d 0a20 2020 2020 2020  ate_a/'..       
+0000da10: 2070 6172 616d 7320 3d20 2773 696e 676c   params = 'singl
+0000da20: 653f 636c 6965 6e74 3d67 7478 2673 6c3d  e?client=gtx&sl=
+0000da30: 272b 7372 632b 2726 746c 3d27 2b64 7374  '+src+'&tl='+dst
+0000da40: 2b27 2664 743d 7426 713d 272b 7465 7874  +'&dt=t&q='+text
+0000da50: 3b0d 0a20 2020 2020 2020 2068 6561 6465  ;..        heade
+0000da60: 7273 203d 207b 2755 7365 722d 4167 656e  rs = {'User-Agen
+0000da70: 7427 3a20 274d 6f7a 696c 6c61 2f35 2e30  t': 'Mozilla/5.0
+0000da80: 2028 5769 6e64 6f77 7320 4e54 2031 302e   (Windows NT 10.
+0000da90: 303b 2057 696e 3634 3b20 7836 3429 272c  0; Win64; x64)',
+0000daa0: 2027 5265 6665 7265 7227 3a20 2768 7474   'Referer': 'htt
+0000dab0: 7073 3a2f 2f74 7261 6e73 6c61 7465 2e67  ps://translate.g
+0000dac0: 6f6f 676c 652e 636f 6d27 2c7d 0d0a 0d0a  oogle.com',}....
+0000dad0: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+0000dae0: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
+0000daf0: 7365 203d 2072 6571 7565 7374 732e 6765  se = requests.ge
+0000db00: 7428 7572 6c2b 7061 7261 6d73 2c20 6865  t(url+params, he
+0000db10: 6164 6572 733d 6865 6164 6572 732c 2074  aders=headers, t
+0000db20: 696d 656f 7574 3d73 656c 662e 7469 6d65  imeout=self.time
+0000db30: 6f75 7429 0d0a 2020 2020 2020 2020 2020  out)..          
+0000db40: 2020 6966 2072 6573 706f 6e73 652e 7374    if response.st
+0000db50: 6174 7573 5f63 6f64 6520 3d3d 2032 3030  atus_code == 200
+0000db60: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000db70: 2020 2072 6573 706f 6e73 655f 6a73 6f6e     response_json
+0000db80: 203d 2072 6573 706f 6e73 652e 6a73 6f6e   = response.json
+0000db90: 2829 5b30 5d0d 0a20 2020 2020 2020 2020  ()[0]..         
+0000dba0: 2020 2020 2020 206c 656e 6774 6820 3d20         length = 
+0000dbb0: 6c65 6e28 7265 7370 6f6e 7365 5f6a 736f  len(response_jso
+0000dbc0: 6e29 0d0a 2020 2020 2020 2020 2020 2020  n)..            
+0000dbd0: 2020 2020 7472 616e 736c 6174 696f 6e20      translation 
+0000dbe0: 3d20 2222 0d0a 2020 2020 2020 2020 2020  = ""..          
+0000dbf0: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+0000dc00: 616e 6765 286c 656e 6774 6829 3a0d 0a20  ange(length):.. 
+0000dc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc20: 2020 2074 7261 6e73 6c61 7469 6f6e 203d     translation =
+0000dc30: 2074 7261 6e73 6c61 7469 6f6e 202b 2072   translation + r
+0000dc40: 6573 706f 6e73 655f 6a73 6f6e 5b69 5d5b  esponse_json[i][
+0000dc50: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
+0000dc60: 2020 2020 7265 7475 726e 2074 7261 6e73      return trans
+0000dc70: 6c61 7469 6f6e 0d0a 2020 2020 2020 2020  lation..        
+0000dc80: 2020 2020 7265 7475 726e 0d0a 0d0a 2020      return....  
+0000dc90: 2020 2020 2020 6578 6365 7074 2072 6571        except req
+0000dca0: 7565 7374 732e 6578 6365 7074 696f 6e73  uests.exceptions
+0000dcb0: 2e43 6f6e 6e65 6374 696f 6e45 7272 6f72  .ConnectionError
+0000dcc0: 3a0d 0a20 2020 2020 2020 2020 2020 2077  :..            w
+0000dcd0: 6974 6820 6874 7470 782e 436c 6965 6e74  ith httpx.Client
+0000dce0: 2829 2061 7320 636c 6965 6e74 3a0d 0a20  () as client:.. 
+0000dcf0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000dd00: 6573 706f 6e73 6520 3d20 636c 6965 6e74  esponse = client
+0000dd10: 2e67 6574 2875 726c 2b70 6172 616d 732c  .get(url+params,
+0000dd20: 2068 6561 6465 7273 3d68 6561 6465 7273   headers=headers
+0000dd30: 2c20 7469 6d65 6f75 743d 7365 6c66 2e74  , timeout=self.t
+0000dd40: 696d 656f 7574 290d 0a20 2020 2020 2020  imeout)..       
+0000dd50: 2020 2020 2020 2020 2069 6620 7265 7370           if resp
+0000dd60: 6f6e 7365 2e73 7461 7475 735f 636f 6465  onse.status_code
+0000dd70: 203d 3d20 3230 303a 0d0a 2020 2020 2020   == 200:..      
+0000dd80: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000dd90: 7370 6f6e 7365 5f6a 736f 6e20 3d20 7265  sponse_json = re
+0000dda0: 7370 6f6e 7365 2e6a 736f 6e28 295b 305d  sponse.json()[0]
+0000ddb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000ddc0: 2020 2020 2020 6c65 6e67 7468 203d 206c        length = l
+0000ddd0: 656e 2872 6573 706f 6e73 655f 6a73 6f6e  en(response_json
+0000dde0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000ddf0: 2020 2020 2020 2074 7261 6e73 6c61 7469         translati
+0000de00: 6f6e 203d 2022 220d 0a20 2020 2020 2020  on = ""..       
+0000de10: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000de20: 2069 2069 6e20 7261 6e67 6528 6c65 6e67   i in range(leng
+0000de30: 7468 293a 0d0a 2020 2020 2020 2020 2020  th):..          
+0000de40: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+0000de50: 616e 736c 6174 696f 6e20 3d20 7472 616e  anslation = tran
+0000de60: 736c 6174 696f 6e20 2b20 7265 7370 6f6e  slation + respon
+0000de70: 7365 5f6a 736f 6e5b 695d 5b30 5d0d 0a20  se_json[i][0].. 
+0000de80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de90: 2020 2072 6574 7572 6e20 7472 616e 736c     return transl
+0000dea0: 6174 696f 6e0d 0a20 2020 2020 2020 2020  ation..         
+0000deb0: 2020 2020 2020 2072 6574 7572 6e0d 0a0d         return...
+0000dec0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+0000ded0: 4b65 7962 6f61 7264 496e 7465 7272 7570  KeyboardInterrup
+0000dee0: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
+0000def0: 6966 2073 656c 662e 6572 726f 725f 6d65  if self.error_me
+0000df00: 7373 6167 6573 5f63 616c 6c62 6163 6b3a  ssages_callback:
+0000df10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000df20: 2020 7365 6c66 2e65 7272 6f72 5f6d 6573    self.error_mes
+0000df30: 7361 6765 735f 6361 6c6c 6261 636b 2822  sages_callback("
+0000df40: 4361 6e63 656c 6c69 6e67 2061 6c6c 2074  Cancelling all t
+0000df50: 6173 6b73 2229 0d0a 2020 2020 2020 2020  asks")..        
+0000df60: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+0000df70: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0000df80: 2822 4361 6e63 656c 6c69 6e67 2061 6c6c  ("Cancelling all
+0000df90: 2074 6173 6b73 2229 0d0a 2020 2020 2020   tasks")..      
+0000dfa0: 2020 2020 2020 7265 7475 726e 0d0a 0d0a        return....
+0000dfb0: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+0000dfc0: 7863 6570 7469 6f6e 2061 7320 653a 0d0a  xception as e:..
+0000dfd0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000dfe0: 656c 662e 6572 726f 725f 6d65 7373 6167  elf.error_messag
+0000dff0: 6573 5f63 616c 6c62 6163 6b3a 0d0a 2020  es_callback:..  
+0000e000: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000e010: 6c66 2e65 7272 6f72 5f6d 6573 7361 6765  lf.error_message
+0000e020: 735f 6361 6c6c 6261 636b 2865 290d 0a20  s_callback(e).. 
+0000e030: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000e040: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e050: 2020 7072 696e 7428 6529 0d0a 2020 2020    print(e)..    
+0000e060: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
+0000e070: 0d0a 0d0a 636c 6173 7320 5375 6274 6974  ....class Subtit
+0000e080: 6c65 466f 726d 6174 7465 723a 0d0a 2020  leFormatter:..  
+0000e090: 2020 7375 7070 6f72 7465 645f 666f 726d    supported_form
+0000e0a0: 6174 7320 3d20 5b27 7372 7427 2c20 2776  ats = ['srt', 'v
+0000e0b0: 7474 272c 2027 6a73 6f6e 272c 2027 7261  tt', 'json', 'ra
+0000e0c0: 7727 5d0d 0a0d 0a20 2020 2064 6566 205f  w']....    def _
+0000e0d0: 5f69 6e69 745f 5f28 7365 6c66 2c20 666f  _init__(self, fo
+0000e0e0: 726d 6174 5f74 7970 652c 2065 7272 6f72  rmat_type, error
+0000e0f0: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
+0000e100: 636b 3d4e 6f6e 6529 3a0d 0a20 2020 2020  ck=None):..     
+0000e110: 2020 2073 656c 662e 666f 726d 6174 5f74     self.format_t
+0000e120: 7970 6520 3d20 666f 726d 6174 5f74 7970  ype = format_typ
+0000e130: 652e 6c6f 7765 7228 290d 0a20 2020 2020  e.lower()..     
+0000e140: 2020 2073 656c 662e 6572 726f 725f 6d65     self.error_me
+0000e150: 7373 6167 6573 5f63 616c 6c62 6163 6b20  ssages_callback 
+0000e160: 3d20 6572 726f 725f 6d65 7373 6167 6573  = error_messages
+0000e170: 5f63 616c 6c62 6163 6b0d 0a20 2020 2020  _callback..     
+0000e180: 2020 200d 0a20 2020 2064 6566 205f 5f63     ..    def __c
+0000e190: 616c 6c5f 5f28 7365 6c66 2c20 7375 6274  all__(self, subt
+0000e1a0: 6974 6c65 732c 2070 6164 6469 6e67 5f62  itles, padding_b
+0000e1b0: 6566 6f72 653d 302c 2070 6164 6469 6e67  efore=0, padding
+0000e1c0: 5f61 6674 6572 3d30 293a 0d0a 2020 2020  _after=0):..    
+0000e1d0: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+0000e1e0: 2020 2020 2020 6966 2073 656c 662e 666f        if self.fo
+0000e1f0: 726d 6174 5f74 7970 6520 3d3d 2027 7372  rmat_type == 'sr
+0000e200: 7427 3a0d 0a20 2020 2020 2020 2020 2020  t':..           
+0000e210: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000e220: 2e73 7274 5f66 6f72 6d61 7474 6572 2873  .srt_formatter(s
+0000e230: 7562 7469 746c 6573 2c20 7061 6464 696e  ubtitles, paddin
+0000e240: 675f 6265 666f 7265 2c20 7061 6464 696e  g_before, paddin
+0000e250: 675f 6166 7465 7229 0d0a 2020 2020 2020  g_after)..      
+0000e260: 2020 2020 2020 656c 6966 2073 656c 662e        elif self.
+0000e270: 666f 726d 6174 5f74 7970 6520 3d3d 2027  format_type == '
+0000e280: 7674 7427 3a0d 0a20 2020 2020 2020 2020  vtt':..         
+0000e290: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000e2a0: 6c66 2e76 7474 5f66 6f72 6d61 7474 6572  lf.vtt_formatter
+0000e2b0: 2873 7562 7469 746c 6573 2c20 7061 6464  (subtitles, padd
+0000e2c0: 696e 675f 6265 666f 7265 2c20 7061 6464  ing_before, padd
+0000e2d0: 696e 675f 6166 7465 7229 0d0a 2020 2020  ing_after)..    
+0000e2e0: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
+0000e2f0: 662e 666f 726d 6174 5f74 7970 6520 3d3d  f.format_type ==
+0000e300: 2027 6a73 6f6e 273a 0d0a 2020 2020 2020   'json':..      
+0000e310: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000e320: 2073 656c 662e 6a73 6f6e 5f66 6f72 6d61   self.json_forma
+0000e330: 7474 6572 2873 7562 7469 746c 6573 290d  tter(subtitles).
+0000e340: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+0000e350: 6620 7365 6c66 2e66 6f72 6d61 745f 7479  f self.format_ty
+0000e360: 7065 203d 3d20 2772 6177 273a 0d0a 2020  pe == 'raw':..  
+0000e370: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000e380: 7475 726e 2073 656c 662e 7261 775f 666f  turn self.raw_fo
+0000e390: 726d 6174 7465 7228 7375 6274 6974 6c65  rmatter(subtitle
+0000e3a0: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
+0000e3b0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+0000e3c0: 2020 2020 2020 2069 6620 6572 726f 725f         if error_
+0000e3d0: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
+0000e3e0: 6b3a 0d0a 2020 2020 2020 2020 2020 2020  k:..            
+0000e3f0: 2020 2020 2020 2020 6572 726f 725f 6d65          error_me
+0000e400: 7373 6167 6573 5f63 616c 6c62 6163 6b28  ssages_callback(
+0000e410: 6627 556e 7375 7070 6f72 7465 6420 666f  f'Unsupported fo
+0000e420: 726d 6174 2074 7970 653a 207b 7365 6c66  rmat type: {self
+0000e430: 2e66 6f72 6d61 745f 7479 7065 7d27 290d  .format_type}').
+0000e440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e450: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+0000e460: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000e470: 6520 5661 6c75 6545 7272 6f72 2866 2755  e ValueError(f'U
+0000e480: 6e73 7570 706f 7274 6564 2066 6f72 6d61  nsupported forma
+0000e490: 7420 7479 7065 3a20 7b73 656c 662e 666f  t type: {self.fo
+0000e4a0: 726d 6174 5f74 7970 657d 2729 0d0a 0d0a  rmat_type}')....
+0000e4b0: 2020 2020 2020 2020 6578 6365 7074 204b          except K
+0000e4c0: 6579 626f 6172 6449 6e74 6572 7275 7074  eyboardInterrupt
+0000e4d0: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
+0000e4e0: 6620 7365 6c66 2e65 7272 6f72 5f6d 6573  f self.error_mes
+0000e4f0: 7361 6765 735f 6361 6c6c 6261 636b 3a0d  sages_callback:.
+0000e500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e510: 2073 656c 662e 6572 726f 725f 6d65 7373   self.error_mess
+0000e520: 6167 6573 5f63 616c 6c62 6163 6b28 2243  ages_callback("C
+0000e530: 616e 6365 6c6c 696e 6720 616c 6c20 7461  ancelling all ta
+0000e540: 736b 7322 290d 0a20 2020 2020 2020 2020  sks")..         
+0000e550: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+0000e560: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+0000e570: 2243 616e 6365 6c6c 696e 6720 616c 6c20  "Cancelling all 
+0000e580: 7461 736b 7322 290d 0a20 2020 2020 2020  tasks")..       
+0000e590: 2020 2020 2072 6574 7572 6e0d 0a0d 0a20       return.... 
+0000e5a0: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+0000e5b0: 6365 7074 696f 6e20 6173 2065 3a0d 0a20  ception as e:.. 
+0000e5c0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000e5d0: 6c66 2e65 7272 6f72 5f6d 6573 7361 6765  lf.error_message
+0000e5e0: 735f 6361 6c6c 6261 636b 3a0d 0a20 2020  s_callback:..   
+0000e5f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000e600: 662e 6572 726f 725f 6d65 7373 6167 6573  f.error_messages
+0000e610: 5f63 616c 6c62 6163 6b28 6529 0d0a 2020  _callback(e)..  
+0000e620: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+0000e630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e640: 2070 7269 6e74 2865 290d 0a20 2020 2020   print(e)..     
+0000e650: 2020 2020 2020 2072 6574 7572 6e0d 0a0d         return...
+0000e660: 0a20 2020 2064 6566 2073 7274 5f66 6f72  .    def srt_for
+0000e670: 6d61 7474 6572 2873 656c 662c 2073 7562  matter(self, sub
+0000e680: 7469 746c 6573 2c20 7061 6464 696e 675f  titles, padding_
+0000e690: 6265 666f 7265 3d30 2c20 7061 6464 696e  before=0, paddin
+0000e6a0: 675f 6166 7465 723d 3029 3a0d 0a20 2020  g_after=0):..   
+0000e6b0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+0000e6c0: 2020 5365 7269 616c 697a 6520 6120 6c69    Serialize a li
+0000e6d0: 7374 206f 6620 7375 6274 6974 6c65 7320  st of subtitles 
+0000e6e0: 6163 636f 7264 696e 6720 746f 2074 6865  according to the
+0000e6f0: 2053 5254 2066 6f72 6d61 742c 2077 6974   SRT format, wit
+0000e700: 6820 6f70 7469 6f6e 616c 2074 696d 6520  h optional time 
+0000e710: 7061 6464 696e 672e 0d0a 2020 2020 2020  padding...      
+0000e720: 2020 2222 220d 0a20 2020 2020 2020 2073    """..        s
+0000e730: 7562 5f72 6970 5f66 696c 6520 3d20 7079  ub_rip_file = py
+0000e740: 7372 742e 5375 6252 6970 4669 6c65 2829  srt.SubRipFile()
+0000e750: 0d0a 2020 2020 2020 2020 666f 7220 692c  ..        for i,
+0000e760: 2028 2873 7461 7274 2c20 656e 6429 2c20   ((start, end), 
+0000e770: 7465 7874 2920 696e 2065 6e75 6d65 7261  text) in enumera
+0000e780: 7465 2873 7562 7469 746c 6573 2c20 7374  te(subtitles, st
+0000e790: 6172 743d 3129 3a0d 0a20 2020 2020 2020  art=1):..       
+0000e7a0: 2020 2020 2069 7465 6d20 3d20 7079 7372       item = pysr
+0000e7b0: 742e 5375 6252 6970 4974 656d 2829 0d0a  t.SubRipItem()..
+0000e7c0: 2020 2020 2020 2020 2020 2020 6974 656d              item
+0000e7d0: 2e69 6e64 6578 203d 2069 0d0a 2020 2020  .index = i..    
+0000e7e0: 2020 2020 2020 2020 6974 656d 2e74 6578          item.tex
+0000e7f0: 7420 3d20 7369 782e 7465 7874 5f74 7970  t = six.text_typ
+0000e800: 6528 7465 7874 290d 0a20 2020 2020 2020  e(text)..       
+0000e810: 2020 2020 2069 7465 6d2e 7374 6172 742e       item.start.
+0000e820: 7365 636f 6e64 7320 3d20 6d61 7828 302c  seconds = max(0,
+0000e830: 2073 7461 7274 202d 2070 6164 6469 6e67   start - padding
+0000e840: 5f62 6566 6f72 6529 0d0a 2020 2020 2020  _before)..      
+0000e850: 2020 2020 2020 6974 656d 2e65 6e64 2e73        item.end.s
+0000e860: 6563 6f6e 6473 203d 2065 6e64 202b 2070  econds = end + p
+0000e870: 6164 6469 6e67 5f61 6674 6572 0d0a 2020  adding_after..  
+0000e880: 2020 2020 2020 2020 2020 7375 625f 7269            sub_ri
+0000e890: 705f 6669 6c65 2e61 7070 656e 6428 6974  p_file.append(it
+0000e8a0: 656d 290d 0a20 2020 2020 2020 2072 6574  em)..        ret
+0000e8b0: 7572 6e20 275c 6e27 2e6a 6f69 6e28 7369  urn '\n'.join(si
+0000e8c0: 782e 7465 7874 5f74 7970 6528 6974 656d  x.text_type(item
+0000e8d0: 2920 666f 7220 6974 656d 2069 6e20 7375  ) for item in su
+0000e8e0: 625f 7269 705f 6669 6c65 290d 0a0d 0a20  b_rip_file).... 
+0000e8f0: 2020 2064 6566 2076 7474 5f66 6f72 6d61     def vtt_forma
+0000e900: 7474 6572 2873 656c 662c 2073 7562 7469  tter(self, subti
+0000e910: 746c 6573 2c20 7061 6464 696e 675f 6265  tles, padding_be
+0000e920: 666f 7265 3d30 2c20 7061 6464 696e 675f  fore=0, padding_
+0000e930: 6166 7465 723d 3029 3a0d 0a20 2020 2020  after=0):..     
+0000e940: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+0000e950: 5365 7269 616c 697a 6520 6120 6c69 7374  Serialize a list
+0000e960: 206f 6620 7375 6274 6974 6c65 7320 6163   of subtitles ac
+0000e970: 636f 7264 696e 6720 746f 2074 6865 2056  cording to the V
+0000e980: 5454 2066 6f72 6d61 742c 2077 6974 6820  TT format, with 
+0000e990: 6f70 7469 6f6e 616c 2074 696d 6520 7061  optional time pa
+0000e9a0: 6464 696e 672e 0d0a 2020 2020 2020 2020  dding...        
+0000e9b0: 2222 220d 0a20 2020 2020 2020 2074 6578  """..        tex
+0000e9c0: 7420 3d20 7365 6c66 2e73 7274 5f66 6f72  t = self.srt_for
+0000e9d0: 6d61 7474 6572 2873 7562 7469 746c 6573  matter(subtitles
+0000e9e0: 2c20 7061 6464 696e 675f 6265 666f 7265  , padding_before
+0000e9f0: 2c20 7061 6464 696e 675f 6166 7465 7229  , padding_after)
+0000ea00: 0d0a 2020 2020 2020 2020 7465 7874 203d  ..        text =
+0000ea10: 2027 5745 4256 5454 5c6e 5c6e 2720 2b20   'WEBVTT\n\n' + 
+0000ea20: 7465 7874 2e72 6570 6c61 6365 2827 2c27  text.replace(','
+0000ea30: 2c20 272e 2729 0d0a 2020 2020 2020 2020  , '.')..        
+0000ea40: 7265 7475 726e 2074 6578 740d 0a0d 0a20  return text.... 
+0000ea50: 2020 2064 6566 206a 736f 6e5f 666f 726d     def json_form
+0000ea60: 6174 7465 7228 7365 6c66 2c20 7375 6274  atter(self, subt
+0000ea70: 6974 6c65 7329 3a0d 0a20 2020 2020 2020  itles):..       
+0000ea80: 2022 2222 0d0a 2020 2020 2020 2020 5365   """..        Se
+0000ea90: 7269 616c 697a 6520 6120 6c69 7374 206f  rialize a list o
+0000eaa0: 6620 7375 6274 6974 6c65 7320 6173 2061  f subtitles as a
+0000eab0: 204a 534f 4e20 626c 6f62 2e0d 0a20 2020   JSON blob...   
+0000eac0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+0000ead0: 2020 7375 6274 6974 6c65 5f64 6963 7473    subtitle_dicts
+0000eae0: 203d 205b 0d0a 2020 2020 2020 2020 2020   = [..          
+0000eaf0: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
+0000eb00: 2020 2020 2027 7374 6172 7427 3a20 7374       'start': st
+0000eb10: 6172 742c 0d0a 2020 2020 2020 2020 2020  art,..          
+0000eb20: 2020 2020 2020 2765 6e64 273a 2065 6e64        'end': end
+0000eb30: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000eb40: 2020 2027 636f 6e74 656e 7427 3a20 7465     'content': te
+0000eb50: 7874 2c0d 0a20 2020 2020 2020 2020 2020  xt,..           
+0000eb60: 207d 0d0a 2020 2020 2020 2020 2020 2020   }..            
+0000eb70: 666f 7220 2828 7374 6172 742c 2065 6e64  for ((start, end
+0000eb80: 292c 2074 6578 7429 0d0a 2020 2020 2020  ), text)..      
+0000eb90: 2020 2020 2020 696e 2073 7562 7469 746c        in subtitl
+0000eba0: 6573 0d0a 2020 2020 2020 2020 5d0d 0a20  es..        ].. 
+0000ebb0: 2020 2020 2020 2072 6574 7572 6e20 6a73         return js
+0000ebc0: 6f6e 2e64 756d 7073 2873 7562 7469 746c  on.dumps(subtitl
+0000ebd0: 655f 6469 6374 7329 0d0a 0d0a 2020 2020  e_dicts)....    
+0000ebe0: 6465 6620 7261 775f 666f 726d 6174 7465  def raw_formatte
+0000ebf0: 7228 7365 6c66 2c20 7375 6274 6974 6c65  r(self, subtitle
+0000ec00: 7329 3a0d 0a20 2020 2020 2020 2022 2222  s):..        """
+0000ec10: 0d0a 2020 2020 2020 2020 5365 7269 616c  ..        Serial
+0000ec20: 697a 6520 6120 6c69 7374 206f 6620 7375  ize a list of su
+0000ec30: 6274 6974 6c65 7320 6173 2061 206e 6577  btitles as a new
+0000ec40: 6c69 6e65 2d64 656c 696d 6974 6564 2073  line-delimited s
+0000ec50: 7472 696e 672e 0d0a 2020 2020 2020 2020  tring...        
+0000ec60: 2222 220d 0a20 2020 2020 2020 2072 6574  """..        ret
+0000ec70: 7572 6e20 2720 272e 6a6f 696e 2874 6578  urn ' '.join(tex
+0000ec80: 7420 666f 7220 285f 726e 672c 2074 6578  t for (_rng, tex
+0000ec90: 7429 2069 6e20 7375 6274 6974 6c65 7329  t) in subtitles)
+0000eca0: 0d0a 0d0a 0d0a 636c 6173 7320 5375 6274  ......class Subt
+0000ecb0: 6974 6c65 5772 6974 6572 3a0d 0a20 2020  itleWriter:..   
+0000ecc0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+0000ecd0: 6c66 2c20 7265 6769 6f6e 732c 2074 7261  lf, regions, tra
+0000ece0: 6e73 6372 6970 7473 2c20 666f 726d 6174  nscripts, format
+0000ecf0: 2c20 6572 726f 725f 6d65 7373 6167 6573  , error_messages
+0000ed00: 5f63 616c 6c62 6163 6b3d 4e6f 6e65 293a  _callback=None):
+0000ed10: 0d0a 2020 2020 2020 2020 7365 6c66 2e72  ..        self.r
+0000ed20: 6567 696f 6e73 203d 2072 6567 696f 6e73  egions = regions
+0000ed30: 0d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
+0000ed40: 7261 6e73 6372 6970 7473 203d 2074 7261  ranscripts = tra
+0000ed50: 6e73 6372 6970 7473 0d0a 2020 2020 2020  nscripts..      
+0000ed60: 2020 7365 6c66 2e66 6f72 6d61 7420 3d20    self.format = 
+0000ed70: 666f 726d 6174 0d0a 2020 2020 2020 2020  format..        
+0000ed80: 7365 6c66 2e74 696d 6564 5f73 7562 7469  self.timed_subti
+0000ed90: 746c 6573 203d 205b 2872 2c20 7429 2066  tles = [(r, t) f
+0000eda0: 6f72 2072 2c20 7420 696e 207a 6970 2873  or r, t in zip(s
+0000edb0: 656c 662e 7265 6769 6f6e 732c 2073 656c  elf.regions, sel
+0000edc0: 662e 7472 616e 7363 7269 7074 7329 2069  f.transcripts) i
+0000edd0: 6620 745d 0d0a 2020 2020 2020 2020 7365  f t]..        se
+0000ede0: 6c66 2e65 7272 6f72 5f6d 6573 7361 6765  lf.error_message
+0000edf0: 735f 6361 6c6c 6261 636b 203d 2065 7272  s_callback = err
+0000ee00: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
+0000ee10: 6261 636b 0d0a 0d0a 2020 2020 6465 6620  back....    def 
+0000ee20: 6765 745f 7469 6d65 645f 7375 6274 6974  get_timed_subtit
+0000ee30: 6c65 7328 7365 6c66 293a 0d0a 2020 2020  les(self):..    
+0000ee40: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0000ee50: 7469 6d65 645f 7375 6274 6974 6c65 730d  timed_subtitles.
+0000ee60: 0a0d 0a20 2020 2064 6566 2077 7269 7465  ...    def write
+0000ee70: 2873 656c 662c 2064 6563 6c61 7265 645f  (self, declared_
+0000ee80: 7375 6274 6974 6c65 5f66 696c 6570 6174  subtitle_filepat
+0000ee90: 6829 3a0d 0a20 2020 2020 2020 2074 7279  h):..        try
+0000eea0: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
+0000eeb0: 6f72 6d61 7474 6572 203d 2053 7562 7469  ormatter = Subti
+0000eec0: 746c 6546 6f72 6d61 7474 6572 2873 656c  tleFormatter(sel
+0000eed0: 662e 666f 726d 6174 290d 0a20 2020 2020  f.format)..     
+0000eee0: 2020 2020 2020 2066 6f72 6d61 7474 6564         formatted
+0000eef0: 5f73 7562 7469 746c 6573 203d 2066 6f72  _subtitles = for
+0000ef00: 6d61 7474 6572 2873 656c 662e 7469 6d65  matter(self.time
+0000ef10: 645f 7375 6274 6974 6c65 7329 0d0a 2020  d_subtitles)..  
+0000ef20: 2020 2020 2020 2020 2020 7361 7665 645f            saved_
+0000ef30: 7375 6274 6974 6c65 5f66 696c 6570 6174  subtitle_filepat
+0000ef40: 6820 3d20 6465 636c 6172 6564 5f73 7562  h = declared_sub
+0000ef50: 7469 746c 655f 6669 6c65 7061 7468 0d0a  title_filepath..
+0000ef60: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000ef70: 6176 6564 5f73 7562 7469 746c 655f 6669  aved_subtitle_fi
+0000ef80: 6c65 7061 7468 3a0d 0a20 2020 2020 2020  lepath:..       
+0000ef90: 2020 2020 2020 2020 2073 7562 7469 746c           subtitl
+0000efa0: 655f 6669 6c65 5f62 6173 652c 2073 7562  e_file_base, sub
+0000efb0: 7469 746c 655f 6669 6c65 5f65 7874 203d  title_file_ext =
+0000efc0: 206f 732e 7061 7468 2e73 706c 6974 6578   os.path.splitex
+0000efd0: 7428 7361 7665 645f 7375 6274 6974 6c65  t(saved_subtitle
+0000efe0: 5f66 696c 6570 6174 6829 0d0a 2020 2020  _filepath)..    
+0000eff0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0000f000: 6f74 2073 7562 7469 746c 655f 6669 6c65  ot subtitle_file
+0000f010: 5f65 7874 3a0d 0a20 2020 2020 2020 2020  _ext:..         
+0000f020: 2020 2020 2020 2020 2020 2073 6176 6564             saved
+0000f030: 5f73 7562 7469 746c 655f 6669 6c65 7061  _subtitle_filepa
+0000f040: 7468 203d 2022 7b62 6173 657d 2e7b 666f  th = "{base}.{fo
+0000f050: 726d 6174 7d22 2e66 6f72 6d61 7428 6261  rmat}".format(ba
+0000f060: 7365 3d73 7562 7469 746c 655f 6669 6c65  se=subtitle_file
+0000f070: 5f62 6173 652c 2066 6f72 6d61 743d 7365  _base, format=se
+0000f080: 6c66 2e66 6f72 6d61 7429 0d0a 2020 2020  lf.format)..    
+0000f090: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0000f0a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000f0b0: 2020 2020 2020 2073 6176 6564 5f73 7562         saved_sub
+0000f0c0: 7469 746c 655f 6669 6c65 7061 7468 203d  title_filepath =
+0000f0d0: 2064 6563 6c61 7265 645f 7375 6274 6974   declared_subtit
+0000f0e0: 6c65 5f66 696c 6570 6174 680d 0a20 2020  le_filepath..   
+0000f0f0: 2020 2020 2020 2020 2077 6974 6820 6f70           with op
+0000f100: 656e 2873 6176 6564 5f73 7562 7469 746c  en(saved_subtitl
+0000f110: 655f 6669 6c65 7061 7468 2c20 2777 6227  e_filepath, 'wb'
+0000f120: 2920 6173 2066 3a0d 0a20 2020 2020 2020  ) as f:..       
+0000f130: 2020 2020 2020 2020 2066 2e77 7269 7465           f.write
+0000f140: 2866 6f72 6d61 7474 6564 5f73 7562 7469  (formatted_subti
+0000f150: 746c 6573 2e65 6e63 6f64 6528 2275 7466  tles.encode("utf
+0000f160: 2d38 2229 290d 0a20 2020 2020 2020 2020  -8"))..         
+0000f170: 2020 2023 7769 7468 206f 7065 6e28 7361     #with open(sa
+0000f180: 7665 645f 7375 6274 6974 6c65 5f66 696c  ved_subtitle_fil
+0000f190: 6570 6174 682c 2027 6127 2920 6173 2066  epath, 'a') as f
+0000f1a0: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
+0000f1b0: 2020 2020 662e 7772 6974 6528 225c 6e22      f.write("\n"
+0000f1c0: 290d 0a0d 0a20 2020 2020 2020 2065 7863  )....        exc
+0000f1d0: 6570 7420 4b65 7962 6f61 7264 496e 7465  ept KeyboardInte
+0000f1e0: 7272 7570 743a 0d0a 2020 2020 2020 2020  rrupt:..        
+0000f1f0: 2020 2020 6966 2073 656c 662e 6572 726f      if self.erro
+0000f200: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
+0000f210: 6163 6b3a 0d0a 2020 2020 2020 2020 2020  ack:..          
+0000f220: 2020 2020 2020 7365 6c66 2e65 7272 6f72        self.error
+0000f230: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
+0000f240: 636b 2822 4361 6e63 656c 6c69 6e67 2061  ck("Cancelling a
+0000f250: 6c6c 2074 6173 6b73 2229 0d0a 2020 2020  ll tasks")..    
+0000f260: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+0000f270: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000f280: 7269 6e74 2822 4361 6e63 656c 6c69 6e67  rint("Cancelling
+0000f290: 2061 6c6c 2074 6173 6b73 2229 0d0a 2020   all tasks")..  
+0000f2a0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000f2b0: 0d0a 0d0a 2020 2020 2020 2020 6578 6365  ....        exce
+0000f2c0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+0000f2d0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000f2e0: 6966 2073 656c 662e 6572 726f 725f 6d65  if self.error_me
+0000f2f0: 7373 6167 6573 5f63 616c 6c62 6163 6b3a  ssages_callback:
+0000f300: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f310: 2020 7365 6c66 2e65 7272 6f72 5f6d 6573    self.error_mes
+0000f320: 7361 6765 735f 6361 6c6c 6261 636b 2865  sages_callback(e
+0000f330: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+0000f340: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+0000f350: 2020 2020 2020 7072 696e 7428 6529 0d0a        print(e)..
+0000f360: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000f370: 726e 0d0a 0d0a 0d0a 636c 6173 7320 5352  rn......class SR
+0000f380: 5446 696c 6552 6561 6465 723a 0d0a 2020  TFileReader:..  
+0000f390: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+0000f3a0: 656c 662c 2073 7274 5f66 696c 655f 7061  elf, srt_file_pa
+0000f3b0: 7468 2c20 6572 726f 725f 6d65 7373 6167  th, error_messag
+0000f3c0: 6573 5f63 616c 6c62 6163 6b3d 4e6f 6e65  es_callback=None
+0000f3d0: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
+0000f3e0: 2e74 696d 6564 5f73 7562 7469 746c 6573  .timed_subtitles
+0000f3f0: 203d 2073 656c 6628 7372 745f 6669 6c65   = self(srt_file
+0000f400: 5f70 6174 6829 0d0a 2020 2020 2020 2020  _path)..        
+0000f410: 7365 6c66 2e65 7272 6f72 5f6d 6573 7361  self.error_messa
+0000f420: 6765 735f 6361 6c6c 6261 636b 203d 2065  ges_callback = e
+0000f430: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
+0000f440: 6c6c 6261 636b 0d0a 0d0a 2020 2020 4073  llback....    @s
+0000f450: 7461 7469 636d 6574 686f 640d 0a20 2020  taticmethod..   
+0000f460: 2064 6566 205f 5f63 616c 6c5f 5f28 7372   def __call__(sr
+0000f470: 745f 6669 6c65 5f70 6174 6829 3a0d 0a20  t_file_path):.. 
+0000f480: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
+0000f490: 2020 2020 2020 2020 2022 2222 0d0a 2020           """..  
+0000f4a0: 2020 2020 2020 2020 2020 5265 6164 2053            Read S
+0000f4b0: 5254 2066 6f72 6d61 7474 6564 2073 7562  RT formatted sub
+0000f4c0: 7469 746c 6520 6669 6c65 2061 6e64 2072  title file and r
+0000f4d0: 6574 7572 6e20 7375 6274 6974 6c65 7320  eturn subtitles 
+0000f4e0: 6173 206c 6973 7420 6f66 2074 7570 6c65  as list of tuple
+0000f4f0: 730d 0a20 2020 2020 2020 2020 2020 2022  s..            "
+0000f500: 2222 0d0a 2020 2020 2020 2020 2020 2020  ""..            
+0000f510: 7469 6d65 645f 7375 6274 6974 6c65 7320  timed_subtitles 
+0000f520: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+0000f530: 2020 7769 7468 206f 7065 6e28 7372 745f    with open(srt_
+0000f540: 6669 6c65 5f70 6174 682c 2027 7227 2920  file_path, 'r') 
+0000f550: 6173 2073 7274 5f66 696c 653a 0d0a 2020  as srt_file:..  
+0000f560: 2020 2020 2020 2020 2020 2020 2020 6c69                li
+0000f570: 6e65 7320 3d20 7372 745f 6669 6c65 2e72  nes = srt_file.r
+0000f580: 6561 646c 696e 6573 2829 0d0a 2020 2020  eadlines()..    
+0000f590: 2020 2020 2020 2020 2020 2020 2320 5370              # Sp
+0000f5a0: 6c69 7420 7468 6520 7375 6274 6974 6c65  lit the subtitle
+0000f5b0: 2066 696c 6520 696e 746f 2073 7562 7469   file into subti
+0000f5c0: 746c 6520 626c 6f63 6b73 0d0a 2020 2020  tle blocks..    
+0000f5d0: 2020 2020 2020 2020 2020 2020 7375 6274              subt
+0000f5e0: 6974 6c65 5f62 6c6f 636b 7320 3d20 5b5d  itle_blocks = []
+0000f5f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f600: 2020 626c 6f63 6b20 3d20 5b5d 0d0a 2020    block = []..  
+0000f610: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0000f620: 7220 6c69 6e65 2069 6e20 6c69 6e65 733a  r line in lines:
+0000f630: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f640: 2020 2020 2020 6966 206c 696e 652e 7374        if line.st
+0000f650: 7269 7028 2920 3d3d 2027 273a 0d0a 2020  rip() == '':..  
+0000f660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f670: 2020 2020 2020 7375 6274 6974 6c65 5f62        subtitle_b
+0000f680: 6c6f 636b 732e 6170 7065 6e64 2862 6c6f  locks.append(blo
+0000f690: 636b 290d 0a20 2020 2020 2020 2020 2020  ck)..           
+0000f6a0: 2020 2020 2020 2020 2020 2020 2062 6c6f               blo
+0000f6b0: 636b 203d 205b 5d0d 0a20 2020 2020 2020  ck = []..       
+0000f6c0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+0000f6d0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000f6e0: 2020 2020 2020 2020 2020 2020 626c 6f63              bloc
+0000f6f0: 6b2e 6170 7065 6e64 286c 696e 652e 7374  k.append(line.st
+0000f700: 7269 7028 2929 0d0a 2020 2020 2020 2020  rip())..        
+0000f710: 2020 2020 2020 2020 7375 6274 6974 6c65          subtitle
+0000f720: 5f62 6c6f 636b 732e 6170 7065 6e64 2862  _blocks.append(b
+0000f730: 6c6f 636b 290d 0a0d 0a20 2020 2020 2020  lock)....       
+0000f740: 2020 2020 2020 2020 2023 2050 6172 7365           # Parse
+0000f750: 2065 6163 6820 7375 6274 6974 6c65 2062   each subtitle b
+0000f760: 6c6f 636b 2061 6e64 2073 746f 7265 2061  lock and store a
+0000f770: 7320 7475 706c 6520 696e 2074 696d 6564  s tuple in timed
+0000f780: 5f73 7562 7469 746c 6573 206c 6973 740d  _subtitles list.
+0000f790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f7a0: 2066 6f72 2062 6c6f 636b 2069 6e20 7375   for block in su
+0000f7b0: 6274 6974 6c65 5f62 6c6f 636b 733a 0d0a  btitle_blocks:..
+0000f7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f7d0: 2020 2020 6966 2062 6c6f 636b 3a0d 0a20      if block:.. 
+0000f7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f7f0: 2020 2020 2020 2023 2045 7874 7261 6374         # Extract
+0000f800: 2073 7461 7274 2061 6e64 2065 6e64 2074   start and end t
+0000f810: 696d 6573 2066 726f 6d20 7375 6274 6974  imes from subtit
+0000f820: 6c65 2062 6c6f 636b 0d0a 2020 2020 2020  le block..      
+0000f830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f840: 2020 7374 6172 745f 7469 6d65 5f73 7472    start_time_str
+0000f850: 2c20 656e 645f 7469 6d65 5f73 7472 203d  , end_time_str =
+0000f860: 2062 6c6f 636b 5b31 5d2e 7370 6c69 7428   block[1].split(
+0000f870: 2720 2d2d 3e20 2729 0d0a 2020 2020 2020  ' --> ')..      
+0000f880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f890: 2020 7469 6d65 5f66 6f72 6d61 7420 3d20    time_format = 
+0000f8a0: 2725 483a 254d 3a25 532c 2566 270d 0a20  '%H:%M:%S,%f'.. 
+0000f8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8c0: 2020 2020 2020 2073 7461 7274 5f74 696d         start_tim
+0000f8d0: 655f 7469 6d65 5f64 656c 7461 203d 2064  e_time_delta = d
+0000f8e0: 6174 6574 696d 652e 7374 7270 7469 6d65  atetime.strptime
+0000f8f0: 2873 7461 7274 5f74 696d 655f 7374 722c  (start_time_str,
+0000f900: 2074 696d 655f 666f 726d 6174 2920 2d20   time_format) - 
+0000f910: 6461 7465 7469 6d65 2e73 7472 7074 696d  datetime.strptim
+0000f920: 6528 2730 303a 3030 3a30 302c 3030 3027  e('00:00:00,000'
+0000f930: 2c20 7469 6d65 5f66 6f72 6d61 7429 0d0a  , time_format)..
+0000f940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f950: 2020 2020 2020 2020 7374 6172 745f 7469          start_ti
+0000f960: 6d65 5f74 6f74 616c 5f73 6563 6f6e 6473  me_total_seconds
+0000f970: 203d 2073 7461 7274 5f74 696d 655f 7469   = start_time_ti
+0000f980: 6d65 5f64 656c 7461 2e74 6f74 616c 5f73  me_delta.total_s
+0000f990: 6563 6f6e 6473 2829 0d0a 2020 2020 2020  econds()..      
+0000f9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9b0: 2020 656e 645f 7469 6d65 5f74 696d 655f    end_time_time_
+0000f9c0: 6465 6c74 6120 3d20 6461 7465 7469 6d65  delta = datetime
+0000f9d0: 2e73 7472 7074 696d 6528 656e 645f 7469  .strptime(end_ti
+0000f9e0: 6d65 5f73 7472 2c20 7469 6d65 5f66 6f72  me_str, time_for
+0000f9f0: 6d61 7429 202d 2064 6174 6574 696d 652e  mat) - datetime.
+0000fa00: 7374 7270 7469 6d65 2827 3030 3a30 303a  strptime('00:00:
+0000fa10: 3030 2c30 3030 272c 2074 696d 655f 666f  00,000', time_fo
+0000fa20: 726d 6174 290d 0a20 2020 2020 2020 2020  rmat)..         
+0000fa30: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000fa40: 6e64 5f74 696d 655f 746f 7461 6c5f 7365  nd_time_total_se
+0000fa50: 636f 6e64 7320 3d20 656e 645f 7469 6d65  conds = end_time
+0000fa60: 5f74 696d 655f 6465 6c74 612e 746f 7461  _time_delta.tota
+0000fa70: 6c5f 7365 636f 6e64 7328 290d 0a20 2020  l_seconds()..   
+0000fa80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa90: 2020 2020 2023 2045 7874 7261 6374 2073       # Extract s
+0000faa0: 7562 7469 746c 6520 7465 7874 2066 726f  ubtitle text fro
+0000fab0: 6d20 7375 6274 6974 6c65 2062 6c6f 636b  m subtitle block
+0000fac0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000fad0: 2020 2020 2020 2020 2020 7375 6274 6974            subtit
+0000fae0: 6c65 203d 2027 2027 2e6a 6f69 6e28 626c  le = ' '.join(bl
+0000faf0: 6f63 6b5b 323a 5d29 0d0a 2020 2020 2020  ock[2:])..      
+0000fb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb10: 2020 7469 6d65 645f 7375 6274 6974 6c65    timed_subtitle
+0000fb20: 732e 6170 7065 6e64 2828 2873 7461 7274  s.append(((start
+0000fb30: 5f74 696d 655f 746f 7461 6c5f 7365 636f  _time_total_seco
+0000fb40: 6e64 732c 2065 6e64 5f74 696d 655f 746f  nds, end_time_to
+0000fb50: 7461 6c5f 7365 636f 6e64 7329 2c20 7375  tal_seconds), su
+0000fb60: 6274 6974 6c65 2929 0d0a 2020 2020 2020  btitle))..      
+0000fb70: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000fb80: 2074 696d 6564 5f73 7562 7469 746c 6573   timed_subtitles
+0000fb90: 0d0a 0d0a 2020 2020 2020 2020 6578 6365  ....        exce
+0000fba0: 7074 204b 6579 626f 6172 6449 6e74 6572  pt KeyboardInter
+0000fbb0: 7275 7074 3a0d 0a20 2020 2020 2020 2020  rupt:..         
+0000fbc0: 2020 2069 6620 7365 6c66 2e65 7272 6f72     if self.error
+0000fbd0: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
+0000fbe0: 636b 3a0d 0a20 2020 2020 2020 2020 2020  ck:..           
+0000fbf0: 2020 2020 2073 656c 662e 6572 726f 725f       self.error_
+0000fc00: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
+0000fc10: 6b28 2243 616e 6365 6c6c 696e 6720 616c  k("Cancelling al
+0000fc20: 6c20 7461 736b 7322 290d 0a20 2020 2020  l tasks")..     
+0000fc30: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+0000fc40: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+0000fc50: 696e 7428 2243 616e 6365 6c6c 696e 6720  int("Cancelling 
+0000fc60: 616c 6c20 7461 736b 7322 290d 0a20 2020  all tasks")..   
+0000fc70: 2020 2020 2020 2020 2072 6574 7572 6e0d           return.
+0000fc80: 0a0d 0a20 2020 2020 2020 2065 7863 6570  ...        excep
+0000fc90: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+0000fca0: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
+0000fcb0: 6620 7365 6c66 2e65 7272 6f72 5f6d 6573  f self.error_mes
+0000fcc0: 7361 6765 735f 6361 6c6c 6261 636b 3a0d  sages_callback:.
+0000fcd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fce0: 2073 656c 662e 6572 726f 725f 6d65 7373   self.error_mess
+0000fcf0: 6167 6573 5f63 616c 6c62 6163 6b28 6529  ages_callback(e)
+0000fd00: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+0000fd10: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+0000fd20: 2020 2020 2070 7269 6e74 2865 290d 0a20       print(e).. 
+0000fd30: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000fd40: 6e0d 0a0d 0a0d 0a64 6566 2073 686f 775f  n......def show_
+0000fd50: 7072 6f67 7265 7373 286d 6564 6961 5f66  progress(media_f
+0000fd60: 696c 6570 6174 682c 2070 726f 6772 6573  ilepath, progres
+0000fd70: 7329 3a0d 0a20 2020 2067 6c6f 6261 6c20  s):..    global 
+0000fd80: 7062 6172 0d0a 2020 2020 7062 6172 2e75  pbar..    pbar.u
+0000fd90: 7064 6174 6528 7072 6f67 7265 7373 290d  pdate(progress).
+0000fda0: 0a0d 0a0d 0a64 6566 2073 686f 775f 6572  .....def show_er
+0000fdb0: 726f 725f 6d65 7373 6167 6573 286d 6573  ror_messages(mes
+0000fdc0: 7361 6765 7329 3a0d 0a20 2020 2070 7269  sages):..    pri
+0000fdd0: 6e74 286d 6573 7361 6765 7329 0d0a 0d0a  nt(messages)....
+0000fde0: 0d0a 6465 6620 6d61 696e 2829 3a0d 0a20  ..def main():.. 
+0000fdf0: 2020 2067 6c6f 6261 6c20 7062 6172 0d0a     global pbar..
+0000fe00: 0d0a 2020 2020 6966 2073 7973 2e70 6c61  ..    if sys.pla
+0000fe10: 7466 6f72 6d20 3d3d 2022 7769 6e33 3222  tform == "win32"
+0000fe20: 3a0d 0a20 2020 2020 2020 2073 746f 705f  :..        stop_
+0000fe30: 6666 6d70 6567 5f77 696e 646f 7773 2865  ffmpeg_windows(e
+0000fe40: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
+0000fe50: 6c6c 6261 636b 3d73 686f 775f 6572 726f  llback=show_erro
+0000fe60: 725f 6d65 7373 6167 6573 290d 0a20 2020  r_messages)..   
+0000fe70: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+0000fe80: 7374 6f70 5f66 666d 7065 675f 6c69 6e75  stop_ffmpeg_linu
+0000fe90: 7828 6572 726f 725f 6d65 7373 6167 6573  x(error_messages
+0000fea0: 5f63 616c 6c62 6163 6b3d 7368 6f77 5f65  _callback=show_e
+0000feb0: 7272 6f72 5f6d 6573 7361 6765 7329 0d0a  rror_messages)..
+0000fec0: 0d0a 2020 2020 7265 6d6f 7665 5f74 656d  ..    remove_tem
+0000fed0: 705f 6669 6c65 7328 2266 6c61 6322 2c20  p_files("flac", 
+0000fee0: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
+0000fef0: 616c 6c62 6163 6b3d 7368 6f77 5f65 7272  allback=show_err
+0000ff00: 6f72 5f6d 6573 7361 6765 7329 0d0a 2020  or_messages)..  
+0000ff10: 2020 7265 6d6f 7665 5f74 656d 705f 6669    remove_temp_fi
+0000ff20: 6c65 7328 2277 6176 222c 2065 7272 6f72  les("wav", error
+0000ff30: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
+0000ff40: 636b 3d73 686f 775f 6572 726f 725f 6d65  ck=show_error_me
+0000ff50: 7373 6167 6573 290d 0a0d 0a20 2020 2070  ssages)....    p
+0000ff60: 6172 7365 7220 3d20 6172 6770 6172 7365  arser = argparse
+0000ff70: 2e41 7267 756d 656e 7450 6172 7365 7228  .ArgumentParser(
+0000ff80: 290d 0a20 2020 2070 6172 7365 722e 6164  )..    parser.ad
+0000ff90: 645f 6172 6775 6d65 6e74 2827 736f 7572  d_argument('sour
+0000ffa0: 6365 5f70 6174 6827 2c20 6865 6c70 3d22  ce_path', help="
+0000ffb0: 5061 7468 2074 6f20 7468 6520 7669 6465  Path to the vide
+0000ffc0: 6f20 6f72 2061 7564 696f 2066 696c 6573  o or audio files
+0000ffd0: 2074 6f20 6765 6e65 7261 7465 2073 7562   to generate sub
+0000ffe0: 7469 746c 6573 2066 696c 6573 2028 7573  titles files (us
+0000fff0: 6520 7769 6c64 6361 7264 2066 6f72 206d  e wildcard for m
+00010000: 756c 7469 706c 6520 6669 6c65 7320 6f72  ultiple files or
+00010010: 2073 6570 6172 6174 6520 7468 656d 2077   separate them w
+00010020: 6974 6820 6120 7370 6163 6520 6368 6172  ith a space char
+00010030: 6163 7465 7220 652e 672e 205c 2266 696c  acter e.g. \"fil
+00010040: 6520 312e 6d70 345c 2220 5c22 6669 6c65  e 1.mp4\" \"file
+00010050: 2032 2e6d 7034 5c22 2922 2c20 6e61 7267   2.mp4\")", narg
+00010060: 733d 272a 2729 0d0a 2020 2020 7061 7273  s='*')..    pars
+00010070: 6572 2e61 6464 5f61 7267 756d 656e 7428  er.add_argument(
+00010080: 272d 6d27 2c20 272d 2d6d 6f64 656c 2d6e  '-m', '--model-n
+00010090: 616d 6527 2c20 6465 6661 756c 743d 2273  ame', default="s
+000100a0: 6d61 6c6c 222c 2068 656c 703d 226e 616d  mall", help="nam
+000100b0: 6520 6f66 2074 6865 2057 6869 7370 6572  e of the Whisper
+000100c0: 206d 6f64 656c 2074 6f20 7573 6522 290d   model to use").
+000100d0: 0a20 2020 2070 6172 7365 722e 6164 645f  .    parser.add_
+000100e0: 6172 6775 6d65 6e74 2827 2d6c 6d27 2c20  argument('-lm', 
+000100f0: 272d 2d6c 6973 742d 6d6f 6465 6c73 272c  '--list-models',
+00010100: 2068 656c 703d 224c 6973 7420 6f66 2057   help="List of W
+00010110: 6869 7370 6572 206d 6f64 656c 7320 6e61  hisper models na
+00010120: 6d65 222c 2061 6374 696f 6e3d 2773 746f  me", action='sto
+00010130: 7265 5f74 7275 6527 290d 0a20 2020 2070  re_true')..    p
+00010140: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
+00010150: 6e74 2827 2d53 272c 2027 2d2d 7372 632d  nt('-S', '--src-
+00010160: 6c61 6e67 7561 6765 272c 2068 656c 703d  language', help=
+00010170: 224c 616e 6775 6167 6520 636f 6465 206f  "Language code o
+00010180: 6620 7468 6520 6175 6469 6f20 6c61 6e67  f the audio lang
+00010190: 7561 6765 2073 706f 6b65 6e20 696e 2076  uage spoken in v
+000101a0: 6964 656f 2f61 7564 696f 2073 6f75 7263  ideo/audio sourc
+000101b0: 655f 7061 7468 222c 2064 6566 6175 6c74  e_path", default
+000101c0: 3d22 656e 2229 0d0a 2020 2020 7061 7273  ="en")..    pars
+000101d0: 6572 2e61 6464 5f61 7267 756d 656e 7428  er.add_argument(
+000101e0: 272d 4427 2c20 272d 2d64 7374 2d6c 616e  '-D', '--dst-lan
+000101f0: 6775 6167 6527 2c20 6865 6c70 3d22 4465  guage', help="De
+00010200: 7369 7265 6420 7472 616e 736c 6174 696f  sired translatio
+00010210: 6e20 6c61 6e67 7561 6765 2063 6f64 6520  n language code 
+00010220: 666f 7220 7468 6520 7375 6274 6974 6c65  for the subtitle
+00010230: 7322 2c20 6465 6661 756c 743d 4e6f 6e65  s", default=None
+00010240: 290d 0a20 2020 2070 6172 7365 722e 6164  )..    parser.ad
+00010250: 645f 6172 6775 6d65 6e74 2827 2d6c 776c  d_argument('-lwl
+00010260: 272c 2027 2d2d 6c69 7374 2d77 6869 7370  ', '--list-whisp
+00010270: 6572 2d6c 616e 6775 6167 6573 272c 2068  er-languages', h
+00010280: 656c 703d 224c 6973 7420 616c 6c20 7768  elp="List all wh
+00010290: 6973 7065 7220 7375 7070 6f72 7465 6420  isper supported 
+000102a0: 6c61 6e67 7561 6765 7322 2c20 6163 7469  languages", acti
+000102b0: 6f6e 3d27 7374 6f72 655f 7472 7565 2729  on='store_true')
+000102c0: 0d0a 2020 2020 7061 7273 6572 2e61 6464  ..    parser.add
+000102d0: 5f61 7267 756d 656e 7428 272d 6c67 6c27  _argument('-lgl'
+000102e0: 2c20 272d 2d6c 6973 742d 676f 6f67 6c65  , '--list-google
+000102f0: 2d6c 616e 6775 6167 6573 272c 2068 656c  -languages', hel
+00010300: 703d 224c 6973 7420 616c 6c20 676f 6f67  p="List all goog
+00010310: 6c65 2074 7261 6e73 6c61 7465 2073 7570  le translate sup
+00010320: 706f 7274 6564 206c 616e 6775 6167 6573  ported languages
+00010330: 222c 2061 6374 696f 6e3d 2773 746f 7265  ", action='store
+00010340: 5f74 7275 6527 290d 0a20 2020 2070 6172  _true')..    par
+00010350: 7365 722e 6164 645f 6172 6775 6d65 6e74  ser.add_argument
+00010360: 2827 2d46 272c 2027 2d2d 666f 726d 6174  ('-F', '--format
+00010370: 272c 2068 656c 703d 2244 6573 6972 6564  ', help="Desired
+00010380: 2073 7562 7469 746c 6520 666f 726d 6174   subtitle format
+00010390: 222c 2064 6566 6175 6c74 3d22 7372 7422  ", default="srt"
+000103a0: 290d 0a20 2020 2070 6172 7365 722e 6164  )..    parser.ad
+000103b0: 645f 6172 6775 6d65 6e74 2827 2d6c 6627  d_argument('-lf'
+000103c0: 2c20 272d 2d6c 6973 742d 666f 726d 6174  , '--list-format
+000103d0: 7327 2c20 6865 6c70 3d22 4c69 7374 2061  s', help="List a
+000103e0: 6c6c 2073 7570 706f 7274 6564 2073 7562  ll supported sub
+000103f0: 7469 746c 6520 666f 726d 6174 7322 2c20  title formats", 
+00010400: 6163 7469 6f6e 3d27 7374 6f72 655f 7472  action='store_tr
+00010410: 7565 2729 0d0a 2020 2020 7061 7273 6572  ue')..    parser
+00010420: 2e61 6464 5f61 7267 756d 656e 7428 272d  .add_argument('-
+00010430: 4327 2c20 272d 2d63 6f6e 6375 7272 656e  C', '--concurren
+00010440: 6379 272c 2068 656c 703d 224e 756d 6265  cy', help="Numbe
+00010450: 7220 6f66 2063 6f6e 6375 7272 656e 7420  r of concurrent 
+00010460: 4150 4920 7265 7175 6573 7473 2074 6f20  API requests to 
+00010470: 6d61 6b65 222c 2074 7970 653d 696e 742c  make", type=int,
+00010480: 2064 6566 6175 6c74 3d31 3029 0d0a 2020   default=10)..  
+00010490: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
+000104a0: 756d 656e 7428 272d 7627 2c20 272d 2d76  ument('-v', '--v
+000104b0: 6572 7369 6f6e 272c 2061 6374 696f 6e3d  ersion', action=
+000104c0: 2776 6572 7369 6f6e 272c 2076 6572 7369  'version', versi
+000104d0: 6f6e 3d56 4552 5349 4f4e 290d 0a0d 0a20  on=VERSION).... 
+000104e0: 2020 2061 7267 7320 3d20 7061 7273 6572     args = parser
+000104f0: 2e70 6172 7365 5f61 7267 7328 290d 0a0d  .parse_args()...
+00010500: 0a20 2020 2073 7263 5f6c 616e 6775 6167  .    src_languag
+00010510: 6520 3d20 6172 6773 2e73 7263 5f6c 616e  e = args.src_lan
+00010520: 6775 6167 650d 0a20 2020 2064 7374 5f6c  guage..    dst_l
+00010530: 616e 6775 6167 6520 3d20 6172 6773 2e64  anguage = args.d
+00010540: 7374 5f6c 616e 6775 6167 650d 0a0d 0a20  st_language.... 
+00010550: 2020 206d 6f64 656c 5f6e 616d 6520 3d20     model_name = 
+00010560: 6172 6773 2e6d 6f64 656c 5f6e 616d 650d  args.model_name.
+00010570: 0a20 2020 2069 6620 6d6f 6465 6c5f 6e61  .    if model_na
+00010580: 6d65 2e65 6e64 7377 6974 6828 222e 656e  me.endswith(".en
+00010590: 2229 3a0d 0a20 2020 2020 2020 2070 7269  "):..        pri
+000105a0: 6e74 2866 227b 6d6f 6465 6c5f 6e61 6d65  nt(f"{model_name
+000105b0: 7d20 6973 2061 6e20 456e 676c 6973 682d  } is an English-
+000105c0: 6f6e 6c79 206d 6f64 656c 2c20 666f 7263  only model, forc
+000105d0: 696e 6720 456e 676c 6973 6820 6465 7465  ing English dete
+000105e0: 6374 696f 6e2e 2229 0d0a 2020 2020 2020  ction.")..      
+000105f0: 2020 6172 6773 2e73 7263 5f6c 616e 6775    args.src_langu
+00010600: 6167 6520 3d20 2265 6e22 0d0a 2020 2020  age = "en"..    
+00010610: 656c 6966 2061 7267 732e 7372 635f 6c61  elif args.src_la
+00010620: 6e67 7561 6765 2021 3d20 2261 7574 6f22  nguage != "auto"
+00010630: 3a0d 0a20 2020 2020 2020 2061 7267 732e  :..        args.
+00010640: 7372 635f 6c61 6e67 7561 6765 203d 2073  src_language = s
+00010650: 7263 5f6c 616e 6775 6167 650d 0a0d 0a20  rc_language.... 
+00010660: 2020 206d 6f64 656c 203d 2077 6869 7370     model = whisp
+00010670: 6572 2e6c 6f61 645f 6d6f 6465 6c28 6d6f  er.load_model(mo
+00010680: 6465 6c5f 6e61 6d65 290d 0a0d 0a20 2020  del_name)....   
+00010690: 2069 6620 6172 6773 2e6c 6973 745f 6d6f   if args.list_mo
+000106a0: 6465 6c73 3a0d 0a20 2020 2020 2020 2070  dels:..        p
+000106b0: 7269 6e74 2822 4c69 7374 206f 6620 7768  rint("List of wh
+000106c0: 6973 7065 7220 6d6f 6465 6c73 3a22 290d  isper models:").
+000106d0: 0a20 2020 2020 2020 2066 6f72 206d 6f64  .        for mod
+000106e0: 656c 5f6e 616d 6520 696e 2077 6869 7370  el_name in whisp
+000106f0: 6572 2e61 7661 696c 6162 6c65 5f6d 6f64  er.available_mod
+00010700: 656c 7328 293a 0d0a 2020 2020 2020 2020  els():..        
+00010710: 2020 2020 7072 696e 7428 6d6f 6465 6c5f      print(model_
+00010720: 6e61 6d65 290d 0a20 2020 2020 2020 2072  name)..        r
+00010730: 6574 7572 6e20 300d 0a0d 0a20 2020 2077  eturn 0....    w
+00010740: 6869 7370 6572 5f6c 616e 6775 6167 6520  hisper_language 
+00010750: 3d20 5768 6973 7065 724c 616e 6775 6167  = WhisperLanguag
+00010760: 6528 290d 0a20 2020 2067 6f6f 676c 655f  e()..    google_
+00010770: 6c61 6e67 7561 6765 203d 2047 6f6f 676c  language = Googl
+00010780: 654c 616e 6775 6167 6528 290d 0a0d 0a20  eLanguage().... 
+00010790: 2020 2069 6620 6172 6773 2e6c 6973 745f     if args.list_
+000107a0: 7768 6973 7065 725f 6c61 6e67 7561 6765  whisper_language
+000107b0: 733a 0d0a 2020 2020 2020 2020 7072 696e  s:..        prin
+000107c0: 7428 224c 6973 7420 6f66 2077 6869 7370  t("List of whisp
+000107d0: 6572 2073 7570 706f 7274 6564 206c 616e  er supported lan
+000107e0: 6775 6167 6573 3a22 290d 0a20 2020 2020  guages:")..     
+000107f0: 2020 2066 6f72 2077 6869 7370 6572 5f63     for whisper_c
+00010800: 6f64 652c 2077 6869 7370 6572 5f6c 616e  ode, whisper_lan
+00010810: 6775 6167 6520 696e 2073 6f72 7465 6428  guage in sorted(
+00010820: 7768 6973 7065 725f 6c61 6e67 7561 6765  whisper_language
+00010830: 2e6e 616d 655f 6f66 5f63 6f64 652e 6974  .name_of_code.it
+00010840: 656d 7328 2929 3a0d 0a20 2020 2020 2020  ems()):..       
+00010850: 2020 2020 2070 7269 6e74 2822 252d 3873       print("%-8s
+00010860: 203a 2025 7322 2025 2877 6869 7370 6572   : %s" %(whisper
+00010870: 5f63 6f64 652c 2077 6869 7370 6572 5f6c  _code, whisper_l
+00010880: 616e 6775 6167 6529 290d 0a20 2020 2020  anguage))..     
+00010890: 2020 2072 6574 7572 6e20 300d 0a0d 0a20     return 0.... 
+000108a0: 2020 2069 6620 6172 6773 2e6c 6973 745f     if args.list_
+000108b0: 676f 6f67 6c65 5f6c 616e 6775 6167 6573  google_languages
+000108c0: 3a0d 0a20 2020 2020 2020 2070 7269 6e74  :..        print
+000108d0: 2822 4c69 7374 206f 6620 676f 6f67 6c65  ("List of google
+000108e0: 2074 7261 6e73 6c61 7465 2073 7570 706f   translate suppo
+000108f0: 7274 6564 206c 616e 6775 6167 6573 3a22  rted languages:"
+00010900: 290d 0a20 2020 2020 2020 2066 6f72 2067  )..        for g
+00010910: 6f6f 676c 655f 636f 6465 2c20 676f 6f67  oogle_code, goog
+00010920: 6c65 5f6c 616e 6775 6167 6520 696e 2073  le_language in s
+00010930: 6f72 7465 6428 676f 6f67 6c65 5f6c 616e  orted(google_lan
+00010940: 6775 6167 652e 6e61 6d65 5f6f 665f 636f  guage.name_of_co
+00010950: 6465 2e69 7465 6d73 2829 293a 0d0a 2020  de.items()):..  
+00010960: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00010970: 2225 2d38 7320 3a20 2573 2220 2528 676f  "%-8s : %s" %(go
+00010980: 6f67 6c65 5f63 6f64 652c 2067 6f6f 676c  ogle_code, googl
+00010990: 655f 6c61 6e67 7561 6765 2929 0d0a 2020  e_language))..  
+000109a0: 2020 2020 2020 7265 7475 726e 2030 0d0a        return 0..
+000109b0: 0d0a 2020 2020 6966 2061 7267 732e 7372  ..    if args.sr
+000109c0: 635f 6c61 6e67 7561 6765 206e 6f74 2069  c_language not i
+000109d0: 6e20 7768 6973 7065 725f 6c61 6e67 7561  n whisper_langua
+000109e0: 6765 2e6e 616d 655f 6f66 5f63 6f64 652e  ge.name_of_code.
+000109f0: 6b65 7973 2829 3a0d 0a20 2020 2020 2020  keys():..       
+00010a00: 2070 7269 6e74 2822 536f 7572 6365 206c   print("Source l
+00010a10: 616e 6775 6167 6520 6973 206e 6f74 2073  anguage is not s
+00010a20: 7570 706f 7274 6564 2e20 5275 6e20 7769  upported. Run wi
+00010a30: 7468 202d 2d6c 6973 742d 7768 6973 7065  th --list-whispe
+00010a40: 722d 6c61 6e67 7561 6765 7320 746f 2073  r-languages to s
+00010a50: 6565 2061 6c6c 2077 6869 7370 6572 2073  ee all whisper s
+00010a60: 7570 706f 7274 6564 206c 616e 6775 6167  upported languag
+00010a70: 6573 2e22 290d 0a20 2020 2020 2020 2072  es.")..        r
+00010a80: 6574 7572 6e20 310d 0a0d 0a20 2020 2069  eturn 1....    i
+00010a90: 6620 6172 6773 2e64 7374 5f6c 616e 6775  f args.dst_langu
+00010aa0: 6167 653a 0d0a 2020 2020 2020 2020 6966  age:..        if
+00010ab0: 206e 6f74 2061 7267 732e 6473 745f 6c61   not args.dst_la
+00010ac0: 6e67 7561 6765 2069 6e20 676f 6f67 6c65  nguage in google
+00010ad0: 5f6c 616e 6775 6167 652e 6e61 6d65 5f6f  _language.name_o
+00010ae0: 665f 636f 6465 2e6b 6579 7328 293a 0d0a  f_code.keys():..
+00010af0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00010b00: 7428 2244 6573 7469 6e61 7469 6f6e 206c  t("Destination l
+00010b10: 616e 6775 6167 6520 6973 206e 6f74 2073  anguage is not s
+00010b20: 7570 706f 7274 6564 2e20 5275 6e20 7769  upported. Run wi
+00010b30: 7468 202d 2d6c 6973 742d 676f 6f67 6c65  th --list-google
+00010b40: 2d6c 616e 6775 6167 6573 2074 6f20 7365  -languages to se
+00010b50: 6520 616c 6c20 676f 6f67 6c65 2074 7261  e all google tra
+00010b60: 6e73 6c61 7465 2073 7570 706f 7274 6564  nslate supported
+00010b70: 206c 616e 6775 6167 6573 2e22 290d 0a20   languages.").. 
+00010b80: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00010b90: 6e20 310d 0a20 2020 2020 2020 2069 6620  n 1..        if 
+00010ba0: 6e6f 7420 6973 5f73 616d 655f 6c61 6e67  not is_same_lang
+00010bb0: 7561 6765 2861 7267 732e 7372 635f 6c61  uage(args.src_la
+00010bc0: 6e67 7561 6765 2c20 6172 6773 2e64 7374  nguage, args.dst
+00010bd0: 5f6c 616e 6775 6167 652c 2065 7272 6f72  _language, error
+00010be0: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
+00010bf0: 636b 3d73 686f 775f 6572 726f 725f 6d65  ck=show_error_me
+00010c00: 7373 6167 6573 293a 0d0a 2020 2020 2020  ssages):..      
+00010c10: 2020 2020 2020 646f 5f74 7261 6e73 6c61        do_transla
+00010c20: 7465 203d 2054 7275 650d 0a20 2020 2020  te = True..     
+00010c30: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00010c40: 2020 2020 2020 646f 5f74 7261 6e73 6c61        do_transla
+00010c50: 7465 203d 2046 616c 7365 0d0a 2020 2020  te = False..    
+00010c60: 656c 7365 3a0d 0a20 2020 2020 2020 2064  else:..        d
+00010c70: 6f5f 7472 616e 736c 6174 6520 3d20 4661  o_translate = Fa
+00010c80: 6c73 650d 0a0d 0a20 2020 2069 6620 6172  lse....    if ar
+00010c90: 6773 2e6c 6973 745f 666f 726d 6174 733a  gs.list_formats:
+00010ca0: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
+00010cb0: 224c 6973 7420 6f66 2073 7570 706f 7274  "List of support
+00010cc0: 6564 2073 7562 7469 746c 6520 666f 726d  ed subtitle form
+00010cd0: 6174 733a 2229 0d0a 2020 2020 2020 2020  ats:")..        
+00010ce0: 666f 7220 7375 6274 6974 6c65 5f66 6f72  for subtitle_for
+00010cf0: 6d61 7420 696e 2053 7562 7469 746c 6546  mat in SubtitleF
+00010d00: 6f72 6d61 7474 6572 2e73 7570 706f 7274  ormatter.support
+00010d10: 6564 5f66 6f72 6d61 7473 3a0d 0a20 2020  ed_formats:..   
+00010d20: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
+00010d30: 7b66 6f72 6d61 747d 222e 666f 726d 6174  {format}".format
+00010d40: 2866 6f72 6d61 743d 7375 6274 6974 6c65  (format=subtitle
+00010d50: 5f66 6f72 6d61 7429 290d 0a20 2020 2020  _format))..     
+00010d60: 2020 2072 6574 7572 6e20 300d 0a0d 0a20     return 0.... 
+00010d70: 2020 2069 6620 6172 6773 2e66 6f72 6d61     if args.forma
+00010d80: 7420 6e6f 7420 696e 2053 7562 7469 746c  t not in Subtitl
+00010d90: 6546 6f72 6d61 7474 6572 2e73 7570 706f  eFormatter.suppo
+00010da0: 7274 6564 5f66 6f72 6d61 7473 3a0d 0a20  rted_formats:.. 
+00010db0: 2020 2020 2020 2070 7269 6e74 2822 5375         print("Su
+00010dc0: 6274 6974 6c65 2066 6f72 6d61 7420 6973  btitle format is
+00010dd0: 206e 6f74 2073 7570 706f 7274 6564 2e20   not supported. 
+00010de0: 5275 6e20 7769 7468 202d 2d6c 6973 742d  Run with --list-
+00010df0: 666f 726d 6174 7320 746f 2073 6565 2061  formats to see a
+00010e00: 6c6c 2073 7570 706f 7274 6564 2066 6f72  ll supported for
+00010e10: 6d61 7473 2e22 290d 0a20 2020 2020 2020  mats.")..       
+00010e20: 2072 6574 7572 6e20 310d 0a0d 0a20 2020   return 1....   
+00010e30: 2069 6620 6e6f 7420 6172 6773 2e73 6f75   if not args.sou
+00010e40: 7263 655f 7061 7468 3a0d 0a20 2020 2020  rce_path:..     
+00010e50: 2020 2070 6172 7365 722e 7072 696e 745f     parser.print_
+00010e60: 6865 6c70 2873 7973 2e73 7464 6572 7229  help(sys.stderr)
+00010e70: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00010e80: 2031 0d0a 0d0a 2020 2020 636f 6d70 6c65   1....    comple
+00010e90: 7465 645f 7461 736b 7320 3d20 300d 0a20  ted_tasks = 0.. 
+00010ea0: 2020 206d 6564 6961 5f66 696c 6570 6174     media_filepat
+00010eb0: 6873 203d 205b 5d0d 0a20 2020 2061 7267  hs = []..    arg
 00010ec0: 5f66 696c 6570 6174 6873 203d 205b 5d0d  _filepaths = [].
-00010ed0: 0a20 2020 2061 7267 5f66 696c 6570 6174  .    arg_filepat
-00010ee0: 6873 203d 205b 5d0d 0a20 2020 2069 6e76  hs = []..    inv
-00010ef0: 616c 6964 5f6d 6564 6961 5f66 696c 6570  alid_media_filep
-00010f00: 6174 6873 203d 205b 5d0d 0a20 2020 206e  aths = []..    n
-00010f10: 6f74 5f65 7869 7374 5f66 696c 6570 6174  ot_exist_filepat
-00010f20: 6873 203d 205b 5d0d 0a20 2020 2061 7267  hs = []..    arg
-00010f30: 7061 7468 203d 204e 6f6e 650d 0a0d 0a20  path = None.... 
-00010f40: 2020 2061 7267 735f 736f 7572 6365 5f70     args_source_p
-00010f50: 6174 6820 3d20 6172 6773 2e73 6f75 7263  ath = args.sourc
-00010f60: 655f 7061 7468 0d0a 0d0a 2020 2020 6966  e_path....    if
-00010f70: 2028 6e6f 7420 2822 2a22 2061 6e64 2022   (not ("*" and "
-00010f80: 3f22 2920 696e 2073 7472 2861 7267 735f  ?") in str(args_
-00010f90: 736f 7572 6365 5f70 6174 6829 293a 0d0a  source_path)):..
-00010fa0: 2020 2020 2020 2020 666f 7220 6669 6c65          for file
-00010fb0: 7061 7468 2069 6e20 6172 6773 5f73 6f75  path in args_sou
-00010fc0: 7263 655f 7061 7468 3a0d 0a20 2020 2020  rce_path:..     
-00010fd0: 2020 2020 2020 2066 7061 7468 203d 2050         fpath = P
-00010fe0: 6174 6828 6669 6c65 7061 7468 290d 0a20  ath(filepath).. 
-00010ff0: 2020 2020 2020 2020 2020 2023 7072 696e             #prin
-00011000: 7428 2266 7061 7468 203d 2025 7322 2025  t("fpath = %s" %
-00011010: 6670 6174 6829 0d0a 2020 2020 2020 2020  fpath)..        
-00011020: 2020 2020 6966 206e 6f74 206f 732e 7061      if not os.pa
-00011030: 7468 2e69 7366 696c 6528 6670 6174 6829  th.isfile(fpath)
-00011040: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00011050: 2020 206e 6f74 5f65 7869 7374 5f66 696c     not_exist_fil
-00011060: 6570 6174 6873 2e61 7070 656e 6428 6669  epaths.append(fi
-00011070: 6c65 7061 7468 290d 0a20 2020 2020 2020  lepath)..       
-00011080: 2020 2020 2020 2020 2023 7072 696e 7428           #print(
-00011090: 7374 7228 6670 6174 6829 202b 2022 2069  str(fpath) + " i
-000110a0: 7320 6e6f 7420 6578 6973 7422 290d 0a0d  s not exist")...
-000110b0: 0a20 2020 2069 6620 7379 732e 706c 6174  .    if sys.plat
-000110c0: 666f 726d 203d 3d20 2277 696e 3332 223a  form == "win32":
-000110d0: 0d0a 2020 2020 2020 2020 666f 7220 6920  ..        for i 
-000110e0: 696e 2072 616e 6765 286c 656e 2861 7267  in range(len(arg
-000110f0: 732e 736f 7572 6365 5f70 6174 6829 293a  s.source_path)):
-00011100: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00011110: 2028 225b 2220 6f72 2022 5d22 2920 696e   ("[" or "]") in
-00011120: 2061 7267 732e 736f 7572 6365 5f70 6174   args.source_pat
-00011130: 685b 695d 3a0d 0a20 2020 2020 2020 2020  h[i]:..         
-00011140: 2020 2020 2020 2070 6c61 6365 686f 6c64         placehold
-00011150: 6572 203d 2022 2354 454d 5023 220d 0a20  er = "#TEMP#".. 
-00011160: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00011170: 7267 735f 736f 7572 6365 5f70 6174 685b  rgs_source_path[
-00011180: 695d 203d 2061 7267 732e 736f 7572 6365  i] = args.source
-00011190: 5f70 6174 685b 695d 2e72 6570 6c61 6365  _path[i].replace
-000111a0: 2822 5b22 2c20 706c 6163 6568 6f6c 6465  ("[", placeholde
-000111b0: 7229 0d0a 2020 2020 2020 2020 2020 2020  r)..            
-000111c0: 2020 2020 6172 6773 5f73 6f75 7263 655f      args_source_
-000111d0: 7061 7468 5b69 5d20 3d20 6172 6773 5f73  path[i] = args_s
-000111e0: 6f75 7263 655f 7061 7468 5b69 5d2e 7265  ource_path[i].re
-000111f0: 706c 6163 6528 225d 222c 2022 5b5d 5d22  place("]", "[]]"
-00011200: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00011210: 2020 2061 7267 735f 736f 7572 6365 5f70     args_source_p
-00011220: 6174 685b 695d 203d 2061 7267 735f 736f  ath[i] = args_so
-00011230: 7572 6365 5f70 6174 685b 695d 2e72 6570  urce_path[i].rep
-00011240: 6c61 6365 2870 6c61 6365 686f 6c64 6572  lace(placeholder
-00011250: 2c20 225b 5b5d 2229 0d0a 2020 2020 2020  , "[[]")..      
-00011260: 2020 2020 2020 2020 2020 2370 7269 6e74            #print
-00011270: 2822 6172 6773 5f73 6f75 7263 655f 7061  ("args_source_pa
-00011280: 7468 203d 2025 7322 2025 2861 7267 735f  th = %s" %(args_
-00011290: 736f 7572 6365 5f70 6174 6829 290d 0a0d  source_path))...
-000112a0: 0a20 2020 2066 6f72 2061 7267 2069 6e20  .    for arg in 
-000112b0: 6172 6773 5f73 6f75 7263 655f 7061 7468  args_source_path
-000112c0: 3a0d 0a20 2020 2020 2020 2069 6620 6e6f  :..        if no
-000112d0: 7420 7379 732e 706c 6174 666f 726d 203d  t sys.platform =
-000112e0: 3d20 2277 696e 3332 2220 3a0d 0a20 2020  = "win32" :..   
-000112f0: 2020 2020 2020 2020 2061 7267 203d 2065           arg = e
-00011300: 7363 6170 6528 6172 6729 0d0a 0d0a 2020  scape(arg)....  
-00011310: 2020 2020 2020 2370 7269 6e74 2822 676c        #print("gl
-00011320: 6f62 2861 7267 2920 3d20 2573 2220 2528  ob(arg) = %s" %(
-00011330: 676c 6f62 2861 7267 2929 290d 0a0d 0a20  glob(arg))).... 
-00011340: 2020 2020 2020 2061 7267 5f66 696c 6570         arg_filep
-00011350: 6174 6873 202b 3d20 676c 6f62 2861 7267  aths += glob(arg
-00011360: 290d 0a0d 0a20 2020 2069 6620 6172 675f  )....    if arg_
-00011370: 6669 6c65 7061 7468 733a 0d0a 2020 2020  filepaths:..    
-00011380: 2020 2020 666f 7220 6172 6770 6174 6820      for argpath 
-00011390: 696e 2061 7267 5f66 696c 6570 6174 6873  in arg_filepaths
-000113a0: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-000113b0: 6620 6f73 2e70 6174 682e 6973 6669 6c65  f os.path.isfile
-000113c0: 2861 7267 7061 7468 293a 0d0a 2020 2020  (argpath):..    
-000113d0: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-000113e0: 6865 636b 5f66 696c 655f 7479 7065 2861  heck_file_type(a
-000113f0: 7267 7061 7468 2c20 6572 726f 725f 6d65  rgpath, error_me
-00011400: 7373 6167 6573 5f63 616c 6c62 6163 6b3d  ssages_callback=
-00011410: 7368 6f77 5f65 7272 6f72 5f6d 6573 7361  show_error_messa
-00011420: 6765 7329 203d 3d20 2776 6964 656f 2720  ges) == 'video' 
-00011430: 6f72 2063 6865 636b 5f66 696c 655f 7479  or check_file_ty
-00011440: 7065 2861 7267 7061 7468 2c20 6572 726f  pe(argpath, erro
-00011450: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
-00011460: 6163 6b3d 7368 6f77 5f65 7272 6f72 5f6d  ack=show_error_m
-00011470: 6573 7361 6765 7329 203d 3d20 2761 7564  essages) == 'aud
-00011480: 696f 273a 0d0a 2020 2020 2020 2020 2020  io':..          
-00011490: 2020 2020 2020 2020 2020 6d65 6469 615f            media_
-000114a0: 6669 6c65 7061 7468 732e 6170 7065 6e64  filepaths.append
-000114b0: 2861 7267 7061 7468 290d 0a20 2020 2020  (argpath)..     
-000114c0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000114d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000114e0: 2020 2020 2020 696e 7661 6c69 645f 6d65        invalid_me
-000114f0: 6469 615f 6669 6c65 7061 7468 732e 6170  dia_filepaths.ap
-00011500: 7065 6e64 2861 7267 7061 7468 290d 0a20  pend(argpath).. 
-00011510: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00011520: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011530: 2020 6e6f 745f 6578 6973 745f 6669 6c65    not_exist_file
-00011540: 7061 7468 732e 6170 7065 6e64 2861 7267  paths.append(arg
-00011550: 7061 7468 290d 0a0d 0a20 2020 2020 2020  path)....       
-00011560: 2069 6620 696e 7661 6c69 645f 6d65 6469   if invalid_medi
-00011570: 615f 6669 6c65 7061 7468 733a 0d0a 2020  a_filepaths:..  
-00011580: 2020 2020 2020 2020 2020 666f 7220 696e            for in
-00011590: 7661 6c69 645f 6d65 6469 615f 6669 6c65  valid_media_file
-000115a0: 7061 7468 2069 6e20 696e 7661 6c69 645f  path in invalid_
-000115b0: 6d65 6469 615f 6669 6c65 7061 7468 733a  media_filepaths:
-000115c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000115d0: 2020 6d73 6720 3d20 227b 7d20 6973 206e    msg = "{} is n
-000115e0: 6f74 2076 616c 6964 2076 6964 656f 206f  ot valid video o
-000115f0: 7220 6175 6469 6f20 6669 6c65 7322 2e66  r audio files".f
-00011600: 6f72 6d61 7428 696e 7661 6c69 645f 6d65  ormat(invalid_me
-00011610: 6469 615f 6669 6c65 7061 7468 290d 0a20  dia_filepath).. 
-00011620: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00011630: 7269 6e74 286d 7367 290d 0a0d 0a20 2020  rint(msg)....   
-00011640: 2023 7072 696e 7428 226e 6f74 5f65 7869   #print("not_exi
-00011650: 7374 5f66 696c 6570 6174 6873 203d 2025  st_filepaths = %
-00011660: 7322 2025 286e 6f74 5f65 7869 7374 5f66  s" %(not_exist_f
-00011670: 696c 6570 6174 6873 2929 0d0a 0d0a 2020  ilepaths))....  
-00011680: 2020 6966 206e 6f74 5f65 7869 7374 5f66    if not_exist_f
-00011690: 696c 6570 6174 6873 3a0d 0a20 2020 2020  ilepaths:..     
-000116a0: 2020 2066 6f72 206e 6f74 5f65 7869 7374     for not_exist
-000116b0: 5f66 696c 6570 6174 6820 696e 206e 6f74  _filepath in not
-000116c0: 5f65 7869 7374 5f66 696c 6570 6174 6873  _exist_filepaths
-000116d0: 3a0d 0a20 2020 2020 2020 2020 2020 206d  :..            m
-000116e0: 7367 203d 2022 7b7d 2069 7320 6e6f 7420  sg = "{} is not 
-000116f0: 6578 6973 7422 2e66 6f72 6d61 7428 6e6f  exist".format(no
-00011700: 745f 6578 6973 745f 6669 6c65 7061 7468  t_exist_filepath
-00011710: 290d 0a20 2020 2020 2020 2020 2020 2070  )..            p
-00011720: 7269 6e74 286d 7367 290d 0a20 2020 2020  rint(msg)..     
-00011730: 2020 2069 6620 286e 6f74 2028 222a 2220     if (not ("*" 
-00011740: 616e 6420 223f 2229 2069 6e20 7374 7228  and "?") in str(
-00011750: 6172 6773 5f73 6f75 7263 655f 7061 7468  args_source_path
-00011760: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
-00011770: 2073 7973 2e65 7869 7428 3029 0d0a 0d0a   sys.exit(0)....
-00011780: 2020 2020 6966 206e 6f74 2061 7267 5f66      if not arg_f
-00011790: 696c 6570 6174 6873 2061 6e64 206e 6f74  ilepaths and not
-000117a0: 206e 6f74 5f65 7869 7374 5f66 696c 6570   not_exist_filep
-000117b0: 6174 6873 3a0d 0a20 2020 2020 2020 2070  aths:..        p
-000117c0: 7269 6e74 2822 4e6f 2061 6e79 2066 696c  rint("No any fil
-000117d0: 6573 206d 6174 6368 696e 6720 6669 6c65  es matching file
-000117e0: 6e61 6d65 7320 796f 7520 7479 7065 6422  names you typed"
-000117f0: 290d 0a20 2020 2020 2020 2073 7973 2e65  )..        sys.e
-00011800: 7869 7428 3029 0d0a 0d0a 2020 2020 706f  xit(0)....    po
-00011810: 6f6c 203d 206d 756c 7469 7072 6f63 6573  ol = multiproces
-00011820: 7369 6e67 2e50 6f6f 6c28 6172 6773 2e63  sing.Pool(args.c
-00011830: 6f6e 6375 7272 656e 6379 290d 0a0d 0a20  oncurrency).... 
-00011840: 2020 2074 7261 6e73 6372 6962 655f 656e     transcribe_en
-00011850: 645f 7469 6d65 203d 204e 6f6e 650d 0a20  d_time = None.. 
-00011860: 2020 2074 7261 6e73 6372 6962 655f 656c     transcribe_el
-00011870: 6170 7365 645f 7469 6d65 203d 204e 6f6e  apsed_time = Non
-00011880: 650d 0a20 2020 2074 7261 6e73 6372 6962  e..    transcrib
-00011890: 655f 7374 6172 745f 7469 6d65 203d 2074  e_start_time = t
-000118a0: 696d 652e 7469 6d65 2829 0d0a 2020 2020  ime.time()..    
-000118b0: 7461 736b 203d 2022 7472 616e 7363 7269  task = "transcri
-000118c0: 6265 220d 0a0d 0a20 2020 2069 6620 6172  be"....    if ar
-000118d0: 6773 2e73 7263 5f6c 616e 6775 6167 6520  gs.src_language 
-000118e0: 3d3d 2028 2262 6122 206f 7220 2262 7222  == ("ba" or "br"
-000118f0: 206f 7220 2266 6f22 206f 7220 226e 6e22   or "fo" or "nn"
-00011900: 206f 7220 226f 6322 206f 7220 2274 6c22   or "oc" or "tl"
-00011910: 206f 7220 2262 6f22 2920 616e 6420 646f   or "bo") and do
-00011920: 5f74 7261 6e73 6c61 7465 3a0d 0a20 2020  _translate:..   
-00011930: 2020 2020 2074 6173 6b20 3d20 2274 7261       task = "tra
-00011940: 6e73 6c61 7465 220d 0a20 2020 2020 2020  nslate"..       
-00011950: 2073 7263 5f6c 616e 6775 6167 6520 3d20   src_language = 
-00011960: 2265 6e22 0d0a 0d0a 2020 2020 666f 7220  "en"....    for 
-00011970: 6d65 6469 615f 6669 6c65 7061 7468 2069  media_filepath i
-00011980: 6e20 6d65 6469 615f 6669 6c65 7061 7468  n media_filepath
-00011990: 733a 0d0a 2020 2020 2020 2020 7072 696e  s:..        prin
-000119a0: 7428 2250 726f 6365 7373 696e 6720 7b7d  t("Processing {}
-000119b0: 203a 222e 666f 726d 6174 286d 6564 6961   :".format(media
-000119c0: 5f66 696c 6570 6174 6829 290d 0a0d 0a20  _filepath)).... 
-000119d0: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
-000119e0: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
-000119f0: 436f 6e76 6572 7469 6e67 2074 6f20 6120  Converting to a 
-00011a00: 7465 6d70 6f72 6172 7920 5741 5620 6669  temporary WAV fi
-00011a10: 6c65 2020 2020 2020 3a20 2229 0d0a 2020  le      : ")..  
-00011a20: 2020 2020 2020 2020 2020 7769 6467 6574            widget
-00011a30: 7320 3d20 5b22 222c 2050 6572 6365 6e74  s = ["", Percent
-00011a40: 6167 6528 292c 2027 2027 2c20 4261 7228  age(), ' ', Bar(
-00011a50: 6d61 726b 6572 3d27 e296 8827 292c 2027  marker='...'), '
-00011a60: 2027 2c20 4554 4128 295d 0d0a 2020 2020   ', ETA()]..    
-00011a70: 2020 2020 2020 2020 7062 6172 203d 2050          pbar = P
-00011a80: 726f 6772 6573 7342 6172 2877 6964 6765  rogressBar(widge
-00011a90: 7473 3d77 6964 6765 7473 2c20 6d61 7876  ts=widgets, maxv
-00011aa0: 616c 3d31 3030 292e 7374 6172 7428 290d  al=100).start().
-00011ab0: 0a20 2020 2020 2020 2020 2020 2077 6176  .            wav
-00011ac0: 5f63 6f6e 7665 7274 6572 203d 2057 6176  _converter = Wav
-00011ad0: 436f 6e76 6572 7465 7228 7072 6f67 7265  Converter(progre
-00011ae0: 7373 5f63 616c 6c62 6163 6b3d 7368 6f77  ss_callback=show
-00011af0: 5f70 726f 6772 6573 732c 2065 7272 6f72  _progress, error
-00011b00: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
-00011b10: 636b 3d73 686f 775f 6572 726f 725f 6d65  ck=show_error_me
-00011b20: 7373 6167 6573 290d 0a20 2020 2020 2020  ssages)..       
-00011b30: 2020 2020 2077 6176 5f66 696c 6570 6174       wav_filepat
-00011b40: 682c 2073 616d 706c 655f 7261 7465 203d  h, sample_rate =
-00011b50: 2077 6176 5f63 6f6e 7665 7274 6572 286d   wav_converter(m
-00011b60: 6564 6961 5f66 696c 6570 6174 6829 0d0a  edia_filepath)..
-00011b70: 2020 2020 2020 2020 2020 2020 7062 6172              pbar
-00011b80: 2e66 696e 6973 6828 290d 0a0d 0a20 2020  .finish()....   
-00011b90: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
-00011ba0: 5065 7266 6f72 6d69 6e67 2073 7065 6563  Performing speec
-00011bb0: 6820 7265 636f 676e 6974 696f 6e20 2020  h recognition   
-00011bc0: 2020 2020 2020 2020 3a20 2229 0d0a 2020          : ")..  
-00011bd0: 2020 2020 2020 2020 2020 7768 6973 7065            whispe
-00011be0: 725f 7265 636f 676e 697a 6572 203d 2057  r_recognizer = W
-00011bf0: 6869 7370 6572 5265 636f 676e 697a 6572  hisperRecognizer
-00011c00: 286c 616e 6775 6167 653d 6172 6773 2e73  (language=args.s
-00011c10: 7263 5f6c 616e 6775 6167 652c 206d 6f64  rc_language, mod
-00011c20: 656c 3d6d 6f64 656c 2c20 6670 3136 3d46  el=model, fp16=F
-00011c30: 616c 7365 2c20 7461 736b 3d74 6173 6b2c  alse, task=task,
-00011c40: 2076 6572 626f 7365 3d46 616c 7365 2c20   verbose=False, 
-00011c50: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
-00011c60: 616c 6c62 6163 6b3d 7368 6f77 5f65 7272  allback=show_err
-00011c70: 6f72 5f6d 6573 7361 6765 7329 0d0a 2020  or_messages)..  
-00011c80: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00011c90: 203d 2077 6869 7370 6572 5f72 6563 6f67   = whisper_recog
-00011ca0: 6e69 7a65 7228 7761 765f 6669 6c65 7061  nizer(wav_filepa
-00011cb0: 7468 290d 0a0d 0a20 2020 2020 2020 2020  th)....         
-00011cc0: 2020 2074 696d 6564 5f73 7562 7469 746c     timed_subtitl
-00011cd0: 6573 203d 205b 5d0d 0a20 2020 2020 2020  es = []..       
-00011ce0: 2020 2020 2072 6567 696f 6e73 203d 205b       regions = [
-00011cf0: 5d0d 0a20 2020 2020 2020 2020 2020 2074  ]..            t
-00011d00: 7261 6e73 6372 6970 7473 203d 205b 5d0d  ranscripts = [].
-00011d10: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00011d20: 2073 6567 6d65 6e74 2069 6e20 7265 7375   segment in resu
-00011d30: 6c74 5b27 7365 676d 656e 7473 275d 3a0d  lt['segments']:.
-00011d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011d50: 2073 7461 7274 203d 2073 6567 6d65 6e74   start = segment
-00011d60: 5b27 7374 6172 7427 5d0d 0a20 2020 2020  ['start']..     
-00011d70: 2020 2020 2020 2020 2020 2065 6e64 203d             end =
-00011d80: 2073 6567 6d65 6e74 5b27 656e 6427 5d0d   segment['end'].
-00011d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011da0: 2074 6578 7420 3d20 7365 676d 656e 745b   text = segment[
-00011db0: 2774 6578 7427 5d0d 0a20 2020 2020 2020  'text']..       
-00011dc0: 2020 2020 2020 2020 2072 6567 696f 6e73           regions
-00011dd0: 2e61 7070 656e 6428 2873 7461 7274 2c20  .append((start, 
-00011de0: 656e 6429 290d 0a20 2020 2020 2020 2020  end))..         
-00011df0: 2020 2020 2020 2074 7261 6e73 6372 6970         transcrip
-00011e00: 7473 2e61 7070 656e 6428 7465 7874 290d  ts.append(text).
-00011e10: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
-00011e20: 6564 5f73 7562 7469 746c 6573 203d 205b  ed_subtitles = [
-00011e30: 2872 2c20 7429 2066 6f72 2072 2c20 7420  (r, t) for r, t 
-00011e40: 696e 207a 6970 2872 6567 696f 6e73 2c20  in zip(regions, 
-00011e50: 7472 616e 7363 7269 7074 7329 2069 6620  transcripts) if 
-00011e60: 745d 0d0a 0d0a 2020 2020 2020 2020 2020  t]....          
-00011e70: 2020 7375 6274 6974 6c65 5f66 6f72 6d61    subtitle_forma
-00011e80: 7420 3d20 6172 6773 2e66 6f72 6d61 740d  t = args.format.
-00011e90: 0a20 2020 2020 2020 2020 2020 2062 6173  .            bas
-00011ea0: 652c 2065 7874 203d 206f 732e 7061 7468  e, ext = os.path
-00011eb0: 2e73 706c 6974 6578 7428 6d65 6469 615f  .splitext(media_
-00011ec0: 6669 6c65 7061 7468 290d 0a20 2020 2020  filepath)..     
-00011ed0: 2020 2020 2020 2073 7562 7469 746c 655f         subtitle_
-00011ee0: 6669 6c65 7061 7468 203d 2022 7b62 6173  filepath = "{bas
-00011ef0: 657d 2e7b 666f 726d 6174 7d22 2e66 6f72  e}.{format}".for
-00011f00: 6d61 7428 6261 7365 3d62 6173 652c 2066  mat(base=base, f
-00011f10: 6f72 6d61 743d 7375 6274 6974 6c65 5f66  ormat=subtitle_f
-00011f20: 6f72 6d61 7429 0d0a 0d0a 2020 2020 2020  ormat)....      
-00011f30: 2020 2020 2020 7772 6974 6572 203d 2053        writer = S
-00011f40: 7562 7469 746c 6557 7269 7465 7228 7265  ubtitleWriter(re
-00011f50: 6769 6f6e 732c 2074 7261 6e73 6372 6970  gions, transcrip
-00011f60: 7473 2c20 7375 6274 6974 6c65 5f66 6f72  ts, subtitle_for
-00011f70: 6d61 742c 2065 7272 6f72 5f6d 6573 7361  mat, error_messa
-00011f80: 6765 735f 6361 6c6c 6261 636b 3d73 686f  ges_callback=sho
-00011f90: 775f 6572 726f 725f 6d65 7373 6167 6573  w_error_messages
-00011fa0: 290d 0a20 2020 2020 2020 2020 2020 2077  )..            w
-00011fb0: 7269 7465 722e 7772 6974 6528 7375 6274  riter.write(subt
-00011fc0: 6974 6c65 5f66 696c 6570 6174 6829 0d0a  itle_filepath)..
-00011fd0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00011fe0: 2064 6f5f 7472 616e 736c 6174 653a 0d0a   do_translate:..
-00011ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012000: 2320 434f 4e43 5552 5245 4e54 2054 5241  # CONCURRENT TRA
-00012010: 4e53 4c41 5449 4f4e 2055 5349 4e47 2063  NSLATION USING c
-00012020: 6c61 7373 2053 656e 7465 6e63 6554 7261  lass SentenceTra
-00012030: 6e73 6c61 746f 7228 6f62 6a65 6374 290d  nslator(object).
-00012040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012050: 2023 204e 4f20 4e45 4544 2054 4f20 5452   # NO NEED TO TR
-00012060: 414e 534c 4154 4520 414c 4c20 7472 616e  ANSLATE ALL tran
-00012070: 7363 7269 7074 2049 4e20 7472 616e 7363  script IN transc
-00012080: 7269 7074 730d 0a20 2020 2020 2020 2020  ripts..         
-00012090: 2020 2020 2020 2023 2042 4543 4155 5345         # BECAUSE
-000120a0: 2053 4f4d 4520 7265 6769 6f6e 2049 4e20   SOME region IN 
-000120b0: 7265 6769 6f6e 7320 4d41 5920 4a55 5354  regions MAY JUST
-000120c0: 2048 4156 4520 7472 616e 7363 7269 7074   HAVE transcript
-000120d0: 2057 4954 4820 454d 5054 5920 5354 5249   WITH EMPTY STRI
-000120e0: 4e47 0d0a 2020 2020 2020 2020 2020 2020  NG..            
-000120f0: 2020 2020 2320 4a55 5354 2054 5241 4e53      # JUST TRANS
-00012100: 4c41 5445 2041 4c52 4541 4459 2043 5245  LATE ALREADY CRE
-00012110: 4154 4544 2073 7562 7469 746c 6573 2045  ATED subtitles E
-00012120: 4e54 5249 4553 2046 524f 4d20 7469 6d65  NTRIES FROM time
-00012130: 645f 7375 6274 6974 6c65 730d 0a20 2020  d_subtitles..   
-00012140: 2020 2020 2020 2020 2020 2020 2074 696d               tim
-00012150: 6564 5f73 7562 7469 746c 6573 203d 2077  ed_subtitles = w
-00012160: 7269 7465 722e 7469 6d65 645f 7375 6274  riter.timed_subt
-00012170: 6974 6c65 730d 0a20 2020 2020 2020 2020  itles..         
-00012180: 2020 2020 2020 2063 7265 6174 6564 5f72         created_r
-00012190: 6567 696f 6e73 203d 205b 5d0d 0a20 2020  egions = []..   
-000121a0: 2020 2020 2020 2020 2020 2020 2063 7265               cre
-000121b0: 6174 6564 5f73 7562 7469 746c 6573 203d  ated_subtitles =
-000121c0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-000121d0: 2020 2020 2066 6f72 2065 6e74 7279 2069       for entry i
-000121e0: 6e20 7469 6d65 645f 7375 6274 6974 6c65  n timed_subtitle
-000121f0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00012200: 2020 2020 2020 2020 6372 6561 7465 645f          created_
-00012210: 7265 6769 6f6e 732e 6170 7065 6e64 2865  regions.append(e
-00012220: 6e74 7279 5b30 5d29 0d0a 2020 2020 2020  ntry[0])..      
-00012230: 2020 2020 2020 2020 2020 2020 2020 6372                cr
-00012240: 6561 7465 645f 7375 6274 6974 6c65 732e  eated_subtitles.
-00012250: 6170 7065 6e64 2865 6e74 7279 5b31 5d29  append(entry[1])
-00012260: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00012270: 2020 2020 7072 696e 7428 2254 7261 6e73      print("Trans
-00012280: 6c61 7469 6e67 2066 726f 6d20 2573 2074  lating from %s t
-00012290: 6f20 2573 2020 203a 2022 2025 2873 7263  o %s   : " %(src
+00010ed0: 0a20 2020 2069 6e76 616c 6964 5f6d 6564  .    invalid_med
+00010ee0: 6961 5f66 696c 6570 6174 6873 203d 205b  ia_filepaths = [
+00010ef0: 5d0d 0a20 2020 206e 6f74 5f65 7869 7374  ]..    not_exist
+00010f00: 5f66 696c 6570 6174 6873 203d 205b 5d0d  _filepaths = [].
+00010f10: 0a20 2020 2061 7267 7061 7468 203d 204e  .    argpath = N
+00010f20: 6f6e 650d 0a0d 0a20 2020 2061 7267 735f  one....    args_
+00010f30: 736f 7572 6365 5f70 6174 6820 3d20 6172  source_path = ar
+00010f40: 6773 2e73 6f75 7263 655f 7061 7468 0d0a  gs.source_path..
+00010f50: 0d0a 2020 2020 6966 2028 6e6f 7420 2822  ..    if (not ("
+00010f60: 2a22 2061 6e64 2022 3f22 2920 696e 2073  *" and "?") in s
+00010f70: 7472 2861 7267 735f 736f 7572 6365 5f70  tr(args_source_p
+00010f80: 6174 6829 293a 0d0a 2020 2020 2020 2020  ath)):..        
+00010f90: 666f 7220 6669 6c65 7061 7468 2069 6e20  for filepath in 
+00010fa0: 6172 6773 5f73 6f75 7263 655f 7061 7468  args_source_path
+00010fb0: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
+00010fc0: 7061 7468 203d 2050 6174 6828 6669 6c65  path = Path(file
+00010fd0: 7061 7468 290d 0a20 2020 2020 2020 2020  path)..         
+00010fe0: 2020 2023 7072 696e 7428 2266 7061 7468     #print("fpath
+00010ff0: 203d 2025 7322 2025 6670 6174 6829 0d0a   = %s" %fpath)..
+00011000: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00011010: 6f74 206f 732e 7061 7468 2e69 7366 696c  ot os.path.isfil
+00011020: 6528 6670 6174 6829 3a0d 0a20 2020 2020  e(fpath):..     
+00011030: 2020 2020 2020 2020 2020 206e 6f74 5f65             not_e
+00011040: 7869 7374 5f66 696c 6570 6174 6873 2e61  xist_filepaths.a
+00011050: 7070 656e 6428 6669 6c65 7061 7468 290d  ppend(filepath).
+00011060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011070: 2023 7072 696e 7428 7374 7228 6670 6174   #print(str(fpat
+00011080: 6829 202b 2022 2069 7320 6e6f 7420 6578  h) + " is not ex
+00011090: 6973 7422 290d 0a0d 0a20 2020 2069 6620  ist")....    if 
+000110a0: 7379 732e 706c 6174 666f 726d 203d 3d20  sys.platform == 
+000110b0: 2277 696e 3332 223a 0d0a 2020 2020 2020  "win32":..      
+000110c0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+000110d0: 286c 656e 2861 7267 732e 736f 7572 6365  (len(args.source
+000110e0: 5f70 6174 6829 293a 0d0a 2020 2020 2020  _path)):..      
+000110f0: 2020 2020 2020 6966 2028 225b 2220 6f72        if ("[" or
+00011100: 2022 5d22 2920 696e 2061 7267 732e 736f   "]") in args.so
+00011110: 7572 6365 5f70 6174 685b 695d 3a0d 0a20  urce_path[i]:.. 
+00011120: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00011130: 6c61 6365 686f 6c64 6572 203d 2022 2354  laceholder = "#T
+00011140: 454d 5023 220d 0a20 2020 2020 2020 2020  EMP#"..         
+00011150: 2020 2020 2020 2061 7267 735f 736f 7572         args_sour
+00011160: 6365 5f70 6174 685b 695d 203d 2061 7267  ce_path[i] = arg
+00011170: 732e 736f 7572 6365 5f70 6174 685b 695d  s.source_path[i]
+00011180: 2e72 6570 6c61 6365 2822 5b22 2c20 706c  .replace("[", pl
+00011190: 6163 6568 6f6c 6465 7229 0d0a 2020 2020  aceholder)..    
+000111a0: 2020 2020 2020 2020 2020 2020 6172 6773              args
+000111b0: 5f73 6f75 7263 655f 7061 7468 5b69 5d20  _source_path[i] 
+000111c0: 3d20 6172 6773 5f73 6f75 7263 655f 7061  = args_source_pa
+000111d0: 7468 5b69 5d2e 7265 706c 6163 6528 225d  th[i].replace("]
+000111e0: 222c 2022 5b5d 5d22 290d 0a20 2020 2020  ", "[]]")..     
+000111f0: 2020 2020 2020 2020 2020 2061 7267 735f             args_
+00011200: 736f 7572 6365 5f70 6174 685b 695d 203d  source_path[i] =
+00011210: 2061 7267 735f 736f 7572 6365 5f70 6174   args_source_pat
+00011220: 685b 695d 2e72 6570 6c61 6365 2870 6c61  h[i].replace(pla
+00011230: 6365 686f 6c64 6572 2c20 225b 5b5d 2229  ceholder, "[[]")
+00011240: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011250: 2020 2370 7269 6e74 2822 6172 6773 5f73    #print("args_s
+00011260: 6f75 7263 655f 7061 7468 203d 2025 7322  ource_path = %s"
+00011270: 2025 2861 7267 735f 736f 7572 6365 5f70   %(args_source_p
+00011280: 6174 6829 290d 0a0d 0a20 2020 2066 6f72  ath))....    for
+00011290: 2061 7267 2069 6e20 6172 6773 5f73 6f75   arg in args_sou
+000112a0: 7263 655f 7061 7468 3a0d 0a20 2020 2020  rce_path:..     
+000112b0: 2020 2069 6620 6e6f 7420 7379 732e 706c     if not sys.pl
+000112c0: 6174 666f 726d 203d 3d20 2277 696e 3332  atform == "win32
+000112d0: 2220 3a0d 0a20 2020 2020 2020 2020 2020  " :..           
+000112e0: 2061 7267 203d 2065 7363 6170 6528 6172   arg = escape(ar
+000112f0: 6729 0d0a 0d0a 2020 2020 2020 2020 2370  g)....        #p
+00011300: 7269 6e74 2822 676c 6f62 2861 7267 2920  rint("glob(arg) 
+00011310: 3d20 2573 2220 2528 676c 6f62 2861 7267  = %s" %(glob(arg
+00011320: 2929 290d 0a0d 0a20 2020 2020 2020 2061  )))....        a
+00011330: 7267 5f66 696c 6570 6174 6873 202b 3d20  rg_filepaths += 
+00011340: 676c 6f62 2861 7267 290d 0a0d 0a20 2020  glob(arg)....   
+00011350: 2069 6620 6172 675f 6669 6c65 7061 7468   if arg_filepath
+00011360: 733a 0d0a 2020 2020 2020 2020 666f 7220  s:..        for 
+00011370: 6172 6770 6174 6820 696e 2061 7267 5f66  argpath in arg_f
+00011380: 696c 6570 6174 6873 3a0d 0a20 2020 2020  ilepaths:..     
+00011390: 2020 2020 2020 2069 6620 6f73 2e70 6174         if os.pat
+000113a0: 682e 6973 6669 6c65 2861 7267 7061 7468  h.isfile(argpath
+000113b0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+000113c0: 2020 2020 6966 2063 6865 636b 5f66 696c      if check_fil
+000113d0: 655f 7479 7065 2861 7267 7061 7468 2c20  e_type(argpath, 
+000113e0: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
+000113f0: 616c 6c62 6163 6b3d 7368 6f77 5f65 7272  allback=show_err
+00011400: 6f72 5f6d 6573 7361 6765 7329 203d 3d20  or_messages) == 
+00011410: 2776 6964 656f 2720 6f72 2063 6865 636b  'video' or check
+00011420: 5f66 696c 655f 7479 7065 2861 7267 7061  _file_type(argpa
+00011430: 7468 2c20 6572 726f 725f 6d65 7373 6167  th, error_messag
+00011440: 6573 5f63 616c 6c62 6163 6b3d 7368 6f77  es_callback=show
+00011450: 5f65 7272 6f72 5f6d 6573 7361 6765 7329  _error_messages)
+00011460: 203d 3d20 2761 7564 696f 273a 0d0a 2020   == 'audio':..  
+00011470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011480: 2020 6d65 6469 615f 6669 6c65 7061 7468    media_filepath
+00011490: 732e 6170 7065 6e64 2861 7267 7061 7468  s.append(argpath
+000114a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000114b0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+000114c0: 2020 2020 2020 2020 2020 2020 2020 696e                in
+000114d0: 7661 6c69 645f 6d65 6469 615f 6669 6c65  valid_media_file
+000114e0: 7061 7468 732e 6170 7065 6e64 2861 7267  paths.append(arg
+000114f0: 7061 7468 290d 0a20 2020 2020 2020 2020  path)..         
+00011500: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00011510: 2020 2020 2020 2020 2020 6e6f 745f 6578            not_ex
+00011520: 6973 745f 6669 6c65 7061 7468 732e 6170  ist_filepaths.ap
+00011530: 7065 6e64 2861 7267 7061 7468 290d 0a0d  pend(argpath)...
+00011540: 0a20 2020 2020 2020 2069 6620 696e 7661  .        if inva
+00011550: 6c69 645f 6d65 6469 615f 6669 6c65 7061  lid_media_filepa
+00011560: 7468 733a 0d0a 2020 2020 2020 2020 2020  ths:..          
+00011570: 2020 666f 7220 696e 7661 6c69 645f 6d65    for invalid_me
+00011580: 6469 615f 6669 6c65 7061 7468 2069 6e20  dia_filepath in 
+00011590: 696e 7661 6c69 645f 6d65 6469 615f 6669  invalid_media_fi
+000115a0: 6c65 7061 7468 733a 0d0a 2020 2020 2020  lepaths:..      
+000115b0: 2020 2020 2020 2020 2020 6d73 6720 3d20            msg = 
+000115c0: 227b 7d20 6973 206e 6f74 2076 616c 6964  "{} is not valid
+000115d0: 2076 6964 656f 206f 7220 6175 6469 6f20   video or audio 
+000115e0: 6669 6c65 7322 2e66 6f72 6d61 7428 696e  files".format(in
+000115f0: 7661 6c69 645f 6d65 6469 615f 6669 6c65  valid_media_file
+00011600: 7061 7468 290d 0a20 2020 2020 2020 2020  path)..         
+00011610: 2020 2020 2020 2070 7269 6e74 286d 7367         print(msg
+00011620: 290d 0a0d 0a20 2020 2023 7072 696e 7428  )....    #print(
+00011630: 226e 6f74 5f65 7869 7374 5f66 696c 6570  "not_exist_filep
+00011640: 6174 6873 203d 2025 7322 2025 286e 6f74  aths = %s" %(not
+00011650: 5f65 7869 7374 5f66 696c 6570 6174 6873  _exist_filepaths
+00011660: 2929 0d0a 0d0a 2020 2020 6966 206e 6f74  ))....    if not
+00011670: 5f65 7869 7374 5f66 696c 6570 6174 6873  _exist_filepaths
+00011680: 3a0d 0a20 2020 2020 2020 2066 6f72 206e  :..        for n
+00011690: 6f74 5f65 7869 7374 5f66 696c 6570 6174  ot_exist_filepat
+000116a0: 6820 696e 206e 6f74 5f65 7869 7374 5f66  h in not_exist_f
+000116b0: 696c 6570 6174 6873 3a0d 0a20 2020 2020  ilepaths:..     
+000116c0: 2020 2020 2020 206d 7367 203d 2022 7b7d         msg = "{}
+000116d0: 2069 7320 6e6f 7420 6578 6973 7422 2e66   is not exist".f
+000116e0: 6f72 6d61 7428 6e6f 745f 6578 6973 745f  ormat(not_exist_
+000116f0: 6669 6c65 7061 7468 290d 0a20 2020 2020  filepath)..     
+00011700: 2020 2020 2020 2070 7269 6e74 286d 7367         print(msg
+00011710: 290d 0a20 2020 2020 2020 2069 6620 286e  )..        if (n
+00011720: 6f74 2028 222a 2220 616e 6420 223f 2229  ot ("*" and "?")
+00011730: 2069 6e20 7374 7228 6172 6773 5f73 6f75   in str(args_sou
+00011740: 7263 655f 7061 7468 2929 3a0d 0a20 2020  rce_path)):..   
+00011750: 2020 2020 2020 2020 2073 7973 2e65 7869           sys.exi
+00011760: 7428 3029 0d0a 0d0a 2020 2020 6966 206e  t(0)....    if n
+00011770: 6f74 2061 7267 5f66 696c 6570 6174 6873  ot arg_filepaths
+00011780: 2061 6e64 206e 6f74 206e 6f74 5f65 7869   and not not_exi
+00011790: 7374 5f66 696c 6570 6174 6873 3a0d 0a20  st_filepaths:.. 
+000117a0: 2020 2020 2020 2070 7269 6e74 2822 4e6f         print("No
+000117b0: 2061 6e79 2066 696c 6573 206d 6174 6368   any files match
+000117c0: 696e 6720 6669 6c65 6e61 6d65 7320 796f  ing filenames yo
+000117d0: 7520 7479 7065 6422 290d 0a20 2020 2020  u typed")..     
+000117e0: 2020 2073 7973 2e65 7869 7428 3029 0d0a     sys.exit(0)..
+000117f0: 0d0a 2020 2020 706f 6f6c 203d 206d 756c  ..    pool = mul
+00011800: 7469 7072 6f63 6573 7369 6e67 2e50 6f6f  tiprocessing.Poo
+00011810: 6c28 6172 6773 2e63 6f6e 6375 7272 656e  l(args.concurren
+00011820: 6379 290d 0a0d 0a20 2020 2074 7261 6e73  cy)....    trans
+00011830: 6372 6962 655f 656e 645f 7469 6d65 203d  cribe_end_time =
+00011840: 204e 6f6e 650d 0a20 2020 2074 7261 6e73   None..    trans
+00011850: 6372 6962 655f 656c 6170 7365 645f 7469  cribe_elapsed_ti
+00011860: 6d65 203d 204e 6f6e 650d 0a20 2020 2074  me = None..    t
+00011870: 7261 6e73 6372 6962 655f 7374 6172 745f  ranscribe_start_
+00011880: 7469 6d65 203d 2074 696d 652e 7469 6d65  time = time.time
+00011890: 2829 0d0a 2020 2020 7461 736b 203d 2022  ()..    task = "
+000118a0: 7472 616e 7363 7269 6265 220d 0a0d 0a20  transcribe".... 
+000118b0: 2020 2069 6620 6172 6773 2e73 7263 5f6c     if args.src_l
+000118c0: 616e 6775 6167 6520 3d3d 2028 2262 6122  anguage == ("ba"
+000118d0: 206f 7220 2262 7222 206f 7220 2266 6f22   or "br" or "fo"
+000118e0: 206f 7220 226e 6e22 206f 7220 226f 6322   or "nn" or "oc"
+000118f0: 206f 7220 2274 6c22 206f 7220 2262 6f22   or "tl" or "bo"
+00011900: 2920 616e 6420 646f 5f74 7261 6e73 6c61  ) and do_transla
+00011910: 7465 3a0d 0a20 2020 2020 2020 2074 6173  te:..        tas
+00011920: 6b20 3d20 2274 7261 6e73 6c61 7465 220d  k = "translate".
+00011930: 0a20 2020 2020 2020 2073 7263 5f6c 616e  .        src_lan
+00011940: 6775 6167 6520 3d20 2265 6e22 0d0a 0d0a  guage = "en"....
+00011950: 2020 2020 666f 7220 6d65 6469 615f 6669      for media_fi
+00011960: 6c65 7061 7468 2069 6e20 6d65 6469 615f  lepath in media_
+00011970: 6669 6c65 7061 7468 733a 0d0a 2020 2020  filepaths:..    
+00011980: 2020 2020 7072 696e 7428 2250 726f 6365      print("Proce
+00011990: 7373 696e 6720 7b7d 203a 222e 666f 726d  ssing {} :".form
+000119a0: 6174 286d 6564 6961 5f66 696c 6570 6174  at(media_filepat
+000119b0: 6829 290d 0a0d 0a20 2020 2020 2020 2074  h))....        t
+000119c0: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+000119d0: 2070 7269 6e74 2822 436f 6e76 6572 7469   print("Converti
+000119e0: 6e67 2074 6f20 6120 7465 6d70 6f72 6172  ng to a temporar
+000119f0: 7920 5741 5620 6669 6c65 2020 2020 2020  y WAV file      
+00011a00: 3a20 2229 0d0a 2020 2020 2020 2020 2020  : ")..          
+00011a10: 2020 7769 6467 6574 7320 3d20 5b22 222c    widgets = ["",
+00011a20: 2050 6572 6365 6e74 6167 6528 292c 2027   Percentage(), '
+00011a30: 2027 2c20 4261 7228 6d61 726b 6572 3d27   ', Bar(marker='
+00011a40: e296 8827 292c 2027 2027 2c20 4554 4128  ...'), ' ', ETA(
+00011a50: 295d 0d0a 2020 2020 2020 2020 2020 2020  )]..            
+00011a60: 7062 6172 203d 2050 726f 6772 6573 7342  pbar = ProgressB
+00011a70: 6172 2877 6964 6765 7473 3d77 6964 6765  ar(widgets=widge
+00011a80: 7473 2c20 6d61 7876 616c 3d31 3030 292e  ts, maxval=100).
+00011a90: 7374 6172 7428 290d 0a20 2020 2020 2020  start()..       
+00011aa0: 2020 2020 2077 6176 5f63 6f6e 7665 7274       wav_convert
+00011ab0: 6572 203d 2057 6176 436f 6e76 6572 7465  er = WavConverte
+00011ac0: 7228 7072 6f67 7265 7373 5f63 616c 6c62  r(progress_callb
+00011ad0: 6163 6b3d 7368 6f77 5f70 726f 6772 6573  ack=show_progres
+00011ae0: 732c 2065 7272 6f72 5f6d 6573 7361 6765  s, error_message
+00011af0: 735f 6361 6c6c 6261 636b 3d73 686f 775f  s_callback=show_
+00011b00: 6572 726f 725f 6d65 7373 6167 6573 290d  error_messages).
+00011b10: 0a20 2020 2020 2020 2020 2020 2077 6176  .            wav
+00011b20: 5f66 696c 6570 6174 682c 2073 616d 706c  _filepath, sampl
+00011b30: 655f 7261 7465 203d 2077 6176 5f63 6f6e  e_rate = wav_con
+00011b40: 7665 7274 6572 286d 6564 6961 5f66 696c  verter(media_fil
+00011b50: 6570 6174 6829 0d0a 2020 2020 2020 2020  epath)..        
+00011b60: 2020 2020 7062 6172 2e66 696e 6973 6828      pbar.finish(
+00011b70: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00011b80: 2070 7269 6e74 2822 5065 7266 6f72 6d69   print("Performi
+00011b90: 6e67 2073 7065 6563 6820 7265 636f 676e  ng speech recogn
+00011ba0: 6974 696f 6e20 2020 2020 2020 2020 2020  ition           
+00011bb0: 3a20 2229 0d0a 2020 2020 2020 2020 2020  : ")..          
+00011bc0: 2020 7768 6973 7065 725f 7265 636f 676e    whisper_recogn
+00011bd0: 697a 6572 203d 2057 6869 7370 6572 5265  izer = WhisperRe
+00011be0: 636f 676e 697a 6572 286c 616e 6775 6167  cognizer(languag
+00011bf0: 653d 6172 6773 2e73 7263 5f6c 616e 6775  e=args.src_langu
+00011c00: 6167 652c 206d 6f64 656c 3d6d 6f64 656c  age, model=model
+00011c10: 2c20 6670 3136 3d46 616c 7365 2c20 7461  , fp16=False, ta
+00011c20: 736b 3d74 6173 6b2c 2076 6572 626f 7365  sk=task, verbose
+00011c30: 3d46 616c 7365 2c20 6572 726f 725f 6d65  =False, error_me
+00011c40: 7373 6167 6573 5f63 616c 6c62 6163 6b3d  ssages_callback=
+00011c50: 7368 6f77 5f65 7272 6f72 5f6d 6573 7361  show_error_messa
+00011c60: 6765 7329 0d0a 2020 2020 2020 2020 2020  ges)..          
+00011c70: 2020 7265 7375 6c74 203d 2077 6869 7370    result = whisp
+00011c80: 6572 5f72 6563 6f67 6e69 7a65 7228 7761  er_recognizer(wa
+00011c90: 765f 6669 6c65 7061 7468 290d 0a0d 0a20  v_filepath).... 
+00011ca0: 2020 2020 2020 2020 2020 2074 696d 6564             timed
+00011cb0: 5f73 7562 7469 746c 6573 203d 205b 5d0d  _subtitles = [].
+00011cc0: 0a20 2020 2020 2020 2020 2020 2072 6567  .            reg
+00011cd0: 696f 6e73 203d 205b 5d0d 0a20 2020 2020  ions = []..     
+00011ce0: 2020 2020 2020 2074 7261 6e73 6372 6970         transcrip
+00011cf0: 7473 203d 205b 5d0d 0a20 2020 2020 2020  ts = []..       
+00011d00: 2020 2020 2066 6f72 2073 6567 6d65 6e74       for segment
+00011d10: 2069 6e20 7265 7375 6c74 5b27 7365 676d   in result['segm
+00011d20: 656e 7473 275d 3a0d 0a20 2020 2020 2020  ents']:..       
+00011d30: 2020 2020 2020 2020 2073 7461 7274 203d           start =
+00011d40: 2073 6567 6d65 6e74 5b27 7374 6172 7427   segment['start'
+00011d50: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00011d60: 2020 2065 6e64 203d 2073 6567 6d65 6e74     end = segment
+00011d70: 5b27 656e 6427 5d0d 0a20 2020 2020 2020  ['end']..       
+00011d80: 2020 2020 2020 2020 2074 6578 7420 3d20           text = 
+00011d90: 7365 676d 656e 745b 2774 6578 7427 5d0d  segment['text'].
+00011da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011db0: 2072 6567 696f 6e73 2e61 7070 656e 6428   regions.append(
+00011dc0: 2873 7461 7274 2c20 656e 6429 290d 0a20  (start, end)).. 
+00011dd0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00011de0: 7261 6e73 6372 6970 7473 2e61 7070 656e  ranscripts.appen
+00011df0: 6428 7465 7874 290d 0a20 2020 2020 2020  d(text)..       
+00011e00: 2020 2020 2074 696d 6564 5f73 7562 7469       timed_subti
+00011e10: 746c 6573 203d 205b 2872 2c20 7429 2066  tles = [(r, t) f
+00011e20: 6f72 2072 2c20 7420 696e 207a 6970 2872  or r, t in zip(r
+00011e30: 6567 696f 6e73 2c20 7472 616e 7363 7269  egions, transcri
+00011e40: 7074 7329 2069 6620 745d 0d0a 0d0a 2020  pts) if t]....  
+00011e50: 2020 2020 2020 2020 2020 7375 6274 6974            subtit
+00011e60: 6c65 5f66 6f72 6d61 7420 3d20 6172 6773  le_format = args
+00011e70: 2e66 6f72 6d61 740d 0a20 2020 2020 2020  .format..       
+00011e80: 2020 2020 2062 6173 652c 2065 7874 203d       base, ext =
+00011e90: 206f 732e 7061 7468 2e73 706c 6974 6578   os.path.splitex
+00011ea0: 7428 6d65 6469 615f 6669 6c65 7061 7468  t(media_filepath
+00011eb0: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+00011ec0: 7562 7469 746c 655f 6669 6c65 7061 7468  ubtitle_filepath
+00011ed0: 203d 2022 7b62 6173 657d 2e7b 666f 726d   = "{base}.{form
+00011ee0: 6174 7d22 2e66 6f72 6d61 7428 6261 7365  at}".format(base
+00011ef0: 3d62 6173 652c 2066 6f72 6d61 743d 7375  =base, format=su
+00011f00: 6274 6974 6c65 5f66 6f72 6d61 7429 0d0a  btitle_format)..
+00011f10: 0d0a 2020 2020 2020 2020 2020 2020 7772  ..            wr
+00011f20: 6974 6572 203d 2053 7562 7469 746c 6557  iter = SubtitleW
+00011f30: 7269 7465 7228 7265 6769 6f6e 732c 2074  riter(regions, t
+00011f40: 7261 6e73 6372 6970 7473 2c20 7375 6274  ranscripts, subt
+00011f50: 6974 6c65 5f66 6f72 6d61 742c 2065 7272  itle_format, err
+00011f60: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
+00011f70: 6261 636b 3d73 686f 775f 6572 726f 725f  back=show_error_
+00011f80: 6d65 7373 6167 6573 290d 0a20 2020 2020  messages)..     
+00011f90: 2020 2020 2020 2077 7269 7465 722e 7772         writer.wr
+00011fa0: 6974 6528 7375 6274 6974 6c65 5f66 696c  ite(subtitle_fil
+00011fb0: 6570 6174 6829 0d0a 0d0a 2020 2020 2020  epath)....      
+00011fc0: 2020 2020 2020 6966 2064 6f5f 7472 616e        if do_tran
+00011fd0: 736c 6174 653a 0d0a 2020 2020 2020 2020  slate:..        
+00011fe0: 2020 2020 2020 2020 2320 434f 4e43 5552          # CONCUR
+00011ff0: 5245 4e54 2054 5241 4e53 4c41 5449 4f4e  RENT TRANSLATION
+00012000: 2055 5349 4e47 2063 6c61 7373 2053 656e   USING class Sen
+00012010: 7465 6e63 6554 7261 6e73 6c61 746f 7228  tenceTranslator(
+00012020: 6f62 6a65 6374 290d 0a20 2020 2020 2020  object)..       
+00012030: 2020 2020 2020 2020 2023 204e 4f20 4e45           # NO NE
+00012040: 4544 2054 4f20 5452 414e 534c 4154 4520  ED TO TRANSLATE 
+00012050: 414c 4c20 7472 616e 7363 7269 7074 2049  ALL transcript I
+00012060: 4e20 7472 616e 7363 7269 7074 730d 0a20  N transcripts.. 
+00012070: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00012080: 2042 4543 4155 5345 2053 4f4d 4520 7265   BECAUSE SOME re
+00012090: 6769 6f6e 2049 4e20 7265 6769 6f6e 7320  gion IN regions 
+000120a0: 4d41 5920 4a55 5354 2048 4156 4520 7472  MAY JUST HAVE tr
+000120b0: 616e 7363 7269 7074 2057 4954 4820 454d  anscript WITH EM
+000120c0: 5054 5920 5354 5249 4e47 0d0a 2020 2020  PTY STRING..    
+000120d0: 2020 2020 2020 2020 2020 2020 2320 4a55              # JU
+000120e0: 5354 2054 5241 4e53 4c41 5445 2041 4c52  ST TRANSLATE ALR
+000120f0: 4541 4459 2043 5245 4154 4544 2073 7562  EADY CREATED sub
+00012100: 7469 746c 6573 2045 4e54 5249 4553 2046  titles ENTRIES F
+00012110: 524f 4d20 7469 6d65 645f 7375 6274 6974  ROM timed_subtit
+00012120: 6c65 730d 0a20 2020 2020 2020 2020 2020  les..           
+00012130: 2020 2020 2074 696d 6564 5f73 7562 7469       timed_subti
+00012140: 746c 6573 203d 2077 7269 7465 722e 7469  tles = writer.ti
+00012150: 6d65 645f 7375 6274 6974 6c65 730d 0a20  med_subtitles.. 
+00012160: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00012170: 7265 6174 6564 5f72 6567 696f 6e73 203d  reated_regions =
+00012180: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00012190: 2020 2020 2063 7265 6174 6564 5f73 7562       created_sub
+000121a0: 7469 746c 6573 203d 205b 5d0d 0a20 2020  titles = []..   
+000121b0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+000121c0: 2065 6e74 7279 2069 6e20 7469 6d65 645f   entry in timed_
+000121d0: 7375 6274 6974 6c65 733a 0d0a 2020 2020  subtitles:..    
+000121e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000121f0: 6372 6561 7465 645f 7265 6769 6f6e 732e  created_regions.
+00012200: 6170 7065 6e64 2865 6e74 7279 5b30 5d29  append(entry[0])
+00012210: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012220: 2020 2020 2020 6372 6561 7465 645f 7375        created_su
+00012230: 6274 6974 6c65 732e 6170 7065 6e64 2865  btitles.append(e
+00012240: 6e74 7279 5b31 5d29 0d0a 0d0a 2020 2020  ntry[1])....    
+00012250: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00012260: 7428 2254 7261 6e73 6c61 7469 6e67 2066  t("Translating f
+00012270: 726f 6d20 2573 2074 6f20 2573 2020 203a  rom %s to %s   :
+00012280: 2022 2025 2873 7263 5f6c 616e 6775 6167   " %(src_languag
+00012290: 652e 6365 6e74 6572 2838 292c 2064 7374  e.center(8), dst
 000122a0: 5f6c 616e 6775 6167 652e 6365 6e74 6572  _language.center
-000122b0: 2838 292c 2064 7374 5f6c 616e 6775 6167  (8), dst_languag
-000122c0: 652e 6365 6e74 6572 2838 2929 290d 0a20  e.center(8))).. 
-000122d0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-000122e0: 6964 6765 7473 203d 205b 2222 2c20 5065  idgets = ["", Pe
-000122f0: 7263 656e 7461 6765 2829 2c20 2720 272c  rcentage(), ' ',
-00012300: 2042 6172 286d 6172 6b65 723d 27e2 9688   Bar(marker='...
-00012310: 2729 2c20 2720 272c 2045 5441 2829 5d0d  '), ' ', ETA()].
-00012320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012330: 2070 6261 7220 3d20 5072 6f67 7265 7373   pbar = Progress
-00012340: 4261 7228 7769 6467 6574 733d 7769 6467  Bar(widgets=widg
-00012350: 6574 732c 206d 6178 7661 6c3d 6c65 6e28  ets, maxval=len(
-00012360: 7469 6d65 645f 7375 6274 6974 6c65 7329  timed_subtitles)
-00012370: 292e 7374 6172 7428 290d 0a0d 0a20 2020  ).start()....   
-00012380: 2020 2020 2020 2020 2020 2020 2074 7261               tra
-00012390: 6e73 6372 6970 745f 7472 616e 736c 6174  nscript_translat
-000123a0: 6f72 203d 2053 656e 7465 6e63 6554 7261  or = SentenceTra
-000123b0: 6e73 6c61 746f 7228 7372 633d 6172 6773  nslator(src=args
-000123c0: 2e73 7263 5f6c 616e 6775 6167 652c 2064  .src_language, d
-000123d0: 7374 3d61 7267 732e 6473 745f 6c61 6e67  st=args.dst_lang
-000123e0: 7561 6765 2c20 6572 726f 725f 6d65 7373  uage, error_mess
-000123f0: 6167 6573 5f63 616c 6c62 6163 6b3d 7368  ages_callback=sh
-00012400: 6f77 5f65 7272 6f72 5f6d 6573 7361 6765  ow_error_message
-00012410: 7329 0d0a 0d0a 2020 2020 2020 2020 2020  s)....          
-00012420: 2020 2020 2020 7472 616e 736c 6174 6564        translated
-00012430: 5f73 7562 7469 746c 6573 203d 205b 5d0d  _subtitles = [].
-00012440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012450: 2066 6f72 2069 2c20 7472 616e 736c 6174   for i, translat
-00012460: 6564 5f73 7562 7469 746c 6520 696e 2065  ed_subtitle in e
-00012470: 6e75 6d65 7261 7465 2870 6f6f 6c2e 696d  numerate(pool.im
-00012480: 6170 2874 7261 6e73 6372 6970 745f 7472  ap(transcript_tr
-00012490: 616e 736c 6174 6f72 2c20 6372 6561 7465  anslator, create
-000124a0: 645f 7375 6274 6974 6c65 7329 293a 0d0a  d_subtitles)):..
-000124b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124c0: 2020 2020 7472 616e 736c 6174 6564 5f73      translated_s
-000124d0: 7562 7469 746c 6573 2e61 7070 656e 6428  ubtitles.append(
-000124e0: 7472 616e 736c 6174 6564 5f73 7562 7469  translated_subti
-000124f0: 746c 6529 0d0a 2020 2020 2020 2020 2020  tle)..          
-00012500: 2020 2020 2020 2020 2020 7062 6172 2e75            pbar.u
-00012510: 7064 6174 6528 6929 0d0a 2020 2020 2020  pdate(i)..      
-00012520: 2020 2020 2020 2020 2020 7062 6172 2e66            pbar.f
-00012530: 696e 6973 6828 290d 0a0d 0a20 2020 2020  inish()....     
-00012540: 2020 2020 2020 2020 2020 2074 7261 6e73             trans
-00012550: 6c61 7465 645f 7375 6274 6974 6c65 5f66  lated_subtitle_f
-00012560: 696c 6570 6174 6820 3d20 7375 6274 6974  ilepath = subtit
-00012570: 6c65 5f66 696c 6570 6174 685b 203a 2d34  le_filepath[ :-4
-00012580: 5d20 2b20 272e 7472 616e 736c 6174 6564  ] + '.translated
-00012590: 2e27 202b 2073 7562 7469 746c 655f 666f  .' + subtitle_fo
-000125a0: 726d 6174 0d0a 2020 2020 2020 2020 2020  rmat..          
-000125b0: 2020 2020 2020 7472 616e 736c 6174 696f        translatio
-000125c0: 6e5f 7772 6974 6572 203d 2053 7562 7469  n_writer = Subti
-000125d0: 746c 6557 7269 7465 7228 6372 6561 7465  tleWriter(create
-000125e0: 645f 7265 6769 6f6e 732c 2074 7261 6e73  d_regions, trans
-000125f0: 6c61 7465 645f 7375 6274 6974 6c65 732c  lated_subtitles,
-00012600: 2073 7562 7469 746c 655f 666f 726d 6174   subtitle_format
-00012610: 2c20 6572 726f 725f 6d65 7373 6167 6573  , error_messages
-00012620: 5f63 616c 6c62 6163 6b3d 7368 6f77 5f65  _callback=show_e
-00012630: 7272 6f72 5f6d 6573 7361 6765 7329 0d0a  rror_messages)..
-00012640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012650: 7472 616e 736c 6174 696f 6e5f 7772 6974  translation_writ
-00012660: 6572 2e77 7269 7465 2874 7261 6e73 6c61  er.write(transla
-00012670: 7465 645f 7375 6274 6974 6c65 5f66 696c  ted_subtitle_fil
-00012680: 6570 6174 6829 0d0a 0d0a 2020 2020 2020  epath)....      
-00012690: 2020 2020 2020 7072 696e 7428 2744 6f6e        print('Don
-000126a0: 652e 2729 0d0a 2020 2020 2020 2020 2020  e.')..          
-000126b0: 2020 6966 2064 6f5f 7472 616e 736c 6174    if do_translat
-000126c0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000126d0: 2020 2020 2370 7269 6e74 2822 4f72 6967      #print("Orig
-000126e0: 696e 616c 2073 7562 7469 746c 6573 2066  inal subtitles f
-000126f0: 696c 6520 6372 6561 7465 6420 6174 2020  ile created at  
-00012700: 2020 2020 3a20 7b7d 222e 666f 726d 6174      : {}".format
-00012710: 2873 7562 7469 746c 655f 6669 6c65 7061  (subtitle_filepa
-00012720: 7468 2929 0d0a 2020 2020 2020 2020 2020  th))..          
-00012730: 2020 2020 2020 6f73 2e72 656d 6f76 6528        os.remove(
-00012740: 7375 6274 6974 6c65 5f66 696c 6570 6174  subtitle_filepat
-00012750: 6829 0d0a 2020 2020 2020 2020 2020 2020  h)..            
-00012760: 2020 2020 7072 696e 7428 2754 7261 6e73      print('Trans
-00012770: 6c61 7465 6420 7375 6274 6974 6c65 7320  lated subtitles 
-00012780: 6669 6c65 2063 7265 6174 6564 2061 7420  file created at 
-00012790: 2020 203a 207b 7d27 202e 666f 726d 6174     : {}' .format
-000127a0: 2874 7261 6e73 6c61 7465 645f 7375 6274  (translated_subt
-000127b0: 6974 6c65 5f66 696c 6570 6174 6829 290d  itle_filepath)).
-000127c0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-000127d0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000127e0: 2020 2020 7072 696e 7428 2253 7562 7469      print("Subti
-000127f0: 746c 6573 2066 696c 6520 6372 6561 7465  tles file create
-00012800: 6420 6174 2020 2020 2020 2020 2020 2020  d at            
-00012810: 2020 203a 207b 7d22 2e66 6f72 6d61 7428     : {}".format(
-00012820: 7375 6274 6974 6c65 5f66 696c 6570 6174  subtitle_filepat
-00012830: 6829 290d 0a20 2020 2020 2020 2020 2020  h))..           
-00012840: 2070 7269 6e74 2827 2729 0d0a 2020 2020   print('')..    
-00012850: 2020 2020 2020 2020 636f 6d70 6c65 7465          complete
-00012860: 645f 7461 736b 7320 2b3d 2031 0d0a 0d0a  d_tasks += 1....
-00012870: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-00012880: 656e 286d 6564 6961 5f66 696c 6570 6174  en(media_filepat
-00012890: 6873 293e 3020 616e 6420 636f 6d70 6c65  hs)>0 and comple
-000128a0: 7465 645f 7461 736b 7320 3d3d 206c 656e  ted_tasks == len
-000128b0: 286d 6564 6961 5f66 696c 6570 6174 6873  (media_filepaths
-000128c0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000128d0: 2020 2020 7472 616e 7363 7269 6265 5f65      transcribe_e
-000128e0: 6e64 5f74 696d 6520 3d20 7469 6d65 2e74  nd_time = time.t
-000128f0: 696d 6528 290d 0a20 2020 2020 2020 2020  ime()..         
-00012900: 2020 2020 2020 2074 7261 6e73 6372 6962         transcrib
-00012910: 655f 656c 6170 7365 645f 7469 6d65 203d  e_elapsed_time =
-00012920: 2074 7261 6e73 6372 6962 655f 656e 645f   transcribe_end_
-00012930: 7469 6d65 202d 2074 7261 6e73 6372 6962  time - transcrib
-00012940: 655f 7374 6172 745f 7469 6d65 0d0a 2020  e_start_time..  
-00012950: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-00012960: 616e 7363 7269 6265 5f65 6c61 7073 6564  anscribe_elapsed
-00012970: 5f74 696d 655f 7365 636f 6e64 7320 3d20  _time_seconds = 
-00012980: 7469 6d65 6465 6c74 6128 7365 636f 6e64  timedelta(second
-00012990: 733d 696e 7428 7472 616e 7363 7269 6265  s=int(transcribe
-000129a0: 5f65 6c61 7073 6564 5f74 696d 6529 290d  _elapsed_time)).
-000129b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000129c0: 2074 7261 6e73 6372 6962 655f 656c 6170   transcribe_elap
-000129d0: 7365 645f 7469 6d65 5f73 7472 203d 2073  sed_time_str = s
-000129e0: 7472 2874 7261 6e73 6372 6962 655f 656c  tr(transcribe_el
-000129f0: 6170 7365 645f 7469 6d65 5f73 6563 6f6e  apsed_time_secon
-00012a00: 6473 290d 0a20 2020 2020 2020 2020 2020  ds)..           
-00012a10: 2020 2020 2068 6f75 722c 206d 696e 7574       hour, minut
-00012a20: 652c 2073 6563 6f6e 6420 3d20 7472 616e  e, second = tran
-00012a30: 7363 7269 6265 5f65 6c61 7073 6564 5f74  scribe_elapsed_t
-00012a40: 696d 655f 7374 722e 7370 6c69 7428 223a  ime_str.split(":
-00012a50: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-00012a60: 2020 2020 6d73 6720 3d20 2254 6f74 616c      msg = "Total
-00012a70: 2074 7261 6e73 6372 6962 6520 7469 6d65   transcribe time
-00012a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a90: 2020 203a 2025 733a 2573 3a25 7322 2025     : %s:%s:%s" %
-00012aa0: 2868 6f75 722e 7a66 696c 6c28 3229 2c20  (hour.zfill(2), 
-00012ab0: 6d69 6e75 7465 2c20 7365 636f 6e64 290d  minute, second).
-00012ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012ad0: 2070 7269 6e74 286d 7367 290d 0a0d 0a20   print(msg).... 
-00012ae0: 2020 2020 2020 2065 7863 6570 7420 4b65         except Ke
-00012af0: 7962 6f61 7264 496e 7465 7272 7570 743a  yboardInterrupt:
-00012b00: 0d0a 2020 2020 2020 2020 2020 2020 7062  ..            pb
-00012b10: 6172 2e66 696e 6973 6828 290d 0a20 2020  ar.finish()..   
-00012b20: 2020 2020 2020 2020 2070 6f6f 6c2e 7465           pool.te
-00012b30: 726d 696e 6174 6528 290d 0a20 2020 2020  rminate()..     
-00012b40: 2020 2020 2020 2070 6f6f 6c2e 636c 6f73         pool.clos
-00012b50: 6528 290d 0a20 2020 2020 2020 2020 2020  e()..           
-00012b60: 2070 6f6f 6c2e 6a6f 696e 2829 0d0a 2020   pool.join()..  
-00012b70: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00012b80: 2243 616e 6365 6c6c 696e 6720 616c 6c20  "Cancelling all 
-00012b90: 7461 736b 7322 290d 0a0d 0a20 2020 2020  tasks")....     
-00012ba0: 2020 2020 2020 2069 6620 7379 732e 706c         if sys.pl
-00012bb0: 6174 666f 726d 203d 3d20 2277 696e 3332  atform == "win32
-00012bc0: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
-00012bd0: 2020 2020 7374 6f70 5f66 666d 7065 675f      stop_ffmpeg_
-00012be0: 7769 6e64 6f77 7328 6572 726f 725f 6d65  windows(error_me
-00012bf0: 7373 6167 6573 5f63 616c 6c62 6163 6b3d  ssages_callback=
-00012c00: 7368 6f77 5f65 7272 6f72 5f6d 6573 7361  show_error_messa
-00012c10: 6765 7329 0d0a 2020 2020 2020 2020 2020  ges)..          
-00012c20: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00012c30: 2020 2020 2020 2020 2073 746f 705f 6666           stop_ff
-00012c40: 6d70 6567 5f6c 696e 7578 2865 7272 6f72  mpeg_linux(error
-00012c50: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
-00012c60: 636b 3d73 686f 775f 6572 726f 725f 6d65  ck=show_error_me
-00012c70: 7373 6167 6573 290d 0a0d 0a20 2020 2020  ssages)....     
-00012c80: 2020 2020 2020 2072 656d 6f76 655f 7465         remove_te
-00012c90: 6d70 5f66 696c 6573 2822 666c 6163 2229  mp_files("flac")
-00012ca0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00012cb0: 6d6f 7665 5f74 656d 705f 6669 6c65 7328  move_temp_files(
-00012cc0: 2277 6176 2229 0d0a 2020 2020 2020 2020  "wav")..        
-00012cd0: 2020 2020 7265 7475 726e 2031 0d0a 0d0a      return 1....
-00012ce0: 2020 2020 2020 2020 6578 6365 7074 2045          except E
-00012cf0: 7863 6570 7469 6f6e 2061 7320 653a 0d0a  xception as e:..
-00012d00: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00012d10: 6f74 204b 6579 626f 6172 6449 6e74 6572  ot KeyboardInter
-00012d20: 7275 7074 2069 6e20 653a 0d0a 2020 2020  rupt in e:..    
-00012d30: 2020 2020 2020 2020 2020 2020 7062 6172              pbar
-00012d40: 2e66 696e 6973 6828 290d 0a20 2020 2020  .finish()..     
-00012d50: 2020 2020 2020 2020 2020 2070 6f6f 6c2e             pool.
-00012d60: 7465 726d 696e 6174 6528 290d 0a20 2020  terminate()..   
-00012d70: 2020 2020 2020 2020 2020 2020 2070 6f6f               poo
-00012d80: 6c2e 636c 6f73 6528 290d 0a20 2020 2020  l.close()..     
-00012d90: 2020 2020 2020 2020 2020 2070 6f6f 6c2e             pool.
-00012da0: 6a6f 696e 2829 0d0a 2020 2020 2020 2020  join()..        
-00012db0: 2020 2020 2020 2020 7072 696e 7428 6529          print(e)
-00012dc0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00012dd0: 2020 2020 6966 2073 7973 2e70 6c61 7466      if sys.platf
-00012de0: 6f72 6d20 3d3d 2022 7769 6e33 3222 3a0d  orm == "win32":.
-00012df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012e00: 2020 2020 2073 746f 705f 6666 6d70 6567       stop_ffmpeg
-00012e10: 5f77 696e 646f 7773 2865 7272 6f72 5f6d  _windows(error_m
-00012e20: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
-00012e30: 3d73 686f 775f 6572 726f 725f 6d65 7373  =show_error_mess
-00012e40: 6167 6573 290d 0a20 2020 2020 2020 2020  ages)..         
-00012e50: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00012e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e70: 2020 7374 6f70 5f66 666d 7065 675f 6c69    stop_ffmpeg_li
-00012e80: 6e75 7828 6572 726f 725f 6d65 7373 6167  nux(error_messag
-00012e90: 6573 5f63 616c 6c62 6163 6b3d 7368 6f77  es_callback=show
-00012ea0: 5f65 7272 6f72 5f6d 6573 7361 6765 7329  _error_messages)
-00012eb0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00012ec0: 2020 2020 7265 6d6f 7665 5f74 656d 705f      remove_temp_
-00012ed0: 6669 6c65 7328 2266 6c61 6322 290d 0a20  files("flac").. 
-00012ee0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00012ef0: 656d 6f76 655f 7465 6d70 5f66 696c 6573  emove_temp_files
-00012f00: 2822 7761 7622 290d 0a20 2020 2020 2020  ("wav")..       
-00012f10: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00012f20: 310d 0a0d 0a20 2020 2069 6620 706f 6f6c  1....    if pool
-00012f30: 3a0d 0a20 2020 2020 2020 2070 6f6f 6c2e  :..        pool.
-00012f40: 636c 6f73 6528 290d 0a20 2020 2020 2020  close()..       
-00012f50: 2070 6f6f 6c2e 6a6f 696e 2829 0d0a 2020   pool.join()..  
-00012f60: 2020 2020 2020 706f 6f6c 203d 204e 6f6e        pool = Non
-00012f70: 650d 0a0d 0a20 2020 2069 6620 7379 732e  e....    if sys.
-00012f80: 706c 6174 666f 726d 203d 3d20 2277 696e  platform == "win
-00012f90: 3332 223a 0d0a 2020 2020 2020 2020 7374  32":..        st
-00012fa0: 6f70 5f66 666d 7065 675f 7769 6e64 6f77  op_ffmpeg_window
-00012fb0: 7328 6572 726f 725f 6d65 7373 6167 6573  s(error_messages
-00012fc0: 5f63 616c 6c62 6163 6b3d 7368 6f77 5f65  _callback=show_e
-00012fd0: 7272 6f72 5f6d 6573 7361 6765 7329 0d0a  rror_messages)..
-00012fe0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00012ff0: 2020 2073 746f 705f 6666 6d70 6567 5f6c     stop_ffmpeg_l
-00013000: 696e 7578 2865 7272 6f72 5f6d 6573 7361  inux(error_messa
-00013010: 6765 735f 6361 6c6c 6261 636b 3d73 686f  ges_callback=sho
-00013020: 775f 6572 726f 725f 6d65 7373 6167 6573  w_error_messages
-00013030: 290d 0a0d 0a20 2020 2072 656d 6f76 655f  )....    remove_
-00013040: 7465 6d70 5f66 696c 6573 2822 666c 6163  temp_files("flac
-00013050: 2229 0d0a 2020 2020 7265 6d6f 7665 5f74  ")..    remove_t
-00013060: 656d 705f 6669 6c65 7328 2277 6176 2229  emp_files("wav")
-00013070: 0d0a 0d0a 6966 205f 5f6e 616d 655f 5f20  ....if __name__ 
-00013080: 3d3d 2027 5f5f 6d61 696e 5f5f 273a 0d0a  == '__main__':..
-00013090: 2020 2020 6d75 6c74 6970 726f 6365 7373      multiprocess
-000130a0: 696e 672e 6672 6565 7a65 5f73 7570 706f  ing.freeze_suppo
-000130b0: 7274 2829 0d0a 2020 2020 7379 732e 6578  rt()..    sys.ex
-000130c0: 6974 286d 6169 6e28 2929 0d0a            it(main())..
+000122b0: 2838 2929 290d 0a20 2020 2020 2020 2020  (8)))..         
+000122c0: 2020 2020 2020 2077 6964 6765 7473 203d         widgets =
+000122d0: 205b 2222 2c20 5065 7263 656e 7461 6765   ["", Percentage
+000122e0: 2829 2c20 2720 272c 2042 6172 286d 6172  (), ' ', Bar(mar
+000122f0: 6b65 723d 27e2 9688 2729 2c20 2720 272c  ker='...'), ' ',
+00012300: 2045 5441 2829 5d0d 0a20 2020 2020 2020   ETA()]..       
+00012310: 2020 2020 2020 2020 2070 6261 7220 3d20           pbar = 
+00012320: 5072 6f67 7265 7373 4261 7228 7769 6467  ProgressBar(widg
+00012330: 6574 733d 7769 6467 6574 732c 206d 6178  ets=widgets, max
+00012340: 7661 6c3d 6c65 6e28 7469 6d65 645f 7375  val=len(timed_su
+00012350: 6274 6974 6c65 7329 292e 7374 6172 7428  btitles)).start(
+00012360: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00012370: 2020 2020 2074 7261 6e73 6372 6970 745f       transcript_
+00012380: 7472 616e 736c 6174 6f72 203d 2053 656e  translator = Sen
+00012390: 7465 6e63 6554 7261 6e73 6c61 746f 7228  tenceTranslator(
+000123a0: 7372 633d 6172 6773 2e73 7263 5f6c 616e  src=args.src_lan
+000123b0: 6775 6167 652c 2064 7374 3d61 7267 732e  guage, dst=args.
+000123c0: 6473 745f 6c61 6e67 7561 6765 2c20 6572  dst_language, er
+000123d0: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
+000123e0: 6c62 6163 6b3d 7368 6f77 5f65 7272 6f72  lback=show_error
+000123f0: 5f6d 6573 7361 6765 7329 0d0a 0d0a 2020  _messages)....  
+00012400: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00012410: 616e 736c 6174 6564 5f73 7562 7469 746c  anslated_subtitl
+00012420: 6573 203d 205b 5d0d 0a20 2020 2020 2020  es = []..       
+00012430: 2020 2020 2020 2020 2066 6f72 2069 2c20           for i, 
+00012440: 7472 616e 736c 6174 6564 5f73 7562 7469  translated_subti
+00012450: 746c 6520 696e 2065 6e75 6d65 7261 7465  tle in enumerate
+00012460: 2870 6f6f 6c2e 696d 6170 2874 7261 6e73  (pool.imap(trans
+00012470: 6372 6970 745f 7472 616e 736c 6174 6f72  cript_translator
+00012480: 2c20 6372 6561 7465 645f 7375 6274 6974  , created_subtit
+00012490: 6c65 7329 293a 0d0a 2020 2020 2020 2020  les)):..        
+000124a0: 2020 2020 2020 2020 2020 2020 7472 616e              tran
+000124b0: 736c 6174 6564 5f73 7562 7469 746c 6573  slated_subtitles
+000124c0: 2e61 7070 656e 6428 7472 616e 736c 6174  .append(translat
+000124d0: 6564 5f73 7562 7469 746c 6529 0d0a 2020  ed_subtitle)..  
+000124e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000124f0: 2020 7062 6172 2e75 7064 6174 6528 6929    pbar.update(i)
+00012500: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012510: 2020 7062 6172 2e66 696e 6973 6828 290d    pbar.finish().
+00012520: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00012530: 2020 2074 7261 6e73 6c61 7465 645f 7375     translated_su
+00012540: 6274 6974 6c65 5f66 696c 6570 6174 6820  btitle_filepath 
+00012550: 3d20 7375 6274 6974 6c65 5f66 696c 6570  = subtitle_filep
+00012560: 6174 685b 203a 2d34 5d20 2b20 272e 7472  ath[ :-4] + '.tr
+00012570: 616e 736c 6174 6564 2e27 202b 2073 7562  anslated.' + sub
+00012580: 7469 746c 655f 666f 726d 6174 0d0a 2020  title_format..  
+00012590: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+000125a0: 616e 736c 6174 696f 6e5f 7772 6974 6572  anslation_writer
+000125b0: 203d 2053 7562 7469 746c 6557 7269 7465   = SubtitleWrite
+000125c0: 7228 6372 6561 7465 645f 7265 6769 6f6e  r(created_region
+000125d0: 732c 2074 7261 6e73 6c61 7465 645f 7375  s, translated_su
+000125e0: 6274 6974 6c65 732c 2073 7562 7469 746c  btitles, subtitl
+000125f0: 655f 666f 726d 6174 2c20 6572 726f 725f  e_format, error_
+00012600: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
+00012610: 6b3d 7368 6f77 5f65 7272 6f72 5f6d 6573  k=show_error_mes
+00012620: 7361 6765 7329 0d0a 2020 2020 2020 2020  sages)..        
+00012630: 2020 2020 2020 2020 7472 616e 736c 6174          translat
+00012640: 696f 6e5f 7772 6974 6572 2e77 7269 7465  ion_writer.write
+00012650: 2874 7261 6e73 6c61 7465 645f 7375 6274  (translated_subt
+00012660: 6974 6c65 5f66 696c 6570 6174 6829 0d0a  itle_filepath)..
+00012670: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+00012680: 696e 7428 2744 6f6e 652e 2729 0d0a 2020  int('Done.')..  
+00012690: 2020 2020 2020 2020 2020 6966 2064 6f5f            if do_
+000126a0: 7472 616e 736c 6174 653a 0d0a 2020 2020  translate:..    
+000126b0: 2020 2020 2020 2020 2020 2020 2370 7269              #pri
+000126c0: 6e74 2822 4f72 6967 696e 616c 2073 7562  nt("Original sub
+000126d0: 7469 746c 6573 2066 696c 6520 6372 6561  titles file crea
+000126e0: 7465 6420 6174 2020 2020 2020 3a20 7b7d  ted at      : {}
+000126f0: 222e 666f 726d 6174 2873 7562 7469 746c  ".format(subtitl
+00012700: 655f 6669 6c65 7061 7468 2929 0d0a 2020  e_filepath))..  
+00012710: 2020 2020 2020 2020 2020 2020 2020 6f73                os
+00012720: 2e72 656d 6f76 6528 7375 6274 6974 6c65  .remove(subtitle
+00012730: 5f66 696c 6570 6174 6829 0d0a 2020 2020  _filepath)..    
+00012740: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00012750: 7428 2754 7261 6e73 6c61 7465 6420 7375  t('Translated su
+00012760: 6274 6974 6c65 7320 6669 6c65 2063 7265  btitles file cre
+00012770: 6174 6564 2061 7420 2020 203a 207b 7d27  ated at    : {}'
+00012780: 202e 666f 726d 6174 2874 7261 6e73 6c61   .format(transla
+00012790: 7465 645f 7375 6274 6974 6c65 5f66 696c  ted_subtitle_fil
+000127a0: 6570 6174 6829 290d 0a20 2020 2020 2020  epath))..       
+000127b0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+000127c0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+000127d0: 7428 2253 7562 7469 746c 6573 2066 696c  t("Subtitles fil
+000127e0: 6520 6372 6561 7465 6420 6174 2020 2020  e created at    
+000127f0: 2020 2020 2020 2020 2020 203a 207b 7d22             : {}"
+00012800: 2e66 6f72 6d61 7428 7375 6274 6974 6c65  .format(subtitle
+00012810: 5f66 696c 6570 6174 6829 290d 0a20 2020  _filepath))..   
+00012820: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
+00012830: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
+00012840: 636f 6d70 6c65 7465 645f 7461 736b 7320  completed_tasks 
+00012850: 2b3d 2031 0d0a 0d0a 2020 2020 2020 2020  += 1....        
+00012860: 2020 2020 6966 206c 656e 286d 6564 6961      if len(media
+00012870: 5f66 696c 6570 6174 6873 293e 3020 616e  _filepaths)>0 an
+00012880: 6420 636f 6d70 6c65 7465 645f 7461 736b  d completed_task
+00012890: 7320 3d3d 206c 656e 286d 6564 6961 5f66  s == len(media_f
+000128a0: 696c 6570 6174 6873 293a 0d0a 2020 2020  ilepaths):..    
+000128b0: 2020 2020 2020 2020 2020 2020 7472 616e              tran
+000128c0: 7363 7269 6265 5f65 6e64 5f74 696d 6520  scribe_end_time 
+000128d0: 3d20 7469 6d65 2e74 696d 6528 290d 0a20  = time.time().. 
+000128e0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000128f0: 7261 6e73 6372 6962 655f 656c 6170 7365  ranscribe_elapse
+00012900: 645f 7469 6d65 203d 2074 7261 6e73 6372  d_time = transcr
+00012910: 6962 655f 656e 645f 7469 6d65 202d 2074  ibe_end_time - t
+00012920: 7261 6e73 6372 6962 655f 7374 6172 745f  ranscribe_start_
+00012930: 7469 6d65 0d0a 2020 2020 2020 2020 2020  time..          
+00012940: 2020 2020 2020 7472 616e 7363 7269 6265        transcribe
+00012950: 5f65 6c61 7073 6564 5f74 696d 655f 7365  _elapsed_time_se
+00012960: 636f 6e64 7320 3d20 7469 6d65 6465 6c74  conds = timedelt
+00012970: 6128 7365 636f 6e64 733d 696e 7428 7472  a(seconds=int(tr
+00012980: 616e 7363 7269 6265 5f65 6c61 7073 6564  anscribe_elapsed
+00012990: 5f74 696d 6529 290d 0a20 2020 2020 2020  _time))..       
+000129a0: 2020 2020 2020 2020 2074 7261 6e73 6372           transcr
+000129b0: 6962 655f 656c 6170 7365 645f 7469 6d65  ibe_elapsed_time
+000129c0: 5f73 7472 203d 2073 7472 2874 7261 6e73  _str = str(trans
+000129d0: 6372 6962 655f 656c 6170 7365 645f 7469  cribe_elapsed_ti
+000129e0: 6d65 5f73 6563 6f6e 6473 290d 0a20 2020  me_seconds)..   
+000129f0: 2020 2020 2020 2020 2020 2020 2068 6f75               hou
+00012a00: 722c 206d 696e 7574 652c 2073 6563 6f6e  r, minute, secon
+00012a10: 6420 3d20 7472 616e 7363 7269 6265 5f65  d = transcribe_e
+00012a20: 6c61 7073 6564 5f74 696d 655f 7374 722e  lapsed_time_str.
+00012a30: 7370 6c69 7428 223a 2229 0d0a 2020 2020  split(":")..    
+00012a40: 2020 2020 2020 2020 2020 2020 6d73 6720              msg 
+00012a50: 3d20 2254 6f74 616c 2074 7261 6e73 6372  = "Total transcr
+00012a60: 6962 6520 7469 6d65 2020 2020 2020 2020  ibe time        
+00012a70: 2020 2020 2020 2020 2020 203a 2025 733a             : %s:
+00012a80: 2573 3a25 7322 2025 2868 6f75 722e 7a66  %s:%s" %(hour.zf
+00012a90: 696c 6c28 3229 2c20 6d69 6e75 7465 2c20  ill(2), minute, 
+00012aa0: 7365 636f 6e64 290d 0a20 2020 2020 2020  second)..       
+00012ab0: 2020 2020 2020 2020 2070 7269 6e74 286d           print(m
+00012ac0: 7367 290d 0a0d 0a20 2020 2020 2020 2065  sg)....        e
+00012ad0: 7863 6570 7420 4b65 7962 6f61 7264 496e  xcept KeyboardIn
+00012ae0: 7465 7272 7570 743a 0d0a 2020 2020 2020  terrupt:..      
+00012af0: 2020 2020 2020 7062 6172 2e66 696e 6973        pbar.finis
+00012b00: 6828 290d 0a20 2020 2020 2020 2020 2020  h()..           
+00012b10: 2070 6f6f 6c2e 7465 726d 696e 6174 6528   pool.terminate(
+00012b20: 290d 0a20 2020 2020 2020 2020 2020 2070  )..            p
+00012b30: 6f6f 6c2e 636c 6f73 6528 290d 0a20 2020  ool.close()..   
+00012b40: 2020 2020 2020 2020 2070 6f6f 6c2e 6a6f           pool.jo
+00012b50: 696e 2829 0d0a 2020 2020 2020 2020 2020  in()..          
+00012b60: 2020 7072 696e 7428 2243 616e 6365 6c6c    print("Cancell
+00012b70: 696e 6720 616c 6c20 7461 736b 7322 290d  ing all tasks").
+00012b80: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
+00012b90: 6620 7379 732e 706c 6174 666f 726d 203d  f sys.platform =
+00012ba0: 3d20 2277 696e 3332 223a 0d0a 2020 2020  = "win32":..    
+00012bb0: 2020 2020 2020 2020 2020 2020 7374 6f70              stop
+00012bc0: 5f66 666d 7065 675f 7769 6e64 6f77 7328  _ffmpeg_windows(
+00012bd0: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
+00012be0: 616c 6c62 6163 6b3d 7368 6f77 5f65 7272  allback=show_err
+00012bf0: 6f72 5f6d 6573 7361 6765 7329 0d0a 2020  or_messages)..  
+00012c00: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+00012c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012c20: 2073 746f 705f 6666 6d70 6567 5f6c 696e   stop_ffmpeg_lin
+00012c30: 7578 2865 7272 6f72 5f6d 6573 7361 6765  ux(error_message
+00012c40: 735f 6361 6c6c 6261 636b 3d73 686f 775f  s_callback=show_
+00012c50: 6572 726f 725f 6d65 7373 6167 6573 290d  error_messages).
+00012c60: 0a0d 0a20 2020 2020 2020 2020 2020 2072  ...            r
+00012c70: 656d 6f76 655f 7465 6d70 5f66 696c 6573  emove_temp_files
+00012c80: 2822 666c 6163 2229 0d0a 2020 2020 2020  ("flac")..      
+00012c90: 2020 2020 2020 7265 6d6f 7665 5f74 656d        remove_tem
+00012ca0: 705f 6669 6c65 7328 2277 6176 2229 0d0a  p_files("wav")..
+00012cb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00012cc0: 726e 2031 0d0a 0d0a 2020 2020 2020 2020  rn 1....        
+00012cd0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+00012ce0: 2061 7320 653a 0d0a 2020 2020 2020 2020   as e:..        
+00012cf0: 2020 2020 6966 206e 6f74 204b 6579 626f      if not Keybo
+00012d00: 6172 6449 6e74 6572 7275 7074 2069 6e20  ardInterrupt in 
+00012d10: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00012d20: 2020 2020 7062 6172 2e66 696e 6973 6828      pbar.finish(
+00012d30: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00012d40: 2020 2070 6f6f 6c2e 7465 726d 696e 6174     pool.terminat
+00012d50: 6528 290d 0a20 2020 2020 2020 2020 2020  e()..           
+00012d60: 2020 2020 2070 6f6f 6c2e 636c 6f73 6528       pool.close(
+00012d70: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00012d80: 2020 2070 6f6f 6c2e 6a6f 696e 2829 0d0a     pool.join()..
+00012d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012da0: 7072 696e 7428 6529 0d0a 0d0a 2020 2020  print(e)....    
+00012db0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00012dc0: 7973 2e70 6c61 7466 6f72 6d20 3d3d 2022  ys.platform == "
+00012dd0: 7769 6e33 3222 3a0d 0a20 2020 2020 2020  win32":..       
+00012de0: 2020 2020 2020 2020 2020 2020 2073 746f               sto
+00012df0: 705f 6666 6d70 6567 5f77 696e 646f 7773  p_ffmpeg_windows
+00012e00: 2865 7272 6f72 5f6d 6573 7361 6765 735f  (error_messages_
+00012e10: 6361 6c6c 6261 636b 3d73 686f 775f 6572  callback=show_er
+00012e20: 726f 725f 6d65 7373 6167 6573 290d 0a20  ror_messages).. 
+00012e30: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00012e40: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00012e50: 2020 2020 2020 2020 2020 7374 6f70 5f66            stop_f
+00012e60: 666d 7065 675f 6c69 6e75 7828 6572 726f  fmpeg_linux(erro
+00012e70: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
+00012e80: 6163 6b3d 7368 6f77 5f65 7272 6f72 5f6d  ack=show_error_m
+00012e90: 6573 7361 6765 7329 0d0a 0d0a 2020 2020  essages)....    
+00012ea0: 2020 2020 2020 2020 2020 2020 7265 6d6f              remo
+00012eb0: 7665 5f74 656d 705f 6669 6c65 7328 2266  ve_temp_files("f
+00012ec0: 6c61 6322 290d 0a20 2020 2020 2020 2020  lac")..         
+00012ed0: 2020 2020 2020 2072 656d 6f76 655f 7465         remove_te
+00012ee0: 6d70 5f66 696c 6573 2822 7761 7622 290d  mp_files("wav").
+00012ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012f00: 2072 6574 7572 6e20 310d 0a0d 0a20 2020   return 1....   
+00012f10: 2069 6620 706f 6f6c 3a0d 0a20 2020 2020   if pool:..     
+00012f20: 2020 2070 6f6f 6c2e 636c 6f73 6528 290d     pool.close().
+00012f30: 0a20 2020 2020 2020 2070 6f6f 6c2e 6a6f  .        pool.jo
+00012f40: 696e 2829 0d0a 2020 2020 2020 2020 706f  in()..        po
+00012f50: 6f6c 203d 204e 6f6e 650d 0a0d 0a20 2020  ol = None....   
+00012f60: 2069 6620 7379 732e 706c 6174 666f 726d   if sys.platform
+00012f70: 203d 3d20 2277 696e 3332 223a 0d0a 2020   == "win32":..  
+00012f80: 2020 2020 2020 7374 6f70 5f66 666d 7065        stop_ffmpe
+00012f90: 675f 7769 6e64 6f77 7328 6572 726f 725f  g_windows(error_
+00012fa0: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
+00012fb0: 6b3d 7368 6f77 5f65 7272 6f72 5f6d 6573  k=show_error_mes
+00012fc0: 7361 6765 7329 0d0a 2020 2020 656c 7365  sages)..    else
+00012fd0: 3a0d 0a20 2020 2020 2020 2073 746f 705f  :..        stop_
+00012fe0: 6666 6d70 6567 5f6c 696e 7578 2865 7272  ffmpeg_linux(err
+00012ff0: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
+00013000: 6261 636b 3d73 686f 775f 6572 726f 725f  back=show_error_
+00013010: 6d65 7373 6167 6573 290d 0a0d 0a20 2020  messages)....   
+00013020: 2072 656d 6f76 655f 7465 6d70 5f66 696c   remove_temp_fil
+00013030: 6573 2822 666c 6163 2229 0d0a 2020 2020  es("flac")..    
+00013040: 7265 6d6f 7665 5f74 656d 705f 6669 6c65  remove_temp_file
+00013050: 7328 2277 6176 2229 0d0a 0d0a 6966 205f  s("wav")....if _
+00013060: 5f6e 616d 655f 5f20 3d3d 2027 5f5f 6d61  _name__ == '__ma
+00013070: 696e 5f5f 273a 0d0a 2020 2020 6d75 6c74  in__':..    mult
+00013080: 6970 726f 6365 7373 696e 672e 6672 6565  iprocessing.free
+00013090: 7a65 5f73 7570 706f 7274 2829 0d0a 2020  ze_support()..  
+000130a0: 2020 7379 732e 6578 6974 286d 6169 6e28    sys.exit(main(
+000130b0: 2929 0d0a                                ))..
```

### Comparing `whisper_autosrt-0.0.1/whisper_autosrt.egg-info/PKG-INFO` & `whisper_autosrt-0.0.2/whisper_autosrt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: whisper-autosrt
-Version: 0.0.1
-Summary: a utility for automatic speech recognition and subtitle generation
+Version: 0.0.2
+Summary: a command line utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/whisper_autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

