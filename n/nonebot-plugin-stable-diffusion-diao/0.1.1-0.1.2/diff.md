# Comparing `tmp/nonebot_plugin_stable_diffusion_diao-0.1.1.tar.gz` & `tmp/nonebot_plugin_stable_diffusion_diao-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.1.2.tar", last modified: Sun May 28 10:22:59 2023, max compression
```

## Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1.tar` & `nonebot_plugin_stable_diffusion_diao-0.1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.1.1/LICENSE
--rw-r--r--   0        0        0      686 2023-05-28 09:58:15.400842 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/__init__.py
--rw-r--r--   0        0        0    18654 2023-05-28 09:58:15.401369 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/aidraw.py
--rw-r--r--   0        0        0     6093 2023-05-28 09:58:15.401892 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
--rw-r--r--   0        0        0    65592 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
--rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
--rw-r--r--   0        0        0    15370 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/backend/base.py
--rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
--rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
--rw-r--r--   0        0        0     6321 2023-05-28 09:58:15.405664 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/backend/sd.py
--rw-r--r--   0        0        0    13441 2023-05-28 09:58:15.405664 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/config.py
--rw-r--r--   0        0        0     9282 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
--rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
--rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
--rw-r--r--   0        0        0     1328 2023-05-28 09:58:15.407673 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
--rw-r--r--   0        0        0     3751 2023-05-28 09:58:15.407673 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
--rw-r--r--   0        0        0    11304 2023-05-28 09:58:15.407673 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
--rw-r--r--   0        0        0     3668 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
--rw-r--r--   0        0        0    28380 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
--rw-r--r--   0        0        0     5964 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/extension/translation.py
--rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/fifo.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/locales/en.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/locales/jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/locales/zh.py
--rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/manage.py
--rw-r--r--   0        0        0     1479 2023-05-28 09:58:15.412189 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
--rw-r--r--   0        0        0     2314 2023-05-28 09:58:15.412189 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/utils/data.py
--rw-r--r--   0        0        0     7545 2023-05-28 09:58:15.412189 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
--rw-r--r--   0        0        0      647 2023-05-28 09:58:15.413187 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
--rw-r--r--   0        0        0      727 2023-05-28 09:58:15.413187 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/utils/save.py
--rw-r--r--   0        0        0     1994 2023-05-28 09:58:15.414188 nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/version.py
--rw-r--r--   0        0        0      698 2023-05-28 10:15:00.412326 nonebot_plugin_stable_diffusion_diao-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    16199 2023-05-28 09:58:15.376490 nonebot_plugin_stable_diffusion_diao-0.1.1/README.md
--rw-r--r--   0        0        0    16374 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.1.2/LICENSE
+-rw-r--r--   0        0        0    16199 2023-05-28 09:58:15.376490 nonebot_plugin_stable_diffusion_diao-0.1.2/README.md
+-rw-r--r--   0        0        0      686 2023-05-28 09:58:15.400842 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/__init__.py
+-rw-r--r--   0        0        0    18654 2023-05-28 09:58:15.401369 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/aidraw.py
+-rw-r--r--   0        0        0     6093 2023-05-28 09:58:15.401892 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
+-rw-r--r--   0        0        0    65592 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
+-rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
+-rw-r--r--   0        0        0    15370 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/backend/base.py
+-rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
+-rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
+-rw-r--r--   0        0        0     6321 2023-05-28 09:58:15.405664 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/backend/sd.py
+-rw-r--r--   0        0        0    13441 2023-05-28 09:58:15.405664 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/config.py
+-rw-r--r--   0        0        0     9282 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
+-rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
+-rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
+-rw-r--r--   0        0        0     1328 2023-05-28 09:58:15.407673 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
+-rw-r--r--   0        0        0     3751 2023-05-28 09:58:15.407673 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
+-rw-r--r--   0        0        0    11304 2023-05-28 09:58:15.407673 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
+-rw-r--r--   0        0        0     3668 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
+-rw-r--r--   0        0        0    28380 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
+-rw-r--r--   0        0        0     5964 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/extension/translation.py
+-rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/fifo.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/locales/en.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/locales/jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/locales/zh.py
+-rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/manage.py
+-rw-r--r--   0        0        0     1479 2023-05-28 09:58:15.412189 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
+-rw-r--r--   0        0        0     2314 2023-05-28 09:58:15.412189 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/utils/data.py
+-rw-r--r--   0        0        0     7545 2023-05-28 09:58:15.412189 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
+-rw-r--r--   0        0        0      647 2023-05-28 09:58:15.413187 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
+-rw-r--r--   0        0        0      727 2023-05-28 09:58:15.413187 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/utils/save.py
+-rw-r--r--   0        0        0     1994 2023-05-28 09:58:15.414188 nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/version.py
+-rw-r--r--   0        0        0      626 2023-05-28 10:22:59.144531 nonebot_plugin_stable_diffusion_diao-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    16442 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1/LICENSE` & `nonebot_plugin_stable_diffusion_diao-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/aidraw.py` & `nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/aidraw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py` & `nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py` & `nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/backend/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/backend/base.py` & `nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/backend/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/backend/naifu.py` & `nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/backend/naifu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/backend/novelai.py` & `nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/backend/novelai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/backend/sd.py` & `nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/backend/sd.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/config.py` & `nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py` & `nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/extension/anlas.py` & `nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/extension/anlas.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/extension/control_net.py` & `nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/extension/control_net.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py` & `nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py` & `nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py` & `nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py` & `nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py` & `nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/extension/translation.py` & `nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/extension/translation.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/manage.py` & `nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/manage.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/utils/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/utils/data.py` & `nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/utils/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py` & `nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py` & `nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/utils/save.py` & `nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/utils/save.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1/nonebot_plugin_stable_diffusion_diao/version.py` & `nonebot_plugin_stable_diffusion_diao-0.1.2/nonebot_plugin_stable_diffusion_diao/version.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1/README.md` & `nonebot_plugin_stable_diffusion_diao-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.1/PKG-INFO` & `nonebot_plugin_stable_diffusion_diao-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-stable-diffusion-diao
-Version: 0.1.1
+Version: 0.1.2
 Summary: 主要面对stable-diffusion-webui-api的nonebot2插件
+Author-Email: DiaoDaiaChan <diaodaiachan@qq.com>
 License: MIT
-Author: DiaoDaiaChan
-Author-email: diaodaiachan@qq.com
-Requires-Python: >=3.10,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.10
+Requires-Dist: aiofiles>=23.1.0
+Requires-Dist: aiohttp>=3.8.4
+Requires-Dist: nonebot-adapter-onebot>=2.1.3
+Requires-Dist: nonebot2>=2.0.0b4
+Requires-Dist: nonebot-plugin-htmlrender==0.2.0.3
+Requires-Dist: Pillow>=9.5.0
+Requires-Dist: qrcode>=7.4.2
+Requires-Dist: tensorflow==2.9.0
 Description-Content-Type: text/markdown
 
 # 首先 这个项目fork自https://github.com/sena-nana/nonebot-plugin-novelai
 ## 感谢 sena喵 感谢 sena喵 感谢 sena喵
 因为懒得更改其他地方了，所以有不少nonebot-plugin-novelai的地方，凑合用就行(
 
 # 支持中文关键词的基于nonebot2的AI绘图插件
@@ -318,8 +321,8 @@
 novelai_extra_pic_audit = False # 是否为二次元的我, chatgpt生成tag等功能添加审核功能
 # 翻译API设置
 bing_key: str = None  # bing的翻译key
 deepl_key: str = None  # deepL的翻译key
 baidu_translate_key: dict = None # 例:{"SECRET_KEY": "", "API_KEY": ""} # https://console.bce.baidu.com/ai/?_=1685076516634#/ai/machinetranslation/overview/index
 novelai_todaygirl = 1 # 可选值 1 和 2 两种不同的方式
 novelai_tagger_site: str = None # 分析功能的地址 例如 127.0.0.1:7860
-```
+```
```

