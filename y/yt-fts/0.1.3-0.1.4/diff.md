# Comparing `tmp/yt-fts-0.1.3.tar.gz` & `tmp/yt-fts-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt-fts-0.1.3.tar", last modified: Sun May 28 07:15:42 2023, max compression
+gzip compressed data, was "yt-fts-0.1.4.tar", last modified: Sun May 28 20:48:27 2023, max compression
```

## Comparing `yt-fts-0.1.3.tar` & `yt-fts-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-28 07:15:42.741631 yt-fts-0.1.3/
--rw-r--r--   0 home       (501) staff       (20)     1211 2023-05-27 17:44:26.000000 yt-fts-0.1.3/LICENSE
--rw-r--r--   0 home       (501) staff       (20)      502 2023-05-28 07:15:42.740894 yt-fts-0.1.3/PKG-INFO
--rw-r--r--   0 home       (501) staff       (20)     3645 2023-05-27 17:58:18.000000 yt-fts-0.1.3/README.md
--rw-r--r--   0 home       (501) staff       (20)       38 2023-05-28 07:15:42.741805 yt-fts-0.1.3/setup.cfg
--rw-r--r--   0 home       (501) staff       (20)      811 2023-05-28 07:15:36.000000 yt-fts-0.1.3/setup.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-28 07:15:42.735995 yt-fts-0.1.3/yt_fts/
--rw-r--r--   0 home       (501) staff       (20)        0 2023-05-28 06:29:11.000000 yt-fts-0.1.3/yt_fts/__init__.py
--rw-r--r--   0 home       (501) staff       (20)       65 2023-05-28 06:34:41.000000 yt-fts-0.1.3/yt_fts/__main__.py
--rw-r--r--   0 home       (501) staff       (20)     3203 2023-05-27 17:35:08.000000 yt-fts-0.1.3/yt_fts/db_scripts.py
--rw-r--r--   0 home       (501) staff       (20)    10150 2023-05-28 06:49:46.000000 yt-fts-0.1.3/yt_fts/yt_fts.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-28 07:15:42.739908 yt-fts-0.1.3/yt_fts.egg-info/
--rw-r--r--   0 home       (501) staff       (20)      502 2023-05-28 07:15:42.000000 yt-fts-0.1.3/yt_fts.egg-info/PKG-INFO
--rw-r--r--   0 home       (501) staff       (20)      284 2023-05-28 07:15:42.000000 yt-fts-0.1.3/yt_fts.egg-info/SOURCES.txt
--rw-r--r--   0 home       (501) staff       (20)        1 2023-05-28 07:15:42.000000 yt-fts-0.1.3/yt_fts.egg-info/dependency_links.txt
--rw-r--r--   0 home       (501) staff       (20)       45 2023-05-28 07:15:42.000000 yt-fts-0.1.3/yt_fts.egg-info/entry_points.txt
--rw-r--r--   0 home       (501) staff       (20)      180 2023-05-28 07:15:42.000000 yt-fts-0.1.3/yt_fts.egg-info/requires.txt
--rw-r--r--   0 home       (501) staff       (20)        7 2023-05-28 07:15:42.000000 yt-fts-0.1.3/yt_fts.egg-info/top_level.txt
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-28 20:48:27.756508 yt-fts-0.1.4/
+-rw-r--r--   0 home       (501) staff       (20)     1211 2023-05-28 20:45:24.000000 yt-fts-0.1.4/LICENSE
+-rw-r--r--   0 home       (501) staff       (20)     4261 2023-05-28 20:48:27.755960 yt-fts-0.1.4/PKG-INFO
+-rw-r--r--   0 home       (501) staff       (20)     3718 2023-05-28 20:45:24.000000 yt-fts-0.1.4/README.md
+-rw-r--r--   0 home       (501) staff       (20)       38 2023-05-28 20:48:27.756669 yt-fts-0.1.4/setup.cfg
+-rw-r--r--   0 home       (501) staff       (20)      969 2023-05-28 20:47:54.000000 yt-fts-0.1.4/setup.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-28 20:48:27.750537 yt-fts-0.1.4/yt_fts/
+-rw-r--r--   0 home       (501) staff       (20)        0 2023-05-28 20:45:24.000000 yt-fts-0.1.4/yt_fts/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)       65 2023-05-28 20:45:24.000000 yt-fts-0.1.4/yt_fts/__main__.py
+-rw-r--r--   0 home       (501) staff       (20)     3203 2023-05-28 20:45:24.000000 yt-fts-0.1.4/yt_fts/db_scripts.py
+-rw-r--r--   0 home       (501) staff       (20)    10150 2023-05-28 20:45:24.000000 yt-fts-0.1.4/yt_fts/yt_fts.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-28 20:48:27.755092 yt-fts-0.1.4/yt_fts.egg-info/
+-rw-r--r--   0 home       (501) staff       (20)     4261 2023-05-28 20:48:27.000000 yt-fts-0.1.4/yt_fts.egg-info/PKG-INFO
+-rw-r--r--   0 home       (501) staff       (20)      284 2023-05-28 20:48:27.000000 yt-fts-0.1.4/yt_fts.egg-info/SOURCES.txt
+-rw-r--r--   0 home       (501) staff       (20)        1 2023-05-28 20:48:27.000000 yt-fts-0.1.4/yt_fts.egg-info/dependency_links.txt
+-rw-r--r--   0 home       (501) staff       (20)       45 2023-05-28 20:48:27.000000 yt-fts-0.1.4/yt_fts.egg-info/entry_points.txt
+-rw-r--r--   0 home       (501) staff       (20)      180 2023-05-28 20:48:27.000000 yt-fts-0.1.4/yt_fts.egg-info/requires.txt
+-rw-r--r--   0 home       (501) staff       (20)        7 2023-05-28 20:48:27.000000 yt-fts-0.1.4/yt_fts.egg-info/top_level.txt
```

### Comparing `yt-fts-0.1.3/LICENSE` & `yt-fts-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yt-fts-0.1.3/README.md` & `yt-fts-0.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,22 +5,29 @@
 query a channel for specific key word or phrase and will generate time stamped youtube urls to
 the video containing the keyword. 
 
 - [Blog Post](https://notjoemartinez.com/blog/youtube_full_text_search/)
 
 ### Installation 
 
+**pip**
+```bash
+pip install yt-fts
+```
+
+**from source**
 ```bash
 git clone https://github.com/NotJoeMartinez/yt-fts
-cd yt-fts
 python3 -m venv .env
 source .env/bin/activate
 pip install -r requirements.txt
+python3 -m yt-fts
 ```
 
+### Dependencies 
 This project requires [yt-dlp](https://github.com/yt-dlp/yt-dlp) installed globally. Platform specific installation instructions are available on the [yt-dlp wiki](https://github.com/yt-dlp/yt-dlp/wiki/Installation). 
 
 **pip**
 ```bash
 python3 -m pip install -U yt-dlp
 ```
 **MacOS/Homebrew**
@@ -28,18 +35,17 @@
 brew install yt-dlp
 ```
 **Windows/winget**
 ```bash
 winget install yt-dlp
 ```
 
-
 ### Usage 
 ```
-Usage: yt_fts.py [OPTIONS] COMMAND [ARGS]...
+Usage: yt-fts [OPTIONS] COMMAND [ARGS]...
 
 Options:
   --help  Show this message and exit.
 
 Commands:
   delete    delete [channel id]
   download  download [channel url]
@@ -47,63 +53,63 @@
   list      Lists channels
   search    search [channel id] [search text]
 ```
 
 ### `download`
 Will download all of a channels vtt files into your database 
 ```bash
-python yt_fts.py download "https://www.youtube.com/@TimDillonShow/videos"
+yt-fts download "https://www.youtube.com/@TimDillonShow/videos"
 ```
 
 **`--channel-id [youtube channel id]`**
 
 If `download` fails you can manually input the channel id with the `--channel-id` flag.
 The channel url should still be an argument 
 ```bash
-python yt_fts.py download --channel-id "UC4woSp8ITBoYDmjkukhEhxg" "https://www.youtube.com/@TimDillonShow/videos" 
+yt-fts download --channel-id "UC4woSp8ITBoYDmjkukhEhxg" "https://www.youtube.com/@TimDillonShow/videos" 
 ```
 
 **`--language [en/fr/es/etc..]`**
 
 Specify subtitles language 
 ```bash
-python yt_fts.py download --language de "https://www.youtube.com/@TimDillonShow/videos" 
+yt-fts download --language de "https://www.youtube.com/@TimDillonShow/videos" 
 ```
 
 **`--number-of-jobs [number]`**
 
 Speed up downloads with multi threading 
 ```bash
-python yt_fts.py download --number-of-jobs 6 "https://www.youtube.com/@TimDillonShow/videos"
+yt-fts download --number-of-jobs 6 "https://www.youtube.com/@TimDillonShow/videos"
 ```
 
 ### `list`
 List all of your downloaded channels 
 ```bash
-python yt_fts.py list
+yt-fts list
 ```
 
 output:
 ```
 Listing channels
 channel_id                channel_name         channel_url
 ------------------------  -------------------  ---------------------------------------------------------------
 UC4woSp8ITBoYDmjkukhEhxg  The Tim Dillon Show  https://www.youtube.com/channel/UC4woSp8ITBoYDmjkukhEhxg/videos
 ```
 
 ### `search`
 Search a channel for text based off the channel id you give it and 
 print a url to that point in the video
 ```bash
-python yt_fts.py search [channel_id] "text you want to find"
+yt-fts search [channel_id] "text you want to find"
 ```
 **EX:**
 
 ```bash
-python yt_fts.py search UC4woSp8ITBoYDmjkukhEhxg "life in the big city"
+yt-fts search UC4woSp8ITBoYDmjkukhEhxg "life in the big city"
 ```
 output:
 ```
 Video title"("#208 - Let's Have A Party | The Tim Dillon Show - YouTube",)"
 
     Quote: "life in the big city Dan is wearing the"
     Time Stamp: 01:50:07.790
@@ -121,13 +127,16 @@
     Time Stamp: 00:27:17.549
     Link: https://youtu.be/dqGyCTbzYmc?t=1634
 ```
 
 ### `Export`
 Similar to `search` except it will export all of the search results to a csv 
 with the format: `Video Title,Quote,Time Stamp,Link` as it's headers
+```bash
+yt-fts export UC4woSp8ITBoYDmjkukhEhxg "life in the big city" 
+```
 
 ### `Delete` 
 Will delete a channel from your database 
 ```bash
-python yt_fts.py delete [channel_id]
+yt-fts delete [channel_id]
 ```
```

### Comparing `yt-fts-0.1.3/setup.py` & `yt-fts-0.1.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     dependencies = f.read().splitlines()
 
+with open('README.md', 'r') as f:
+    long_description = f.read()
+
+
 entry_points = {
     'console_scripts': [
         'yt-fts=yt_fts.yt_fts:cli',
     ],
 }
 
 setup(
     name='yt-fts', 
-    version='0.1.3',
-    description='yt-fts is a simple python script that uses yt-dlp to scrape all of a youtube channels subtitles and load them into an sqlite database that is searchable from the command line. It allows you to query a channel for specific key word or phrase and will generate time stamped youtube urls to the video containing the keyword.', 
+    version='0.1.4',
+    description='yt-fts is a simple python script that uses yt-dlp to scrape all of a youtube channels subtitles and load them into an sqlite database that is searchable from the command line. It allows you to query a channel for specific key word or phrase and will generate time stamped youtube urls to the video containing the keyword.',
+    long_description=long_description,
+    long_description_content_type='text/markdown', 
     author='NotJoeMartinez',
     url='https://github.com/NotJoeMartinez/yt-fts',  
     packages=find_packages(),
     install_requires=dependencies,
     entry_points=entry_points,
     python_requires='>=3.11',
 )
```

### Comparing `yt-fts-0.1.3/yt_fts/db_scripts.py` & `yt-fts-0.1.4/yt_fts/db_scripts.py`

 * *Files identical despite different names*

### Comparing `yt-fts-0.1.3/yt_fts/yt_fts.py` & `yt-fts-0.1.4/yt_fts/yt_fts.py`

 * *Files identical despite different names*

