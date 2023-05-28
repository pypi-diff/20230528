# Comparing `tmp/khoj_assistant-0.6.2.dev6.tar.gz` & `tmp/khoj_assistant-0.6.3.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Thu Apr 27 12:45:16 2023, max compression
+gzip compressed data, last modified: Sun May 28 04:51:54 2023, max compression
```

## Comparing `khoj_assistant-0.6.2.dev6.tar` & `khoj_assistant-0.6.3.dev3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0        0 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/__init__.py
--rw-r--r--   0        0        0     9136 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/configure.py
--rw-r--r--   0        0        0     4929 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2904 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/interface/desktop/file_browser.py
--rw-r--r--   0        0        0      861 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/interface/desktop/labelled_text_field.py
--rw-r--r--   0        0        0    15746 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1316 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0     9685 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0      546 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0    11635 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      438 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      406 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0      437 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/interface/web/assets/config.css
--rw-r--r--   0        0        0     4515 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/interface/web/assets/config.js
--rw-r--r--   0        0        0   275822 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58507 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    26348 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0   162910 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/interface/web/assets/icons/favicon-144x144.ico
--rw-r--r--   0        0        0    29325 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/interface/web/assets/icons/favicon-144x144.png
--rw-r--r--   0        0        0   113060 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0        0 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     3515 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     8972 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     5182 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3930 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/processor/ledger/__init__.py
--rw-r--r--   0        0        0     5701 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/processor/ledger/beancount_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     5898 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     6116 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16789 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0     9613 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/routers/api.py
--rw-r--r--   0        0        0     1941 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0      803 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      463 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7470 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2713 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3690 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11375 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    10755 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2012 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2325 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/utils/config.py
--rw-r--r--   0        0        0     2381 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     4258 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1607 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/utils/models.py
--rw-r--r--   0        0        0     3463 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0      977 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1239 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/.gitignore
--rw-r--r--   0        0        0    32472 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/LICENSE
--rw-r--r--   0        0        0    21780 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/README.md
--rw-r--r--   0        0        0     2650 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/pyproject.toml
--rw-r--r--   0        0        0    23925 2023-04-27 12:45:16.000000 khoj_assistant-0.6.2.dev6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/__init__.py
+-rw-r--r--   0        0        0     9769 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/configure.py
+-rw-r--r--   0        0        0     4929 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2904 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/desktop/file_browser.py
+-rw-r--r--   0        0        0      861 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/desktop/labelled_text_field.py
+-rw-r--r--   0        0        0    15746 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1316 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0     9685 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0      546 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0    11635 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      438 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      406 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0      437 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/config.css
+-rw-r--r--   0        0        0     4515 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/config.js
+-rw-r--r--   0        0        0   275822 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58507 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    26348 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0   162910 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/icons/favicon-144x144.ico
+-rw-r--r--   0        0        0    29325 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/icons/favicon-144x144.png
+-rw-r--r--   0        0        0   113060 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0        0 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4216 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     9530 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     5182 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3930 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/processor/ledger/__init__.py
+-rw-r--r--   0        0        0     5701 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/processor/ledger/beancount_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     6577 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     6526 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16789 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    10226 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/routers/api.py
+-rw-r--r--   0        0        0     1941 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0      803 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      463 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7470 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2713 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3690 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11375 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    10930 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2012 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2379 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     2478 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     6703 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1607 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     3744 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1047 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1239 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/.gitignore
+-rw-r--r--   0        0        0    32472 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/LICENSE
+-rw-r--r--   0        0        0    21760 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/README.md
+-rw-r--r--   0        0        0     2650 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/pyproject.toml
+-rw-r--r--   0        0        0    23905 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/PKG-INFO
```

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/configure.py` & `khoj_assistant-0.6.3.dev3/src/khoj/configure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Standard Packages
 import sys
 import logging
 import json
 from enum import Enum
+import requests
 
 # External Packages
 import schedule
 from fastapi.staticfiles import StaticFiles
 
 # Internal Packages
 from khoj.processor.conversation.gpt import summarize
@@ -58,15 +59,15 @@
 
     app.mount("/static", StaticFiles(directory=constants.web_directory), name="static")
     app.include_router(api, prefix="/api")
     app.include_router(api_beta, prefix="/api/beta")
     app.include_router(web_client)
 
 
-@schedule.repeat(schedule.every(1).hour)
+@schedule.repeat(schedule.every(61).minutes)
 def update_search_index():
     state.search_index_lock.acquire()
     state.model = configure_search(state.model, state.config, regenerate=False)
     state.search_index_lock.release()
     logger.info("📬 Search index updated via Scheduler")
 
 
@@ -185,15 +186,15 @@
         # Initialize Conversation Logs
         conversation_processor.meta_log = {}
         conversation_processor.chat_session = ""
 
     return conversation_processor
 
 
-@schedule.repeat(schedule.every(15).minutes)
+@schedule.repeat(schedule.every(17).minutes)
 def save_chat_session():
     # No need to create empty log file
     if not (
         state.processor_config
         and state.processor_config.conversation
         and state.processor_config.conversation.meta_log
         and state.processor_config.conversation.chat_session
@@ -219,7 +220,23 @@
     conversation_logfile = resolve_absolute_path(state.processor_config.conversation.conversation_logfile)
     conversation_logfile.parent.mkdir(parents=True, exist_ok=True)  # create conversation directory if doesn't exist
     with open(conversation_logfile, "w+", encoding="utf-8") as logfile:
         json.dump(conversation_log, logfile, indent=2)
 
     state.processor_config.conversation.chat_session = None
     logger.info("📩 Saved current chat session to conversation logs")
+
+
+@schedule.repeat(schedule.every(59).minutes)
+def upload_telemetry():
+    if not state.config.app.should_log_telemetry or not state.telemetry:
+        message = "📡 No telemetry to upload" if not state.telemetry else "📡 Telemetry logging disabled"
+        logger.debug(message)
+        return
+
+    try:
+        logger.debug(f"📡 Upload usage telemetry to {constants.telemetry_server}:\n{state.telemetry}")
+        requests.post(constants.telemetry_server, json=state.telemetry)
+    except Exception as e:
+        logger.error(f"📡 Error uploading telemetry: {e}")
+    else:
+        state.telemetry = []
```

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/main.py` & `khoj_assistant-0.6.3.dev3/src/khoj/main.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/interface/desktop/file_browser.py` & `khoj_assistant-0.6.3.dev3/src/khoj/interface/desktop/file_browser.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/interface/desktop/labelled_text_field.py` & `khoj_assistant-0.6.3.dev3/src/khoj/interface/desktop/labelled_text_field.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/interface/desktop/main_window.py` & `khoj_assistant-0.6.3.dev3/src/khoj/interface/desktop/main_window.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.6.3.dev3/src/khoj/interface/desktop/system_tray.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/interface/web/chat.html` & `khoj_assistant-0.6.3.dev3/src/khoj/interface/web/chat.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/interface/web/config.html` & `khoj_assistant-0.6.3.dev3/src/khoj/interface/web/config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/interface/web/index.html` & `khoj_assistant-0.6.3.dev3/src/khoj/interface/web/index.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/interface/web/assets/config.js` & `khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/config.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/interface/web/assets/icons/favicon-144x144.ico` & `khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/icons/favicon-144x144.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/interface/web/assets/icons/favicon-144x144.png` & `khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/icons/favicon-144x144.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.6.3.dev3/src/khoj/processor/text_to_jsonl.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,22 +27,41 @@
     @staticmethod
     def split_entries_by_max_tokens(
         entries: List[Entry], max_tokens: int = 256, max_word_length: int = 500
     ) -> List[Entry]:
         "Split entries if compiled entry length exceeds the max tokens supported by the ML model."
         chunked_entries: List[Entry] = []
         for entry in entries:
+            # Split entry into words
             compiled_entry_words = [word for word in entry.compiled.split(" ") if word != ""]
+
             # Drop long words instead of having entry truncated to maintain quality of entry processed by models
             compiled_entry_words = [word for word in compiled_entry_words if len(word) <= max_word_length]
+
+            # Split entry into chunks of max tokens
             for chunk_index in range(0, len(compiled_entry_words), max_tokens):
                 compiled_entry_words_chunk = compiled_entry_words[chunk_index : chunk_index + max_tokens]
                 compiled_entry_chunk = " ".join(compiled_entry_words_chunk)
-                entry_chunk = Entry(compiled=compiled_entry_chunk, raw=entry.raw, file=entry.file)
-                chunked_entries.append(entry_chunk)
+
+                # Prepend heading to all other chunks, the first chunk already has heading from original entry
+                if chunk_index > 0:
+                    # Snip heading to avoid crossing max_tokens limit
+                    # Keep last 100 characters of heading as entry heading more important than filename
+                    snipped_heading = entry.heading[-100:]
+                    compiled_entry_chunk = f"{snipped_heading}.\n{compiled_entry_chunk}"
+
+                chunked_entries.append(
+                    Entry(
+                        compiled=compiled_entry_chunk,
+                        raw=entry.raw,
+                        heading=entry.heading,
+                        file=entry.file,
+                    )
+                )
+
         return chunked_entries
 
     def mark_entries_for_update(
         self, current_entries: List[Entry], previous_entries: List[Entry], key="compiled", logger=None
     ) -> List[Tuple[int, Entry]]:
         # Hash all current and previous entries to identify new entries
         with timer("Hash previous, current entries", logger):
```

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/processor/conversation/gpt.py` & `khoj_assistant-0.6.3.dev3/src/khoj/processor/conversation/gpt.py`

 * *Files 4% similar despite different names*

```diff
@@ -232,31 +232,44 @@
     )
 
     # Extract, Clean Message from GPT's Response
     story = str(response["choices"][0]["text"])
     return json.loads(story.strip(empty_escape_sequences))
 
 
-def converse(references, user_query, conversation_log={}, api_key=None, temperature=0.2):
+def converse(references, user_query, conversation_log={}, model="gpt-3.5-turbo", api_key=None, temperature=0.2):
     """
     Converse with user using OpenAI's ChatGPT
     """
     # Initialize Variables
-    model = "gpt-3.5-turbo"
     compiled_references = "\n\n".join({f"# {item}" for item in references})
 
     personality_primer = "You are Khoj, a friendly, smart and helpful personal assistant."
-    conversation_primer = f"""
+    conversation_primers = {
+        "general": f"""
+Using your general knowledge and our past conversations as context, answer the following question.
+Current Date: {datetime.now().strftime("%Y-%m-%d")}
+
+Question: {user_query}
+""".strip(),
+        "notes": f"""
 Using the notes and our past conversations as context, answer the following question.
 Current Date: {datetime.now().strftime("%Y-%m-%d")}
 
 Notes:
 {compiled_references}
 
-Question: {user_query}"""
+Question: {user_query}
+""".strip(),
+    }
+
+    # Get Conversation Primer appropriate to Conversation Type
+    conversation_type = "general" if user_query.startswith("@general") or compiled_references.strip() == "" else "notes"
+    logger.debug(f"Conversation Type: {conversation_type}")
+    conversation_primer = conversation_primers.get(conversation_type)
 
     # Setup Prompt with Primer or Conversation History
     messages = generate_chatml_messages_with_context(
         conversation_primer,
         personality_primer,
         conversation_log,
         model,
```

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/processor/conversation/utils.py` & `khoj_assistant-0.6.3.dev3/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.6.3.dev3/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/processor/ledger/beancount_to_jsonl.py` & `khoj_assistant-0.6.3.dev3/src/khoj/processor/ledger/beancount_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/processor/markdown/markdown_to_jsonl.py` & `khoj_assistant-0.6.3.dev3/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Standard Packages
 import glob
 import logging
 import re
-import time
 from pathlib import Path
 from typing import List
 
 # Internal Packages
 from khoj.processor.text_to_jsonl import TextToJsonl
 from khoj.utils.helpers import get_absolute_path, is_none_or_empty, timer
 from khoj.utils.constants import empty_escape_sequences
@@ -106,33 +105,46 @@
 
         entries = []
         entry_to_file_map = []
         for markdown_file in markdown_files:
             with open(markdown_file, "r", encoding="utf8") as f:
                 markdown_content = f.read()
                 markdown_entries_per_file = []
+                any_headings = re.search(markdown_heading_regex, markdown_content, flags=re.MULTILINE)
                 for entry in re.split(markdown_heading_regex, markdown_content, flags=re.MULTILINE):
-                    prefix = "#" if entry.startswith("#") else "# "
-                    if entry.strip(empty_escape_sequences) != "":
-                        markdown_entries_per_file.append(f"{prefix}{entry.strip(empty_escape_sequences)}")
+                    # Add heading level as the regex split removed it from entries with headings
+                    prefix = "#" if entry.startswith("#") else "# " if any_headings else ""
+                    stripped_entry = entry.strip(empty_escape_sequences)
+                    if stripped_entry != "":
+                        markdown_entries_per_file.append(f"{prefix}{stripped_entry}")
 
                 entry_to_file_map += zip(markdown_entries_per_file, [markdown_file] * len(markdown_entries_per_file))
                 entries.extend(markdown_entries_per_file)
 
         return entries, dict(entry_to_file_map)
 
     @staticmethod
     def convert_markdown_entries_to_maps(parsed_entries: List[str], entry_to_file_map) -> List[Entry]:
         "Convert each Markdown entries into a dictionary"
         entries = []
         for parsed_entry in parsed_entries:
             entry_filename = Path(entry_to_file_map[parsed_entry])
+            heading = parsed_entry.splitlines()[0] if re.search("^#+\s", parsed_entry) else ""
             # Append base filename to compiled entry for context to model
-            compiled_entry = f"{parsed_entry}\n{entry_filename.stem}"
-            entries.append(Entry(compiled=compiled_entry, raw=parsed_entry, file=f"{entry_filename}"))
+            # Increment heading level for heading entries and make filename as its top level heading
+            prefix = f"# {entry_filename.stem}\n#" if heading else f"# {entry_filename.stem}\n"
+            compiled_entry = f"{prefix}{parsed_entry}"
+            entries.append(
+                Entry(
+                    compiled=compiled_entry,
+                    raw=parsed_entry,
+                    heading=f"{prefix}{heading}",
+                    file=f"{entry_filename}",
+                )
+            )
 
         logger.debug(f"Converted {len(parsed_entries)} markdown entries to dictionaries")
 
         return entries
 
     @staticmethod
     def convert_markdown_maps_to_jsonl(entries: List[Entry]):
```

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.6.3.dev3/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Standard Packages
 import glob
 import logging
-import time
+from pathlib import Path
 from typing import Iterable, List
 
 # Internal Packages
 from khoj.processor.org_mode import orgnode
 from khoj.processor.text_to_jsonl import TextToJsonl
 from khoj.utils.helpers import get_absolute_path, is_none_or_empty, timer
 from khoj.utils.jsonl import dump_jsonl, compress_jsonl_data
@@ -109,15 +109,19 @@
         "Convert Org-Mode nodes into list of Entry objects"
         entries: List[Entry] = []
         for parsed_entry in parsed_entries:
             if not parsed_entry.hasBody and not index_heading_entries:
                 # Ignore title notes i.e notes with just headings and empty body
                 continue
 
-            compiled = f"{parsed_entry.heading}."
+            # Prepend filename as top heading to entry
+            filename = Path(entry_to_file_map[parsed_entry]).stem
+            heading = f"* {filename}\n** {parsed_entry.heading}." if parsed_entry.heading else f"* {filename}."
+
+            compiled = heading
             if state.verbose > 2:
                 logger.debug(f"Title: {parsed_entry.heading}")
 
             if parsed_entry.tags:
                 tags_str = " ".join(parsed_entry.tags)
                 compiled += f"\t {tags_str}."
                 if state.verbose > 2:
@@ -135,15 +139,22 @@
 
             if parsed_entry.hasBody:
                 compiled += f"\n {parsed_entry.body}"
                 if state.verbose > 2:
                     logger.debug(f"Body: {parsed_entry.body}")
 
             if compiled:
-                entries += [Entry(compiled=compiled, raw=f"{parsed_entry}", file=f"{entry_to_file_map[parsed_entry]}")]
+                entries.append(
+                    Entry(
+                        compiled=compiled,
+                        raw=f"{parsed_entry}",
+                        heading=f"{heading}",
+                        file=f"{entry_to_file_map[parsed_entry]}",
+                    )
+                )
 
         return entries
 
     @staticmethod
     def convert_org_entries_to_jsonl(entries: Iterable[Entry]) -> str:
         "Convert each Org-Mode entry to JSON and collate as JSONL"
         return "".join([f"{entry_dict.to_json()}\n" for entry_dict in entries])
```

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.6.3.dev3/src/khoj/processor/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/routers/api.py` & `khoj_assistant-0.6.3.dev3/src/khoj/routers/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from fastapi import HTTPException
 
 # Internal Packages
 from khoj.configure import configure_processor, configure_search
 from khoj.processor.conversation.gpt import converse, extract_questions
 from khoj.processor.conversation.utils import message_to_log, message_to_prompt
 from khoj.search_type import image_search, text_search
-from khoj.utils.helpers import timer
+from khoj.utils.helpers import log_telemetry, timer
 from khoj.utils.rawconfig import FullConfig, SearchResponse
 from khoj.utils.state import SearchType
 from khoj.utils import state, constants
 
 # Initialize Router
 api = APIRouter()
 logger = logging.getLogger(__name__)
@@ -164,14 +164,19 @@
         # collate and return results
         with timer("Collating results took", logger):
             results = text_search.collate_results(hits, entries, results_count)
 
     # Cache results
     state.query_cache[query_cache_key] = results
 
+    # Only log telemetry if query is new and not a continuation of previous query
+    if state.previous_query is None or state.previous_query not in user_query:
+        state.telemetry += [log_telemetry(telemetry_type="api", api="search", app_config=state.config.app)]
+    state.previous_query = user_query
+
     return results
 
 
 @api.get("/update")
 def update(t: Optional[SearchType] = None, force: Optional[bool] = False):
     try:
         state.search_index_lock.acquire()
@@ -187,14 +192,16 @@
         state.processor_config = configure_processor(state.config.processor)
     except ValueError as e:
         logger.error(e)
         raise HTTPException(status_code=500, detail=str(e))
     else:
         logger.info("📬 Processor reconfigured via API")
 
+    state.telemetry += [log_telemetry(telemetry_type="api", api="update", app_config=state.config.app)]
+
     return {"status": "ok", "message": "khoj reloaded"}
 
 
 @api.get("/chat")
 def chat(q: Optional[str] = None):
     if (
         state.processor_config is None
@@ -204,14 +211,15 @@
         raise HTTPException(
             status_code=500, detail="Chat processor not configured. Configure OpenAI API key on server and restart it."
         )
 
     # Initialize Variables
     api_key = state.processor_config.conversation.openai_api_key
     model = state.processor_config.conversation.model
+    chat_model = state.processor_config.conversation.chat_model
     user_message_time = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
 
     # Load Conversation History
     chat_session = state.processor_config.conversation.chat_session
     meta_log = state.processor_config.conversation.meta_log
 
     # If user query is empty, return chat history
@@ -230,15 +238,15 @@
         result_list = []
         for query in inferred_queries:
             result_list.extend(search(query, n=5, r=True, score_threshold=-5.0, dedupe=False))
         compiled_references = [item.additional["compiled"] for item in result_list]
 
     try:
         with timer("Generating chat response took", logger):
-            gpt_response = converse(compiled_references, q, meta_log, api_key=api_key)
+            gpt_response = converse(compiled_references, q, meta_log, model=chat_model, api_key=api_key)
         status = "ok"
     except Exception as e:
         gpt_response = str(e)
         status = "error"
 
     # Update Conversation History
     state.processor_config.conversation.chat_session = message_to_prompt(q, chat_session, gpt_message=gpt_response)
@@ -246,8 +254,10 @@
         q,
         gpt_response,
         user_message_metadata={"created": user_message_time},
         khoj_message_metadata={"context": compiled_references, "intent": {"inferred-queries": inferred_queries}},
         conversation_log=meta_log.get("chat", []),
     )
 
+    state.telemetry += [log_telemetry(telemetry_type="api", api="chat", app_config=state.config.app)]
+
     return {"status": status, "response": gpt_response, "context": compiled_references}
```

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/routers/api_beta.py` & `khoj_assistant-0.6.3.dev3/src/khoj/routers/api_beta.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/routers/web_client.py` & `khoj_assistant-0.6.3.dev3/src/khoj/routers/web_client.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.6.3.dev3/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.6.3.dev3/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.6.3.dev3/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/search_type/image_search.py` & `khoj_assistant-0.6.3.dev3/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/search_type/text_search.py` & `khoj_assistant-0.6.3.dev3/src/khoj/search_type/text_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,28 +69,30 @@
     if embeddings_file.exists() and not regenerate:
         corpus_embeddings = torch.load(get_absolute_path(embeddings_file), map_location=state.device)
         logger.debug(f"Loaded {len(corpus_embeddings)} text embeddings from {embeddings_file}")
 
         # Encode any new entries in the corpus and update corpus embeddings
         new_entries = [entry.compiled for id, entry in entries_with_ids if id == -1]
         if new_entries:
+            logger.info(f"📩 Indexing {len(new_entries)} text entries.")
             new_embeddings = bi_encoder.encode(
                 new_entries, convert_to_tensor=True, device=state.device, show_progress_bar=True
             )
             existing_entry_ids = [id for id, _ in entries_with_ids if id != -1]
             if existing_entry_ids:
                 existing_embeddings = torch.index_select(
                     corpus_embeddings, 0, torch.tensor(existing_entry_ids, device=state.device)
                 )
             else:
                 existing_embeddings = torch.tensor([], device=state.device)
             corpus_embeddings = torch.cat([existing_embeddings, new_embeddings], dim=0)
     # Else compute the corpus embeddings from scratch
     else:
         new_entries = [entry.compiled for _, entry in entries_with_ids]
+        logger.info(f"📩 Indexing {len(new_entries)} text entries. Creating index from scratch.")
         corpus_embeddings = bi_encoder.encode(
             new_entries, convert_to_tensor=True, device=state.device, show_progress_bar=True
         )
 
     # Save regenerated or updated embeddings to file
     if new_entries:
         corpus_embeddings = util.normalize_embeddings(corpus_embeddings)
```

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/utils/cli.py` & `khoj_assistant-0.6.3.dev3/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/utils/config.py` & `khoj_assistant-0.6.3.dev3/src/khoj/utils/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
     plugin_search: Dict[str, TextSearchModel] = None
 
 
 class ConversationProcessorConfigModel:
     def __init__(self, processor_config: ConversationProcessorConfig):
         self.openai_api_key = processor_config.openai_api_key
         self.model = processor_config.model
+        self.chat_model = processor_config.chat_model
         self.conversation_logfile = Path(processor_config.conversation_logfile)
         self.chat_session = ""
         self.meta_log: dict = {}
 
 
 @dataclass
 class ProcessorConfigModel:
```

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/utils/constants.py` & `khoj_assistant-0.6.3.dev3/src/khoj/utils/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from pathlib import Path
 
 app_root_directory = Path(__file__).parent.parent.parent
 web_directory = app_root_directory / "khoj/interface/web/"
 empty_escape_sequences = "\n|\r|\t| "
+app_env_filepath = "~/.khoj/env"
+telemetry_server = "https://khoj.beta.haletic.com/v1/telemetry"
 
 # default app config to use
 default_config = {
     "content-type": {
         "org": {
             "input-files": None,
             "input-filter": None,
```

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/utils/jsonl.py` & `khoj_assistant-0.6.3.dev3/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/utils/models.py` & `khoj_assistant-0.6.3.dev3/src/khoj/utils/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # External Packages
 import openai
 import torch
 from tqdm import trange
 
 # Internal Packages
-from khoj.utils.state import processor_config, config_file
+from khoj.utils import state
 
 
 class BaseEncoder(ABC):
     @abstractmethod
     def __init__(self, model_name: str, device: torch.device = None, **kwargs):
         ...
 
@@ -21,22 +21,22 @@
         ...
 
 
 class OpenAI(BaseEncoder):
     def __init__(self, model_name, device=None):
         self.model_name = model_name
         if (
-            not processor_config
-            or not processor_config.conversation
-            or not processor_config.conversation.openai_api_key
+            not state.processor_config
+            or not state.processor_config.conversation
+            or not state.processor_config.conversation.openai_api_key
         ):
             raise Exception(
-                f"Set OpenAI API key under processor-config > conversation > openai-api-key in config file: {config_file}"
+                f"Set OpenAI API key under processor-config > conversation > openai-api-key in config file: {state.config_file}"
             )
-        openai.api_key = processor_config.conversation.openai_api_key
+        openai.api_key = state.processor_config.conversation.openai_api_key
         self.embedding_dimensions = None
 
     def encode(self, entries, device=None, **kwargs):
         embedding_tensors = []
 
         for index in trange(0, len(entries)):
             # OpenAI models create better embeddings for entries without newlines
```

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.6.3.dev3/src/khoj/utils/rawconfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,40 +78,50 @@
     image: Optional[ImageSearchConfig]
 
 
 class ConversationProcessorConfig(ConfigBase):
     openai_api_key: str
     conversation_logfile: Path
     model: Optional[str] = "text-davinci-003"
+    chat_model: Optional[str] = "gpt-3.5-turbo"
 
 
 class ProcessorConfig(ConfigBase):
     conversation: Optional[ConversationProcessorConfig]
 
 
+class AppConfig(ConfigBase):
+    should_log_telemetry: bool
+
+
 class FullConfig(ConfigBase):
     content_type: Optional[ContentConfig]
     search_type: Optional[SearchConfig]
     processor: Optional[ProcessorConfig]
+    app: Optional[AppConfig] = AppConfig(should_log_telemetry=True)
 
 
 class SearchResponse(ConfigBase):
     entry: str
     score: str
     additional: Optional[dict]
 
 
 class Entry:
     raw: str
     compiled: str
+    heading: Optional[str]
     file: Optional[str]
 
-    def __init__(self, raw: str = None, compiled: str = None, file: Optional[str] = None):
+    def __init__(
+        self, raw: str = None, compiled: str = None, heading: Optional[str] = None, file: Optional[str] = None
+    ):
         self.raw = raw
         self.compiled = compiled
+        self.heading = heading
         self.file = file
 
     def to_json(self) -> str:
         return json.dumps(self.__dict__, ensure_ascii=False)
 
     def __repr__(self) -> str:
         return self.__dict__.__repr__()
```

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/utils/state.py` & `khoj_assistant-0.6.3.dev3/src/khoj/utils/state.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Standard Packages
 import threading
-from typing import List
+from typing import List, Dict
 from packaging import version
 
 # External Packages
 import torch
 from pathlib import Path
 
 # Internal Packages
@@ -21,14 +21,16 @@
 verbose: int = 0
 host: str = None
 port: int = None
 cli_args: List[str] = None
 query_cache = LRU()
 search_index_lock = threading.Lock()
 SearchType = utils_config.SearchType
+telemetry: List[Dict[str, str]] = []
+previous_query: str = None
 
 if torch.cuda.is_available():
     # Use CUDA GPU
     device = torch.device("cuda:0")
 elif version.parse(torch.__version__) >= version.parse("1.13.0.dev") and torch.backends.mps.is_available():
     # Use Apple M1 Metal Acceleration
     device = torch.device("mps")
```

### Comparing `khoj_assistant-0.6.2.dev6/src/khoj/utils/yaml.py` & `khoj_assistant-0.6.3.dev3/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/.gitignore` & `khoj_assistant-0.6.3.dev3/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/LICENSE` & `khoj_assistant-0.6.3.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/README.md` & `khoj_assistant-0.6.3.dev3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
   - **Natural**: Advanced natural language understanding using Transformer based ML Models
   - **Pluggable**: Modular architecture makes it easy to plug in new data sources, frontends and ML models
   - **Multiple Sources**: Index your Org-mode and Markdown notes, Beancount transactions and Photos
   - **Multiple Interfaces**: Interact from your [Web Browser](./src/khoj/interface/web/index.html), [Emacs](./src/interface/emacs/khoj.el) or [Obsidian](./src/interface/obsidian/)
 
 ## Demos
 ### Khoj in Obsidian
-https://user-images.githubusercontent.com/6413477/210486007-36ee3407-e6aa-4185-8a26-b0bfc0a4344f.mp4
+https://github.com/debanjum/khoj/assets/6413477/3e33d8ea-25bb-46c8-a3bf-c92f78d0f56b
 
 <details><summary>Description</summary>
 
 - Install Khoj via `pip` and start Khoj backend in non-gui mode
 - Install Khoj plugin via Community Plugins settings pane on Obsidian app
 - Check the new Khoj plugin settings
 - Let Khoj backend index the markdown files in the current Vault
@@ -269,15 +269,15 @@
 ### Use OpenAI Models for Search
 #### Setup
 1. Set `encoder-type`, `encoder` and `model-directory` under `asymmetric` and/or `symmetric` `search-type` in your `khoj.yml`[^1]:
    ```diff
       asymmetric:
    -    encoder: "sentence-transformers/multi-qa-MiniLM-L6-cos-v1"
    +    encoder: text-embedding-ada-002
-   +    encoder-type: src.khoj.utils.models.OpenAI
+   +    encoder-type: khoj.utils.models.OpenAI
         cross-encoder: "cross-encoder/ms-marco-MiniLM-L-6-v2"
    -    encoder-type: sentence_transformers.SentenceTransformer
    -    model_directory: "~/.khoj/search/asymmetric/"
    +    model-directory: null
    ```
 2. [Setup your OpenAI API key in Khoj](#set-your-openai-api-key-in-khoj)
 3. Restart Khoj server to generate embeddings. It will take longer than with offline models.
```

### Comparing `khoj_assistant-0.6.2.dev6/pyproject.toml` & `khoj_assistant-0.6.3.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.2.dev6/PKG-INFO` & `khoj_assistant-0.6.3.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.6.2.dev6
+Version: 0.6.3.dev3
 Summary: A natural language search engine for your personal notes, transactions and images
 Project-URL: Homepage, https://github.com/debanjum/khoj#readme
 Project-URL: Issues, https://github.com/debanjum/khoj/issues
 Project-URL: Discussions, https://github.com/debanjum/khoj/discussions
 Project-URL: Releases, https://github.com/debanjum/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
@@ -115,15 +115,15 @@
   - **Natural**: Advanced natural language understanding using Transformer based ML Models
   - **Pluggable**: Modular architecture makes it easy to plug in new data sources, frontends and ML models
   - **Multiple Sources**: Index your Org-mode and Markdown notes, Beancount transactions and Photos
   - **Multiple Interfaces**: Interact from your [Web Browser](./src/khoj/interface/web/index.html), [Emacs](./src/interface/emacs/khoj.el) or [Obsidian](./src/interface/obsidian/)
 
 ## Demos
 ### Khoj in Obsidian
-https://user-images.githubusercontent.com/6413477/210486007-36ee3407-e6aa-4185-8a26-b0bfc0a4344f.mp4
+https://github.com/debanjum/khoj/assets/6413477/3e33d8ea-25bb-46c8-a3bf-c92f78d0f56b
 
 <details><summary>Description</summary>
 
 - Install Khoj via `pip` and start Khoj backend in non-gui mode
 - Install Khoj plugin via Community Plugins settings pane on Obsidian app
 - Check the new Khoj plugin settings
 - Let Khoj backend index the markdown files in the current Vault
@@ -320,15 +320,15 @@
 ### Use OpenAI Models for Search
 #### Setup
 1. Set `encoder-type`, `encoder` and `model-directory` under `asymmetric` and/or `symmetric` `search-type` in your `khoj.yml`[^1]:
    ```diff
       asymmetric:
    -    encoder: "sentence-transformers/multi-qa-MiniLM-L6-cos-v1"
    +    encoder: text-embedding-ada-002
-   +    encoder-type: src.khoj.utils.models.OpenAI
+   +    encoder-type: khoj.utils.models.OpenAI
         cross-encoder: "cross-encoder/ms-marco-MiniLM-L-6-v2"
    -    encoder-type: sentence_transformers.SentenceTransformer
    -    model_directory: "~/.khoj/search/asymmetric/"
    +    model-directory: null
    ```
 2. [Setup your OpenAI API key in Khoj](#set-your-openai-api-key-in-khoj)
 3. Restart Khoj server to generate embeddings. It will take longer than with offline models.
```

