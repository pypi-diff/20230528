# Comparing `tmp/yt-fts-0.1.1.tar.gz` & `tmp/yt-fts-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt-fts-0.1.1.tar", last modified: Sun May 28 04:24:52 2023, max compression
+gzip compressed data, was "yt-fts-0.1.2.tar", last modified: Sun May 28 07:05:41 2023, max compression
```

## Comparing `yt-fts-0.1.1.tar` & `yt-fts-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-28 04:24:52.060311 yt-fts-0.1.1/
--rw-r--r--   0 home       (501) staff       (20)     1211 2023-05-28 03:53:46.000000 yt-fts-0.1.1/LICENSE
--rw-r--r--   0 home       (501) staff       (20)      502 2023-05-28 04:24:52.059799 yt-fts-0.1.1/PKG-INFO
--rw-r--r--   0 home       (501) staff       (20)     3645 2023-05-28 03:53:46.000000 yt-fts-0.1.1/README.md
--rw-r--r--   0 home       (501) staff       (20)       38 2023-05-28 04:24:52.060508 yt-fts-0.1.1/setup.cfg
--rw-r--r--   0 home       (501) staff       (20)      811 2023-05-28 04:24:22.000000 yt-fts-0.1.1/setup.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-28 04:24:52.055588 yt-fts-0.1.1/yt_fts/
--rw-r--r--   0 home       (501) staff       (20)        0 2023-05-28 03:54:10.000000 yt-fts-0.1.1/yt_fts/__init__.py
--rw-r--r--   0 home       (501) staff       (20)     3203 2023-05-28 03:53:46.000000 yt-fts-0.1.1/yt_fts/db_scripts.py
--rw-r--r--   0 home       (501) staff       (20)    10139 2023-05-28 04:21:44.000000 yt-fts-0.1.1/yt_fts/yt_fts.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-28 04:24:52.059075 yt-fts-0.1.1/yt_fts.egg-info/
--rw-r--r--   0 home       (501) staff       (20)      502 2023-05-28 04:24:52.000000 yt-fts-0.1.1/yt_fts.egg-info/PKG-INFO
--rw-r--r--   0 home       (501) staff       (20)      265 2023-05-28 04:24:52.000000 yt-fts-0.1.1/yt_fts.egg-info/SOURCES.txt
--rw-r--r--   0 home       (501) staff       (20)        1 2023-05-28 04:24:52.000000 yt-fts-0.1.1/yt_fts.egg-info/dependency_links.txt
--rw-r--r--   0 home       (501) staff       (20)       45 2023-05-28 04:24:52.000000 yt-fts-0.1.1/yt_fts.egg-info/entry_points.txt
--rw-r--r--   0 home       (501) staff       (20)      180 2023-05-28 04:24:52.000000 yt-fts-0.1.1/yt_fts.egg-info/requires.txt
--rw-r--r--   0 home       (501) staff       (20)        7 2023-05-28 04:24:52.000000 yt-fts-0.1.1/yt_fts.egg-info/top_level.txt
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-28 07:05:41.975672 yt-fts-0.1.2/
+-rw-r--r--   0 home       (501) staff       (20)     1211 2023-05-27 17:44:26.000000 yt-fts-0.1.2/LICENSE
+-rw-r--r--   0 home       (501) staff       (20)      502 2023-05-28 07:05:41.975318 yt-fts-0.1.2/PKG-INFO
+-rw-r--r--   0 home       (501) staff       (20)     3645 2023-05-27 17:58:18.000000 yt-fts-0.1.2/README.md
+-rw-r--r--   0 home       (501) staff       (20)       38 2023-05-28 07:05:41.975814 yt-fts-0.1.2/setup.cfg
+-rw-r--r--   0 home       (501) staff       (20)      811 2023-05-28 06:59:51.000000 yt-fts-0.1.2/setup.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-28 07:05:41.971634 yt-fts-0.1.2/yt_fts/
+-rw-r--r--   0 home       (501) staff       (20)        0 2023-05-28 06:29:11.000000 yt-fts-0.1.2/yt_fts/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)       65 2023-05-28 06:34:41.000000 yt-fts-0.1.2/yt_fts/__main__.py
+-rw-r--r--   0 home       (501) staff       (20)     3203 2023-05-27 17:35:08.000000 yt-fts-0.1.2/yt_fts/db_scripts.py
+-rw-r--r--   0 home       (501) staff       (20)    10150 2023-05-28 06:49:46.000000 yt-fts-0.1.2/yt_fts/yt_fts.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-28 07:05:41.974653 yt-fts-0.1.2/yt_fts.egg-info/
+-rw-r--r--   0 home       (501) staff       (20)      502 2023-05-28 07:05:41.000000 yt-fts-0.1.2/yt_fts.egg-info/PKG-INFO
+-rw-r--r--   0 home       (501) staff       (20)      284 2023-05-28 07:05:41.000000 yt-fts-0.1.2/yt_fts.egg-info/SOURCES.txt
+-rw-r--r--   0 home       (501) staff       (20)        1 2023-05-28 07:05:41.000000 yt-fts-0.1.2/yt_fts.egg-info/dependency_links.txt
+-rw-r--r--   0 home       (501) staff       (20)       45 2023-05-28 07:05:41.000000 yt-fts-0.1.2/yt_fts.egg-info/entry_points.txt
+-rw-r--r--   0 home       (501) staff       (20)      180 2023-05-28 07:05:41.000000 yt-fts-0.1.2/yt_fts.egg-info/requires.txt
+-rw-r--r--   0 home       (501) staff       (20)        7 2023-05-28 07:05:41.000000 yt-fts-0.1.2/yt_fts.egg-info/top_level.txt
```

### Comparing `yt-fts-0.1.1/LICENSE` & `yt-fts-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yt-fts-0.1.1/README.md` & `yt-fts-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `yt-fts-0.1.1/setup.py` & `yt-fts-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     'console_scripts': [
         'yt_fts=yt_fts.yt_fts:cli',
     ],
 }
 
 setup(
     name='yt-fts', 
-    version='0.1.1',
+    version='0.1.2',
     description='yt-fts is a simple python script that uses yt-dlp to scrape all of a youtube channels subtitles and load them into an sqlite database that is searchable from the command line. It allows you to query a channel for specific key word or phrase and will generate time stamped youtube urls to the video containing the keyword.', 
     author='NotJoeMartinez',
     url='https://github.com/NotJoeMartinez/yt-fts',  
     packages=find_packages(),
     install_requires=dependencies,
     entry_points=entry_points,
     python_requires='>=3.11',
```

### Comparing `yt-fts-0.1.1/yt_fts/db_scripts.py` & `yt-fts-0.1.2/yt_fts/db_scripts.py`

 * *Files identical despite different names*

### Comparing `yt-fts-0.1.1/yt_fts/yt_fts.py` & `yt-fts-0.1.2/yt_fts/yt_fts.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-import click, re, sqlite3 
+import click, re, sqlite3, json 
 import os, tempfile, subprocess, requests, datetime, csv
 
 from tabulate import tabulate
 from progress.bar import Bar
-
 from concurrent.futures import ThreadPoolExecutor
-
 from bs4 import BeautifulSoup
-import json
 
-
-from yt_fts.db_scripts import * 
+from yt_fts.db_scripts import *
 
 @click.group()
 def cli():
     make_db()
 
 @click.command(help="Lists channels")
 def list():
@@ -26,19 +22,23 @@
 @click.command( help='download [channel url]')
 @click.argument('channel_url', required=True)
 @click.option('--channel-id', default=None, help='Optional channel id to override the one from the url')
 @click.option('--language', default="en", help='Language of the subtitles to download')
 @click.option('--number-of-jobs', type=int, default=1, help='Optional number of jobs to parallelize the run')
 @click.option('--language', default="en", help='Language of the subtitles to download')
 def download(channel_url, channel_id, language, number_of_jobs):
-    handle_reject_consent_cookie(channel_url)
+    s = requests.session()
+    handle_reject_consent_cookie(channel_url, s)
     if channel_id is None:
-        channel_id = get_channel_id(channel_url)
+        channel_id = get_channel_id(channel_url, s)
+    
+    channel_name = get_channel_name(channel_id, s)
+
     if channel_id:
-        download_channel(channel_id, language, number_of_jobs)
+        download_channel(channel_id, channel_name, language, number_of_jobs, s)
     else:
         print("Error finding channel id try --channel-id option")
 
 
 @click.command( help='search [channel id] [search text]')
 @click.argument('channel_id', required=True)
 @click.argument('search_text', required=True)
@@ -74,28 +74,27 @@
 
 cli.add_command(list)
 cli.add_command(download)
 cli.add_command(search)
 cli.add_command(delete)
 cli.add_command(export)
 
-def download_channel(channel_id, language, number_of_jobs):
+def download_channel(channel_id, channel_name, language, number_of_jobs, s):
     print("Downloading channel")
     with tempfile.TemporaryDirectory() as tmp_dir:
         print('Saving vtt files to', tmp_dir)
 
-        channel_name = get_channel_name(channel_id)
         channel_url = f"https://www.youtube.com/channel/{channel_id}/videos"
         list_of_videos_urls = get_videos_list(channel_url)
 
         download_vtts(number_of_jobs, list_of_videos_urls, language, tmp_dir)
         add_channel_info(channel_id, channel_name, channel_url)
 
         print("Adding VTT data to db")
-        vtt_to_db(channel_id, tmp_dir)
+        vtt_to_db(channel_id, tmp_dir, s)
 
 
 def download_vtts(number_of_jobs, list_of_videos_urls, language ,tmp_dir):
     executor = ThreadPoolExecutor(number_of_jobs)
     futures = []
     for video_id in list_of_videos_urls:
         video_url = f'https://www.youtube.com/watch?v={video_id}'
@@ -114,28 +113,29 @@
         "--convert-subs", "vtt",
         "--skip-download",
             "--sub-langs", f"{language},-live_chat",
         "--sub-langs", f"{language},-live_chat",
         video_url
     ])
 
+
 def get_videos_list(channel_url):
     cmd = [
         "yt-dlp",
         "--flat-playlist",
         "--print",
         "id",
         f"{channel_url}"
     ]
     res = subprocess.run(cmd, capture_output=True, check=True)
     list_of_videos_urls = res.stdout.decode().splitlines()
     return list_of_videos_urls
 
 
-def vtt_to_db(channel_id, dir_path):
+def vtt_to_db(channel_id, dir_path, s):
     items = os.listdir(dir_path)
 
     file_paths = []
 
     for item in items:
         item_path = os.path.join(dir_path, item)
         if os.path.isfile(item_path):
@@ -146,30 +146,30 @@
 
     bar = Bar('Processing', max=len(file_paths))
 
     for vtt in file_paths:
         base_name = os.path.basename(vtt)
         vid_id = re.match(r'^([^.]*)', base_name).group(1)
         vid_url = f"https://youtu.be/{vid_id}"
-        vid_title = get_vid_title(vid_url)
+        vid_title = get_vid_title(vid_url, s)
         add_video(channel_id, vid_id, vid_title, vid_url)
 
         vtt_json = parse_vtt(vtt)
 
         for sub in vtt_json:
             start_time = sub['start_time']
             text = sub['text']
             cur.execute(f"INSERT INTO Subtitles (video_id, timestamp, text) VALUES (?, ?, ?)", (vid_id, start_time, text))
 
         con.commit()
         bar.next()
 
     bar.finish() 
     con.close()
-        
+
 
 def parse_vtt(file_path):
 
     result = []
 
     time_pattern = "^(.*) align:start position:0%"
 
@@ -191,61 +191,14 @@
                     'start_time': start_time,
                     'text': sub_titles.strip('\n'),
                 })
         
     return result 
 
 
-def get_vid_title(vid_url):
-    res = s.get(vid_url)
-    if res.status_code == 200:
-        html = res.text
-        soup = BeautifulSoup(html, 'html.parser')
-        title = soup.title.string
-        return title 
-    else:
-        return None
-        
-
- 
-def get_channel_id(url):
-    res = s.get(url)
-    if res.status_code == 200:
-        html = res.text
-        channel_id = re.search('channelId":"(.{24})"', html).group(1)
-        print(channel_id)
-        return channel_id
-    else:
-        return None
-
-def get_channel_name(channel_id):
-
-    res = s.get(f"https://www.youtube.com/channel/{channel_id}/videos")
-
-    if res.status_code == 200:
-
-        html = res.text
-        soup = BeautifulSoup(html, 'html.parser')
-        script = soup.find('script', type='application/ld+json')
-
-        # Hot fix for channels with special characters in the name
-        try:
-            print("Trying to parse json normally")
-            data = json.loads(script.string)
-        except:
-            print("json parse failed retrying with escaped backslashes")
-            script = script.string.replace('\\', '\\\\')
-            data = json.loads(script)
-
-        channel_name = data['itemListElement'][0]['item']['name']
-        print(channel_name)
-        return channel_name 
-    else:
-        return None
-
 def get_quotes(channel_id, text):
     res = search_channel(channel_id, text)
 
     if len(res) == 0:
         print("No matches found")
     else:
 
@@ -308,15 +261,64 @@
     hours = int(time_rex.group(1)) * 3600 
     mins = int(time_rex.group(2)) * 60
     secs = int(time_rex.group(3)) 
 
     total_secs =  hours + mins + secs
     return total_secs - 3
 
-def handle_reject_consent_cookie(channel_url):
+
+def get_vid_title(vid_url, s):
+    res = s.get(vid_url)
+    if res.status_code == 200:
+        html = res.text
+        soup = BeautifulSoup(html, 'html.parser')
+        title = soup.title.string
+        return title 
+    else:
+        return None
+        
+ 
+def get_channel_id(url, s):
+    res = s.get(url)
+    if res.status_code == 200:
+        html = res.text
+        channel_id = re.search('channelId":"(.{24})"', html).group(1)
+        print(channel_id)
+        return channel_id
+    else:
+        return None
+
+
+def get_channel_name(channel_id, s):
+
+    res = s.get(f"https://www.youtube.com/channel/{channel_id}/videos")
+
+    if res.status_code == 200:
+
+        html = res.text
+        soup = BeautifulSoup(html, 'html.parser')
+        script = soup.find('script', type='application/ld+json')
+
+        # Hot fix for channels with special characters in the name
+        try:
+            print("Trying to parse json normally")
+            data = json.loads(script.string)
+        except:
+            print("json parse failed retrying with escaped backslashes")
+            script = script.string.replace('\\', '\\\\')
+            data = json.loads(script)
+
+        channel_name = data['itemListElement'][0]['item']['name']
+        print(channel_name)
+        return channel_name 
+    else:
+        return None
+
+
+def handle_reject_consent_cookie(channel_url, s):
     r = s.get(channel_url)
     if "https://consent.youtube.com" in r.url:
         m = re.search(r"<input type=\"hidden\" name=\"bl\" value=\"([^\"]*)\"", r.text)
         if m:
             data = {
                 "gl":"DE",
                 "pc":"yt",
@@ -325,13 +327,7 @@
                 "bl":m.group(1),
                 "hl":"de",
                 "set_eom":"true"
             }
             s.post("https://consent.youtube.com/save", data=data)
 
 
-
-
-
-if __name__ == '__main__':
-    s = requests.session()
-    cli()
```

