# Comparing `tmp/dxsp-2.5.5.tar.gz` & `tmp/dxsp-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.5.5.tar", max compression
+gzip compressed data, was "dxsp-2.6.0.tar", max compression
```

## Comparing `dxsp-2.5.5.tar` & `dxsp-2.6.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-05-27 13:48:18.044194 dxsp-2.5.5/LICENSE
--rw-r--r--   0        0        0     2439 2023-05-27 13:48:18.044194 dxsp-2.5.5/README.md
--rw-r--r--   0        0        0       86 2023-05-27 13:48:18.676208 dxsp-2.5.5/dxsp/__init__.py
--rw-r--r--   0        0        0      386 2023-05-27 13:48:18.044194 dxsp-2.5.5/dxsp/config.py
--rw-r--r--   0        0        0     3548 2023-05-27 13:48:18.044194 dxsp-2.5.5/dxsp/default_settings.toml
--rw-r--r--   0        0        0    20785 2023-05-27 13:48:18.044194 dxsp-2.5.5/dxsp/main.py
--rw-r--r--   0        0        0     1994 2023-05-27 13:48:18.676208 dxsp-2.5.5/pyproject.toml
--rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 dxsp-2.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-28 17:08:53.609362 dxsp-2.6.0/LICENSE
+-rw-r--r--   0        0        0     2439 2023-05-28 17:08:53.609362 dxsp-2.6.0/README.md
+-rw-r--r--   0        0        0       86 2023-05-28 17:08:54.277380 dxsp-2.6.0/dxsp/__init__.py
+-rw-r--r--   0        0        0      386 2023-05-28 17:08:53.609362 dxsp-2.6.0/dxsp/config.py
+-rw-r--r--   0        0        0     3548 2023-05-28 17:08:53.609362 dxsp-2.6.0/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    20968 2023-05-28 17:08:53.609362 dxsp-2.6.0/dxsp/main.py
+-rw-r--r--   0        0        0     1542 2023-05-28 17:08:54.273380 dxsp-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 dxsp-2.6.0/PKG-INFO
```

### Comparing `dxsp-2.5.5/LICENSE` & `dxsp-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.5.5/README.md` & `dxsp-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.5.5/dxsp/default_settings.toml` & `dxsp-2.6.0/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-2.5.5/dxsp/main.py` & `dxsp-2.6.0/dxsp/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -397,14 +397,19 @@
             else:
                 self.logger.warning("No ABI identified")
                 return None
         except Exception as e:
             self.logger.error("get_abi %s", e)
             return None
 
+    async def get_name(self):
+        try:
+            return settings.dex_router_contract_addr[-8:]
+        except Exception as e:
+            self.logger.error("router name %s", e)
 # 🔒 USER RELATED
     async def get_token_balance(self, token):
         try:
             contract = await self.get_token_contract(token)
             balance = contract.functions.balanceOf(self.wallet_address).call()
             return max(0, balance)
         except Exception as e:
```

### Comparing `dxsp-2.5.5/pyproject.toml` & `dxsp-2.6.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,58 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.5.5"
+version = "2.6.0"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
-
+packages = [
+    {include = "dxsp"}
+]
 
 [tool.poetry.urls]
 "Changelog" =  "https://github.com/mraniki/dxsp/blob/dev/CHANGELOG.rst"
 "Support" =  "https://github.com/mraniki/dxsp/discussions"
 "Issues" =  "https://github.com/mraniki/dxsp/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 asyncio = "*"
 dynaconf = "*"
 web3 = "^6.4.0"
 pycoingecko = "*"
-# uniswap-python = "*"
-# web3client = "*"
-#web3-ethereum-defi = "*"
-# web3client = ">=1.1.8"
-# # many-abis = ">=0.1.7"
-# apollox-connector-python = "*"
-
 
 [tool.poetry.dev-dependencies]
 python-semantic-release = "*"
 pytest = "*"
 pytest-cov = "*"
 pytest-asyncio = "*"
 pytest-mock = "*"
 
 [tool.pytest.ini_options]
-testpaths = "tests/"
-python_classes = [
-  "Test*",
-  "*Test"
-]
+pythonpath = "."
+testpaths = "tests"
+python_classes = "Test*"
 log_format = "%(asctime)s - %(levelname)s - %(name)s - %(message)s"
 log_level = "DEBUG"
-pythonpath = [
-  "."
+
+[tool.coverage.run]
+omit = [
+    "tests/*",
+    "examples/*"
 ]
-addopts = "--capture=no --ignore-glob=example*"
-ignore="test example"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 version_variable = ["pyproject.toml:version","dxsp/__init__.py:__version__"]
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "pip install poetry && poetry build"
 commit_parser = "semantic_release.history.emoji_parser"
 use_textual_changelog_sections = true
-major_emoji = "💥,:boom:,BREAKING CHANGE"
-minor_emoji = "feat,🥚,🚀,💄,✨,:rocket:,:sparkles:,:lipstick:,:egg:"
-patch_emoji = "fix,🎨,🐛,🚑,⚡,🔥,🚨,♻️,🔧,⬆️,🩹,👷,📝,🔒,👽,💬,🥅,✅,🐳,🙈,⚗️,🧐,🔇,🔊,:mute:,:loud_sound:,:monocle_face:,:alembic:,:see_no_evil:,:white_check_mark:,:arrow_up:,:recycle:,:fire,:whale:,:art:,:ambulance:,:lock:,:arrow_up:,:bug:,:zap:,:goal_net:,:alien:,:speech_balloon:,:rotating_light:,:construction_worker:"
+major_emoji = "💥"
+minor_emoji = "🥚,🚀,💄,✨"
+patch_emoji = "🎨,🐛,🚑,⚡,🔥,🚨,♻️,🔧,⬆️,🩹,👷,📝,🔒,👽,💬,🥅,✅,🐳,🙈,⚗️,🧐,🔇,🔊"
```

### Comparing `dxsp-2.5.5/PKG-INFO` & `dxsp-2.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.5.5
+Version: 2.6.0
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

