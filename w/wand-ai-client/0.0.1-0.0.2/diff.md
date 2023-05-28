# Comparing `tmp/wand-ai-client-0.0.1.tar.gz` & `tmp/wand-ai-client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wand-ai-client-0.0.1.tar", last modified: Sat May 27 19:56:31 2023, max compression
+gzip compressed data, was "wand-ai-client-0.0.2.tar", last modified: Sun May 28 09:05:02 2023, max compression
```

## Comparing `wand-ai-client-0.0.1.tar` & `wand-ai-client-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-27 19:56:31.205309 wand-ai-client-0.0.1/
--rw-r--r--   0 romasku   (1000) romasku   (1000)      884 2023-05-27 19:56:31.205309 wand-ai-client-0.0.1/PKG-INFO
--rw-r--r--   0 romasku   (1000) romasku   (1000)     1075 2023-05-22 19:10:31.000000 wand-ai-client-0.0.1/README.md
--rw-r--r--   0 romasku   (1000) romasku   (1000)      176 2023-05-27 16:26:52.000000 wand-ai-client-0.0.1/pyproject.toml
--rw-r--r--   0 romasku   (1000) romasku   (1000)     1861 2023-05-27 19:56:31.205309 wand-ai-client-0.0.1/setup.cfg
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-27 19:56:31.205309 wand-ai-client-0.0.1/wand_ai_client.egg-info/
--rw-r--r--   0 romasku   (1000) romasku   (1000)      884 2023-05-27 19:56:31.000000 wand-ai-client-0.0.1/wand_ai_client.egg-info/PKG-INFO
--rw-r--r--   0 romasku   (1000) romasku   (1000)      485 2023-05-27 19:56:31.000000 wand-ai-client-0.0.1/wand_ai_client.egg-info/SOURCES.txt
--rw-r--r--   0 romasku   (1000) romasku   (1000)        1 2023-05-27 19:56:31.000000 wand-ai-client-0.0.1/wand_ai_client.egg-info/dependency_links.txt
--rw-r--r--   0 romasku   (1000) romasku   (1000)       54 2023-05-27 19:56:31.000000 wand-ai-client-0.0.1/wand_ai_client.egg-info/entry_points.txt
--rw-r--r--   0 romasku   (1000) romasku   (1000)        1 2023-05-27 19:56:31.000000 wand-ai-client-0.0.1/wand_ai_client.egg-info/not-zip-safe
--rw-r--r--   0 romasku   (1000) romasku   (1000)      228 2023-05-27 19:56:31.000000 wand-ai-client-0.0.1/wand_ai_client.egg-info/requires.txt
--rw-r--r--   0 romasku   (1000) romasku   (1000)       12 2023-05-27 19:56:31.000000 wand-ai-client-0.0.1/wand_ai_client.egg-info/top_level.txt
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-27 19:56:31.205309 wand-ai-client-0.0.1/wand_client/
--rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-26 17:07:29.000000 wand-ai-client-0.0.1/wand_client/__init__.py
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-27 19:56:31.205309 wand-ai-client-0.0.1/wand_client/cli/
--rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-27 15:55:30.000000 wand-ai-client-0.0.1/wand_client/cli/__init__.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     1189 2023-05-27 19:51:51.000000 wand-ai-client-0.0.1/wand_client/cli/config.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     2578 2023-05-27 19:20:56.000000 wand-ai-client-0.0.1/wand_client/cli/formatters.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     5296 2023-05-27 19:48:08.000000 wand-ai-client-0.0.1/wand_client/cli/main.py
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-27 19:56:31.205309 wand-ai-client-0.0.1/wand_client/sdk/
--rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-27 15:04:20.000000 wand-ai-client-0.0.1/wand_client/sdk/__init__.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     4796 2023-05-27 19:51:51.000000 wand-ai-client-0.0.1/wand_client/sdk/core.py
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-28 09:05:02.336634 wand-ai-client-0.0.2/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      884 2023-05-28 09:05:02.336634 wand-ai-client-0.0.2/PKG-INFO
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     1075 2023-05-22 19:10:31.000000 wand-ai-client-0.0.2/README.md
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      176 2023-05-27 16:26:52.000000 wand-ai-client-0.0.2/pyproject.toml
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     1861 2023-05-28 09:05:02.339968 wand-ai-client-0.0.2/setup.cfg
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-28 09:05:02.336634 wand-ai-client-0.0.2/wand_ai_client.egg-info/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      884 2023-05-28 09:05:02.000000 wand-ai-client-0.0.2/wand_ai_client.egg-info/PKG-INFO
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      485 2023-05-28 09:05:02.000000 wand-ai-client-0.0.2/wand_ai_client.egg-info/SOURCES.txt
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        1 2023-05-28 09:05:02.000000 wand-ai-client-0.0.2/wand_ai_client.egg-info/dependency_links.txt
+-rw-r--r--   0 romasku   (1000) romasku   (1000)       54 2023-05-28 09:05:02.000000 wand-ai-client-0.0.2/wand_ai_client.egg-info/entry_points.txt
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        1 2023-05-27 19:56:31.000000 wand-ai-client-0.0.2/wand_ai_client.egg-info/not-zip-safe
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      228 2023-05-28 09:05:02.000000 wand-ai-client-0.0.2/wand_ai_client.egg-info/requires.txt
+-rw-r--r--   0 romasku   (1000) romasku   (1000)       12 2023-05-28 09:05:02.000000 wand-ai-client-0.0.2/wand_ai_client.egg-info/top_level.txt
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-28 09:05:02.336634 wand-ai-client-0.0.2/wand_client/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-26 17:07:29.000000 wand-ai-client-0.0.2/wand_client/__init__.py
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-28 09:05:02.336634 wand-ai-client-0.0.2/wand_client/cli/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-27 15:55:30.000000 wand-ai-client-0.0.2/wand_client/cli/__init__.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     1148 2023-05-28 09:03:50.000000 wand-ai-client-0.0.2/wand_client/cli/config.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     2546 2023-05-28 08:59:31.000000 wand-ai-client-0.0.2/wand_client/cli/formatters.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     5288 2023-05-28 09:03:27.000000 wand-ai-client-0.0.2/wand_client/cli/main.py
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-28 09:05:02.336634 wand-ai-client-0.0.2/wand_client/sdk/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-27 15:04:20.000000 wand-ai-client-0.0.2/wand_client/sdk/__init__.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     4774 2023-05-28 09:03:50.000000 wand-ai-client-0.0.2/wand_client/sdk/core.py
```

### Comparing `wand-ai-client-0.0.1/PKG-INFO` & `wand-ai-client-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wand-ai-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: Wand AI API client
 Author: Wand.AI Team
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `wand-ai-client-0.0.1/README.md` & `wand-ai-client-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `wand-ai-client-0.0.1/setup.cfg` & `wand-ai-client-0.0.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wand-ai-client
-version = 0.0.1
+version = 0.0.2
 description = Wand AI API client
 author = Wand.AI Team
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
```

### Comparing `wand-ai-client-0.0.1/wand_ai_client.egg-info/PKG-INFO` & `wand-ai-client-0.0.2/wand_ai_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wand-ai-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: Wand AI API client
 Author: Wand.AI Team
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `wand-ai-client-0.0.1/wand_client/cli/config.py` & `wand-ai-client-0.0.2/wand_client/cli/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,26 @@
-from __future__ import annotations
-
 import json
-from collections.abc import Sequence
 from pathlib import Path
-from typing import Any
+from typing import Any, Dict, Optional, Sequence
 
 from pydantic import BaseSettings
 
 CONFIG_PATH = Path("~/.wand/config.json")
 
 
-def json_config_settings_source(settings: BaseSettings) -> dict[str, Any]:
+def json_config_settings_source(settings: BaseSettings) -> Dict[str, Any]:
     encoding = settings.__config__.env_file_encoding
     if CONFIG_PATH.exists():
         return json.loads(CONFIG_PATH.read_text(encoding))
     return {}
 
 
 class WandCliSettings(BaseSettings):
-    WAND_API_URL: str | None = None
-    WAND_TOKEN: str | None = None
+    WAND_API_URL: Optional[str] = None
+    WAND_TOKEN: Optional[str] = None
 
     def check_complete(self) -> None:
         if self.WAND_API_URL is None:
             raise ValueError("Settings WAND_API_URL is not set")
         if self.WAND_TOKEN is None:
             raise ValueError("Settings WAND_TOKEN is not set")
```

### Comparing `wand-ai-client-0.0.1/wand_client/cli/formatters.py` & `wand-ai-client-0.0.2/wand_client/cli/formatters.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-from __future__ import annotations
-
 import operator
-from collections.abc import Sequence
+from typing import Optional, Sequence
 
 from rich import box
 from rich.console import RenderableType
 from rich.table import Table
 
 from wand_client.cli.config import WandCliSettings
 from wand_client.sdk.core import Model, Source
@@ -19,15 +17,15 @@
             show_edge=False,
         )
         table.add_column()
         table.add_column(style="bold")
         table.add_row("WAND_API_URL", settings.WAND_API_URL)
         if settings.WAND_TOKEN and ":" in settings.WAND_TOKEN:
             token_id, token_secret = settings.WAND_TOKEN.split(":")
-            token_str: str | None = f"{token_id}:{'*' * len(token_secret)}"
+            token_str: Optional[str] = f"{token_id}:{'*' * len(token_secret)}"
         else:
             token_str = settings.WAND_TOKEN
         table.add_row("WAND_TOKEN", token_str)
         return table
 
 
 class SourceFormatter:
```

### Comparing `wand-ai-client-0.0.1/wand_client/cli/main.py` & `wand-ai-client-0.0.2/wand_client/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-from __future__ import annotations
-
 import json
 from pathlib import Path
-from typing import Any
+from typing import Any, Dict, List, Optional
 
 import click
 import rich
 from click import Context
 from prompt_toolkit import PromptSession
 from rich.progress import Progress
 
@@ -23,15 +21,15 @@
     Model,
     TrainingListener,
     WandClient,
 )
 
 
 class Root:
-    def __init__(self, option_settings: dict[str, Any]) -> None:
+    def __init__(self, option_settings: Dict[str, Any]) -> None:
         self._option_settings = option_settings
 
     def get_settings(self) -> WandCliSettings:
         return WandCliSettings(**self._option_settings)
 
     def get_client(self) -> WandClient:
         settings = self.get_settings()
@@ -42,15 +40,15 @@
         )
 
 
 @click.group()
 @click.option("--api_url", type=str, default=None)
 @click.option("--token", type=str, default=None)
 @click.pass_context
-def cli(ctx: Context, api_url: str | None, token: str | None) -> None:
+def cli(ctx: Context, api_url: Optional[str], token: Optional[str]) -> None:
     option_settings = {
         "WAND_API_URL": api_url,
         "WAND_TOKEN": token,
     }
     option_settings = {
         key: value for key, value in option_settings.items() if value is not None
     }
@@ -109,15 +107,15 @@
     rich.print(SourceFormatter()(source))
 
 
 @source.command()
 @click.option("--max-pages", type=int, default=1000)
 @click.argument("url", type=click.STRING, nargs=-1)
 @click.pass_context
-def web(ctx: Context, url: list[str], max_pages: int = 1000) -> None:
+def web(ctx: Context, url: List[str], max_pages: int = 1000) -> None:
     """Upload a file as a source"""
     client: WandClient = ctx.obj.get_client()
     source = client.source.create_web(url, max_pages)
     rich.print(SourceFormatter()(source))
 
 
 @cli.group()
@@ -126,15 +124,15 @@
     Operations with ml models
     """
 
 
 @source.command()
 @click.argument("source_id", type=click.STRING, nargs=-1)
 @click.pass_context
-def train(ctx: Context, source_id: list[str]) -> None:
+def train(ctx: Context, source_id: List[str]) -> None:
     """Upload a file as a source"""
     client: WandClient = ctx.obj.get_client()
 
     with Progress() as progress:
         task = progress.add_task("Training model")
 
         class _Listener(TrainingListener):
@@ -171,15 +169,15 @@
 
 @model.command()
 @click.argument("model_id", type=click.STRING)
 @click.pass_context
 def chat(ctx: Context, model_id: str) -> None:
     """Upload a file as a source"""
     client: WandClient = ctx.obj.get_client()
-    history: list[ChatMessage] = []
+    history: List[ChatMessage] = []
 
     print(f"You are talking to model with id {model_id}. Type 'exit' to close.")
 
     session: PromptSession[str] = PromptSession()
     console = rich.console.Console()
     while True:
         prompt_text = session.prompt("> ")
```

### Comparing `wand-ai-client-0.0.1/wand_client/sdk/core.py` & `wand-ai-client-0.0.2/wand_client/sdk/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,25 @@
-from __future__ import annotations
-
 import abc
 import enum
 import time
-from collections.abc import Mapping, Sequence
 from pathlib import Path
-from typing import Any
+from typing import Any, Dict, List, Mapping, Optional, Sequence, Union
 
 import requests
 from pydantic import BaseModel
 from requests import Response
 
 
 class WandCoreClient:
     def __init__(self, token: str, base_url: str) -> None:
         self._token = token
         self._base_url = base_url
 
     def request(
-        self, method: str, path: str, json: dict[str, Any] | None = None
+        self, method: str, path: str, json: Optional[Dict[str, Any]] = None
     ) -> Response:
         resp = requests.request(
             method=method,
             url=self._base_url + path,
             headers={"Authorization": f"Bearer {self._token}"},
             json=json,
         )
@@ -41,15 +38,15 @@
 
 class Sources:
     def __init__(self, core: WandCoreClient) -> None:
         self._core = core
 
     def create_web(
         self,
-        urls: list[str],
+        urls: List[str],
         max_crawl_pages: int = 20,
     ) -> Source:
         res = self._core.request(
             method="post",
             path="/source/web_scraper",
             json={
                 "urls": urls,
@@ -66,30 +63,30 @@
                 "filename": filename,
             },
         ).json()
         return FileSourceCreationResult(
             source=Source(id=res["source_id"]), upload_url=res["upload_signed_url"]
         )
 
-    def create_from_filepath(self, filepath: str | Path) -> Source:
+    def create_from_filepath(self, filepath: Union[str, Path]) -> Source:
         path = Path(filepath)
         res = self.create_file(path.name)
         with path.open() as file:
             requests.put(res.upload_url, data=file)
         return res.source
 
 
 class ModelStatus(BaseModel):
     progress: int
     training_completed: bool
 
 
 class Model(BaseModel):
     id: str
-    source_ids: list[str]
+    source_ids: List[str]
     status: ModelStatus
 
 
 class ChatMessageAuthor(str, enum.Enum):
     AI = "ai"
     HUMAN = "human"
 
@@ -115,15 +112,15 @@
             source_ids=payload["source_ids"],
             status=ModelStatus(
                 progress=payload["status"]["progress"],
                 training_completed=payload["status"]["training_completed"],
             ),
         )
 
-    def start_training(self, source_ids: list[str]) -> Model:
+    def start_training(self, source_ids: List[str]) -> Model:
         res = self._core.request(
             method="post",
             path="/models",
             json={
                 "source_ids": source_ids,
             },
         ).json()
@@ -132,15 +129,15 @@
     def get(self, model_id: str) -> Model:
         res = self._core.request(
             method="GET",
             path=f"/models/{model_id}",
         ).json()
         return self._parse_model_payload(res)
 
-    def list_all(self) -> list[Model]:
+    def list_all(self) -> List[Model]:
         res = self._core.request(
             method="GET",
             path=f"/models",
         ).json()
         return [self._parse_model_payload(it) for it in res]
 
     def infer(
@@ -159,15 +156,15 @@
                     for it in chat_history
                 ],
             },
         )
         return res.json()
 
     def train(
-        self, source_ids: list[str], listener: TrainingListener | None = None
+        self, source_ids: List[str], listener: Optional[TrainingListener] = None
     ) -> Model:
         model = self.start_training(source_ids)
         while True:
             model = self.get(model.id)
             if listener:
                 listener.on_model_progress(model)
             if model.status.training_completed:
```

