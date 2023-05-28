# Comparing `tmp/streamlit-chat-askgdpr-0.0.2.3.tar.gz` & `tmp/streamlit-chat-askgdpr-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-chat-askgdpr-0.0.2.3.tar", last modified: Sun May 28 17:56:25 2023, max compression
+gzip compressed data, was "streamlit-chat-askgdpr-0.1.tar", last modified: Sun May 28 21:45:39 2023, max compression
```

## Comparing `streamlit-chat-askgdpr-0.0.2.3.tar` & `streamlit-chat-askgdpr-0.1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 17:56:25.761594 streamlit-chat-askgdpr-0.0.2.3/
--rw-r--r--   0 grek       (501) staff       (20)     1064 2023-05-28 17:24:10.000000 streamlit-chat-askgdpr-0.0.2.3/LICENSE
--rw-r--r--   0 grek       (501) staff       (20)       50 2023-05-28 17:24:10.000000 streamlit-chat-askgdpr-0.0.2.3/MANIFEST.in
--rw-r--r--   0 grek       (501) staff       (20)     4157 2023-05-28 17:56:25.761402 streamlit-chat-askgdpr-0.0.2.3/PKG-INFO
--rw-r--r--   0 grek       (501) staff       (20)     3687 2023-05-28 17:24:10.000000 streamlit-chat-askgdpr-0.0.2.3/README.md
--rw-r--r--   0 grek       (501) staff       (20)       38 2023-05-28 17:56:25.761650 streamlit-chat-askgdpr-0.0.2.3/setup.cfg
--rw-r--r--   0 grek       (501) staff       (20)      927 2023-05-28 17:55:34.000000 streamlit-chat-askgdpr-0.0.2.3/setup.py
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 17:56:25.736258 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/
--rw-r--r--   0 grek       (501) staff       (20)     3479 2023-05-28 17:24:10.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/__init__.py
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 17:56:25.735170 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 17:56:25.737745 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/
--rw-r--r--   0 grek       (501) staff       (20)     1150 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/asset-manifest.json
--rw-r--r--   0 grek       (501) staff       (20)   197459 2023-05-28 17:53:41.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/bootstrap.min.css
--rw-r--r--   0 grek       (501) staff       (20)   646432 2023-05-28 17:53:41.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/bootstrap.min.css.map
--rw-r--r--   0 grek       (501) staff       (20)     2209 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/index.html
--rw-r--r--   0 grek       (501) staff       (20)     8091 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/precache-manifest.ef63ad040edbb9ce675c41c512a1e329.js
--rw-r--r--   0 grek       (501) staff       (20)     1183 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/service-worker.js
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 17:56:25.735441 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 17:56:25.738090 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/css/
--rw-r--r--   0 grek       (501) staff       (20)    48144 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css
--rw-r--r--   0 grek       (501) staff       (20)    64407 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css.map
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 17:56:25.744825 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/
--rw-r--r--   0 grek       (501) staff       (20)  1608824 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js
--rw-r--r--   0 grek       (501) staff       (20)     2015 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.LICENSE.txt
--rw-r--r--   0 grek       (501) staff       (20)  5402535 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.map
--rw-r--r--   0 grek       (501) staff       (20)     2106 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/main.4b51ce30.chunk.js
--rw-r--r--   0 grek       (501) staff       (20)     5213 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/main.4b51ce30.chunk.js.map
--rw-r--r--   0 grek       (501) staff       (20)     1598 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js
--rw-r--r--   0 grek       (501) staff       (20)     8317 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js.map
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 17:56:25.760184 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/
--rw-r--r--   0 grek       (501) staff       (20)    33516 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.10824af7.woff
--rw-r--r--   0 grek       (501) staff       (20)    63632 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.56573229.ttf
--rw-r--r--   0 grek       (501) staff       (20)    28076 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.66c67820.woff2
--rw-r--r--   0 grek       (501) staff       (20)    12368 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.497bf407.ttf
--rw-r--r--   0 grek       (501) staff       (20)     6912 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.a9e9b095.woff2
--rw-r--r--   0 grek       (501) staff       (20)     7716 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.de2ba279.woff
--rw-r--r--   0 grek       (501) staff       (20)     6908 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.08d95d99.woff2
--rw-r--r--   0 grek       (501) staff       (20)     7656 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.a25140fb.woff
--rw-r--r--   0 grek       (501) staff       (20)    12344 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.e6fb499f.ttf
--rw-r--r--   0 grek       (501) staff       (20)    13296 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.40934fc0.woff
--rw-r--r--   0 grek       (501) staff       (20)    11348 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.796f3797.woff2
--rw-r--r--   0 grek       (501) staff       (20)    19584 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.b9d7c449.ttf
--rw-r--r--   0 grek       (501) staff       (20)    19572 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.97a699d8.ttf
--rw-r--r--   0 grek       (501) staff       (20)    13208 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.e435cda5.woff
--rw-r--r--   0 grek       (501) staff       (20)    11316 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.f9e6a99f.woff2
--rw-r--r--   0 grek       (501) staff       (20)    29912 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.4cdba646.woff
--rw-r--r--   0 grek       (501) staff       (20)    51336 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.8e431f7e.ttf
--rw-r--r--   0 grek       (501) staff       (20)    25324 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.a9382e25.woff2
--rw-r--r--   0 grek       (501) staff       (20)    32968 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.52fb39b0.ttf
--rw-r--r--   0 grek       (501) staff       (20)    19412 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.5f875f98.woff
--rw-r--r--   0 grek       (501) staff       (20)    16780 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.d8737343.woff2
--rw-r--r--   0 grek       (501) staff       (20)    33580 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.39349e0a.ttf
--rw-r--r--   0 grek       (501) staff       (20)    16988 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.65297062.woff2
--rw-r--r--   0 grek       (501) staff       (20)    19676 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.8ffd28f6.woff
--rw-r--r--   0 grek       (501) staff       (20)    53580 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.818582da.ttf
--rw-r--r--   0 grek       (501) staff       (20)    30772 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f1cdb692.woff
--rw-r--r--   0 grek       (501) staff       (20)    26272 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f8a7f19f.woff2
--rw-r--r--   0 grek       (501) staff       (20)    16400 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.1320454d.woff2
--rw-r--r--   0 grek       (501) staff       (20)    18668 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.48155e43.woff
--rw-r--r--   0 grek       (501) staff       (20)    31196 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.6589c4f1.ttf
--rw-r--r--   0 grek       (501) staff       (20)    16440 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.d8b7a801.woff2
--rw-r--r--   0 grek       (501) staff       (20)    18748 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.ed7aea12.woff
--rw-r--r--   0 grek       (501) staff       (20)    31308 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.fe5ed587.ttf
--rw-r--r--   0 grek       (501) staff       (20)    14408 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.0e897d27.woff
--rw-r--r--   0 grek       (501) staff       (20)    12216 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.ad546b47.woff2
--rw-r--r--   0 grek       (501) staff       (20)    24504 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.f2ac7312.ttf
--rw-r--r--   0 grek       (501) staff       (20)    12028 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.e934cbc8.woff2
--rw-r--r--   0 grek       (501) staff       (20)    14112 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.ef725de5.woff
--rw-r--r--   0 grek       (501) staff       (20)    22364 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.f60b4a34.ttf
--rw-r--r--   0 grek       (501) staff       (20)    10344 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.1ac3ed6e.woff2
--rw-r--r--   0 grek       (501) staff       (20)    19436 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.3243452e.ttf
--rw-r--r--   0 grek       (501) staff       (20)    12316 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.5f8637ee.woff
--rw-r--r--   0 grek       (501) staff       (20)     9644 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.1b3161eb.woff2
--rw-r--r--   0 grek       (501) staff       (20)    16648 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a189c37d.ttf
--rw-r--r--   0 grek       (501) staff       (20)    10588 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a82fa2a7.woff
--rw-r--r--   0 grek       (501) staff       (20)    12228 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.0d8d9204.ttf
--rw-r--r--   0 grek       (501) staff       (20)     6496 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.4788ba5b.woff
--rw-r--r--   0 grek       (501) staff       (20)     5468 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.82ef26dc.woff2
--rw-r--r--   0 grek       (501) staff       (20)    11508 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.1fdda0e5.ttf
--rw-r--r--   0 grek       (501) staff       (20)     5208 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.95a1da91.woff2
--rw-r--r--   0 grek       (501) staff       (20)     6188 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.b0628bfd.woff
--rw-r--r--   0 grek       (501) staff       (20)     4420 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.4de844d4.woff
--rw-r--r--   0 grek       (501) staff       (20)     3624 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.9108a400.woff2
--rw-r--r--   0 grek       (501) staff       (20)     7588 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.963af864.ttf
--rw-r--r--   0 grek       (501) staff       (20)    10364 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.27a23ee6.ttf
--rw-r--r--   0 grek       (501) staff       (20)     5980 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.3045a61f.woff
--rw-r--r--   0 grek       (501) staff       (20)     4928 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.61522cd3.woff2
--rw-r--r--   0 grek       (501) staff       (20)    16028 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.0e046058.woff
--rw-r--r--   0 grek       (501) staff       (20)    27556 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.6bf42875.ttf
--rw-r--r--   0 grek       (501) staff       (20)    13568 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.b8b8393d.woff2
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 17:56:25.761141 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat_askgdpr.egg-info/
--rw-r--r--   0 grek       (501) staff       (20)     4157 2023-05-28 17:56:25.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat_askgdpr.egg-info/PKG-INFO
--rw-r--r--   0 grek       (501) staff       (20)     5876 2023-05-28 17:56:25.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat_askgdpr.egg-info/SOURCES.txt
--rw-r--r--   0 grek       (501) staff       (20)        1 2023-05-28 17:56:25.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat_askgdpr.egg-info/dependency_links.txt
--rw-r--r--   0 grek       (501) staff       (20)       16 2023-05-28 17:56:25.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat_askgdpr.egg-info/requires.txt
--rw-r--r--   0 grek       (501) staff       (20)       15 2023-05-28 17:56:25.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat_askgdpr.egg-info/top_level.txt
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:45:39.433693 streamlit-chat-askgdpr-0.1/
+-rw-r--r--   0 grek       (501) staff       (20)     1064 2023-05-28 17:24:10.000000 streamlit-chat-askgdpr-0.1/LICENSE
+-rw-r--r--   0 grek       (501) staff       (20)       50 2023-05-28 17:24:10.000000 streamlit-chat-askgdpr-0.1/MANIFEST.in
+-rw-r--r--   0 grek       (501) staff       (20)     4154 2023-05-28 21:45:39.433503 streamlit-chat-askgdpr-0.1/PKG-INFO
+-rw-r--r--   0 grek       (501) staff       (20)     3687 2023-05-28 17:24:10.000000 streamlit-chat-askgdpr-0.1/README.md
+-rw-r--r--   0 grek       (501) staff       (20)       38 2023-05-28 21:45:39.433743 streamlit-chat-askgdpr-0.1/setup.cfg
+-rw-r--r--   0 grek       (501) staff       (20)      924 2023-05-28 21:33:19.000000 streamlit-chat-askgdpr-0.1/setup.py
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:45:39.399799 streamlit-chat-askgdpr-0.1/streamlit_chat/
+-rw-r--r--   0 grek       (501) staff       (20)     3595 2023-05-28 21:31:47.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/__init__.py
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:45:39.398250 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:45:39.403348 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/
+-rw-r--r--   0 grek       (501) staff       (20)     1150 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/asset-manifest.json
+-rw-r--r--   0 grek       (501) staff       (20)   197459 2023-05-28 21:32:34.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/bootstrap.min.css
+-rw-r--r--   0 grek       (501) staff       (20)   646432 2023-05-28 21:32:34.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/bootstrap.min.css.map
+-rw-r--r--   0 grek       (501) staff       (20)     2209 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/index.html
+-rw-r--r--   0 grek       (501) staff       (20)     8091 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/precache-manifest.913e70ff508b34716fa805cc28b9d423.js
+-rw-r--r--   0 grek       (501) staff       (20)     1183 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/service-worker.js
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:45:39.398523 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:45:39.403748 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/css/
+-rw-r--r--   0 grek       (501) staff       (20)    48144 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css
+-rw-r--r--   0 grek       (501) staff       (20)    64407 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css.map
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:45:39.417174 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/
+-rw-r--r--   0 grek       (501) staff       (20)  1608824 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js
+-rw-r--r--   0 grek       (501) staff       (20)     2015 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.LICENSE.txt
+-rw-r--r--   0 grek       (501) staff       (20)  5402535 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.map
+-rw-r--r--   0 grek       (501) staff       (20)     2106 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/main.e9a08b4d.chunk.js
+-rw-r--r--   0 grek       (501) staff       (20)     5207 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/main.e9a08b4d.chunk.js.map
+-rw-r--r--   0 grek       (501) staff       (20)     1598 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js
+-rw-r--r--   0 grek       (501) staff       (20)     8317 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js.map
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:45:39.432075 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/
+-rw-r--r--   0 grek       (501) staff       (20)    33516 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.10824af7.woff
+-rw-r--r--   0 grek       (501) staff       (20)    63632 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.56573229.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    28076 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.66c67820.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    12368 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.497bf407.ttf
+-rw-r--r--   0 grek       (501) staff       (20)     6912 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.a9e9b095.woff2
+-rw-r--r--   0 grek       (501) staff       (20)     7716 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.de2ba279.woff
+-rw-r--r--   0 grek       (501) staff       (20)     6908 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.08d95d99.woff2
+-rw-r--r--   0 grek       (501) staff       (20)     7656 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.a25140fb.woff
+-rw-r--r--   0 grek       (501) staff       (20)    12344 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.e6fb499f.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    13296 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.40934fc0.woff
+-rw-r--r--   0 grek       (501) staff       (20)    11348 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.796f3797.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    19584 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.b9d7c449.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    19572 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.97a699d8.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    13208 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.e435cda5.woff
+-rw-r--r--   0 grek       (501) staff       (20)    11316 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.f9e6a99f.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    29912 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.4cdba646.woff
+-rw-r--r--   0 grek       (501) staff       (20)    51336 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.8e431f7e.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    25324 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.a9382e25.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    32968 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.52fb39b0.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    19412 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.5f875f98.woff
+-rw-r--r--   0 grek       (501) staff       (20)    16780 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.d8737343.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    33580 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.39349e0a.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    16988 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.65297062.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    19676 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.8ffd28f6.woff
+-rw-r--r--   0 grek       (501) staff       (20)    53580 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.818582da.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    30772 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f1cdb692.woff
+-rw-r--r--   0 grek       (501) staff       (20)    26272 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f8a7f19f.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    16400 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.1320454d.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    18668 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.48155e43.woff
+-rw-r--r--   0 grek       (501) staff       (20)    31196 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.6589c4f1.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    16440 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.d8b7a801.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    18748 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.ed7aea12.woff
+-rw-r--r--   0 grek       (501) staff       (20)    31308 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.fe5ed587.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    14408 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.0e897d27.woff
+-rw-r--r--   0 grek       (501) staff       (20)    12216 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.ad546b47.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    24504 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.f2ac7312.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    12028 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.e934cbc8.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    14112 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.ef725de5.woff
+-rw-r--r--   0 grek       (501) staff       (20)    22364 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.f60b4a34.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    10344 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.1ac3ed6e.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    19436 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.3243452e.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    12316 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.5f8637ee.woff
+-rw-r--r--   0 grek       (501) staff       (20)     9644 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.1b3161eb.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    16648 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a189c37d.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    10588 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a82fa2a7.woff
+-rw-r--r--   0 grek       (501) staff       (20)    12228 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.0d8d9204.ttf
+-rw-r--r--   0 grek       (501) staff       (20)     6496 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.4788ba5b.woff
+-rw-r--r--   0 grek       (501) staff       (20)     5468 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.82ef26dc.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    11508 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.1fdda0e5.ttf
+-rw-r--r--   0 grek       (501) staff       (20)     5208 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.95a1da91.woff2
+-rw-r--r--   0 grek       (501) staff       (20)     6188 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.b0628bfd.woff
+-rw-r--r--   0 grek       (501) staff       (20)     4420 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.4de844d4.woff
+-rw-r--r--   0 grek       (501) staff       (20)     3624 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.9108a400.woff2
+-rw-r--r--   0 grek       (501) staff       (20)     7588 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.963af864.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    10364 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.27a23ee6.ttf
+-rw-r--r--   0 grek       (501) staff       (20)     5980 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.3045a61f.woff
+-rw-r--r--   0 grek       (501) staff       (20)     4928 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.61522cd3.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    16028 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.0e046058.woff
+-rw-r--r--   0 grek       (501) staff       (20)    27556 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.6bf42875.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    13568 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.b8b8393d.woff2
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:45:39.433270 streamlit-chat-askgdpr-0.1/streamlit_chat_askgdpr.egg-info/
+-rw-r--r--   0 grek       (501) staff       (20)     4154 2023-05-28 21:45:39.000000 streamlit-chat-askgdpr-0.1/streamlit_chat_askgdpr.egg-info/PKG-INFO
+-rw-r--r--   0 grek       (501) staff       (20)     5876 2023-05-28 21:45:39.000000 streamlit-chat-askgdpr-0.1/streamlit_chat_askgdpr.egg-info/SOURCES.txt
+-rw-r--r--   0 grek       (501) staff       (20)        1 2023-05-28 21:45:39.000000 streamlit-chat-askgdpr-0.1/streamlit_chat_askgdpr.egg-info/dependency_links.txt
+-rw-r--r--   0 grek       (501) staff       (20)       16 2023-05-28 21:45:39.000000 streamlit-chat-askgdpr-0.1/streamlit_chat_askgdpr.egg-info/requires.txt
+-rw-r--r--   0 grek       (501) staff       (20)       15 2023-05-28 21:45:39.000000 streamlit-chat-askgdpr-0.1/streamlit_chat_askgdpr.egg-info/top_level.txt
```

### Comparing `streamlit-chat-askgdpr-0.0.2.3/LICENSE` & `streamlit-chat-askgdpr-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/PKG-INFO` & `streamlit-chat-askgdpr-0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: streamlit-chat-askgdpr
-Version: 0.0.2.3
+Version: 0.1
 Summary: A streamlit component, to make chatbots
 Home-page: https://github.com/AI-Yash/st-chat
-Author: Yash Pravin Pawar, Yash Vardhan Kapil
+Author: Grzegorz Kossakowski, Maciej Zdanowicz
 Author-email: yashpawarp@gmail.com
 Keywords: chat streamlit streamlit-component
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `streamlit-chat-askgdpr-0.0.2.3/README.md` & `streamlit-chat-askgdpr-0.1/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/setup.py` & `streamlit-chat-askgdpr-0.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setuptools.setup(
     name="streamlit-chat-askgdpr",
-    version="0.0.2.3",
-    author="Yash Pravin Pawar, Yash Vardhan Kapil",
+    version="0.1",
+    author="Grzegorz Kossakowski, Maciej Zdanowicz",
     author_email="yashpawarp@gmail.com",
     description="A streamlit component, to make chatbots",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/AI-Yash/st-chat",
     packages=setuptools.find_packages(),
     include_package_data=True,
```

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/__init__.py` & `streamlit-chat-askgdpr-0.1/streamlit_chat/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,30 +3,29 @@
 from typing import Optional, Union
 
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
-
-_RELEASE = True
+_RELEASE = False
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
-        url = "http://localhost:3001"
+        url = "http://localhost:3000"
     )
 
 # data type for avatar style
 AvatarStyle = Literal[
     "adventurer",
     "adventurer-neutral",
     "avataaars",
@@ -97,8 +96,17 @@
     Designed to convincingly simulate the way a human would behave as a conversational partner, chatbot systems typically require continuous tuning and testing, and many in production remain unable to adequately converse, while none of them can pass the standard Turing test. 
     The term "ChatterBot" was originally coined by Michael Mauldin (creator of the first Verbot) in 1994 to describe these conversational programs.
     """
 
     message("Hello, I am a Chatbot, how may I help you?")
     message("Hey, \nwhat's a chatbot?", is_user=True)
     message(long_message)
+    markdown_msg = """
+Some text
+
+> A quote
+> spanning multuple lines
+
+Some more text
+"""
+    message(markdown_msg)
     st.text_input("Message:")
```

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/asset-manifest.json` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/asset-manifest.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8464285714285714%*

 * *Differences: {"'entrypoints'": "{insert: [(3, 'static/js/main.e9a08b4d.chunk.js')], delete: [3]}",*

 * * "'files'": "{'main.js': './static/js/main.e9a08b4d.chunk.js', 'main.js.map': "*

 * *            "'./static/js/main.e9a08b4d.chunk.js.map', "*

 * *            "'precache-manifest.913e70ff508b34716fa805cc28b9d423.js': "*

 * *            "'./precache-manifest.913e70ff508b34716fa805cc28b9d423.js', delete: "*

 * *            "['precache-manifest.ef63ad040edbb9ce675c41c512a1e329.js']}"}*

```diff
@@ -1,19 +1,19 @@
 {
     "entrypoints": [
         "static/js/runtime-main.11ec9aca.js",
         "static/css/2.4fdd6c40.chunk.css",
         "static/js/2.96b2a504.chunk.js",
-        "static/js/main.4b51ce30.chunk.js"
+        "static/js/main.e9a08b4d.chunk.js"
     ],
     "files": {
         "index.html": "./index.html",
-        "main.js": "./static/js/main.4b51ce30.chunk.js",
-        "main.js.map": "./static/js/main.4b51ce30.chunk.js.map",
-        "precache-manifest.ef63ad040edbb9ce675c41c512a1e329.js": "./precache-manifest.ef63ad040edbb9ce675c41c512a1e329.js",
+        "main.js": "./static/js/main.e9a08b4d.chunk.js",
+        "main.js.map": "./static/js/main.e9a08b4d.chunk.js.map",
+        "precache-manifest.913e70ff508b34716fa805cc28b9d423.js": "./precache-manifest.913e70ff508b34716fa805cc28b9d423.js",
         "runtime-main.js": "./static/js/runtime-main.11ec9aca.js",
         "runtime-main.js.map": "./static/js/runtime-main.11ec9aca.js.map",
         "service-worker.js": "./service-worker.js",
         "static/css/2.4fdd6c40.chunk.css": "./static/css/2.4fdd6c40.chunk.css",
         "static/css/2.4fdd6c40.chunk.css.map": "./static/css/2.4fdd6c40.chunk.css.map",
         "static/js/2.96b2a504.chunk.js": "./static/js/2.96b2a504.chunk.js",
         "static/js/2.96b2a504.chunk.js.LICENSE.txt": "./static/js/2.96b2a504.chunk.js.LICENSE.txt",
```

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/bootstrap.min.css` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/bootstrap.min.css.map` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/index.html` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/><style>table,td,th{border:1px solid}</style><link href="./static/css/2.4fdd6c40.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.96b2a504.chunk.js"></script><script src="./static/js/main.4b51ce30.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/><style>table,td,th{border:1px solid}</style><link href="./static/css/2.4fdd6c40.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.96b2a504.chunk.js"></script><script src="./static/js/main.e9a08b4d.chunk.js"></script></body></html>
```

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/precache-manifest.ef63ad040edbb9ce675c41c512a1e329.js` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/precache-manifest.913e70ff508b34716fa805cc28b9d423.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,22 @@
 self.__precacheManifest = (self.__precacheManifest || []).concat([{
-    "revision": "1a41acc7eabdd301760b384bf8c210fa",
+    "revision": "d3737756586c638b2122a660934b5273",
     "url": "./index.html"
 }, {
     "revision": "69ed66f17e024c470102",
     "url": "./static/css/2.4fdd6c40.chunk.css"
 }, {
     "revision": "69ed66f17e024c470102",
     "url": "./static/js/2.96b2a504.chunk.js"
 }, {
     "revision": "d448927d184e31601f199ee8b38a43f4",
     "url": "./static/js/2.96b2a504.chunk.js.LICENSE.txt"
 }, {
-    "revision": "d5d156dbc96588c95610",
-    "url": "./static/js/main.4b51ce30.chunk.js"
+    "revision": "97ba086a3245ea63db60",
+    "url": "./static/js/main.e9a08b4d.chunk.js"
 }, {
     "revision": "7c26bca7e16783d14d15",
     "url": "./static/js/runtime-main.11ec9aca.js"
 }, {
     "revision": "10824af77e9961cfd548c8a458f10851",
     "url": "./static/media/KaTeX_AMS-Regular.10824af7.woff"
 }, {
```

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/service-worker.js` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/service-worker.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -10,15 +10,15 @@
  * and re-run your build process.
  * See https://goo.gl/2aRDsh
  */
 
 importScripts("https://storage.googleapis.com/workbox-cdn/releases/4.3.1/workbox-sw.js");
 
 importScripts(
-    "./precache-manifest.ef63ad040edbb9ce675c41c512a1e329.js"
+    "./precache-manifest.913e70ff508b34716fa805cc28b9d423.js"
 );
 
 self.addEventListener('message', (event) => {
     if (event.data && event.data.type === 'SKIP_WAITING') {
         self.skipWaiting();
     }
 });
```

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css.map` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.LICENSE.txt` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.map` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/main.4b51ce30.chunk.js` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/main.e9a08b4d.chunk.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -63,23 +63,23 @@
                                     whiteSpace: m ? "normal" : "pre-line"
                                 }),
                                 _ = h.a.div({
                                     display: "flex",
                                     fontFamily: "".concat(b.font, ", 'Segoe UI', 'Roboto', sans-serif"),
                                     height: "auto",
                                     margin: 0,
-                                    width: "100%",
-                                    className: "markdown-body"
+                                    width: "100%"
                                 }, (function(e) {
                                     return e.isUser ? Object(f.a)(r || (r = Object(d.a)(["\n          flex-direction: row-reverse;\n          & > div {\n            text-align: right;\n          }\n        "]))) : Object(f.a)(n || (n = Object(d.a)([""])))
                                 })),
                                 S = [x.a, O.a],
                                 U = [j.a].concat(Object(l.a)(p ? [w.a] : []));
                             return c.a.createElement(_, {
-                                isUser: t
+                                isUser: t,
+                                className: "markdown-body"
                             }, c.a.createElement(k, {
                                 src: u,
                                 alt: "profile",
                                 draggable: "false"
                             }), c.a.createElement(E, null, c.a.createElement(v.a, {
                                 remarkPlugins: S,
                                 rehypePlugins: [].concat(Object(l.a)(U), [
@@ -96,8 +96,8 @@
             s.a.render(c.a.createElement(c.a.StrictMode, null, c.a.createElement(E, null)), document.getElementById("root"))
         }
     },
     [
         [153, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.4b51ce30.chunk.js.map
+//# sourceMappingURL=main.e9a08b4d.chunk.js.map
```

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/main.4b51ce30.chunk.js.map` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/main.e9a08b4d.chunk.js.map`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8068783068783069%*

 * *Differences: {"'file'": "'static/js/main.e9a08b4d.chunk.js'",*

 * * "'mappings'": "'8VAqBMA,G,iOACGC,OAAS,WACdC,IAAUC,eAAeC,OAAOC,aAChC,MAAqE,EAAKC,MAAMC,KAAxEC,EAAR,EAAQA,OAAQC,EAAhB,EAAgBA,YAAaC,EAA7B,EAA6BA,KAAMC,EAAnC,EAAmCA,QAASC,EAA5C,EAA4CA,WAAYC,EAAxD,EAAwDA,SAClDC,EAAS,uCAAmCL,EAAnC,qBAA2DC,GAKlEK,EAAU,EAAKT,MAAfS,MAIR,IAAKA,EACH,OAAO,oFAIT,IAAMC,EAASC,IAAOC,IAAI,CACxBC,OAAO,wBACPC,aAAc,MACdC,OAAQ,OACRC,MAAO,OACPC,OAAQ,IAIJC,EAAUP,IAAOQ,IAAI,CACzBC,QAAS,eACTC,WAAYZ,EAAMa,yBAClBT,OAAQ,wBACRC,aAAc,OACdS,QAAS,YACTN,OAA […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.4b51ce30.chunk.js",
-    "mappings": "8VAqBMA,G,iOACGC,OAAS,WACdC,IAAUC,eAAeC,OAAOC,aAChC,MAAqE,EAAKC,MAAMC,KAAxEC,EAAR,EAAQA,OAAQC,EAAhB,EAAgBA,YAAaC,EAA7B,EAA6BA,KAAMC,EAAnC,EAAmCA,QAASC,EAA5C,EAA4CA,WAAYC,EAAxD,EAAwDA,SAClDC,EAAS,uCAAmCL,EAAnC,qBAA2DC,GAKlEK,EAAU,EAAKT,MAAfS,MAIR,IAAKA,EACH,OAAO,oFAIT,IAAMC,EAASC,IAAOC,IAAI,CACxBC,OAAO,wBACPC,aAAc,MACdC,OAAQ,OACRC,MAAO,OACPC,OAAQ,IAIJC,EAAUP,IAAOQ,IAAI,CACzBC,QAAS,eACTC,WAAYZ,EAAMa,yBAClBT,OAAQ,wBACRC,aAAc,OACdS,QAAS,YACTN,OAAQ,WACRO,SAAU,MACVC,WAAalB,EAAwB,SAAb,aAIpBb,EAAOiB,IAAOQ,IAAI,CACtBC,QAAS,OAETM,WAAW,GAAD,OAAKjB,EAAMkB,KAAX,sCACVZ,OAAQ,OACRE,OAAQ,EACRD,MAAO,OACPY,UAAW,kBAEb,SAAC5B,GACC,OAAIA,EAAME,OACD2B,YAAP,8IAOKA,YAAP,6BAIIC,EAAgB,CACpBC,IACAC,KAEIC,EAAa,CACjBC,KADiB,mBAEb5B,EAAa,CAAC6B,KAAa,KAGjC,OACE,kBAAC,EAAD,CAAMjC,OAAQA,GACZ,kBAACQ,EAAD,CAAQ0B,IAAK5B,EAAW6B,IAAI,UAAUC,UAAU,UAChD,kBAACpB,EAAD,KACE,kBAAC,IAAD,CACEY,cAAeA,EACfG,cAAa,sBAAMA,GAAN,CAAqB,CAACM,IAAiB,CAACC,QAAQ,OAE5DnC,M,yBA9EMoC,MAsFJC,cAAwBhD,GCvGvCiD,IAAShD,OACP,kBAAC,IAAMiD,WAAP,KACE,kBAAC,EAAD,OAEFC,SAASC,eAAe,W",
+    "file": "static/js/main.e9a08b4d.chunk.js",
+    "mappings": "8VAqBMA,G,iOACGC,OAAS,WACdC,IAAUC,eAAeC,OAAOC,aAChC,MAAqE,EAAKC,MAAMC,KAAxEC,EAAR,EAAQA,OAAQC,EAAhB,EAAgBA,YAAaC,EAA7B,EAA6BA,KAAMC,EAAnC,EAAmCA,QAASC,EAA5C,EAA4CA,WAAYC,EAAxD,EAAwDA,SAClDC,EAAS,uCAAmCL,EAAnC,qBAA2DC,GAKlEK,EAAU,EAAKT,MAAfS,MAIR,IAAKA,EACH,OAAO,oFAIT,IAAMC,EAASC,IAAOC,IAAI,CACxBC,OAAO,wBACPC,aAAc,MACdC,OAAQ,OACRC,MAAO,OACPC,OAAQ,IAIJC,EAAUP,IAAOQ,IAAI,CACzBC,QAAS,eACTC,WAAYZ,EAAMa,yBAClBT,OAAQ,wBACRC,aAAc,OACdS,QAAS,YACTN,OAAQ,WACRO,SAAU,MACVC,WAAalB,EAAwB,SAAb,aAIpBb,EAAOiB,IAAOQ,IAAI,CACtBC,QAAS,OAETM,WAAW,GAAD,OAAKjB,EAAMkB,KAAX,sCACVZ,OAAQ,OACRE,OAAQ,EACRD,MAAO,SAET,SAAChB,GACC,OAAIA,EAAME,OACD0B,YAAP,8IAOKA,YAAP,6BAIIC,EAAgB,CACpBC,IACAC,KAEIC,EAAa,CACjBC,KADiB,mBAEb3B,EAAa,CAAC4B,KAAa,KAGjC,OACE,kBAAC,EAAD,CAAMhC,OAAQA,EAAQiC,UAAU,iBAC9B,kBAACzB,EAAD,CAAQ0B,IAAK5B,EAAW6B,IAAI,UAAUC,UAAU,UAChD,kBAACpB,EAAD,KACE,kBAAC,IAAD,CACEW,cAAeA,EACfG,cAAa,sBAAMA,GAAN,CAAqB,CAACO,IAAiB,CAACC,QAAQ,OAE5DnC,M,yBA7EMoC,MAqFJC,cAAwBhD,GCtGvCiD,IAAShD,OACP,kBAAC,IAAMiD,WAAP,KACE,kBAAC,EAAD,OAEFC,SAASC,eAAe,W",
     "names": [
         "Chat",
         "render",
         "Streamlit",
         "setFrameHeight",
         "window",
         "innerHeight",
@@ -32,22 +32,22 @@
         "background",
         "secondaryBackgroundColor",
         "padding",
         "maxWidth",
         "whiteSpace",
         "fontFamily",
         "font",
-        "className",
         "css",
         "remarkPlugins",
         "remarkMath",
         "remarkGfm",
         "rehypePlugins",
         "rehypeKatex",
         "rehypeRaw",
+        "className",
         "src",
         "alt",
         "draggable",
         "rehypeHighlight",
         "detect",
         "StreamlitComponentBase",
         "withStreamlitConnection",
@@ -58,12 +58,12 @@
     ],
     "sourceRoot": "",
     "sources": [
         "stChat.tsx",
         "index.tsx"
     ],
     "sourcesContent": [
-        "import {\n  // eslint-disable-next-line \n  Streamlit,\n  StreamlitComponentBase,\n  withStreamlitConnection,\n} from \"streamlit-component-lib\"\nimport React, { ReactNode } from \"react\"\nimport styled from '@emotion/styled'\nimport { css } from '@emotion/react'\n\nimport ReactMarkdown from \"react-markdown\"\nimport remarkMath from \"remark-math\"\nimport rehypeKatex from \"rehype-katex\"\nimport rehypeRaw from \"rehype-raw\"\nimport remarkGfm from \"remark-gfm\"\nimport rehypeHighlight from \"rehype-highlight\"\n\nimport 'katex/dist/katex.min.css'\nimport 'highlight.js/styles/monokai-sublime.css'\nimport 'github-markdown-css/github-markdown.css'\n\nclass Chat extends StreamlitComponentBase {\n  public render = (): ReactNode => {\n    Streamlit.setFrameHeight(window.innerHeight)\n    const { isUser, avatarStyle, seed, message, allow_html, is_table } = this.props.args;\n    const avatarUrl = `https://api.dicebear.com/5.x/${avatarStyle}/svg?seed=${seed}`\n    \n    // Streamlit sends us a theme object via props that we can use to ensure\n    // that our component has visuals that match the active theme in a\n    // streamlit app.\n    const { theme } = this.props\n    \n    // Maintain compatibility with older versions of Streamlit that don't send\n    // a theme object.\n    if (!theme) {\n      return <div>Theme is undefined, please check streamlit version.</div>\n    }\n    \n    // styles for the avatar image\n    const Avatar = styled.img({\n      border: `1px solid transparent`,\n      borderRadius: '50%',\n      height: '3rem',\n      width: '3rem',\n      margin: 0\n    })\n    \n    // styles for the message box\n    const Message = styled.div({\n      display: 'inline-block',\n      background: theme.secondaryBackgroundColor,\n      border: '1px solid transparent',\n      borderRadius: '10px',\n      padding: '10px 14px',\n      margin: '5px 20px',\n      maxWidth: '70%',\n      whiteSpace: !is_table ? 'pre-line' : 'normal'\n    })\n    \n    // styles for the container\n    const Chat = styled.div({\n      display: 'flex',\n      // flexDirection: 'row',\n      fontFamily: `${theme.font}, 'Segoe UI', 'Roboto', sans-serif`, \n      height: 'auto',\n      margin: 0,\n      width: '100%',\n      className: 'markdown-body'\n    },\n    (props: {isUser: boolean}) => {  // specific styles\n      if (props.isUser){\n        return css`\n          flex-direction: row-reverse;\n          & > div {\n            text-align: right;\n          }\n        `\n      }\n      return css``\n    })\n\n    // Init React Markdown plugins\n    const remarkPlugins = [\n      remarkMath, \n      remarkGfm\n    ]\n    const rehypePlugins = [\n      rehypeKatex,\n      ...(allow_html ? [rehypeRaw] : [])\n    ]\n\n    return (\n      <Chat isUser={isUser}>\n        <Avatar src={avatarUrl} alt=\"profile\" draggable=\"false\"/>\n        <Message>\n          <ReactMarkdown \n            remarkPlugins={remarkPlugins}\n            rehypePlugins={[...rehypePlugins, [rehypeHighlight, {detect: true}]]}\n          >\n            {message}\n          </ReactMarkdown>\n        </Message>\n      </Chat>\n    )\n  }\n}\n\nexport default withStreamlitConnection(Chat);\n",
+        "import {\n  // eslint-disable-next-line \n  Streamlit,\n  StreamlitComponentBase,\n  withStreamlitConnection,\n} from \"streamlit-component-lib\"\nimport React, { ReactNode } from \"react\"\nimport styled from '@emotion/styled'\nimport { css } from '@emotion/react'\n\nimport ReactMarkdown from \"react-markdown\"\nimport remarkMath from \"remark-math\"\nimport rehypeKatex from \"rehype-katex\"\nimport rehypeRaw from \"rehype-raw\"\nimport remarkGfm from \"remark-gfm\"\nimport rehypeHighlight from \"rehype-highlight\"\n\nimport 'katex/dist/katex.min.css'\nimport 'highlight.js/styles/monokai-sublime.css'\nimport 'github-markdown-css/github-markdown.css'\n\nclass Chat extends StreamlitComponentBase {\n  public render = (): ReactNode => {\n    Streamlit.setFrameHeight(window.innerHeight)\n    const { isUser, avatarStyle, seed, message, allow_html, is_table } = this.props.args;\n    const avatarUrl = `https://api.dicebear.com/5.x/${avatarStyle}/svg?seed=${seed}`\n    \n    // Streamlit sends us a theme object via props that we can use to ensure\n    // that our component has visuals that match the active theme in a\n    // streamlit app.\n    const { theme } = this.props\n    \n    // Maintain compatibility with older versions of Streamlit that don't send\n    // a theme object.\n    if (!theme) {\n      return <div>Theme is undefined, please check streamlit version.</div>\n    }\n    \n    // styles for the avatar image\n    const Avatar = styled.img({\n      border: `1px solid transparent`,\n      borderRadius: '50%',\n      height: '3rem',\n      width: '3rem',\n      margin: 0\n    })\n    \n    // styles for the message box\n    const Message = styled.div({\n      display: 'inline-block',\n      background: theme.secondaryBackgroundColor,\n      border: '1px solid transparent',\n      borderRadius: '10px',\n      padding: '10px 14px',\n      margin: '5px 20px',\n      maxWidth: '70%',\n      whiteSpace: !is_table ? 'pre-line' : 'normal'\n    })\n    \n    // styles for the container\n    const Chat = styled.div({\n      display: 'flex',\n      // flexDirection: 'row',\n      fontFamily: `${theme.font}, 'Segoe UI', 'Roboto', sans-serif`, \n      height: 'auto',\n      margin: 0,\n      width: '100%'\n    },\n    (props: {isUser: boolean}) => {  // specific styles\n      if (props.isUser){\n        return css`\n          flex-direction: row-reverse;\n          & > div {\n            text-align: right;\n          }\n        `\n      }\n      return css``\n    })\n\n    // Init React Markdown plugins\n    const remarkPlugins = [\n      remarkMath, \n      remarkGfm\n    ]\n    const rehypePlugins = [\n      rehypeKatex,\n      ...(allow_html ? [rehypeRaw] : [])\n    ]\n\n    return (\n      <Chat isUser={isUser} className='markdown-body'>\n        <Avatar src={avatarUrl} alt=\"profile\" draggable=\"false\"/>\n        <Message>\n          <ReactMarkdown \n            remarkPlugins={remarkPlugins}\n            rehypePlugins={[...rehypePlugins, [rehypeHighlight, {detect: true}]]}\n          >\n            {message}\n          </ReactMarkdown>\n        </Message>\n      </Chat>\n    )\n  }\n}\n\nexport default withStreamlitConnection(Chat);\n",
         "import React from \"react\"\nimport ReactDOM from \"react-dom\"\nimport Chat from \"./stChat\"\n\nReactDOM.render(\n  <React.StrictMode>\n    <Chat />\n  </React.StrictMode>,\n  document.getElementById(\"root\")\n)\n"
     ],
     "version": 3
 }
```

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js.map` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.10824af7.woff` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.10824af7.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.56573229.ttf` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.56573229.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.66c67820.woff2` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.66c67820.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.497bf407.ttf` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.497bf407.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.a9e9b095.woff2` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.a9e9b095.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.de2ba279.woff` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.de2ba279.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.08d95d99.woff2` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.08d95d99.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.a25140fb.woff` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.a25140fb.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.e6fb499f.ttf` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.e6fb499f.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.40934fc0.woff` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.40934fc0.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.796f3797.woff2` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.796f3797.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.b9d7c449.ttf` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.b9d7c449.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.97a699d8.ttf` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.97a699d8.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.e435cda5.woff` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.e435cda5.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.f9e6a99f.woff2` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.f9e6a99f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.4cdba646.woff` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.4cdba646.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.8e431f7e.ttf` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.8e431f7e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.a9382e25.woff2` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.a9382e25.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.52fb39b0.ttf` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.52fb39b0.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.5f875f98.woff` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.5f875f98.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.d8737343.woff2` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.d8737343.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.39349e0a.ttf` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.39349e0a.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.65297062.woff2` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.65297062.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.8ffd28f6.woff` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.8ffd28f6.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.818582da.ttf` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.818582da.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f1cdb692.woff` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f1cdb692.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f8a7f19f.woff2` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f8a7f19f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.1320454d.woff2` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.1320454d.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.48155e43.woff` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.48155e43.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.6589c4f1.ttf` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.6589c4f1.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.d8b7a801.woff2` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.d8b7a801.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.ed7aea12.woff` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.ed7aea12.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.fe5ed587.ttf` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.fe5ed587.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.0e897d27.woff` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.0e897d27.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.ad546b47.woff2` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.ad546b47.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.f2ac7312.ttf` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.f2ac7312.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.e934cbc8.woff2` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.e934cbc8.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.ef725de5.woff` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.ef725de5.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.f60b4a34.ttf` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.f60b4a34.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.1ac3ed6e.woff2` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.1ac3ed6e.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.3243452e.ttf` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.3243452e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.5f8637ee.woff` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.5f8637ee.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.1b3161eb.woff2` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.1b3161eb.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a189c37d.ttf` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a189c37d.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a82fa2a7.woff` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a82fa2a7.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.0d8d9204.ttf` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.0d8d9204.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.4788ba5b.woff` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.4788ba5b.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.82ef26dc.woff2` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.82ef26dc.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.1fdda0e5.ttf` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.1fdda0e5.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.95a1da91.woff2` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.95a1da91.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.b0628bfd.woff` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.b0628bfd.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.4de844d4.woff` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.4de844d4.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.9108a400.woff2` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.9108a400.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.963af864.ttf` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.963af864.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.27a23ee6.ttf` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.27a23ee6.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.3045a61f.woff` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.3045a61f.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.61522cd3.woff2` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.61522cd3.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.0e046058.woff` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.0e046058.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.6bf42875.ttf` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.6bf42875.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.b8b8393d.woff2` & `streamlit-chat-askgdpr-0.1/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.b8b8393d.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat_askgdpr.egg-info/PKG-INFO` & `streamlit-chat-askgdpr-0.1/streamlit_chat_askgdpr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: streamlit-chat-askgdpr
-Version: 0.0.2.3
+Version: 0.1
 Summary: A streamlit component, to make chatbots
 Home-page: https://github.com/AI-Yash/st-chat
-Author: Yash Pravin Pawar, Yash Vardhan Kapil
+Author: Grzegorz Kossakowski, Maciej Zdanowicz
 Author-email: yashpawarp@gmail.com
 Keywords: chat streamlit streamlit-component
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat_askgdpr.egg-info/SOURCES.txt` & `streamlit-chat-askgdpr-0.1/streamlit_chat_askgdpr.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 README.md
 setup.py
 streamlit_chat/__init__.py
 streamlit_chat/frontend/build/asset-manifest.json
 streamlit_chat/frontend/build/bootstrap.min.css
 streamlit_chat/frontend/build/bootstrap.min.css.map
 streamlit_chat/frontend/build/index.html
-streamlit_chat/frontend/build/precache-manifest.ef63ad040edbb9ce675c41c512a1e329.js
+streamlit_chat/frontend/build/precache-manifest.913e70ff508b34716fa805cc28b9d423.js
 streamlit_chat/frontend/build/service-worker.js
 streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css
 streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css.map
 streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js
 streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.LICENSE.txt
 streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.map
-streamlit_chat/frontend/build/static/js/main.4b51ce30.chunk.js
-streamlit_chat/frontend/build/static/js/main.4b51ce30.chunk.js.map
+streamlit_chat/frontend/build/static/js/main.e9a08b4d.chunk.js
+streamlit_chat/frontend/build/static/js/main.e9a08b4d.chunk.js.map
 streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js
 streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js.map
 streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.10824af7.woff
 streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.56573229.ttf
 streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.66c67820.woff2
 streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.497bf407.ttf
 streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.a9e9b095.woff2
```

