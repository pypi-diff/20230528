# Comparing `tmp/cyberdrop-dl-4.2.48.tar.gz` & `tmp/cyberdrop-dl-4.2.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.2.48.tar", last modified: Thu May 25 01:01:12 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.2.49.tar", last modified: Sun May 28 21:25:00 2023, max compression
```

## Comparing `cyberdrop-dl-4.2.48.tar` & `cyberdrop-dl-4.2.49.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:01:12.287219 cyberdrop-dl-4.2.48/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-05-25 01:01:12.287219 cyberdrop-dl-4.2.48/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17720 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:01:12.267218 cyberdrop-dl-4.2.48/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:01:12.271218 cyberdrop-dl-4.2.48/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:01:12.275219 cyberdrop-dl-4.2.48/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:01:12.283219 cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:01:12.283219 cyberdrop-dl-4.2.48/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18627 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    12870 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17799 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:01:12.287219 cyberdrop-dl-4.2.48/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20625 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:01:12.271218 cyberdrop-dl-4.2.48/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-05-25 01:01:12.000000 cyberdrop-dl-4.2.48/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-25 01:01:12.000000 cyberdrop-dl-4.2.48/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 01:01:12.000000 cyberdrop-dl-4.2.48/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-25 01:01:12.000000 cyberdrop-dl-4.2.48/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-25 01:01:12.000000 cyberdrop-dl-4.2.48/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 01:01:12.000000 cyberdrop-dl-4.2.48/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-25 01:01:12.287219 cyberdrop-dl-4.2.48/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 01:01:01.000000 cyberdrop-dl-4.2.48/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:00.698375 cyberdrop-dl-4.2.49/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-05-28 21:25:00.698375 cyberdrop-dl-4.2.49/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17777 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:00.694375 cyberdrop-dl-4.2.49/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:00.694375 cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:00.694375 cyberdrop-dl-4.2.49/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:00.698375 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:00.698375 cyberdrop-dl-4.2.49/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18292 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12908 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17678 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20640 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:00.698375 cyberdrop-dl-4.2.49/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20748 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:00.694375 cyberdrop-dl-4.2.49/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-05-28 21:25:00.000000 cyberdrop-dl-4.2.49/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-28 21:25:00.000000 cyberdrop-dl-4.2.49/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 21:25:00.000000 cyberdrop-dl-4.2.49/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-28 21:25:00.000000 cyberdrop-dl-4.2.49/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-28 21:25:00.000000 cyberdrop-dl-4.2.49/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-28 21:25:00.000000 cyberdrop-dl-4.2.49/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-28 21:25:00.698375 cyberdrop-dl-4.2.49/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/setup.py
```

### Comparing `cyberdrop-dl-4.2.48/LICENSE` & `cyberdrop-dl-4.2.49/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.48/PKG-INFO` & `cyberdrop-dl-4.2.49/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.48
+Version: 4.2.49
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -153,15 +153,15 @@
 --max-concurrent-threads                number of threads to download simultaneously
 --max-concurrent-domains                number of domains to download simultaneously
 --max-concurrent-albums                 number of albums to download simultaneously
 --max-concurrent-downloads-per-domain   number of simultaneous downloads per domain
 --skip-download-mark-completed          sets the scraped files as downloaded without downloading
 --output-errored-urls                   sets the failed urls to be output to the errored urls file
 --output-unsupported-urls               sets the unsupported urls to be output to the unsupported urls file
---proxy                                 HTTP/HTTPS proxy used for downloading, format [protocal]://[ip]:[port]
+--proxy                                 HTTP/HTTPS proxy used for downloading, format [protocol]://[ip]:[port]
 --remove-bunkr-identifier               removes the bunkr added identifier from output filenames
 --required-free-space                   required free space (in gigabytes) for the program to run
 
 --sort-downloads        sorts downloaded files after downloads have finished
 --sort-directory        folder to download files to
 --sorted-audio          schema to sort audio
 --sorted-images         schema to sort images
@@ -173,14 +173,15 @@
 --throttle              this is a throttle between requests during the downloading phase, the number is in seconds
 
 --output-last-forum-post        outputs the last post of a forum scrape to use as a starting point for future runs
 --scrape-single-post            scrapes a single post from a forum thread
 --separate-posts                separates forum scraping into folders by post number
 
 --gofile-api-key                api key for premium gofile
+--gofile-website-token          website token for gofile
 --pixeldrain-api-key            api key for premium pixeldrain
 --nudostar-username             username to login to nudostar
 --nudostar-password             password to login to nudostar
 --simpcity-username             username to login to simpcity
 --simpcity-password             password to login to simpcity
 --socialmediagirls-username     username to login to socialmediagirls
 --socialmediagirls-password     password to login to socialmediagirls
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.48 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.49 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
@@ -135,49 +135,49 @@
 download simultaneously --max-concurrent-domains number of domains to download
 simultaneously --max-concurrent-albums number of albums to download
 simultaneously --max-concurrent-downloads-per-domain number of simultaneous
 downloads per domain --skip-download-mark-completed sets the scraped files as
 downloaded without downloading --output-errored-urls sets the failed urls to be
 output to the errored urls file --output-unsupported-urls sets the unsupported
 urls to be output to the unsupported urls file --proxy HTTP/HTTPS proxy used
-for downloading, format [protocal]://[ip]:[port] --remove-bunkr-identifier
+for downloading, format [protocol]://[ip]:[port] --remove-bunkr-identifier
 removes the bunkr added identifier from output filenames --required-free-space
 required free space (in gigabytes) for the program to run --sort-downloads
 sorts downloaded files after downloads have finished --sort-directory folder to
 download files to --sorted-audio schema to sort audio --sorted-images schema to
 sort images --sorted-others schema to sort other --sorted-videos schema to sort
 videos --connection-timeout number of seconds to wait attempting to connect to
 a URL during the downloading phase --ratelimit this applies to requests made in
 the program during scraping, the number you provide is in requests/seconds --
 throttle this is a throttle between requests during the downloading phase, the
 number is in seconds --output-last-forum-post outputs the last post of a forum
 scrape to use as a starting point for future runs --scrape-single-post scrapes
 a single post from a forum thread --separate-posts separates forum scraping
 into folders by post number --gofile-api-key api key for premium gofile --
-pixeldrain-api-key api key for premium pixeldrain --nudostar-username username
-to login to nudostar --nudostar-password password to login to nudostar --
-simpcity-username username to login to simpcity --simpcity-password password to
-login to simpcity --socialmediagirls-username username to login to
-socialmediagirls --socialmediagirls-password password to login to
-socialmediagirls --xbunker-username username to login to xbunker --xbunker-
-password password to login to xbunker --apply-jdownloader enables sending
-unsupported URLs to a running jdownloader2 instance to download --jdownloader-
-username username to login to jdownloader --jdownloader-password password to
-login to jdownloader --jdownloader-device device name to login to for
-jdownloader --hide-new-progress disables the new rich progress entirely and
-uses older methods --hide-overall-progress removes overall progress section
-while downloading --hide-forum-progress removes forum progress section while
-downloading --hide-thread-progress removes thread progress section while
-downloading --hide-domain-progress removes domain progress section while
-downloading --hide-album-progress removes album progress section while
-downloading --hide-file-progress removes file progress section while
-downloading --refresh-rate changes the refresh rate of the progress table --
-visible-rows-threads number of visible rows to use for the threads table --
-visible-rows-domains number of visible rows to use for the domains table --
-visible-rows-albums number of visible rows to use for the albums table --
-visible-rows-files number of visible rows to use for the files table ``` `--
-only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr",
-"coomer.party", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello",
-"gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox",
-"jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "nudostar",
-"pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity",
-"socialmediagirls", "xbunker", "xbunkr"`
+gofile-website-token website token for gofile --pixeldrain-api-key api key for
+premium pixeldrain --nudostar-username username to login to nudostar --
+nudostar-password password to login to nudostar --simpcity-username username to
+login to simpcity --simpcity-password password to login to simpcity --
+socialmediagirls-username username to login to socialmediagirls --
+socialmediagirls-password password to login to socialmediagirls --xbunker-
+username username to login to xbunker --xbunker-password password to login to
+xbunker --apply-jdownloader enables sending unsupported URLs to a running
+jdownloader2 instance to download --jdownloader-username username to login to
+jdownloader --jdownloader-password password to login to jdownloader --
+jdownloader-device device name to login to for jdownloader --hide-new-progress
+disables the new rich progress entirely and uses older methods --hide-overall-
+progress removes overall progress section while downloading --hide-forum-
+progress removes forum progress section while downloading --hide-thread-
+progress removes thread progress section while downloading --hide-domain-
+progress removes domain progress section while downloading --hide-album-
+progress removes album progress section while downloading --hide-file-progress
+removes file progress section while downloading --refresh-rate changes the
+refresh rate of the progress table --visible-rows-threads number of visible
+rows to use for the threads table --visible-rows-domains number of visible rows
+to use for the domains table --visible-rows-albums number of visible rows to
+use for the albums table --visible-rows-files number of visible rows to use for
+the files table ``` `--only-hosts` and `--skip-hosts` can use: `"anonfiles",
+"bayfiles", "bunkr", "coomer.party", "cyberdrop", "cyberfile", "e-hentai",
+"erome", "fapello", "gfycat", "gallery.deltaporno.com", "gofile", "hgamecg",
+"img.kiwi", "imgbox", "jpg.church", "jpg.fish", "kemono.party", "lovefap",
+"nsfw.xxx", "nudostar", "pimpandhost", "pixeldrain", "pixl.li", "postimg",
+"saint", "simpcity", "socialmediagirls", "xbunker", "xbunkr"`
```

### Comparing `cyberdrop-dl-4.2.48/README.md` & `cyberdrop-dl-4.2.49/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 --max-concurrent-threads                number of threads to download simultaneously
 --max-concurrent-domains                number of domains to download simultaneously
 --max-concurrent-albums                 number of albums to download simultaneously
 --max-concurrent-downloads-per-domain   number of simultaneous downloads per domain
 --skip-download-mark-completed          sets the scraped files as downloaded without downloading
 --output-errored-urls                   sets the failed urls to be output to the errored urls file
 --output-unsupported-urls               sets the unsupported urls to be output to the unsupported urls file
---proxy                                 HTTP/HTTPS proxy used for downloading, format [protocal]://[ip]:[port]
+--proxy                                 HTTP/HTTPS proxy used for downloading, format [protocol]://[ip]:[port]
 --remove-bunkr-identifier               removes the bunkr added identifier from output filenames
 --required-free-space                   required free space (in gigabytes) for the program to run
 
 --sort-downloads        sorts downloaded files after downloads have finished
 --sort-directory        folder to download files to
 --sorted-audio          schema to sort audio
 --sorted-images         schema to sort images
@@ -161,14 +161,15 @@
 --throttle              this is a throttle between requests during the downloading phase, the number is in seconds
 
 --output-last-forum-post        outputs the last post of a forum scrape to use as a starting point for future runs
 --scrape-single-post            scrapes a single post from a forum thread
 --separate-posts                separates forum scraping into folders by post number
 
 --gofile-api-key                api key for premium gofile
+--gofile-website-token          website token for gofile
 --pixeldrain-api-key            api key for premium pixeldrain
 --nudostar-username             username to login to nudostar
 --nudostar-password             password to login to nudostar
 --simpcity-username             username to login to simpcity
 --simpcity-password             password to login to simpcity
 --socialmediagirls-username     username to login to socialmediagirls
 --socialmediagirls-password     password to login to socialmediagirls
```

#### html2text {}

```diff
@@ -129,49 +129,49 @@
 download simultaneously --max-concurrent-domains number of domains to download
 simultaneously --max-concurrent-albums number of albums to download
 simultaneously --max-concurrent-downloads-per-domain number of simultaneous
 downloads per domain --skip-download-mark-completed sets the scraped files as
 downloaded without downloading --output-errored-urls sets the failed urls to be
 output to the errored urls file --output-unsupported-urls sets the unsupported
 urls to be output to the unsupported urls file --proxy HTTP/HTTPS proxy used
-for downloading, format [protocal]://[ip]:[port] --remove-bunkr-identifier
+for downloading, format [protocol]://[ip]:[port] --remove-bunkr-identifier
 removes the bunkr added identifier from output filenames --required-free-space
 required free space (in gigabytes) for the program to run --sort-downloads
 sorts downloaded files after downloads have finished --sort-directory folder to
 download files to --sorted-audio schema to sort audio --sorted-images schema to
 sort images --sorted-others schema to sort other --sorted-videos schema to sort
 videos --connection-timeout number of seconds to wait attempting to connect to
 a URL during the downloading phase --ratelimit this applies to requests made in
 the program during scraping, the number you provide is in requests/seconds --
 throttle this is a throttle between requests during the downloading phase, the
 number is in seconds --output-last-forum-post outputs the last post of a forum
 scrape to use as a starting point for future runs --scrape-single-post scrapes
 a single post from a forum thread --separate-posts separates forum scraping
 into folders by post number --gofile-api-key api key for premium gofile --
-pixeldrain-api-key api key for premium pixeldrain --nudostar-username username
-to login to nudostar --nudostar-password password to login to nudostar --
-simpcity-username username to login to simpcity --simpcity-password password to
-login to simpcity --socialmediagirls-username username to login to
-socialmediagirls --socialmediagirls-password password to login to
-socialmediagirls --xbunker-username username to login to xbunker --xbunker-
-password password to login to xbunker --apply-jdownloader enables sending
-unsupported URLs to a running jdownloader2 instance to download --jdownloader-
-username username to login to jdownloader --jdownloader-password password to
-login to jdownloader --jdownloader-device device name to login to for
-jdownloader --hide-new-progress disables the new rich progress entirely and
-uses older methods --hide-overall-progress removes overall progress section
-while downloading --hide-forum-progress removes forum progress section while
-downloading --hide-thread-progress removes thread progress section while
-downloading --hide-domain-progress removes domain progress section while
-downloading --hide-album-progress removes album progress section while
-downloading --hide-file-progress removes file progress section while
-downloading --refresh-rate changes the refresh rate of the progress table --
-visible-rows-threads number of visible rows to use for the threads table --
-visible-rows-domains number of visible rows to use for the domains table --
-visible-rows-albums number of visible rows to use for the albums table --
-visible-rows-files number of visible rows to use for the files table ``` `--
-only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr",
-"coomer.party", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello",
-"gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox",
-"jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "nudostar",
-"pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity",
-"socialmediagirls", "xbunker", "xbunkr"`
+gofile-website-token website token for gofile --pixeldrain-api-key api key for
+premium pixeldrain --nudostar-username username to login to nudostar --
+nudostar-password password to login to nudostar --simpcity-username username to
+login to simpcity --simpcity-password password to login to simpcity --
+socialmediagirls-username username to login to socialmediagirls --
+socialmediagirls-password password to login to socialmediagirls --xbunker-
+username username to login to xbunker --xbunker-password password to login to
+xbunker --apply-jdownloader enables sending unsupported URLs to a running
+jdownloader2 instance to download --jdownloader-username username to login to
+jdownloader --jdownloader-password password to login to jdownloader --
+jdownloader-device device name to login to for jdownloader --hide-new-progress
+disables the new rich progress entirely and uses older methods --hide-overall-
+progress removes overall progress section while downloading --hide-forum-
+progress removes forum progress section while downloading --hide-thread-
+progress removes thread progress section while downloading --hide-domain-
+progress removes domain progress section while downloading --hide-album-
+progress removes album progress section while downloading --hide-file-progress
+removes file progress section while downloading --refresh-rate changes the
+refresh rate of the progress table --visible-rows-threads number of visible
+rows to use for the threads table --visible-rows-domains number of visible rows
+to use for the domains table --visible-rows-albums number of visible rows to
+use for the albums table --visible-rows-files number of visible rows to use for
+the files table ``` `--only-hosts` and `--skip-hosts` can use: `"anonfiles",
+"bayfiles", "bunkr", "coomer.party", "cyberdrop", "cyberfile", "e-hentai",
+"erome", "fapello", "gfycat", "gallery.deltaporno.com", "gofile", "hgamecg",
+"img.kiwi", "imgbox", "jpg.church", "jpg.fish", "kemono.party", "lovefap",
+"nsfw.xxx", "nudostar", "pimpandhost", "pixeldrain", "pixl.li", "postimg",
+"saint", "simpcity", "socialmediagirls", "xbunker", "xbunkr"`
```

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/base_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 
     async def write_errored_scrape_header(self):
         """Writes to the error file"""
         if not self.output_errored:
             return
 
         async with aiofiles.open(self.errored_scrapes, 'a') as f:
-            await f.write(f"URL,Exception\n")
+            await f.write("URL,Exception\n")
 
     async def write_errored_download(self, url: URL, referer: URL, error_message: str) -> None:
         """Writes to the error file"""
         if not self.output_errored:
             return
 
         async with aiofiles.open(self.errored_downloads, 'a') as f:
@@ -173,15 +173,15 @@
 
     async def write_unsupported_header(self):
         """Writes to the error file"""
         if not self.output_unsupported:
             return
 
         async with aiofiles.open(self.unsupported, 'a') as f:
-            await f.write(f"URL,REFERER,TITLE\n")
+            await f.write("URL,REFERER,TITLE\n")
 
     async def write_last_post(self, url: URL) -> None:
         """Writes to the error file"""
         if not self.output_last_post:
             return
 
         async with aiofiles.open(self.last_post, 'a') as f:
```

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/config_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Dict
 
 config_default: Dict = {
     "Apply_Config": False,
     "Configuration": {
         "Authentication": {
             "gofile_api_key": "",
+            "gofile_website_token": "",
             "pixeldrain_api_key": "",
             "nudostar_username": "",
             "nudostar_password": "",
             "simpcity_username": "",
             "simpcity_password": "",
             "socialmediagirls_username": "",
             "socialmediagirls_password": "",
```

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/data_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         new_title = title + '/' + self.title
         self.title = new_title
 
     async def extend(self, album) -> None:
         self.media.extend(album.media)
 
     async def is_empty(self) -> bool:
-        return True if not self.media else False
+        return not self.media
 
 
 @dataclass
 class DomainItem:
     """Class for keeping track of albums for each scraper type"""
     domain: str
     albums: Dict
```

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/client/client.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,38 +60,37 @@
                 return album_obj
             await album_obj.add_media(media)
             log(f"Finished: {url}", quiet=self.quiet, style="green")
             if not media.complete:
                 await self.SQL_Helper.insert_media("bunkr", "", media)
             return album_obj
 
-        elif "a" in url.parts:
+        if "a" in url.parts:
             album_obj = await self.get_album(session, url)
             await self.SQL_Helper.insert_album("bunkr", url, album_obj)
 
             if album_obj.media:
                 log(f"Finished: {url}", quiet=self.quiet, style="green")
             return album_obj
 
+        ext = '.' + url.parts[-1].split('.')[-1]
+        if ext:
+            ext = ext.lower()
+        if ext in FILE_FORMATS['Images']:
+            filename, ext = await get_filename_and_ext(url.name)
+            original_filename, filename = await self.remove_id(filename, ext)
+
+            await self.SQL_Helper.fix_bunkr_entries(url, original_filename)
+            check_complete = await self.SQL_Helper.check_complete_singular("bunkr", url)
+
+            media_item = MediaItem(url, url, check_complete, filename, ext, original_filename)
+            await album_obj.add_media(media_item)
         else:
-            ext = '.' + url.parts[-1].split('.')[-1]
-            if ext:
-                ext = ext.lower()
-            if ext in FILE_FORMATS['Images']:
-                filename, ext = await get_filename_and_ext(url.name)
-                original_filename, filename = await self.remove_id(filename, ext)
-
-                await self.SQL_Helper.fix_bunkr_entries(url, original_filename)
-                check_complete = await self.SQL_Helper.check_complete_singular("bunkr", url)
-
-                media_item = MediaItem(url, url, check_complete, filename, ext, original_filename)
-                await album_obj.add_media(media_item)
-            else:
-                media_item = await self.get_file(session, url)
-                await album_obj.add_media(media_item)
+            media_item = await self.get_file(session, url)
+            await album_obj.add_media(media_item)
 
         await self.SQL_Helper.insert_album("bunkr", url, album_obj)
         log(f"Finished: {url}", quiet=self.quiet, style="green")
         return album_obj
 
     async def remove_id(self, filename: str, ext: str):
         """Removes the additional string bunkr adds to the end of every filename"""
```

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 import http
 import re
-from typing import TYPE_CHECKING, Union, List, Dict
+from typing import TYPE_CHECKING, Dict, List, Union
 
 from aiolimiter import AsyncLimiter
 from yarl import URL
 
-from ..base_functions.base_functions import log, logger, make_title_safe, get_filename_and_ext
+from ..base_functions.base_functions import get_filename_and_ext, log, logger, make_title_safe
 from ..base_functions.data_classes import DomainItem, MediaItem
 from ..base_functions.error_classes import NoExtensionFailure
 
 if TYPE_CHECKING:
     from ..base_functions.base_functions import ErrorFileWriter
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
@@ -49,19 +49,23 @@
             else:
                 raise
         except Exception as e:
             logger.debug("Error encountered while getting GoFile token", exc_info=True)
             log("Error: Couldn't generate GoFile token", quiet=self.quiet, style="red")
             logger.debug(e)
 
-    async def get_website_token(self, session: ScrapeSession):
+    async def get_website_token(self, session: ScrapeSession, website_token: str = None):
         """Creates an anon gofile account to use."""
         if self.websiteToken:
             return
 
+        if website_token:
+            self.websiteToken = website_token
+            return
+
         try:
             async with self.limiter:
                 js_obj = await session.get_text(self.js_address)
             self.websiteToken = re.search(r'fetchData\.websiteToken\s*=\s*"(.*?)"', js_obj).group(1)
         except Exception as e:
             logger.debug("Error encountered while getting GoFile websiteToken", exc_info=True)
             log("Error: Couldn't generate GoFile websiteToken", quiet=self.quiet, style="red")
```

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/NSFWXXX_Spider.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/NSFWXXX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import asyncio
 import re
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Dict, List, Tuple
 
-import aiofiles
 from bs4 import BeautifulSoup
 from yarl import URL
 
 from ..base_functions.base_functions import (
     get_filename_and_ext,
     log,
     logger,
```

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     free_space = shutil.disk_usage(download_directory.parent).free
     free_space_gb = free_space / 1024 ** 3
     return free_space_gb >= required_space_gb
 
 
 def get_threads_number(args: Dict, domain: str) -> int:
     threads = args["Runtime"]["max_concurrent_downloads_per_domain"] or multiprocessing.cpu_count()
-    if any(s in domain for s in ('anonfiles', 'bunkr', 'pixeldrain')):
+    if any(s in domain for s in ('anonfiles', 'bunkr', 'pixeldrain', 'cyberfile')):
         return min(threads, 2)
     return threads
 
 
 async def is_4xx_client_error(status_code: int) -> bool:
     """Checks whether the HTTP status code is 4xx client error"""
     return HTTPStatus.BAD_REQUEST <= status_code < HTTPStatus.INTERNAL_SERVER_ERROR
```

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/downloader/downloaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,18 +96,15 @@
         self.albums_limit = asyncio.Semaphore(args["Runtime"]["max_concurrent_albums"]) if args["Runtime"]["max_concurrent_albums"] else None
 
         # API Keys
         self.pixeldrain_api_key = args["Authentication"]["pixeldrain_api_key"]
 
     def get_throttle(self, domain: str) -> float:
         """Get the throttle for a domain"""
-        if domain in self.delay:
-            return self.delay[domain]
-        else:
-            return self.client.throttle
+        return self.delay.get(domain, self.client.throttle)
 
 
 class Downloader:
     """Downloader class, directs downloading for domain objects"""
 
     def __init__(self, domain: str, CDL_Helper: CDLHelper, Progress_Master: ProgressMaster):
         self.domain = domain
@@ -297,25 +294,17 @@
 
 class DownloadManager:
     def __init__(self, CDL_Helper: CDLHelper, Progress_Master: ProgressMaster):
         self.downloaders: Dict[str, Downloader] = {}
         self.CDL_Helper = CDL_Helper
         self.Progress_Master = Progress_Master
 
-    async def create_downloader(self, domain: str):
-        if domain in self.downloaders:
-            return self.downloaders[domain]
-        else:
-            new_downloader = Downloader(domain, self.CDL_Helper, self.Progress_Master)
-            self.downloaders[domain] = new_downloader
-            return new_downloader
-
-    async def get_downloader(self, domain: str):
+    async def get_downloader(self, domain: str) -> Downloader:
         if domain not in self.downloaders:
-            return await self.create_downloader(domain)
+            self.downloaders[domain] = Downloader(domain, self.CDL_Helper, self.Progress_Master)
         return self.downloaders[domain]
 
 
 class DownloadDirector:
     def __init__(self, args: Dict, Forums: ForumItem, SQL_Helper: SQLHelper, client: Client,
                  error_writer: ErrorFileWriter):
         self.Progress_Master = ProgressMaster(args["Progress_Options"])
```

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from __future__ import annotations
 
 import asyncio
 import itertools
 import logging
 from http import HTTPStatus
-from pathlib import Path
 from random import gauss
-from typing import Dict, Any
+from typing import TYPE_CHECKING, Any, Dict
 
 import aiohttp.client_exceptions
 from tqdm import tqdm
 
 from cyberdrop_dl.base_functions.base_functions import (
-    clear,
     ErrorFileWriter,
+    clear,
     log,
     logger,
 )
 from cyberdrop_dl.base_functions.data_classes import AlbumItem, DomainItem, FileLock, ForumItem, MediaItem
 from cyberdrop_dl.base_functions.error_classes import DownloadFailure
 from cyberdrop_dl.base_functions.sql_helper import SQLHelper, get_db_path
 from cyberdrop_dl.client.client import Client, DownloadSession
@@ -28,14 +27,17 @@
     basic_auth,
     check_free_space,
     get_threads_number,
     is_4xx_client_error,
     retry,
 )
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 
 class Files:
     """Class that keeps track of completed, skipped and failed files"""
 
     def __init__(self, progress: tqdm):
         self.progress = progress
         self.completed_files = 0
```

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 from __future__ import annotations
 
-import asyncio
 import contextlib
-from functools import wraps
-from typing import Dict, Tuple, List
+from typing import Dict, List, Tuple
 
 from rich.console import Group
 from rich.panel import Panel
-from rich.progress import Progress, BarColumn, SpinnerColumn, TransferSpeedColumn, DownloadColumn, TimeRemainingColumn, \
-    TaskID
+from rich.progress import (
+    BarColumn,
+    DownloadColumn,
+    Progress,
+    SpinnerColumn,
+    TaskID,
+    TimeRemainingColumn,
+    TransferSpeedColumn,
+)
 from rich.table import Table
 
 
 def adjust_title(s: str, length: int = 40, placeholder: str = "...") -> str:
     """Collapse and truncate or pad the given string to fit in the given length"""
     return f"{s[:length - len(placeholder)]}{placeholder}" if len(s) >= length else s.ljust(length)
 
@@ -244,22 +249,20 @@
         self.domains: Dict[str, TaskID] = {}
         self.domain_totals: Dict[str, int] = {}
 
     async def add_domain(self, domain: str, total_albums: int) -> TaskID:
         if domain in self.domains:
             self.domain_totals[domain] += total_albums
             await self.progress.update_total(self.domains[domain], self.domain_totals[domain])
-            await self.progress.redraw()
-            return self.domains[domain]
         else:
-            task_id = await self.progress.add_task(domain.upper(), total_albums)
-            self.domains[domain] = task_id
+            self.domains[domain] = await self.progress.add_task(domain.upper(), total_albums)
             self.domain_totals[domain] = total_albums
-            await self.progress.redraw()
-            return task_id
+
+        await self.progress.redraw()
+        return self.domains[domain]
 
     async def advance_domain(self, task_id: TaskID) -> None:
         await self.progress.advance_task(task_id, 1)
 
     async def mark_domain_completed(self, domain: str, task_id: TaskID) -> None:
         task = [x for x in self.domain_progress.tasks if x.id == task_id][0]
         if task.finished:
```

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/main.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     runtime_opts.add_argument("--max_concurrent-threads", type=int, default=config_group["max_concurrent_threads"], help="Number of threads to download simultaneously (default: %(default)s)")
     runtime_opts.add_argument("--max_concurrent-domains", type=int, default=config_group["max_concurrent_domains"], help="Number of domains to download simultaneously (default: %(default)s)")
     runtime_opts.add_argument("--max_concurrent-albums", type=int, default=config_group["max_concurrent_albums"], help="Number of albums to download simultaneously (default: %(default)s)")
     runtime_opts.add_argument("--max_concurrent-downloads-per-domain", type=int, default=config_group["max_concurrent_downloads_per_domain"], help="Number of simultaneous downloads per domain (default: %(default)s)")
     runtime_opts.add_argument("--skip-download-mark-completed", help="sets the scraped files as downloaded without downloading", action="store_true")
     runtime_opts.add_argument("--output-errored-urls", help="sets the failed urls to be output to the errored urls file", action="store_true")
     runtime_opts.add_argument("--output-unsupported-urls", help="sets the unsupported urls to be output to the unsupported urls file", action="store_true")
-    runtime_opts.add_argument("--proxy", help="HTTP/HTTPS proxy used for downloading, format [protocal]://[ip]:[port]", default=config_group["proxy"])
+    runtime_opts.add_argument("--proxy", help="HTTP/HTTPS proxy used for downloading, format [protocol]://[ip]:[port]", default=config_group["proxy"])
     runtime_opts.add_argument("--remove-bunkr-identifier", help="removes the bunkr added identifier from output filenames", action="store_true")
     runtime_opts.add_argument("--required-free-space", type=int, default=config_group["required_free_space"], help="required free space (in gigabytes) for the program to run (default: %(default)s)")
 
     # Sorting
     config_group = config_data["Sorting"]
     sort_opts = parser.add_argument_group("Sorting options")
     sort_opts.add_argument("--sort-downloads", help="sorts downloaded files after downloads have finished", action="store_true")
@@ -99,14 +99,15 @@
     forum_opts.add_argument("--separate-posts", help="separates forum scraping into folders by post number", action="store_true")
     forum_opts.add_argument("--scrape-single-post", help="Scrapes only a single post from the given forum links", action="store_true")
 
     # Authentication details
     config_group = config_data["Authentication"]
     auth_opts = parser.add_argument_group("Authentication options")
     auth_opts.add_argument("--gofile-api-key", help="api key for premium gofile", default=config_group["gofile_api_key"])
+    auth_opts.add_argument("--gofile-website-token", help="website token for gofile", default=config_group["gofile_website_token"])
     auth_opts.add_argument("--pixeldrain-api-key", help="api key for premium pixeldrain", default=config_group["pixeldrain_api_key"])
     auth_opts.add_argument("--nudostar-username", help="username to login to nudostar", default=config_group["nudostar_username"])
     auth_opts.add_argument("--nudostar-password", help="password to login to nudostar", default=config_group['nudostar_password'])
     auth_opts.add_argument("--simpcity-username", help="username to login to simpcity", default=config_group["simpcity_username"])
     auth_opts.add_argument("--simpcity-password", help="password to login to simpcity", default=config_group['simpcity_password'])
     auth_opts.add_argument("--socialmediagirls-username", help="username to login to socialmediagirls", default=config_group["socialmediagirls_username"])
     auth_opts.add_argument("--socialmediagirls-password", help="password to login to socialmediagirls", default=config_group["socialmediagirls_password"])
```

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.2.49/cyberdrop_dl/scraper/Scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import asyncio
-from typing import TYPE_CHECKING, Optional, Dict
+from typing import TYPE_CHECKING, Dict, Optional
 
 from yarl import URL
 
 from cyberdrop_dl.base_functions.base_functions import log
 from cyberdrop_dl.base_functions.data_classes import AlbumItem, CascadeItem, DomainItem, ForumItem, SkipData
 from cyberdrop_dl.client.client import Client, ScrapeSession
 from cyberdrop_dl.crawlers.Anonfiles_Spider import AnonfilesCrawler
@@ -190,15 +190,16 @@
         if not self.gofile_crawler:
             self.gofile_crawler = GoFileCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper,
                                                 error_writer=self.error_writer)
 
         async with self.gofile_semaphore:
             await self.gofile_crawler.get_acct_token(session=gofile_session,
                                                      api_token=self.args['Authentication']['gofile_api_key'])
-            await self.gofile_crawler.get_website_token(session=gofile_session)
+            await self.gofile_crawler.get_website_token(session=gofile_session,
+                                                        website_token=self.args['Authentication']['gofile_website_token'])
         domain_obj = await self.gofile_crawler.fetch(gofile_session, url)
         await self._handle_domain_additions("gofile", domain_obj, title)
         await gofile_session.exit_handler()
 
     async def HGameCG(self, url, title=None):
         hgamecg_session = ScrapeSession(self.client)
         if not self.hgamecg_crawler:
```

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.2.49/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.48
+Version: 4.2.49
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -153,15 +153,15 @@
 --max-concurrent-threads                number of threads to download simultaneously
 --max-concurrent-domains                number of domains to download simultaneously
 --max-concurrent-albums                 number of albums to download simultaneously
 --max-concurrent-downloads-per-domain   number of simultaneous downloads per domain
 --skip-download-mark-completed          sets the scraped files as downloaded without downloading
 --output-errored-urls                   sets the failed urls to be output to the errored urls file
 --output-unsupported-urls               sets the unsupported urls to be output to the unsupported urls file
---proxy                                 HTTP/HTTPS proxy used for downloading, format [protocal]://[ip]:[port]
+--proxy                                 HTTP/HTTPS proxy used for downloading, format [protocol]://[ip]:[port]
 --remove-bunkr-identifier               removes the bunkr added identifier from output filenames
 --required-free-space                   required free space (in gigabytes) for the program to run
 
 --sort-downloads        sorts downloaded files after downloads have finished
 --sort-directory        folder to download files to
 --sorted-audio          schema to sort audio
 --sorted-images         schema to sort images
@@ -173,14 +173,15 @@
 --throttle              this is a throttle between requests during the downloading phase, the number is in seconds
 
 --output-last-forum-post        outputs the last post of a forum scrape to use as a starting point for future runs
 --scrape-single-post            scrapes a single post from a forum thread
 --separate-posts                separates forum scraping into folders by post number
 
 --gofile-api-key                api key for premium gofile
+--gofile-website-token          website token for gofile
 --pixeldrain-api-key            api key for premium pixeldrain
 --nudostar-username             username to login to nudostar
 --nudostar-password             password to login to nudostar
 --simpcity-username             username to login to simpcity
 --simpcity-password             password to login to simpcity
 --socialmediagirls-username     username to login to socialmediagirls
 --socialmediagirls-password     password to login to socialmediagirls
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.48 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.49 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
@@ -135,49 +135,49 @@
 download simultaneously --max-concurrent-domains number of domains to download
 simultaneously --max-concurrent-albums number of albums to download
 simultaneously --max-concurrent-downloads-per-domain number of simultaneous
 downloads per domain --skip-download-mark-completed sets the scraped files as
 downloaded without downloading --output-errored-urls sets the failed urls to be
 output to the errored urls file --output-unsupported-urls sets the unsupported
 urls to be output to the unsupported urls file --proxy HTTP/HTTPS proxy used
-for downloading, format [protocal]://[ip]:[port] --remove-bunkr-identifier
+for downloading, format [protocol]://[ip]:[port] --remove-bunkr-identifier
 removes the bunkr added identifier from output filenames --required-free-space
 required free space (in gigabytes) for the program to run --sort-downloads
 sorts downloaded files after downloads have finished --sort-directory folder to
 download files to --sorted-audio schema to sort audio --sorted-images schema to
 sort images --sorted-others schema to sort other --sorted-videos schema to sort
 videos --connection-timeout number of seconds to wait attempting to connect to
 a URL during the downloading phase --ratelimit this applies to requests made in
 the program during scraping, the number you provide is in requests/seconds --
 throttle this is a throttle between requests during the downloading phase, the
 number is in seconds --output-last-forum-post outputs the last post of a forum
 scrape to use as a starting point for future runs --scrape-single-post scrapes
 a single post from a forum thread --separate-posts separates forum scraping
 into folders by post number --gofile-api-key api key for premium gofile --
-pixeldrain-api-key api key for premium pixeldrain --nudostar-username username
-to login to nudostar --nudostar-password password to login to nudostar --
-simpcity-username username to login to simpcity --simpcity-password password to
-login to simpcity --socialmediagirls-username username to login to
-socialmediagirls --socialmediagirls-password password to login to
-socialmediagirls --xbunker-username username to login to xbunker --xbunker-
-password password to login to xbunker --apply-jdownloader enables sending
-unsupported URLs to a running jdownloader2 instance to download --jdownloader-
-username username to login to jdownloader --jdownloader-password password to
-login to jdownloader --jdownloader-device device name to login to for
-jdownloader --hide-new-progress disables the new rich progress entirely and
-uses older methods --hide-overall-progress removes overall progress section
-while downloading --hide-forum-progress removes forum progress section while
-downloading --hide-thread-progress removes thread progress section while
-downloading --hide-domain-progress removes domain progress section while
-downloading --hide-album-progress removes album progress section while
-downloading --hide-file-progress removes file progress section while
-downloading --refresh-rate changes the refresh rate of the progress table --
-visible-rows-threads number of visible rows to use for the threads table --
-visible-rows-domains number of visible rows to use for the domains table --
-visible-rows-albums number of visible rows to use for the albums table --
-visible-rows-files number of visible rows to use for the files table ``` `--
-only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr",
-"coomer.party", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello",
-"gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox",
-"jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "nudostar",
-"pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity",
-"socialmediagirls", "xbunker", "xbunkr"`
+gofile-website-token website token for gofile --pixeldrain-api-key api key for
+premium pixeldrain --nudostar-username username to login to nudostar --
+nudostar-password password to login to nudostar --simpcity-username username to
+login to simpcity --simpcity-password password to login to simpcity --
+socialmediagirls-username username to login to socialmediagirls --
+socialmediagirls-password password to login to socialmediagirls --xbunker-
+username username to login to xbunker --xbunker-password password to login to
+xbunker --apply-jdownloader enables sending unsupported URLs to a running
+jdownloader2 instance to download --jdownloader-username username to login to
+jdownloader --jdownloader-password password to login to jdownloader --
+jdownloader-device device name to login to for jdownloader --hide-new-progress
+disables the new rich progress entirely and uses older methods --hide-overall-
+progress removes overall progress section while downloading --hide-forum-
+progress removes forum progress section while downloading --hide-thread-
+progress removes thread progress section while downloading --hide-domain-
+progress removes domain progress section while downloading --hide-album-
+progress removes album progress section while downloading --hide-file-progress
+removes file progress section while downloading --refresh-rate changes the
+refresh rate of the progress table --visible-rows-threads number of visible
+rows to use for the threads table --visible-rows-domains number of visible rows
+to use for the domains table --visible-rows-albums number of visible rows to
+use for the albums table --visible-rows-files number of visible rows to use for
+the files table ``` `--only-hosts` and `--skip-hosts` can use: `"anonfiles",
+"bayfiles", "bunkr", "coomer.party", "cyberdrop", "cyberfile", "e-hentai",
+"erome", "fapello", "gfycat", "gallery.deltaporno.com", "gofile", "hgamecg",
+"img.kiwi", "imgbox", "jpg.church", "jpg.fish", "kemono.party", "lovefap",
+"nsfw.xxx", "nudostar", "pimpandhost", "pixeldrain", "pixl.li", "postimg",
+"saint", "simpcity", "socialmediagirls", "xbunker", "xbunkr"`
```

### Comparing `cyberdrop-dl-4.2.48/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.2.49/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.48/setup.cfg` & `cyberdrop-dl-4.2.49/setup.cfg`

 * *Files identical despite different names*

