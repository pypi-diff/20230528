# Comparing `tmp/streamlit-chat-askgdpr-0.0.2.2.tar.gz` & `tmp/streamlit-chat-askgdpr-0.0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-chat-askgdpr-0.0.2.2.tar", last modified: Sun May 28 17:41:13 2023, max compression
+gzip compressed data, was "streamlit-chat-askgdpr-0.0.2.3.tar", last modified: Sun May 28 17:56:25 2023, max compression
```

## Comparing `streamlit-chat-askgdpr-0.0.2.2.tar` & `streamlit-chat-askgdpr-0.0.2.3.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 17:41:13.077062 streamlit-chat-askgdpr-0.0.2.2/
--rw-r--r--   0 grek       (501) staff       (20)     1064 2023-05-28 17:24:10.000000 streamlit-chat-askgdpr-0.0.2.2/LICENSE
--rw-r--r--   0 grek       (501) staff       (20)       50 2023-05-28 17:24:10.000000 streamlit-chat-askgdpr-0.0.2.2/MANIFEST.in
--rw-r--r--   0 grek       (501) staff       (20)     4157 2023-05-28 17:41:13.076860 streamlit-chat-askgdpr-0.0.2.2/PKG-INFO
--rw-r--r--   0 grek       (501) staff       (20)     3687 2023-05-28 17:24:10.000000 streamlit-chat-askgdpr-0.0.2.2/README.md
--rw-r--r--   0 grek       (501) staff       (20)       38 2023-05-28 17:41:13.077113 streamlit-chat-askgdpr-0.0.2.2/setup.cfg
--rw-r--r--   0 grek       (501) staff       (20)      927 2023-05-28 17:33:28.000000 streamlit-chat-askgdpr-0.0.2.2/setup.py
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 17:41:13.050274 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/
--rw-r--r--   0 grek       (501) staff       (20)     3479 2023-05-28 17:24:10.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/__init__.py
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 17:41:13.048995 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 17:41:13.052020 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/
--rw-r--r--   0 grek       (501) staff       (20)     1150 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/asset-manifest.json
--rw-r--r--   0 grek       (501) staff       (20)   197459 2023-05-28 17:25:26.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/bootstrap.min.css
--rw-r--r--   0 grek       (501) staff       (20)   646432 2023-05-28 17:25:26.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/bootstrap.min.css.map
--rw-r--r--   0 grek       (501) staff       (20)     2209 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/index.html
--rw-r--r--   0 grek       (501) staff       (20)     8091 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/precache-manifest.23251c9018266309f6f19dbaa6149265.js
--rw-r--r--   0 grek       (501) staff       (20)     1183 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/service-worker.js
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 17:41:13.049285 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 17:41:13.052353 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/css/
--rw-r--r--   0 grek       (501) staff       (20)    25275 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/css/2.95a91b17.chunk.css
--rw-r--r--   0 grek       (501) staff       (20)    30768 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/css/2.95a91b17.chunk.css.map
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 17:41:13.066424 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/js/
--rw-r--r--   0 grek       (501) staff       (20)  1608806 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/js/2.53d4e8c0.chunk.js
--rw-r--r--   0 grek       (501) staff       (20)     2015 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/js/2.53d4e8c0.chunk.js.LICENSE.txt
--rw-r--r--   0 grek       (501) staff       (20)  5402535 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/js/2.53d4e8c0.chunk.js.map
--rw-r--r--   0 grek       (501) staff       (20)     2073 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/js/main.a4e8bdc7.chunk.js
--rw-r--r--   0 grek       (501) staff       (20)     5107 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/js/main.a4e8bdc7.chunk.js.map
--rw-r--r--   0 grek       (501) staff       (20)     1598 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js
--rw-r--r--   0 grek       (501) staff       (20)     8317 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js.map
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 17:41:13.075919 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/
--rw-r--r--   0 grek       (501) staff       (20)    33516 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.10824af7.woff
--rw-r--r--   0 grek       (501) staff       (20)    63632 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.56573229.ttf
--rw-r--r--   0 grek       (501) staff       (20)    28076 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.66c67820.woff2
--rw-r--r--   0 grek       (501) staff       (20)    12368 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.497bf407.ttf
--rw-r--r--   0 grek       (501) staff       (20)     6912 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.a9e9b095.woff2
--rw-r--r--   0 grek       (501) staff       (20)     7716 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.de2ba279.woff
--rw-r--r--   0 grek       (501) staff       (20)     6908 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.08d95d99.woff2
--rw-r--r--   0 grek       (501) staff       (20)     7656 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.a25140fb.woff
--rw-r--r--   0 grek       (501) staff       (20)    12344 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.e6fb499f.ttf
--rw-r--r--   0 grek       (501) staff       (20)    13296 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.40934fc0.woff
--rw-r--r--   0 grek       (501) staff       (20)    11348 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.796f3797.woff2
--rw-r--r--   0 grek       (501) staff       (20)    19584 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.b9d7c449.ttf
--rw-r--r--   0 grek       (501) staff       (20)    19572 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.97a699d8.ttf
--rw-r--r--   0 grek       (501) staff       (20)    13208 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.e435cda5.woff
--rw-r--r--   0 grek       (501) staff       (20)    11316 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.f9e6a99f.woff2
--rw-r--r--   0 grek       (501) staff       (20)    29912 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.4cdba646.woff
--rw-r--r--   0 grek       (501) staff       (20)    51336 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.8e431f7e.ttf
--rw-r--r--   0 grek       (501) staff       (20)    25324 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.a9382e25.woff2
--rw-r--r--   0 grek       (501) staff       (20)    32968 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.52fb39b0.ttf
--rw-r--r--   0 grek       (501) staff       (20)    19412 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.5f875f98.woff
--rw-r--r--   0 grek       (501) staff       (20)    16780 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.d8737343.woff2
--rw-r--r--   0 grek       (501) staff       (20)    33580 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.39349e0a.ttf
--rw-r--r--   0 grek       (501) staff       (20)    16988 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.65297062.woff2
--rw-r--r--   0 grek       (501) staff       (20)    19676 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.8ffd28f6.woff
--rw-r--r--   0 grek       (501) staff       (20)    53580 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.818582da.ttf
--rw-r--r--   0 grek       (501) staff       (20)    30772 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f1cdb692.woff
--rw-r--r--   0 grek       (501) staff       (20)    26272 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f8a7f19f.woff2
--rw-r--r--   0 grek       (501) staff       (20)    16400 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.1320454d.woff2
--rw-r--r--   0 grek       (501) staff       (20)    18668 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.48155e43.woff
--rw-r--r--   0 grek       (501) staff       (20)    31196 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.6589c4f1.ttf
--rw-r--r--   0 grek       (501) staff       (20)    16440 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.d8b7a801.woff2
--rw-r--r--   0 grek       (501) staff       (20)    18748 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.ed7aea12.woff
--rw-r--r--   0 grek       (501) staff       (20)    31308 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.fe5ed587.ttf
--rw-r--r--   0 grek       (501) staff       (20)    14408 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.0e897d27.woff
--rw-r--r--   0 grek       (501) staff       (20)    12216 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.ad546b47.woff2
--rw-r--r--   0 grek       (501) staff       (20)    24504 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.f2ac7312.ttf
--rw-r--r--   0 grek       (501) staff       (20)    12028 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.e934cbc8.woff2
--rw-r--r--   0 grek       (501) staff       (20)    14112 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.ef725de5.woff
--rw-r--r--   0 grek       (501) staff       (20)    22364 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.f60b4a34.ttf
--rw-r--r--   0 grek       (501) staff       (20)    10344 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.1ac3ed6e.woff2
--rw-r--r--   0 grek       (501) staff       (20)    19436 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.3243452e.ttf
--rw-r--r--   0 grek       (501) staff       (20)    12316 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.5f8637ee.woff
--rw-r--r--   0 grek       (501) staff       (20)     9644 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.1b3161eb.woff2
--rw-r--r--   0 grek       (501) staff       (20)    16648 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a189c37d.ttf
--rw-r--r--   0 grek       (501) staff       (20)    10588 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a82fa2a7.woff
--rw-r--r--   0 grek       (501) staff       (20)    12228 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.0d8d9204.ttf
--rw-r--r--   0 grek       (501) staff       (20)     6496 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.4788ba5b.woff
--rw-r--r--   0 grek       (501) staff       (20)     5468 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.82ef26dc.woff2
--rw-r--r--   0 grek       (501) staff       (20)    11508 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.1fdda0e5.ttf
--rw-r--r--   0 grek       (501) staff       (20)     5208 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.95a1da91.woff2
--rw-r--r--   0 grek       (501) staff       (20)     6188 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.b0628bfd.woff
--rw-r--r--   0 grek       (501) staff       (20)     4420 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.4de844d4.woff
--rw-r--r--   0 grek       (501) staff       (20)     3624 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.9108a400.woff2
--rw-r--r--   0 grek       (501) staff       (20)     7588 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.963af864.ttf
--rw-r--r--   0 grek       (501) staff       (20)    10364 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.27a23ee6.ttf
--rw-r--r--   0 grek       (501) staff       (20)     5980 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.3045a61f.woff
--rw-r--r--   0 grek       (501) staff       (20)     4928 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.61522cd3.woff2
--rw-r--r--   0 grek       (501) staff       (20)    16028 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.0e046058.woff
--rw-r--r--   0 grek       (501) staff       (20)    27556 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.6bf42875.ttf
--rw-r--r--   0 grek       (501) staff       (20)    13568 2023-05-28 17:25:42.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.b8b8393d.woff2
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 17:41:13.076606 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat_askgdpr.egg-info/
--rw-r--r--   0 grek       (501) staff       (20)     4157 2023-05-28 17:41:12.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat_askgdpr.egg-info/PKG-INFO
--rw-r--r--   0 grek       (501) staff       (20)     5876 2023-05-28 17:41:12.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat_askgdpr.egg-info/SOURCES.txt
--rw-r--r--   0 grek       (501) staff       (20)        1 2023-05-28 17:41:12.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat_askgdpr.egg-info/dependency_links.txt
--rw-r--r--   0 grek       (501) staff       (20)       16 2023-05-28 17:41:12.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat_askgdpr.egg-info/requires.txt
--rw-r--r--   0 grek       (501) staff       (20)       15 2023-05-28 17:41:12.000000 streamlit-chat-askgdpr-0.0.2.2/streamlit_chat_askgdpr.egg-info/top_level.txt
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 17:56:25.761594 streamlit-chat-askgdpr-0.0.2.3/
+-rw-r--r--   0 grek       (501) staff       (20)     1064 2023-05-28 17:24:10.000000 streamlit-chat-askgdpr-0.0.2.3/LICENSE
+-rw-r--r--   0 grek       (501) staff       (20)       50 2023-05-28 17:24:10.000000 streamlit-chat-askgdpr-0.0.2.3/MANIFEST.in
+-rw-r--r--   0 grek       (501) staff       (20)     4157 2023-05-28 17:56:25.761402 streamlit-chat-askgdpr-0.0.2.3/PKG-INFO
+-rw-r--r--   0 grek       (501) staff       (20)     3687 2023-05-28 17:24:10.000000 streamlit-chat-askgdpr-0.0.2.3/README.md
+-rw-r--r--   0 grek       (501) staff       (20)       38 2023-05-28 17:56:25.761650 streamlit-chat-askgdpr-0.0.2.3/setup.cfg
+-rw-r--r--   0 grek       (501) staff       (20)      927 2023-05-28 17:55:34.000000 streamlit-chat-askgdpr-0.0.2.3/setup.py
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 17:56:25.736258 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/
+-rw-r--r--   0 grek       (501) staff       (20)     3479 2023-05-28 17:24:10.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/__init__.py
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 17:56:25.735170 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 17:56:25.737745 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/
+-rw-r--r--   0 grek       (501) staff       (20)     1150 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/asset-manifest.json
+-rw-r--r--   0 grek       (501) staff       (20)   197459 2023-05-28 17:53:41.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/bootstrap.min.css
+-rw-r--r--   0 grek       (501) staff       (20)   646432 2023-05-28 17:53:41.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/bootstrap.min.css.map
+-rw-r--r--   0 grek       (501) staff       (20)     2209 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/index.html
+-rw-r--r--   0 grek       (501) staff       (20)     8091 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/precache-manifest.ef63ad040edbb9ce675c41c512a1e329.js
+-rw-r--r--   0 grek       (501) staff       (20)     1183 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/service-worker.js
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 17:56:25.735441 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 17:56:25.738090 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/css/
+-rw-r--r--   0 grek       (501) staff       (20)    48144 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css
+-rw-r--r--   0 grek       (501) staff       (20)    64407 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css.map
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 17:56:25.744825 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/
+-rw-r--r--   0 grek       (501) staff       (20)  1608824 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js
+-rw-r--r--   0 grek       (501) staff       (20)     2015 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.LICENSE.txt
+-rw-r--r--   0 grek       (501) staff       (20)  5402535 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.map
+-rw-r--r--   0 grek       (501) staff       (20)     2106 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/main.4b51ce30.chunk.js
+-rw-r--r--   0 grek       (501) staff       (20)     5213 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/main.4b51ce30.chunk.js.map
+-rw-r--r--   0 grek       (501) staff       (20)     1598 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js
+-rw-r--r--   0 grek       (501) staff       (20)     8317 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js.map
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 17:56:25.760184 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/
+-rw-r--r--   0 grek       (501) staff       (20)    33516 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.10824af7.woff
+-rw-r--r--   0 grek       (501) staff       (20)    63632 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.56573229.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    28076 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.66c67820.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    12368 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.497bf407.ttf
+-rw-r--r--   0 grek       (501) staff       (20)     6912 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.a9e9b095.woff2
+-rw-r--r--   0 grek       (501) staff       (20)     7716 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.de2ba279.woff
+-rw-r--r--   0 grek       (501) staff       (20)     6908 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.08d95d99.woff2
+-rw-r--r--   0 grek       (501) staff       (20)     7656 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.a25140fb.woff
+-rw-r--r--   0 grek       (501) staff       (20)    12344 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.e6fb499f.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    13296 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.40934fc0.woff
+-rw-r--r--   0 grek       (501) staff       (20)    11348 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.796f3797.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    19584 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.b9d7c449.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    19572 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.97a699d8.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    13208 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.e435cda5.woff
+-rw-r--r--   0 grek       (501) staff       (20)    11316 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.f9e6a99f.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    29912 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.4cdba646.woff
+-rw-r--r--   0 grek       (501) staff       (20)    51336 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.8e431f7e.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    25324 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.a9382e25.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    32968 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.52fb39b0.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    19412 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.5f875f98.woff
+-rw-r--r--   0 grek       (501) staff       (20)    16780 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.d8737343.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    33580 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.39349e0a.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    16988 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.65297062.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    19676 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.8ffd28f6.woff
+-rw-r--r--   0 grek       (501) staff       (20)    53580 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.818582da.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    30772 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f1cdb692.woff
+-rw-r--r--   0 grek       (501) staff       (20)    26272 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f8a7f19f.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    16400 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.1320454d.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    18668 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.48155e43.woff
+-rw-r--r--   0 grek       (501) staff       (20)    31196 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.6589c4f1.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    16440 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.d8b7a801.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    18748 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.ed7aea12.woff
+-rw-r--r--   0 grek       (501) staff       (20)    31308 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.fe5ed587.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    14408 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.0e897d27.woff
+-rw-r--r--   0 grek       (501) staff       (20)    12216 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.ad546b47.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    24504 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.f2ac7312.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    12028 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.e934cbc8.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    14112 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.ef725de5.woff
+-rw-r--r--   0 grek       (501) staff       (20)    22364 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.f60b4a34.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    10344 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.1ac3ed6e.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    19436 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.3243452e.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    12316 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.5f8637ee.woff
+-rw-r--r--   0 grek       (501) staff       (20)     9644 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.1b3161eb.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    16648 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a189c37d.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    10588 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a82fa2a7.woff
+-rw-r--r--   0 grek       (501) staff       (20)    12228 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.0d8d9204.ttf
+-rw-r--r--   0 grek       (501) staff       (20)     6496 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.4788ba5b.woff
+-rw-r--r--   0 grek       (501) staff       (20)     5468 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.82ef26dc.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    11508 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.1fdda0e5.ttf
+-rw-r--r--   0 grek       (501) staff       (20)     5208 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.95a1da91.woff2
+-rw-r--r--   0 grek       (501) staff       (20)     6188 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.b0628bfd.woff
+-rw-r--r--   0 grek       (501) staff       (20)     4420 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.4de844d4.woff
+-rw-r--r--   0 grek       (501) staff       (20)     3624 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.9108a400.woff2
+-rw-r--r--   0 grek       (501) staff       (20)     7588 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.963af864.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    10364 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.27a23ee6.ttf
+-rw-r--r--   0 grek       (501) staff       (20)     5980 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.3045a61f.woff
+-rw-r--r--   0 grek       (501) staff       (20)     4928 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.61522cd3.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    16028 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.0e046058.woff
+-rw-r--r--   0 grek       (501) staff       (20)    27556 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.6bf42875.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    13568 2023-05-28 17:53:52.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.b8b8393d.woff2
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 17:56:25.761141 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat_askgdpr.egg-info/
+-rw-r--r--   0 grek       (501) staff       (20)     4157 2023-05-28 17:56:25.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat_askgdpr.egg-info/PKG-INFO
+-rw-r--r--   0 grek       (501) staff       (20)     5876 2023-05-28 17:56:25.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat_askgdpr.egg-info/SOURCES.txt
+-rw-r--r--   0 grek       (501) staff       (20)        1 2023-05-28 17:56:25.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat_askgdpr.egg-info/dependency_links.txt
+-rw-r--r--   0 grek       (501) staff       (20)       16 2023-05-28 17:56:25.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat_askgdpr.egg-info/requires.txt
+-rw-r--r--   0 grek       (501) staff       (20)       15 2023-05-28 17:56:25.000000 streamlit-chat-askgdpr-0.0.2.3/streamlit_chat_askgdpr.egg-info/top_level.txt
```

### Comparing `streamlit-chat-askgdpr-0.0.2.2/LICENSE` & `streamlit-chat-askgdpr-0.0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/PKG-INFO` & `streamlit-chat-askgdpr-0.0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-chat-askgdpr
-Version: 0.0.2.2
+Version: 0.0.2.3
 Summary: A streamlit component, to make chatbots
 Home-page: https://github.com/AI-Yash/st-chat
 Author: Yash Pravin Pawar, Yash Vardhan Kapil
 Author-email: yashpawarp@gmail.com
 Keywords: chat streamlit streamlit-component
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `streamlit-chat-askgdpr-0.0.2.2/README.md` & `streamlit-chat-askgdpr-0.0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/setup.py` & `streamlit-chat-askgdpr-0.0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setuptools.setup(
     name="streamlit-chat-askgdpr",
-    version="0.0.2.2",
+    version="0.0.2.3",
     author="Yash Pravin Pawar, Yash Vardhan Kapil",
     author_email="yashpawarp@gmail.com",
     description="A streamlit component, to make chatbots",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/AI-Yash/st-chat",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/__init__.py` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/asset-manifest.json` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/asset-manifest.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6146616541353384%*

 * *Differences: {"'entrypoints'": "{insert: [(1, 'static/css/2.4fdd6c40.chunk.css'), (2, "*

 * *                  "'static/js/2.96b2a504.chunk.js'), (3, 'static/js/main.4b51ce30.chunk.js')], "*

 * *                  'delete: [3, 2, 1]}',*

 * * "'files'": "{'main.js': './static/js/main.4b51ce30.chunk.js', 'main.js.map': "*

 * *            "'./static/js/main.4b51ce30.chunk.js.map', 'static/css/2.4fdd6c40.chunk.css': "*

 * *            "'./static/css/2.4fdd6c40.chunk.css', 'static/js/2.96b2a504.chunk.js': "*

 * *            "'./static/js/2.96b2a504.chunk. […]*

```diff
@@ -1,23 +1,23 @@
 {
     "entrypoints": [
         "static/js/runtime-main.11ec9aca.js",
-        "static/css/2.95a91b17.chunk.css",
-        "static/js/2.53d4e8c0.chunk.js",
-        "static/js/main.a4e8bdc7.chunk.js"
+        "static/css/2.4fdd6c40.chunk.css",
+        "static/js/2.96b2a504.chunk.js",
+        "static/js/main.4b51ce30.chunk.js"
     ],
     "files": {
         "index.html": "./index.html",
-        "main.js": "./static/js/main.a4e8bdc7.chunk.js",
-        "main.js.map": "./static/js/main.a4e8bdc7.chunk.js.map",
-        "precache-manifest.23251c9018266309f6f19dbaa6149265.js": "./precache-manifest.23251c9018266309f6f19dbaa6149265.js",
+        "main.js": "./static/js/main.4b51ce30.chunk.js",
+        "main.js.map": "./static/js/main.4b51ce30.chunk.js.map",
+        "precache-manifest.ef63ad040edbb9ce675c41c512a1e329.js": "./precache-manifest.ef63ad040edbb9ce675c41c512a1e329.js",
         "runtime-main.js": "./static/js/runtime-main.11ec9aca.js",
         "runtime-main.js.map": "./static/js/runtime-main.11ec9aca.js.map",
         "service-worker.js": "./service-worker.js",
-        "static/css/2.95a91b17.chunk.css": "./static/css/2.95a91b17.chunk.css",
-        "static/css/2.95a91b17.chunk.css.map": "./static/css/2.95a91b17.chunk.css.map",
-        "static/js/2.53d4e8c0.chunk.js": "./static/js/2.53d4e8c0.chunk.js",
-        "static/js/2.53d4e8c0.chunk.js.LICENSE.txt": "./static/js/2.53d4e8c0.chunk.js.LICENSE.txt",
-        "static/js/2.53d4e8c0.chunk.js.map": "./static/js/2.53d4e8c0.chunk.js.map",
+        "static/css/2.4fdd6c40.chunk.css": "./static/css/2.4fdd6c40.chunk.css",
+        "static/css/2.4fdd6c40.chunk.css.map": "./static/css/2.4fdd6c40.chunk.css.map",
+        "static/js/2.96b2a504.chunk.js": "./static/js/2.96b2a504.chunk.js",
+        "static/js/2.96b2a504.chunk.js.LICENSE.txt": "./static/js/2.96b2a504.chunk.js.LICENSE.txt",
+        "static/js/2.96b2a504.chunk.js.map": "./static/js/2.96b2a504.chunk.js.map",
         "static/media/katex.min.css": "./static/media/KaTeX_Typewriter-Regular.b8b8393d.woff2"
     }
 }
```

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/bootstrap.min.css` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/bootstrap.min.css.map` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/index.html` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/><style>table,td,th{border:1px solid}</style><link href="./static/css/2.95a91b17.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.53d4e8c0.chunk.js"></script><script src="./static/js/main.a4e8bdc7.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/><style>table,td,th{border:1px solid}</style><link href="./static/css/2.4fdd6c40.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.96b2a504.chunk.js"></script><script src="./static/js/main.4b51ce30.chunk.js"></script></body></html>
```

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/precache-manifest.23251c9018266309f6f19dbaa6149265.js` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/precache-manifest.ef63ad040edbb9ce675c41c512a1e329.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,22 @@
 self.__precacheManifest = (self.__precacheManifest || []).concat([{
-    "revision": "8cc980128f8ddf31040355a4fff20c7c",
+    "revision": "1a41acc7eabdd301760b384bf8c210fa",
     "url": "./index.html"
 }, {
-    "revision": "b128f781e874bbac0101",
-    "url": "./static/css/2.95a91b17.chunk.css"
+    "revision": "69ed66f17e024c470102",
+    "url": "./static/css/2.4fdd6c40.chunk.css"
 }, {
-    "revision": "b128f781e874bbac0101",
-    "url": "./static/js/2.53d4e8c0.chunk.js"
+    "revision": "69ed66f17e024c470102",
+    "url": "./static/js/2.96b2a504.chunk.js"
 }, {
     "revision": "d448927d184e31601f199ee8b38a43f4",
-    "url": "./static/js/2.53d4e8c0.chunk.js.LICENSE.txt"
+    "url": "./static/js/2.96b2a504.chunk.js.LICENSE.txt"
 }, {
-    "revision": "8882eb77c2a52fa05479",
-    "url": "./static/js/main.a4e8bdc7.chunk.js"
+    "revision": "d5d156dbc96588c95610",
+    "url": "./static/js/main.4b51ce30.chunk.js"
 }, {
     "revision": "7c26bca7e16783d14d15",
     "url": "./static/js/runtime-main.11ec9aca.js"
 }, {
     "revision": "10824af77e9961cfd548c8a458f10851",
     "url": "./static/media/KaTeX_AMS-Regular.10824af7.woff"
 }, {
```

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/service-worker.js` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/service-worker.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -10,15 +10,15 @@
  * and re-run your build process.
  * See https://goo.gl/2aRDsh
  */
 
 importScripts("https://storage.googleapis.com/workbox-cdn/releases/4.3.1/workbox-sw.js");
 
 importScripts(
-    "./precache-manifest.23251c9018266309f6f19dbaa6149265.js"
+    "./precache-manifest.ef63ad040edbb9ce675c41c512a1e329.js"
 );
 
 self.addEventListener('message', (event) => {
     if (event.data && event.data.type === 'SKIP_WAITING') {
         self.skipWaiting();
     }
 });
```

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/js/2.53d4e8c0.chunk.js` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 2.53d4e8c0.chunk.js.LICENSE.txt */
+/*! For license information please see 2.96b2a504.chunk.js.LICENSE.txt */
 (this.webpackJsonpstreamlit_component_template = this.webpackJsonpstreamlit_component_template || []).push([
     [2],
     [function(e, t, n) {
         "use strict";
 
         function r(e, t) {
             for (var n = 0; n < t.length; n++) {
@@ -239,15 +239,15 @@
                 return e.__proto__ || Object.getPrototypeOf(e)
             })(e)
         }
         n.d(t, "a", (function() {
             return r
         }))
     }, function(e, t, n) {
-        e.exports = n(193)()
+        e.exports = n(194)()
     }, function(e, t, n) {
         "use strict";
 
         function r(e, t, n, r) {
             var i, a = e.length,
                 o = 0;
             if (t = t < 0 ? -t > a ? 0 : a + t : t > a ? a : t, n = n > 0 ? n : 0, r.length < 1e4)(i = Array.from(r)).unshift(t, n), [].splice.apply(e, i);
@@ -1297,15 +1297,15 @@
                     configurable: !0
                 }
             }), t && r(e, t)
         }
     }, function(e, t, n) {
         var r = n(46),
             i = n(90),
-            a = n(168);
+            a = n(169);
         e.exports = function(e) {
             return function() {
                 var t, n = r(e);
                 if (i()) {
                     var o = r(this).constructor;
                     t = Reflect.construct(n, arguments, o)
                 } else t = n.apply(this, arguments);
@@ -1407,16 +1407,16 @@
                 for (var g in e) u.call(e, g) && "css" !== g && g !== f && (m[g] = e[g]);
                 m.ref = n, m.className = h;
                 var E = Object(r.createElement)(s, m),
                     b = Object(r.createElement)(d, null);
                 return Object(r.createElement)(r.Fragment, null, b, E)
             }))
     }, function(e, t, n) {
-        var r = n(197),
-            i = n(200),
+        var r = n(198),
+            i = n(201),
             a = n(20),
             o = n(21),
             u = n(78),
             s = n(15),
             c = n(16),
             l = {
                 exports: {}
@@ -5594,17 +5594,17 @@
             for (; ++u < i.length;) s !== i[u] && a.push(e.slice(s, i[u])), a.push("\\"), s = i[u];
             return a.push(e.slice(s)), a.join("")
         }
     }, function(e, t, n) {
         "use strict";
         var r = n(15),
             i = n(16),
-            a = n(163),
+            a = n(164),
             o = n(70),
-            u = n(164),
+            u = n(165),
             s = n(71),
             c = o.CODE_POINTS,
             l = o.CODE_POINT_SEQUENCES,
             f = {
                 128: 8364,
                 130: 8218,
                 131: 402,
@@ -6389,17 +6389,17 @@
                 if (e.attrs[n].name === t) return e.attrs[n].value;
             return null
         }, e.exports = C
     }, function(e, t, n) {
         "use strict";
         var r = n(15),
             i = n(16),
-            a = n(180),
+            a = n(181),
             o = n(74),
-            u = n(181),
+            u = n(182),
             s = n(75),
             c = o.CODE_POINTS,
             l = o.CODE_POINT_SEQUENCES,
             f = {
                 128: 8364,
                 130: 8218,
                 131: 402,
@@ -7185,15 +7185,15 @@
             return null
         }, e.exports = C
     }, function(e, t, n) {
         "use strict";
         n.d(t, "a", (function() {
             return i
         }));
-        var r = n(240);
+        var r = n(241);
         var i = function(e, t, n, i) {
             "function" === typeof t && "function" !== typeof n && (i = n, n = t, t = null);
             var a = Object(r.a)(t),
                 o = i ? -1 : 1;
             ! function e(r, u, s) {
                 var c = r && "object" === typeof r ? r : {};
                 if ("string" === typeof c.type) {
@@ -24059,18 +24059,18 @@
             if (e) {
                 if ("string" === typeof e) return r(e, t);
                 var n = Object.prototype.toString.call(e).slice(8, -1);
                 return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(n) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? r(e, t) : void 0
             }
         }
     }, function(e, t, n) {
-        var r = n(204),
-            i = n(205),
+        var r = n(205),
+            i = n(206),
             a = n(77),
-            o = n(206);
+            o = n(207);
         e.exports = function(e) {
             return r(e) || i(e) || a(e) || o()
         }
     }, function(e, t, n) {
         "use strict";
         var r = n(47),
             i = n.n(r);
@@ -34341,15 +34341,15 @@
                             }
                         }
                     }
                 }]), n
             }(n(27));
         e.exports = u
     }, function(e, t, n) {
-        var r = n(175);
+        var r = n(176);
 
         function i(t, n, a) {
             return "undefined" !== typeof Reflect && Reflect.get ? e.exports = i = Reflect.get : e.exports = i = function(e, t, n) {
                 var i = r(e, t);
                 if (i) {
                     var a = Object.getOwnPropertyDescriptor(i, t);
                     return a.get ? a.get.call(n) : a.value
@@ -34573,23 +34573,23 @@
         }
     }, function(e, t, n) {
         "use strict";
         var r, i, a, o, u, s, c, l, f, h, d, p, m, g, E, b, v, y, T, D, _, A, C, k, O, S, w = n(15),
             N = n(16),
             x = n(39),
             F = n(56),
-            I = n(165),
-            M = n(166),
-            B = n(167),
-            R = n(172),
+            I = n(166),
+            M = n(167),
+            B = n(168),
+            R = n(173),
             L = n(27),
-            P = n(176),
-            j = n(177),
-            U = n(178),
-            H = n(179),
+            P = n(177),
+            j = n(178),
+            U = n(179),
+            H = n(180),
             z = n(71),
             G = n(70),
             K = n(40),
             q = K.TAG_NAMES,
             V = K.NAMESPACES,
             Y = K.ATTRS,
             W = {
@@ -35517,23 +35517,23 @@
         e.exports = J
     }, function(e, t, n) {
         "use strict";
         var r, i, a, o, u, s, c, l, f, h, d, p, m, g, E, b, v, y, T, D, _, A, C, k, O, S, w = n(15),
             N = n(16),
             x = n(39),
             F = n(57),
-            I = n(182),
-            M = n(183),
-            B = n(184),
-            R = n(186),
+            I = n(183),
+            M = n(184),
+            B = n(185),
+            R = n(187),
             L = n(28),
-            P = n(189),
-            j = n(190),
-            U = n(191),
-            H = n(192),
+            P = n(190),
+            j = n(191),
+            U = n(192),
+            H = n(193),
             z = n(75),
             G = n(74),
             K = n(41),
             q = K.TAG_NAMES,
             V = K.NAMESPACES,
             Y = K.ATTRS,
             W = {
@@ -36457,17 +36457,17 @@
 
         function Qe(e, t) {
             e.insertionMode = "IN_BODY_MODE", e._processToken(t)
         }
         e.exports = J
     }, function(e, t, n) {
         "use strict";
-        e.exports = n(195)
+        e.exports = n(196)
     }, function(e, t, n) {
-        var r = n(196);
+        var r = n(197);
 
         function i(e, t) {
             var n, i = null;
             if (!e || "string" !== typeof e) return i;
             for (var a, o, u = r(e), s = "function" === typeof t, c = 0, l = u.length; c < l; c++) a = (n = u[c]).property, o = n.value, s ? t(a, o, n) : o && (i || (i = {}), i[a] = o);
             return i
         }
@@ -40021,15 +40021,15 @@
                     className: "operator",
                     begin: /[-+*/=%^~]|&&?|\|\|?|!=?|<(?:=>?|<|>)?|>[>=]?/,
                     relevance: 0
                 }]
             }
         }
     }, function(e, t, n) {
-        var r = n(207),
+        var r = n(208),
             i = n(78);
 
         function a(e) {
             return e ? "string" === typeof e ? e : e.source : null
         }
 
         function o(e) {
@@ -41807,15 +41807,15 @@
             var n = String(e);
             if ("string" !== typeof t) throw new TypeError("Expected character");
             for (var r = 0, i = n.indexOf(t); - 1 !== i;) r++, i = n.indexOf(t, i + t.length);
             return r
         }
         var Y = n(7);
         var W = n(58),
-            Q = n(240),
+            Q = n(241),
             $ = {}.hasOwnProperty,
             X = function(e, t, n, r) {
                 var i, a;
                 "string" === typeof t || t instanceof RegExp ? (a = [
                     [t, n]
                 ], i = r) : (a = t, i = n), i || (i = {});
                 for (var o = Object(Q.a)(i.ignore || []), u = function(e) {
@@ -42809,17 +42809,17 @@
         "use strict";
         n.d(t, "a", (function() {
             return S
         }));
         var r = n(8),
             i = n(103),
             a = n.n(i),
-            o = n(243),
-            u = n(242),
-            s = n(246),
+            o = n(244),
+            u = n(243),
+            s = n(247),
             c = n(36),
             l = n(19),
             f = n(94),
             h = n(35),
             d = n(33),
             p = {}.hasOwnProperty;
 
@@ -43122,20 +43122,20 @@
     }, function(e, t, n) {
         "use strict";
         n.d(t, "a", (function() {
             return g
         }));
         var r = n(82),
             i = n.n(r),
-            a = n(242);
-        var o = n(249),
-            u = n(248),
+            a = n(243);
+        var o = n(250),
+            u = n(249),
             s = n(102),
             c = n.n(s),
-            l = n(246),
+            l = n(247),
             f = {
                 abandonedHeadElementChild: {
                     reason: "Unexpected metadata element after head",
                     description: "Unexpected element after head. Expected the element before `</head>`",
                     url: !1
                 },
                 abruptClosingOfEmptyComment: {
@@ -49704,15 +49704,15 @@
             }, e
         }(e.exports);
         try {
             regeneratorRuntime = r
         } catch (i) {
             "object" === typeof globalThis ? globalThis.regeneratorRuntime = r : Function("r", "regeneratorRuntime = r")(r)
         }
-    }, function(e, t, n) {}, function(e, t, n) {}, function(e, t, n) {
+    }, function(e, t, n) {}, function(e, t, n) {}, function(e, t, n) {}, function(e, t, n) {
         "use strict";
         var r = n(15),
             i = n(16),
             a = n(70),
             o = n(71),
             u = a.CODE_POINTS,
             s = function() {
@@ -50188,15 +50188,15 @@
         var r = n(15),
             i = n(16),
             a = n(20),
             o = n(21),
             u = n(27),
             s = n(56),
             c = n(91),
-            l = n(171),
+            l = n(172),
             f = n(40).TAG_NAMES,
             h = function(e) {
                 a(n, e);
                 var t = o(n);
 
                 function n(e) {
                     var i;
@@ -50305,16 +50305,16 @@
                             }
                         }
                     }
                 }]), n
             }(u);
         e.exports = h
     }, function(e, t, n) {
-        var r = n(169),
-            i = n(170);
+        var r = n(170),
+            i = n(171);
         e.exports = function(e, t) {
             return !t || "object" !== r(t) && "function" !== typeof t ? i(e) : t
         }
     }, function(e, t) {
         function n(t) {
             return "function" === typeof Symbol && "symbol" === typeof Symbol.iterator ? e.exports = n = function(e) {
                 return typeof e
@@ -50364,15 +50364,15 @@
     }, function(e, t, n) {
         "use strict";
         var r = n(15),
             i = n(16),
             a = n(20),
             o = n(21),
             u = n(73),
-            s = n(173),
+            s = n(174),
             c = n(91),
             l = n(27),
             f = function(e) {
                 a(n, e);
                 var t = o(n);
 
                 function n(e, i) {
@@ -50405,15 +50405,15 @@
     }, function(e, t, n) {
         "use strict";
         var r = n(16),
             i = n(15),
             a = n(20),
             o = n(21),
             u = n(73),
-            s = n(174),
+            s = n(175),
             c = n(27),
             l = function(e) {
                 a(n, e);
                 var t = o(n);
 
                 function n(e, r) {
                     var a;
@@ -51305,15 +51305,15 @@
         var r = n(15),
             i = n(16),
             a = n(20),
             o = n(21),
             u = n(28),
             s = n(57),
             c = n(95),
-            l = n(185),
+            l = n(186),
             f = n(41).TAG_NAMES,
             h = function(e) {
                 a(n, e);
                 var t = o(n);
 
                 function n(e) {
                     var i;
@@ -51461,15 +51461,15 @@
     }, function(e, t, n) {
         "use strict";
         var r = n(15),
             i = n(16),
             a = n(20),
             o = n(21),
             u = n(76),
-            s = n(187),
+            s = n(188),
             c = n(95),
             l = n(28),
             f = function(e) {
                 a(n, e);
                 var t = o(n);
 
                 function n(e, i) {
@@ -51502,15 +51502,15 @@
     }, function(e, t, n) {
         "use strict";
         var r = n(16),
             i = n(15),
             a = n(20),
             o = n(21),
             u = n(76),
-            s = n(188),
+            s = n(189),
             c = n(28),
             l = function(e) {
                 a(n, e);
                 var t = o(n);
 
                 function n(e, r) {
                     var a;
@@ -51914,15 +51914,15 @@
                         } return t === s.SVG && (e === u.FOREIGN_OBJECT || e === u.DESC || e === u.TITLE)
             }(e, t, n)) || !(r && r !== s.MATHML || ! function(e, t) {
                 return t === s.MATHML && (e === u.MI || e === u.MO || e === u.MN || e === u.MS || e === u.MTEXT)
             }(e, t))
         }
     }, function(e, t, n) {
         "use strict";
-        var r = n(194);
+        var r = n(195);
 
         function i() {}
 
         function a() {}
         a.resetWarningCache = i, e.exports = function() {
             function e(e, t, n, i, a, o) {
                 if (o !== r) {
@@ -52144,16 +52144,16 @@
                     for (v(t); e = T();) !1 !== e && (t.push(e), v(t));
                     return t
                 }()
         }
     }, function(e, t, n) {
         var r = n(46),
             i = n(72),
-            a = n(198),
-            o = n(199);
+            a = n(199),
+            o = n(200);
 
         function u(t) {
             var n = "function" === typeof Map ? new Map : void 0;
             return e.exports = u = function(e) {
                 if (null === e || !a(e)) return e;
                 if ("function" !== typeof e) throw new TypeError("Super expression must either be null or a function");
                 if ("undefined" !== typeof n) {
@@ -52189,18 +52189,18 @@
                 i.push.apply(i, t);
                 var a = new(Function.bind.apply(e, i));
                 return n && r(a, n.prototype), a
             }, a.apply(null, arguments)
         }
         e.exports = a
     }, function(e, t, n) {
-        var r = n(201),
-            i = n(202),
+        var r = n(202),
+            i = n(203),
             a = n(77),
-            o = n(203);
+            o = n(204);
         e.exports = function(e, t) {
             return r(e) || i(e, t) || a(e, t) || o()
         }
     }, function(e, t) {
         e.exports = function(e) {
             if (Array.isArray(e)) return e
         }
@@ -52420,16 +52420,16 @@
             return Ne
         })), n.d(r, "disable", (function() {
             return xe
         }));
         var i = n(8),
             a = n(10),
             o = n.n(a),
-            u = n(245),
-            s = n(248),
+            u = n(246),
+            s = n(249),
             c = n(7);
 
         function l(e, t) {
             return function(e) {
                 return Boolean(e && "object" === typeof e)
             }(e) && ("value" in e && e.value || t && "alt" in e && e.alt || "children" in e && f(e.children, t)) || Array.isArray(e) && f(e, t) || ""
         }
@@ -54016,15 +54016,15 @@
             },
             xe = {
                 null: []
             };
         var Fe = /[\0\t\n\r]/g;
         var Ie = n(65),
             Me = n(64),
-            Be = n(241),
+            Be = n(242),
             Re = {}.hasOwnProperty,
             Le = function(e, t, n) {
                 return "string" !== typeof t && (n = t, t = void 0),
                     function(e) {
                         var t = {
                             transforms: [],
                             canContainEols: ["emphasis", "fragment", "heading", "paragraph", "strong"],
@@ -54593,16 +54593,16 @@
                             extensions: t.data("micromarkExtensions") || [],
                             mdastExtensions: t.data("fromMarkdownExtensions") || []
                         }))
                     }
                 })
             },
             ze = n(22);
-        var Ge = n(242),
-            Ke = n(243);
+        var Ge = n(243),
+            Ke = n(244);
         var qe = {}.hasOwnProperty;
 
         function Ve(e) {
             return String(e || "").toUpperCase()
         }
 
         function Ye(e, t) {
@@ -55502,15 +55502,15 @@
                         enumerable: !1,
                         writable: !0,
                         configurable: !0
                     }
                 }), Object(f.a)(r, e)
             })(e)
         }
-        var p = n(241),
+        var p = n(242),
             m = function(e) {
                 Object(s.a)(n, e);
                 var t = Object(c.a)(n);
 
                 function n(e, r, a) {
                     var o;
                     Object(i.a)(this, n);
@@ -56278,16 +56278,16 @@
                     else
                         for (n in e) Fe.call(e, n) && Oe.a.registerAliases(e[n], {
                             languageName: n
                         })
                 }
             };
         Be.registerLanguage("arduino", i.a), Be.registerLanguage("bash", o.a), Be.registerLanguage("c", s.a), Be.registerLanguage("cpp", l.a), Be.registerLanguage("csharp", h.a), Be.registerLanguage("css", p.a), Be.registerLanguage("diff", g.a), Be.registerLanguage("go", b.a), Be.registerLanguage("graphql", y.a), Be.registerLanguage("ini", D.a), Be.registerLanguage("java", A.a), Be.registerLanguage("javascript", k.a), Be.registerLanguage("json", S.a), Be.registerLanguage("kotlin", N.a), Be.registerLanguage("less", F.a), Be.registerLanguage("lua", M.a), Be.registerLanguage("makefile", R.a), Be.registerLanguage("markdown", P.a), Be.registerLanguage("objectivec", U.a), Be.registerLanguage("perl", z.a), Be.registerLanguage("php", K.a), Be.registerLanguage("php-template", V.a), Be.registerLanguage("plaintext", W.a), Be.registerLanguage("python", $.a), Be.registerLanguage("python-repl", Z.a), Be.registerLanguage("r", ee.a), Be.registerLanguage("ruby", ne.a), Be.registerLanguage("rust", ie.a), Be.registerLanguage("scss", oe.a), Be.registerLanguage("shell", se.a), Be.registerLanguage("sql", le.a), Be.registerLanguage("swift", he.a), Be.registerLanguage("typescript", pe.a), Be.registerLanguage("vbnet", ge.a), Be.registerLanguage("wasm", be.a), Be.registerLanguage("xml", ye.a), Be.registerLanguage("yaml", De.a);
-        var Re = n(249),
-            Le = n(242),
+        var Re = n(250),
+            Le = n(243),
             Pe = {}.hasOwnProperty;
 
         function je() {
             var e, t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {},
                 n = t.aliases,
                 r = t.languages,
                 i = t.prefix,
@@ -56391,15 +56391,15 @@
                 }
             }
 
             function i(e) {
                 r(null, e)
             }
         }
-        var g = n(245),
+        var g = n(246),
             E = function e() {
                 var t, n = function() {
                         var e = [],
                             t = {
                                 run: function() {
                                     for (var t = arguments.length, n = new Array(t), r = 0; r < t; r++) n[r] = arguments[r];
                                     var i = -1,
@@ -56623,15 +56623,15 @@
                 return u(t) && Boolean(e.call.apply(e, [this, t].concat(r)))
             }
         }
 
         function u(e) {
             return Boolean(e && "object" === typeof e && "element" === e.type && "string" === typeof e.tagName)
         }
-        var s = n(240),
+        var s = n(241),
             c = function(e, t, n) {
                 var r = Object(s.a)(n);
                 if (!e || !e.type || !e.children) throw new Error("Expected parent node");
                 if ("number" === typeof t) {
                     if (t < 0 || t === Number.POSITIVE_INFINITY) throw new Error("Expected positive finite number as index")
                 } else if ((t = e.children.indexOf(t)) < 0) throw new Error("Expected child node or index");
                 for (; ++t < e.children.length;)
@@ -56740,8 +56740,8 @@
                         return "pre-wrap"
                 }
             }
             return t.whitespace
         }
     }]
 ]);
-//# sourceMappingURL=2.53d4e8c0.chunk.js.map
+//# sourceMappingURL=2.96b2a504.chunk.js.map
```

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/js/2.53d4e8c0.chunk.js.LICENSE.txt` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/js/2.53d4e8c0.chunk.js.map` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {"'file'": "'static/js/2.96b2a504.chunk.js'",*

 * * "'mappings'": "';0IAAA,SAASA,EAAkBC,EAAQC,GACjC,IAAK,IAAIC,EAAI,EAAGA,EAAID,EAAME,OAAQD,IAAK,CACrC,IAAIE,EAAaH,EAAMC,GACvBE,EAAWC,WAAaD,EAAWC,aAAc,EACjDD,EAAWE,cAAe,EACtB,UAAWF,IAAYA,EAAWG,UAAW,GACjDC,OAAOC,eAAeT,EAAQI,EAAWM,IAAKN,IAInC,SAASO,EAAaC,EAAaC,EAAYC,GAG5D,OAFID,GAAYd,EAAkBa,EAAYG,UAAWF,GACrDC,GAAaf,EAAkBa,EAAaE,GACzCF,EAbT,mC,6BCAe,SAASI,EAAgBC,EAAUL,GAChD,KAAMK,aAAoBL,GACxB,MAAM,IAAIM,UAAU,qCAFxB,mC,6BCAA,8CACe,SAASC,EAAUC,EAAUC,GAC1C,GAA0B,oBAAfA,G […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/2.53d4e8c0.chunk.js",
+    "file": "static/js/2.96b2a504.chunk.js",
     "names": [
         "_defineProperties",
         "target",
         "props",
         "i",
         "length",
         "descriptor",
```

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/js/main.a4e8bdc7.chunk.js` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/main.4b51ce30.chunk.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,102 +1,103 @@
 (this.webpackJsonpstreamlit_component_template = this.webpackJsonpstreamlit_component_template || []).push([
     [0], {
-        153: function(e, t, a) {
-            e.exports = a(208)
+        153: function(e, a, t) {
+            e.exports = t(209)
         },
-        208: function(e, t, a) {
+        209: function(e, a, t) {
             "use strict";
-            a.r(t);
-            var r, n, i = a(10),
-                c = a.n(i),
-                o = a(99),
-                l = a.n(o),
-                s = a(7),
-                d = a(81),
-                p = a(0),
-                m = a(1),
-                u = a(2),
-                b = a(3),
-                g = a(68),
-                h = a(69),
-                f = a(50),
-                v = a(244),
-                x = a(145),
-                j = a(147),
-                O = a(146),
-                w = a(144),
-                y = a(247),
-                E = (a(161), a(162), function(e) {
-                    Object(u.a)(a, e);
-                    var t = Object(b.a)(a);
+            t.r(a);
+            var r, n, i = t(10),
+                c = t.n(i),
+                o = t(99),
+                s = t.n(o),
+                l = t(7),
+                d = t(81),
+                p = t(0),
+                m = t(1),
+                u = t(2),
+                b = t(3),
+                g = t(68),
+                h = t(69),
+                f = t(50),
+                v = t(245),
+                x = t(145),
+                j = t(147),
+                w = t(146),
+                O = t(144),
+                y = t(248),
+                k = (t(161), t(162), t(163), function(e) {
+                    Object(u.a)(t, e);
+                    var a = Object(b.a)(t);
 
-                    function a() {
+                    function t() {
                         var e;
-                        Object(m.a)(this, a);
-                        for (var i = arguments.length, o = new Array(i), l = 0; l < i; l++) o[l] = arguments[l];
-                        return (e = t.call.apply(t, [this].concat(o))).render = function() {
+                        Object(m.a)(this, t);
+                        for (var i = arguments.length, o = new Array(i), s = 0; s < i; s++) o[s] = arguments[s];
+                        return (e = a.call.apply(a, [this].concat(o))).render = function() {
                             g.a.setFrameHeight(window.innerHeight);
-                            var t = e.props.args,
-                                a = t.isUser,
-                                i = t.avatarStyle,
-                                o = t.seed,
-                                l = t.message,
-                                p = t.allow_html,
-                                m = t.is_table,
+                            var a = e.props.args,
+                                t = a.isUser,
+                                i = a.avatarStyle,
+                                o = a.seed,
+                                s = a.message,
+                                p = a.allow_html,
+                                m = a.is_table,
                                 u = "https://api.dicebear.com/5.x/".concat(i, "/svg?seed=").concat(o),
                                 b = e.props.theme;
                             if (!b) return c.a.createElement("div", null, "Theme is undefined, please check streamlit version.");
-                            var E = h.a.img({
+                            var k = h.a.img({
                                     border: "1px solid transparent",
                                     borderRadius: "50%",
                                     height: "3rem",
                                     width: "3rem",
                                     margin: 0
                                 }),
-                                k = h.a.div({
+                                E = h.a.div({
                                     display: "inline-block",
                                     background: b.secondaryBackgroundColor,
                                     border: "1px solid transparent",
                                     borderRadius: "10px",
                                     padding: "10px 14px",
                                     margin: "5px 20px",
                                     maxWidth: "70%",
                                     whiteSpace: m ? "normal" : "pre-line"
                                 }),
                                 _ = h.a.div({
                                     display: "flex",
                                     fontFamily: "".concat(b.font, ", 'Segoe UI', 'Roboto', sans-serif"),
                                     height: "auto",
                                     margin: 0,
-                                    width: "100%"
+                                    width: "100%",
+                                    className: "markdown-body"
                                 }, (function(e) {
                                     return e.isUser ? Object(f.a)(r || (r = Object(d.a)(["\n          flex-direction: row-reverse;\n          & > div {\n            text-align: right;\n          }\n        "]))) : Object(f.a)(n || (n = Object(d.a)([""])))
                                 })),
-                                S = [x.a, w.a],
-                                U = [j.a].concat(Object(s.a)(p ? [O.a] : []));
+                                S = [x.a, O.a],
+                                U = [j.a].concat(Object(l.a)(p ? [w.a] : []));
                             return c.a.createElement(_, {
-                                isUser: a
-                            }, c.a.createElement(E, {
+                                isUser: t
+                            }, c.a.createElement(k, {
                                 src: u,
                                 alt: "profile",
                                 draggable: "false"
-                            }), c.a.createElement(k, null, c.a.createElement(v.a, {
+                            }), c.a.createElement(E, null, c.a.createElement(v.a, {
                                 remarkPlugins: S,
-                                rehypePlugins: [].concat(Object(s.a)(U), [
+                                rehypePlugins: [].concat(Object(l.a)(U), [
                                     [y.a, {
                                         detect: !0
                                     }]
                                 ])
-                            }, l)))
+                            }, s)))
                         }, e
                     }
-                    return Object(p.a)(a)
+                    return Object(p.a)(t)
                 }(g.b)),
-                k = Object(g.c)(E);
-            l.a.render(c.a.createElement(c.a.StrictMode, null, c.a.createElement(k, null)), document.getElementById("root"))
+                E = Object(g.c)(k);
+            s.a.render(c.a.createElement(c.a.StrictMode, null, c.a.createElement(E, null)), document.getElementById("root"))
         }
     },
     [
         [153, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.a4e8bdc7.chunk.js.map
+//# sourceMappingURL=main.4b51ce30.chunk.js.map
```

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/js/main.a4e8bdc7.chunk.js.map` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/main.4b51ce30.chunk.js.map`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8081761006289307%*

 * *Differences: {"'file'": "'static/js/main.4b51ce30.chunk.js'",*

 * * "'mappings'": "'8VAqBMA,G,iOACGC,OAAS,WACdC,IAAUC,eAAeC,OAAOC,aAChC,MAAqE,EAAKC,MAAMC,KAAxEC,EAAR,EAAQA,OAAQC,EAAhB,EAAgBA,YAAaC,EAA7B,EAA6BA,KAAMC,EAAnC,EAAmCA,QAASC,EAA5C,EAA4CA,WAAYC,EAAxD,EAAwDA,SAClDC,EAAS,uCAAmCL,EAAnC,qBAA2DC,GAKlEK,EAAU,EAAKT,MAAfS,MAIR,IAAKA,EACH,OAAO,oFAIT,IAAMC,EAASC,IAAOC,IAAI,CACxBC,OAAO,wBACPC,aAAc,MACdC,OAAQ,OACRC,MAAO,OACPC,OAAQ,IAIJC,EAAUP,IAAOQ,IAAI,CACzBC,QAAS,eACTC,WAAYZ,EAAMa,yBAClBT,OAAQ,wBACRC,aAAc,OACdS,QAAS,YACTN,OAA […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.a4e8bdc7.chunk.js",
-    "mappings": "8VAqBMA,G,0NACGC,OAAS,WACdC,IAAUC,eAAeC,OAAOC,aAChC,MAAqE,EAAKC,MAAMC,KAAxEC,EAAR,EAAQA,OAAQC,EAAhB,EAAgBA,YAAaC,EAA7B,EAA6BA,KAAMC,EAAnC,EAAmCA,QAASC,EAA5C,EAA4CA,WAAYC,EAAxD,EAAwDA,SAClDC,EAAS,uCAAmCL,EAAnC,qBAA2DC,GAKlEK,EAAU,EAAKT,MAAfS,MAIR,IAAKA,EACH,OAAO,oFAIT,IAAMC,EAASC,IAAOC,IAAI,CACxBC,OAAO,wBACPC,aAAc,MACdC,OAAQ,OACRC,MAAO,OACPC,OAAQ,IAIJC,EAAUP,IAAOQ,IAAI,CACzBC,QAAS,eACTC,WAAYZ,EAAMa,yBAClBT,OAAQ,wBACRC,aAAc,OACdS,QAAS,YACTN,OAAQ,WACRO,SAAU,MACVC,WAAalB,EAAwB,SAAb,aAIpBb,EAAOiB,IAAOQ,IAAI,CACtBC,QAAS,OAETM,WAAW,GAAD,OAAKjB,EAAMkB,KAAX,sCACVZ,OAAQ,OACRE,OAAQ,EACRD,MAAO,SAET,SAAChB,GACC,OAAIA,EAAME,OACD0B,YAAP,8IAOKA,YAAP,6BAIIC,EAAgB,CACpBC,IACAC,KAEIC,EAAa,CACjBC,KADiB,mBAEb3B,EAAa,CAAC4B,KAAa,KAGjC,OACE,kBAAC,EAAD,CAAMhC,OAAQA,GACZ,kBAACQ,EAAD,CAAQyB,IAAK3B,EAAW4B,IAAI,UAAUC,UAAU,UAChD,kBAACnB,EAAD,KACE,kBAAC,IAAD,CACEW,cAAeA,EACfG,cAAa,sBAAMA,GAAN,CAAqB,CAACM,IAAiB,CAACC,QAAQ,OAE5DlC,M,yBA7EMmC,MAqFJC,cAAwB/C,GCtGvCgD,IAAS/C,OACP,kBAAC,IAAMgD,WAAP,KACE,kBAAC,EAAD,OAEFC,SAASC,eAAe,W",
+    "file": "static/js/main.4b51ce30.chunk.js",
+    "mappings": "8VAqBMA,G,iOACGC,OAAS,WACdC,IAAUC,eAAeC,OAAOC,aAChC,MAAqE,EAAKC,MAAMC,KAAxEC,EAAR,EAAQA,OAAQC,EAAhB,EAAgBA,YAAaC,EAA7B,EAA6BA,KAAMC,EAAnC,EAAmCA,QAASC,EAA5C,EAA4CA,WAAYC,EAAxD,EAAwDA,SAClDC,EAAS,uCAAmCL,EAAnC,qBAA2DC,GAKlEK,EAAU,EAAKT,MAAfS,MAIR,IAAKA,EACH,OAAO,oFAIT,IAAMC,EAASC,IAAOC,IAAI,CACxBC,OAAO,wBACPC,aAAc,MACdC,OAAQ,OACRC,MAAO,OACPC,OAAQ,IAIJC,EAAUP,IAAOQ,IAAI,CACzBC,QAAS,eACTC,WAAYZ,EAAMa,yBAClBT,OAAQ,wBACRC,aAAc,OACdS,QAAS,YACTN,OAAQ,WACRO,SAAU,MACVC,WAAalB,EAAwB,SAAb,aAIpBb,EAAOiB,IAAOQ,IAAI,CACtBC,QAAS,OAETM,WAAW,GAAD,OAAKjB,EAAMkB,KAAX,sCACVZ,OAAQ,OACRE,OAAQ,EACRD,MAAO,OACPY,UAAW,kBAEb,SAAC5B,GACC,OAAIA,EAAME,OACD2B,YAAP,8IAOKA,YAAP,6BAIIC,EAAgB,CACpBC,IACAC,KAEIC,EAAa,CACjBC,KADiB,mBAEb5B,EAAa,CAAC6B,KAAa,KAGjC,OACE,kBAAC,EAAD,CAAMjC,OAAQA,GACZ,kBAACQ,EAAD,CAAQ0B,IAAK5B,EAAW6B,IAAI,UAAUC,UAAU,UAChD,kBAACpB,EAAD,KACE,kBAAC,IAAD,CACEY,cAAeA,EACfG,cAAa,sBAAMA,GAAN,CAAqB,CAACM,IAAiB,CAACC,QAAQ,OAE5DnC,M,yBA9EMoC,MAsFJC,cAAwBhD,GCvGvCiD,IAAShD,OACP,kBAAC,IAAMiD,WAAP,KACE,kBAAC,EAAD,OAEFC,SAASC,eAAe,W",
     "names": [
         "Chat",
         "render",
         "Streamlit",
         "setFrameHeight",
         "window",
         "innerHeight",
@@ -32,14 +32,15 @@
         "background",
         "secondaryBackgroundColor",
         "padding",
         "maxWidth",
         "whiteSpace",
         "fontFamily",
         "font",
+        "className",
         "css",
         "remarkPlugins",
         "remarkMath",
         "remarkGfm",
         "rehypePlugins",
         "rehypeKatex",
         "rehypeRaw",
@@ -57,12 +58,12 @@
     ],
     "sourceRoot": "",
     "sources": [
         "stChat.tsx",
         "index.tsx"
     ],
     "sourcesContent": [
-        "import {\n  // eslint-disable-next-line \n  Streamlit,\n  StreamlitComponentBase,\n  withStreamlitConnection,\n} from \"streamlit-component-lib\"\nimport React, { ReactNode } from \"react\"\nimport styled from '@emotion/styled'\nimport { css } from '@emotion/react'\n\nimport ReactMarkdown from \"react-markdown\"\nimport remarkMath from \"remark-math\"\nimport rehypeKatex from \"rehype-katex\"\nimport rehypeRaw from \"rehype-raw\"\nimport remarkGfm from \"remark-gfm\"\nimport rehypeHighlight from \"rehype-highlight\"\n\nimport 'katex/dist/katex.min.css'\nimport 'highlight.js/styles/monokai-sublime.css'\n\n\nclass Chat extends StreamlitComponentBase {\n  public render = (): ReactNode => {\n    Streamlit.setFrameHeight(window.innerHeight)\n    const { isUser, avatarStyle, seed, message, allow_html, is_table } = this.props.args;\n    const avatarUrl = `https://api.dicebear.com/5.x/${avatarStyle}/svg?seed=${seed}`\n    \n    // Streamlit sends us a theme object via props that we can use to ensure\n    // that our component has visuals that match the active theme in a\n    // streamlit app.\n    const { theme } = this.props\n    \n    // Maintain compatibility with older versions of Streamlit that don't send\n    // a theme object.\n    if (!theme) {\n      return <div>Theme is undefined, please check streamlit version.</div>\n    }\n    \n    // styles for the avatar image\n    const Avatar = styled.img({\n      border: `1px solid transparent`,\n      borderRadius: '50%',\n      height: '3rem',\n      width: '3rem',\n      margin: 0\n    })\n    \n    // styles for the message box\n    const Message = styled.div({\n      display: 'inline-block',\n      background: theme.secondaryBackgroundColor,\n      border: '1px solid transparent',\n      borderRadius: '10px',\n      padding: '10px 14px',\n      margin: '5px 20px',\n      maxWidth: '70%',\n      whiteSpace: !is_table ? 'pre-line' : 'normal'\n    })\n    \n    // styles for the container\n    const Chat = styled.div({\n      display: 'flex',\n      // flexDirection: 'row',\n      fontFamily: `${theme.font}, 'Segoe UI', 'Roboto', sans-serif`, \n      height: 'auto',\n      margin: 0,\n      width: '100%'\n    }, \n    (props: {isUser: boolean}) => {  // specific styles\n      if (props.isUser){\n        return css`\n          flex-direction: row-reverse;\n          & > div {\n            text-align: right;\n          }\n        `\n      }\n      return css``\n    })\n\n    // Init React Markdown plugins\n    const remarkPlugins = [\n      remarkMath, \n      remarkGfm\n    ]\n    const rehypePlugins = [\n      rehypeKatex,\n      ...(allow_html ? [rehypeRaw] : [])\n    ]\n\n    return (\n      <Chat isUser={isUser}>\n        <Avatar src={avatarUrl} alt=\"profile\" draggable=\"false\"/>\n        <Message>\n          <ReactMarkdown \n            remarkPlugins={remarkPlugins}\n            rehypePlugins={[...rehypePlugins, [rehypeHighlight, {detect: true}]]}\n          >\n            {message}\n          </ReactMarkdown>\n        </Message>\n      </Chat>\n    )\n  }\n}\n\nexport default withStreamlitConnection(Chat);\n",
+        "import {\n  // eslint-disable-next-line \n  Streamlit,\n  StreamlitComponentBase,\n  withStreamlitConnection,\n} from \"streamlit-component-lib\"\nimport React, { ReactNode } from \"react\"\nimport styled from '@emotion/styled'\nimport { css } from '@emotion/react'\n\nimport ReactMarkdown from \"react-markdown\"\nimport remarkMath from \"remark-math\"\nimport rehypeKatex from \"rehype-katex\"\nimport rehypeRaw from \"rehype-raw\"\nimport remarkGfm from \"remark-gfm\"\nimport rehypeHighlight from \"rehype-highlight\"\n\nimport 'katex/dist/katex.min.css'\nimport 'highlight.js/styles/monokai-sublime.css'\nimport 'github-markdown-css/github-markdown.css'\n\nclass Chat extends StreamlitComponentBase {\n  public render = (): ReactNode => {\n    Streamlit.setFrameHeight(window.innerHeight)\n    const { isUser, avatarStyle, seed, message, allow_html, is_table } = this.props.args;\n    const avatarUrl = `https://api.dicebear.com/5.x/${avatarStyle}/svg?seed=${seed}`\n    \n    // Streamlit sends us a theme object via props that we can use to ensure\n    // that our component has visuals that match the active theme in a\n    // streamlit app.\n    const { theme } = this.props\n    \n    // Maintain compatibility with older versions of Streamlit that don't send\n    // a theme object.\n    if (!theme) {\n      return <div>Theme is undefined, please check streamlit version.</div>\n    }\n    \n    // styles for the avatar image\n    const Avatar = styled.img({\n      border: `1px solid transparent`,\n      borderRadius: '50%',\n      height: '3rem',\n      width: '3rem',\n      margin: 0\n    })\n    \n    // styles for the message box\n    const Message = styled.div({\n      display: 'inline-block',\n      background: theme.secondaryBackgroundColor,\n      border: '1px solid transparent',\n      borderRadius: '10px',\n      padding: '10px 14px',\n      margin: '5px 20px',\n      maxWidth: '70%',\n      whiteSpace: !is_table ? 'pre-line' : 'normal'\n    })\n    \n    // styles for the container\n    const Chat = styled.div({\n      display: 'flex',\n      // flexDirection: 'row',\n      fontFamily: `${theme.font}, 'Segoe UI', 'Roboto', sans-serif`, \n      height: 'auto',\n      margin: 0,\n      width: '100%',\n      className: 'markdown-body'\n    },\n    (props: {isUser: boolean}) => {  // specific styles\n      if (props.isUser){\n        return css`\n          flex-direction: row-reverse;\n          & > div {\n            text-align: right;\n          }\n        `\n      }\n      return css``\n    })\n\n    // Init React Markdown plugins\n    const remarkPlugins = [\n      remarkMath, \n      remarkGfm\n    ]\n    const rehypePlugins = [\n      rehypeKatex,\n      ...(allow_html ? [rehypeRaw] : [])\n    ]\n\n    return (\n      <Chat isUser={isUser}>\n        <Avatar src={avatarUrl} alt=\"profile\" draggable=\"false\"/>\n        <Message>\n          <ReactMarkdown \n            remarkPlugins={remarkPlugins}\n            rehypePlugins={[...rehypePlugins, [rehypeHighlight, {detect: true}]]}\n          >\n            {message}\n          </ReactMarkdown>\n        </Message>\n      </Chat>\n    )\n  }\n}\n\nexport default withStreamlitConnection(Chat);\n",
         "import React from \"react\"\nimport ReactDOM from \"react-dom\"\nimport Chat from \"./stChat\"\n\nReactDOM.render(\n  <React.StrictMode>\n    <Chat />\n  </React.StrictMode>,\n  document.getElementById(\"root\")\n)\n"
     ],
     "version": 3
 }
```

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js.map` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.10824af7.woff` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.10824af7.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.56573229.ttf` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.56573229.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.66c67820.woff2` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.66c67820.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.497bf407.ttf` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.497bf407.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.a9e9b095.woff2` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.a9e9b095.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.de2ba279.woff` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.de2ba279.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.08d95d99.woff2` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.08d95d99.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.a25140fb.woff` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.a25140fb.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.e6fb499f.ttf` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.e6fb499f.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.40934fc0.woff` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.40934fc0.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.796f3797.woff2` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.796f3797.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.b9d7c449.ttf` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.b9d7c449.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.97a699d8.ttf` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.97a699d8.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.e435cda5.woff` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.e435cda5.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.f9e6a99f.woff2` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.f9e6a99f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.4cdba646.woff` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.4cdba646.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.8e431f7e.ttf` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.8e431f7e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.a9382e25.woff2` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.a9382e25.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.52fb39b0.ttf` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.52fb39b0.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.5f875f98.woff` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.5f875f98.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.d8737343.woff2` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.d8737343.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.39349e0a.ttf` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.39349e0a.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.65297062.woff2` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.65297062.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.8ffd28f6.woff` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.8ffd28f6.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.818582da.ttf` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.818582da.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f1cdb692.woff` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f1cdb692.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f8a7f19f.woff2` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f8a7f19f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.1320454d.woff2` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.1320454d.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.48155e43.woff` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.48155e43.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.6589c4f1.ttf` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.6589c4f1.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.d8b7a801.woff2` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.d8b7a801.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.ed7aea12.woff` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.ed7aea12.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.fe5ed587.ttf` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.fe5ed587.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.0e897d27.woff` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.0e897d27.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.ad546b47.woff2` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.ad546b47.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.f2ac7312.ttf` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.f2ac7312.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.e934cbc8.woff2` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.e934cbc8.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.ef725de5.woff` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.ef725de5.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.f60b4a34.ttf` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.f60b4a34.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.1ac3ed6e.woff2` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.1ac3ed6e.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.3243452e.ttf` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.3243452e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.5f8637ee.woff` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.5f8637ee.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.1b3161eb.woff2` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.1b3161eb.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a189c37d.ttf` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a189c37d.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a82fa2a7.woff` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a82fa2a7.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.0d8d9204.ttf` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.0d8d9204.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.4788ba5b.woff` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.4788ba5b.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.82ef26dc.woff2` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.82ef26dc.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.1fdda0e5.ttf` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.1fdda0e5.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.95a1da91.woff2` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.95a1da91.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.b0628bfd.woff` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.b0628bfd.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.4de844d4.woff` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.4de844d4.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.9108a400.woff2` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.9108a400.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.963af864.ttf` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.963af864.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.27a23ee6.ttf` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.27a23ee6.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.3045a61f.woff` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.3045a61f.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.61522cd3.woff2` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.61522cd3.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.0e046058.woff` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.0e046058.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.6bf42875.ttf` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.6bf42875.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.b8b8393d.woff2` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.b8b8393d.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat_askgdpr.egg-info/PKG-INFO` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat_askgdpr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-chat-askgdpr
-Version: 0.0.2.2
+Version: 0.0.2.3
 Summary: A streamlit component, to make chatbots
 Home-page: https://github.com/AI-Yash/st-chat
 Author: Yash Pravin Pawar, Yash Vardhan Kapil
 Author-email: yashpawarp@gmail.com
 Keywords: chat streamlit streamlit-component
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `streamlit-chat-askgdpr-0.0.2.2/streamlit_chat_askgdpr.egg-info/SOURCES.txt` & `streamlit-chat-askgdpr-0.0.2.3/streamlit_chat_askgdpr.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 README.md
 setup.py
 streamlit_chat/__init__.py
 streamlit_chat/frontend/build/asset-manifest.json
 streamlit_chat/frontend/build/bootstrap.min.css
 streamlit_chat/frontend/build/bootstrap.min.css.map
 streamlit_chat/frontend/build/index.html
-streamlit_chat/frontend/build/precache-manifest.23251c9018266309f6f19dbaa6149265.js
+streamlit_chat/frontend/build/precache-manifest.ef63ad040edbb9ce675c41c512a1e329.js
 streamlit_chat/frontend/build/service-worker.js
-streamlit_chat/frontend/build/static/css/2.95a91b17.chunk.css
-streamlit_chat/frontend/build/static/css/2.95a91b17.chunk.css.map
-streamlit_chat/frontend/build/static/js/2.53d4e8c0.chunk.js
-streamlit_chat/frontend/build/static/js/2.53d4e8c0.chunk.js.LICENSE.txt
-streamlit_chat/frontend/build/static/js/2.53d4e8c0.chunk.js.map
-streamlit_chat/frontend/build/static/js/main.a4e8bdc7.chunk.js
-streamlit_chat/frontend/build/static/js/main.a4e8bdc7.chunk.js.map
+streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css
+streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css.map
+streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js
+streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.LICENSE.txt
+streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.map
+streamlit_chat/frontend/build/static/js/main.4b51ce30.chunk.js
+streamlit_chat/frontend/build/static/js/main.4b51ce30.chunk.js.map
 streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js
 streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js.map
 streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.10824af7.woff
 streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.56573229.ttf
 streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.66c67820.woff2
 streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.497bf407.ttf
 streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.a9e9b095.woff2
```
