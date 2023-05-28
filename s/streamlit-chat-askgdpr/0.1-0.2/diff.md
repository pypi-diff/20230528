# Comparing `tmp/streamlit-chat-askgdpr-0.1.tar.gz` & `tmp/streamlit-chat-askgdpr-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-chat-askgdpr-0.1.tar", last modified: Sun May 28 21:45:39 2023, max compression
+gzip compressed data, was "streamlit-chat-askgdpr-0.2.tar", last modified: Sun May 28 21:49:26 2023, max compression
```

## Comparing `streamlit-chat-askgdpr-0.1.tar` & `streamlit-chat-askgdpr-0.2.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:45:39.433693 streamlit-chat-askgdpr-0.1/
--rw-r--r--   0 grek       (501) staff       (20)     1064 2023-05-28 17:24:10.000000 streamlit-chat-askgdpr-0.1/LICENSE
--rw-r--r--   0 grek       (501) staff       (20)       50 2023-05-28 17:24:10.000000 streamlit-chat-askgdpr-0.1/MANIFEST.in
--rw-r--r--   0 grek       (501) staff       (20)     4154 2023-05-28 21:45:39.433503 streamlit-chat-askgdpr-0.1/PKG-INFO
--rw-r--r--   0 grek       (501) staff       (20)     3687 2023-05-28 17:24:10.000000 streamlit-chat-askgdpr-0.1/README.md
--rw-r--r--   0 grek       (501) staff       (20)       38 2023-05-28 21:45:39.433743 streamlit-chat-askgdpr-0.1/setup.cfg
--rw-r--r--   0 grek       (501) staff       (20)      924 2023-05-28 21:33:19.000000 streamlit-chat-askgdpr-0.1/setup.py
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:45:39.399799 streamlit-chat-askgdpr-0.1/streamlit_chat/
--rw-r--r--   0 grek       (501) staff       (20)     3595 2023-05-28 21:31:47.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/__init__.py
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:45:39.398250 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:45:39.403348 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/
--rw-r--r--   0 grek       (501) staff       (20)     1150 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/asset-manifest.json
--rw-r--r--   0 grek       (501) staff       (20)   197459 2023-05-28 21:32:34.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/bootstrap.min.css
--rw-r--r--   0 grek       (501) staff       (20)   646432 2023-05-28 21:32:34.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/bootstrap.min.css.map
--rw-r--r--   0 grek       (501) staff       (20)     2209 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/index.html
--rw-r--r--   0 grek       (501) staff       (20)     8091 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/precache-manifest.913e70ff508b34716fa805cc28b9d423.js
--rw-r--r--   0 grek       (501) staff       (20)     1183 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/service-worker.js
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:45:39.398523 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:45:39.403748 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/css/
--rw-r--r--   0 grek       (501) staff       (20)    48144 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css
--rw-r--r--   0 grek       (501) staff       (20)    64407 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css.map
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:45:39.417174 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/
--rw-r--r--   0 grek       (501) staff       (20)  1608824 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js
--rw-r--r--   0 grek       (501) staff       (20)     2015 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.LICENSE.txt
--rw-r--r--   0 grek       (501) staff       (20)  5402535 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.map
--rw-r--r--   0 grek       (501) staff       (20)     2106 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/main.e9a08b4d.chunk.js
--rw-r--r--   0 grek       (501) staff       (20)     5207 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/main.e9a08b4d.chunk.js.map
--rw-r--r--   0 grek       (501) staff       (20)     1598 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js
--rw-r--r--   0 grek       (501) staff       (20)     8317 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js.map
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:45:39.432075 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/
--rw-r--r--   0 grek       (501) staff       (20)    33516 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.10824af7.woff
--rw-r--r--   0 grek       (501) staff       (20)    63632 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.56573229.ttf
--rw-r--r--   0 grek       (501) staff       (20)    28076 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.66c67820.woff2
--rw-r--r--   0 grek       (501) staff       (20)    12368 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.497bf407.ttf
--rw-r--r--   0 grek       (501) staff       (20)     6912 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.a9e9b095.woff2
--rw-r--r--   0 grek       (501) staff       (20)     7716 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.de2ba279.woff
--rw-r--r--   0 grek       (501) staff       (20)     6908 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.08d95d99.woff2
--rw-r--r--   0 grek       (501) staff       (20)     7656 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.a25140fb.woff
--rw-r--r--   0 grek       (501) staff       (20)    12344 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.e6fb499f.ttf
--rw-r--r--   0 grek       (501) staff       (20)    13296 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.40934fc0.woff
--rw-r--r--   0 grek       (501) staff       (20)    11348 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.796f3797.woff2
--rw-r--r--   0 grek       (501) staff       (20)    19584 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.b9d7c449.ttf
--rw-r--r--   0 grek       (501) staff       (20)    19572 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.97a699d8.ttf
--rw-r--r--   0 grek       (501) staff       (20)    13208 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.e435cda5.woff
--rw-r--r--   0 grek       (501) staff       (20)    11316 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.f9e6a99f.woff2
--rw-r--r--   0 grek       (501) staff       (20)    29912 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.4cdba646.woff
--rw-r--r--   0 grek       (501) staff       (20)    51336 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.8e431f7e.ttf
--rw-r--r--   0 grek       (501) staff       (20)    25324 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.a9382e25.woff2
--rw-r--r--   0 grek       (501) staff       (20)    32968 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.52fb39b0.ttf
--rw-r--r--   0 grek       (501) staff       (20)    19412 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.5f875f98.woff
--rw-r--r--   0 grek       (501) staff       (20)    16780 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.d8737343.woff2
--rw-r--r--   0 grek       (501) staff       (20)    33580 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.39349e0a.ttf
--rw-r--r--   0 grek       (501) staff       (20)    16988 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.65297062.woff2
--rw-r--r--   0 grek       (501) staff       (20)    19676 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.8ffd28f6.woff
--rw-r--r--   0 grek       (501) staff       (20)    53580 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.818582da.ttf
--rw-r--r--   0 grek       (501) staff       (20)    30772 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f1cdb692.woff
--rw-r--r--   0 grek       (501) staff       (20)    26272 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f8a7f19f.woff2
--rw-r--r--   0 grek       (501) staff       (20)    16400 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.1320454d.woff2
--rw-r--r--   0 grek       (501) staff       (20)    18668 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.48155e43.woff
--rw-r--r--   0 grek       (501) staff       (20)    31196 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.6589c4f1.ttf
--rw-r--r--   0 grek       (501) staff       (20)    16440 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.d8b7a801.woff2
--rw-r--r--   0 grek       (501) staff       (20)    18748 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.ed7aea12.woff
--rw-r--r--   0 grek       (501) staff       (20)    31308 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.fe5ed587.ttf
--rw-r--r--   0 grek       (501) staff       (20)    14408 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.0e897d27.woff
--rw-r--r--   0 grek       (501) staff       (20)    12216 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.ad546b47.woff2
--rw-r--r--   0 grek       (501) staff       (20)    24504 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.f2ac7312.ttf
--rw-r--r--   0 grek       (501) staff       (20)    12028 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.e934cbc8.woff2
--rw-r--r--   0 grek       (501) staff       (20)    14112 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.ef725de5.woff
--rw-r--r--   0 grek       (501) staff       (20)    22364 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.f60b4a34.ttf
--rw-r--r--   0 grek       (501) staff       (20)    10344 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.1ac3ed6e.woff2
--rw-r--r--   0 grek       (501) staff       (20)    19436 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.3243452e.ttf
--rw-r--r--   0 grek       (501) staff       (20)    12316 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.5f8637ee.woff
--rw-r--r--   0 grek       (501) staff       (20)     9644 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.1b3161eb.woff2
--rw-r--r--   0 grek       (501) staff       (20)    16648 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a189c37d.ttf
--rw-r--r--   0 grek       (501) staff       (20)    10588 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a82fa2a7.woff
--rw-r--r--   0 grek       (501) staff       (20)    12228 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.0d8d9204.ttf
--rw-r--r--   0 grek       (501) staff       (20)     6496 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.4788ba5b.woff
--rw-r--r--   0 grek       (501) staff       (20)     5468 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.82ef26dc.woff2
--rw-r--r--   0 grek       (501) staff       (20)    11508 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.1fdda0e5.ttf
--rw-r--r--   0 grek       (501) staff       (20)     5208 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.95a1da91.woff2
--rw-r--r--   0 grek       (501) staff       (20)     6188 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.b0628bfd.woff
--rw-r--r--   0 grek       (501) staff       (20)     4420 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.4de844d4.woff
--rw-r--r--   0 grek       (501) staff       (20)     3624 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.9108a400.woff2
--rw-r--r--   0 grek       (501) staff       (20)     7588 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.963af864.ttf
--rw-r--r--   0 grek       (501) staff       (20)    10364 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.27a23ee6.ttf
--rw-r--r--   0 grek       (501) staff       (20)     5980 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.3045a61f.woff
--rw-r--r--   0 grek       (501) staff       (20)     4928 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.61522cd3.woff2
--rw-r--r--   0 grek       (501) staff       (20)    16028 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.0e046058.woff
--rw-r--r--   0 grek       (501) staff       (20)    27556 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.6bf42875.ttf
--rw-r--r--   0 grek       (501) staff       (20)    13568 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.b8b8393d.woff2
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:45:39.433270 streamlit-chat-askgdpr-0.1/streamlit_chat_askgdpr.egg-info/
--rw-r--r--   0 grek       (501) staff       (20)     4154 2023-05-28 21:45:39.000000 streamlit-chat-askgdpr-0.1/streamlit_chat_askgdpr.egg-info/PKG-INFO
--rw-r--r--   0 grek       (501) staff       (20)     5876 2023-05-28 21:45:39.000000 streamlit-chat-askgdpr-0.1/streamlit_chat_askgdpr.egg-info/SOURCES.txt
--rw-r--r--   0 grek       (501) staff       (20)        1 2023-05-28 21:45:39.000000 streamlit-chat-askgdpr-0.1/streamlit_chat_askgdpr.egg-info/dependency_links.txt
--rw-r--r--   0 grek       (501) staff       (20)       16 2023-05-28 21:45:39.000000 streamlit-chat-askgdpr-0.1/streamlit_chat_askgdpr.egg-info/requires.txt
--rw-r--r--   0 grek       (501) staff       (20)       15 2023-05-28 21:45:39.000000 streamlit-chat-askgdpr-0.1/streamlit_chat_askgdpr.egg-info/top_level.txt
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:49:26.399790 streamlit-chat-askgdpr-0.2/
+-rw-r--r--   0 grek       (501) staff       (20)     1064 2023-05-28 17:24:10.000000 streamlit-chat-askgdpr-0.2/LICENSE
+-rw-r--r--   0 grek       (501) staff       (20)       50 2023-05-28 17:24:10.000000 streamlit-chat-askgdpr-0.2/MANIFEST.in
+-rw-r--r--   0 grek       (501) staff       (20)     4154 2023-05-28 21:49:26.399591 streamlit-chat-askgdpr-0.2/PKG-INFO
+-rw-r--r--   0 grek       (501) staff       (20)     3687 2023-05-28 17:24:10.000000 streamlit-chat-askgdpr-0.2/README.md
+-rw-r--r--   0 grek       (501) staff       (20)       38 2023-05-28 21:49:26.399841 streamlit-chat-askgdpr-0.2/setup.cfg
+-rw-r--r--   0 grek       (501) staff       (20)      924 2023-05-28 21:49:13.000000 streamlit-chat-askgdpr-0.2/setup.py
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:49:26.373478 streamlit-chat-askgdpr-0.2/streamlit_chat/
+-rw-r--r--   0 grek       (501) staff       (20)     3594 2023-05-28 21:49:21.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/__init__.py
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:49:26.372173 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:49:26.375414 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/
+-rw-r--r--   0 grek       (501) staff       (20)     1150 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/asset-manifest.json
+-rw-r--r--   0 grek       (501) staff       (20)   197459 2023-05-28 21:32:34.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/bootstrap.min.css
+-rw-r--r--   0 grek       (501) staff       (20)   646432 2023-05-28 21:32:34.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/bootstrap.min.css.map
+-rw-r--r--   0 grek       (501) staff       (20)     2209 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/index.html
+-rw-r--r--   0 grek       (501) staff       (20)     8091 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/precache-manifest.913e70ff508b34716fa805cc28b9d423.js
+-rw-r--r--   0 grek       (501) staff       (20)     1183 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/service-worker.js
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:49:26.372483 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:49:26.376000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/css/
+-rw-r--r--   0 grek       (501) staff       (20)    48144 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css
+-rw-r--r--   0 grek       (501) staff       (20)    64407 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css.map
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:49:26.388444 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/
+-rw-r--r--   0 grek       (501) staff       (20)  1608824 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js
+-rw-r--r--   0 grek       (501) staff       (20)     2015 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.LICENSE.txt
+-rw-r--r--   0 grek       (501) staff       (20)  5402535 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.map
+-rw-r--r--   0 grek       (501) staff       (20)     2106 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/main.e9a08b4d.chunk.js
+-rw-r--r--   0 grek       (501) staff       (20)     5207 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/main.e9a08b4d.chunk.js.map
+-rw-r--r--   0 grek       (501) staff       (20)     1598 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js
+-rw-r--r--   0 grek       (501) staff       (20)     8317 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js.map
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:49:26.398717 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/
+-rw-r--r--   0 grek       (501) staff       (20)    33516 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.10824af7.woff
+-rw-r--r--   0 grek       (501) staff       (20)    63632 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.56573229.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    28076 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.66c67820.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    12368 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.497bf407.ttf
+-rw-r--r--   0 grek       (501) staff       (20)     6912 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.a9e9b095.woff2
+-rw-r--r--   0 grek       (501) staff       (20)     7716 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.de2ba279.woff
+-rw-r--r--   0 grek       (501) staff       (20)     6908 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.08d95d99.woff2
+-rw-r--r--   0 grek       (501) staff       (20)     7656 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.a25140fb.woff
+-rw-r--r--   0 grek       (501) staff       (20)    12344 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.e6fb499f.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    13296 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.40934fc0.woff
+-rw-r--r--   0 grek       (501) staff       (20)    11348 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.796f3797.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    19584 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.b9d7c449.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    19572 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.97a699d8.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    13208 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.e435cda5.woff
+-rw-r--r--   0 grek       (501) staff       (20)    11316 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.f9e6a99f.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    29912 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.4cdba646.woff
+-rw-r--r--   0 grek       (501) staff       (20)    51336 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.8e431f7e.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    25324 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.a9382e25.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    32968 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.52fb39b0.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    19412 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.5f875f98.woff
+-rw-r--r--   0 grek       (501) staff       (20)    16780 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.d8737343.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    33580 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.39349e0a.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    16988 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.65297062.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    19676 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.8ffd28f6.woff
+-rw-r--r--   0 grek       (501) staff       (20)    53580 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.818582da.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    30772 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f1cdb692.woff
+-rw-r--r--   0 grek       (501) staff       (20)    26272 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f8a7f19f.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    16400 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.1320454d.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    18668 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.48155e43.woff
+-rw-r--r--   0 grek       (501) staff       (20)    31196 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.6589c4f1.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    16440 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.d8b7a801.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    18748 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.ed7aea12.woff
+-rw-r--r--   0 grek       (501) staff       (20)    31308 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.fe5ed587.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    14408 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.0e897d27.woff
+-rw-r--r--   0 grek       (501) staff       (20)    12216 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.ad546b47.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    24504 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.f2ac7312.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    12028 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.e934cbc8.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    14112 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.ef725de5.woff
+-rw-r--r--   0 grek       (501) staff       (20)    22364 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.f60b4a34.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    10344 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.1ac3ed6e.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    19436 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.3243452e.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    12316 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.5f8637ee.woff
+-rw-r--r--   0 grek       (501) staff       (20)     9644 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.1b3161eb.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    16648 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a189c37d.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    10588 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a82fa2a7.woff
+-rw-r--r--   0 grek       (501) staff       (20)    12228 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.0d8d9204.ttf
+-rw-r--r--   0 grek       (501) staff       (20)     6496 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.4788ba5b.woff
+-rw-r--r--   0 grek       (501) staff       (20)     5468 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.82ef26dc.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    11508 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.1fdda0e5.ttf
+-rw-r--r--   0 grek       (501) staff       (20)     5208 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.95a1da91.woff2
+-rw-r--r--   0 grek       (501) staff       (20)     6188 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.b0628bfd.woff
+-rw-r--r--   0 grek       (501) staff       (20)     4420 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.4de844d4.woff
+-rw-r--r--   0 grek       (501) staff       (20)     3624 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.9108a400.woff2
+-rw-r--r--   0 grek       (501) staff       (20)     7588 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.963af864.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    10364 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.27a23ee6.ttf
+-rw-r--r--   0 grek       (501) staff       (20)     5980 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.3045a61f.woff
+-rw-r--r--   0 grek       (501) staff       (20)     4928 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.61522cd3.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    16028 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.0e046058.woff
+-rw-r--r--   0 grek       (501) staff       (20)    27556 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.6bf42875.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    13568 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.b8b8393d.woff2
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:49:26.399353 streamlit-chat-askgdpr-0.2/streamlit_chat_askgdpr.egg-info/
+-rw-r--r--   0 grek       (501) staff       (20)     4154 2023-05-28 21:49:26.000000 streamlit-chat-askgdpr-0.2/streamlit_chat_askgdpr.egg-info/PKG-INFO
+-rw-r--r--   0 grek       (501) staff       (20)     5876 2023-05-28 21:49:26.000000 streamlit-chat-askgdpr-0.2/streamlit_chat_askgdpr.egg-info/SOURCES.txt
+-rw-r--r--   0 grek       (501) staff       (20)        1 2023-05-28 21:49:26.000000 streamlit-chat-askgdpr-0.2/streamlit_chat_askgdpr.egg-info/dependency_links.txt
+-rw-r--r--   0 grek       (501) staff       (20)       16 2023-05-28 21:49:26.000000 streamlit-chat-askgdpr-0.2/streamlit_chat_askgdpr.egg-info/requires.txt
+-rw-r--r--   0 grek       (501) staff       (20)       15 2023-05-28 21:49:26.000000 streamlit-chat-askgdpr-0.2/streamlit_chat_askgdpr.egg-info/top_level.txt
```

### Comparing `streamlit-chat-askgdpr-0.1/LICENSE` & `streamlit-chat-askgdpr-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/PKG-INFO` & `streamlit-chat-askgdpr-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-chat-askgdpr
-Version: 0.1
+Version: 0.2
 Summary: A streamlit component, to make chatbots
 Home-page: https://github.com/AI-Yash/st-chat
 Author: Grzegorz Kossakowski, Maciej Zdanowicz
 Author-email: yashpawarp@gmail.com
 Keywords: chat streamlit streamlit-component
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `streamlit-chat-askgdpr-0.1/README.md` & `streamlit-chat-askgdpr-0.2/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/setup.py` & `streamlit-chat-askgdpr-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setuptools.setup(
     name="streamlit-chat-askgdpr",
-    version="0.1",
+    version="0.2",
     author="Grzegorz Kossakowski, Maciej Zdanowicz",
     author_email="yashpawarp@gmail.com",
     description="A streamlit component, to make chatbots",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/AI-Yash/st-chat",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/__init__.py` & `streamlit-chat-askgdpr-0.2/streamlit_chat/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 from typing import Optional, Union
 
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
-_RELEASE = False
+_RELEASE = True
 COMPONENT_NAME = "streamlit_chat"
 
 if _RELEASE:  # use the build instead of development if release is true
     root_dir = os.path.dirname(os.path.abspath(__file__))
     build_dir = os.path.join(root_dir, "frontend/build")
 
     _streamlit_chat = components.declare_component(
         COMPONENT_NAME,
         path = build_dir
     )
 else:
     _streamlit_chat = components.declare_component(
         COMPONENT_NAME,
-        url = "http://localhost:3000"
+        url = "http://localhost:3001"
     )
 
 # data type for avatar style
 AvatarStyle = Literal[
     "adventurer",
     "adventurer-neutral",
     "avataaars",
```

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/asset-manifest.json` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/bootstrap.min.css` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/bootstrap.min.css.map` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/index.html` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/precache-manifest.913e70ff508b34716fa805cc28b9d423.js` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/precache-manifest.913e70ff508b34716fa805cc28b9d423.js`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/service-worker.js` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css.map` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.LICENSE.txt` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.map` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/main.e9a08b4d.chunk.js` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/main.e9a08b4d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/main.e9a08b4d.chunk.js.map` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/main.e9a08b4d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js.map` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.10824af7.woff` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.10824af7.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.56573229.ttf` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.56573229.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.66c67820.woff2` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.66c67820.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.497bf407.ttf` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.497bf407.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.a9e9b095.woff2` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.a9e9b095.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.de2ba279.woff` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.de2ba279.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.08d95d99.woff2` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.08d95d99.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.a25140fb.woff` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.a25140fb.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.e6fb499f.ttf` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.e6fb499f.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.40934fc0.woff` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.40934fc0.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.796f3797.woff2` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.796f3797.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.b9d7c449.ttf` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.b9d7c449.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.97a699d8.ttf` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.97a699d8.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.e435cda5.woff` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.e435cda5.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.f9e6a99f.woff2` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.f9e6a99f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.4cdba646.woff` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.4cdba646.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.8e431f7e.ttf` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.8e431f7e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.a9382e25.woff2` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.a9382e25.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.52fb39b0.ttf` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.52fb39b0.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.5f875f98.woff` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.5f875f98.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.d8737343.woff2` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.d8737343.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.39349e0a.ttf` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.39349e0a.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.65297062.woff2` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.65297062.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.8ffd28f6.woff` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.8ffd28f6.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.818582da.ttf` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.818582da.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f1cdb692.woff` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f1cdb692.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f8a7f19f.woff2` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f8a7f19f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.1320454d.woff2` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.1320454d.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.48155e43.woff` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.48155e43.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.6589c4f1.ttf` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.6589c4f1.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.d8b7a801.woff2` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.d8b7a801.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.ed7aea12.woff` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.ed7aea12.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.fe5ed587.ttf` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.fe5ed587.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.0e897d27.woff` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.0e897d27.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.ad546b47.woff2` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.ad546b47.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.f2ac7312.ttf` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.f2ac7312.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.e934cbc8.woff2` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.e934cbc8.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.ef725de5.woff` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.ef725de5.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.f60b4a34.ttf` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.f60b4a34.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.1ac3ed6e.woff2` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.1ac3ed6e.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.3243452e.ttf` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.3243452e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.5f8637ee.woff` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.5f8637ee.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.1b3161eb.woff2` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.1b3161eb.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a189c37d.ttf` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a189c37d.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a82fa2a7.woff` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a82fa2a7.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.0d8d9204.ttf` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.0d8d9204.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.4788ba5b.woff` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.4788ba5b.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.82ef26dc.woff2` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.82ef26dc.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.1fdda0e5.ttf` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.1fdda0e5.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.95a1da91.woff2` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.95a1da91.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.b0628bfd.woff` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.b0628bfd.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.4de844d4.woff` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.4de844d4.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.9108a400.woff2` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.9108a400.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.963af864.ttf` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.963af864.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.27a23ee6.ttf` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.27a23ee6.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.3045a61f.woff` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.3045a61f.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.61522cd3.woff2` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.61522cd3.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.0e046058.woff` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.0e046058.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.6bf42875.ttf` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.6bf42875.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.b8b8393d.woff2` & `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.b8b8393d.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat_askgdpr.egg-info/PKG-INFO` & `streamlit-chat-askgdpr-0.2/streamlit_chat_askgdpr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-chat-askgdpr
-Version: 0.1
+Version: 0.2
 Summary: A streamlit component, to make chatbots
 Home-page: https://github.com/AI-Yash/st-chat
 Author: Grzegorz Kossakowski, Maciej Zdanowicz
 Author-email: yashpawarp@gmail.com
 Keywords: chat streamlit streamlit-component
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `streamlit-chat-askgdpr-0.1/streamlit_chat_askgdpr.egg-info/SOURCES.txt` & `streamlit-chat-askgdpr-0.2/streamlit_chat_askgdpr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

