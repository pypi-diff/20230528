# Comparing `tmp/attacus-0.1.2-cp310-cp310-win_amd64.whl.zip` & `tmp/attacus-0.1.3-cp310-cp310-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,18 @@
-Zip file size: 901123 bytes, number of entries: 17
+Zip file size: 900391 bytes, number of entries: 16
 -rw-rw-rw-  2.0 fat       23 b- defN 23-May-26 10:35 attacus/__about__.py
 -rw-rw-rw-  2.0 fat      165 b- defN 23-May-27 06:52 attacus/__init__.py
 -rw-rw-rw-  2.0 fat      189 b- defN 23-May-26 08:44 attacus/app.py
--rw-rw-rw-  2.0 fat     2398 b- defN 23-May-28 01:19 attacus/artifacts.py
+-rw-rw-rw-  2.0 fat     2771 b- defN 23-May-28 16:10 attacus/artifacts.py
 -rw-rw-rw-  2.0 fat  2275328 b- defN 23-May-28 07:29 attacus/attacus.pyd
 -rw-rw-rw-  2.0 fat      412 b- defN 23-May-28 06:53 attacus/build.py
--rw-rw-rw-  2.0 fat     1650 b- defN 23-May-26 09:47 attacus/ensure.py
 -rw-rw-rw-  2.0 fat      429 b- defN 23-May-28 01:20 attacus/flutter_config.py
 -rw-rw-rw-  2.0 fat      355 b- defN 23-May-27 08:23 attacus/flutter_view.py
 -rw-rw-rw-  2.0 fat      480 b- defN 23-May-28 06:31 attacus/install.py
--rw-rw-rw-  2.0 fat      372 b- defN 23-May-28 06:52 attacus/post_build.py
+-rw-rw-rw-  2.0 fat      636 b- defN 23-May-28 12:49 attacus/post_build.py
 -rw-rw-rw-  2.0 fat      186 b- defN 23-May-28 06:30 attacus/uninstall.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-May-28 07:30 attacus-0.1.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4221 b- defN 23-May-28 07:30 attacus-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-May-28 07:30 attacus-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-28 07:30 attacus-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1295 b- defN 23-May-28 07:30 attacus-0.1.2.dist-info/RECORD
-17 files, 2288704 bytes uncompressed, 899027 bytes compressed:  60.7%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-May-28 17:17 attacus-0.1.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4271 b- defN 23-May-28 17:17 attacus-0.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-May-28 17:17 attacus-0.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-28 17:17 attacus-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1221 b- defN 23-May-28 17:17 attacus-0.1.3.dist-info/RECORD
+16 files, 2287667 bytes uncompressed, 898405 bytes compressed:  60.7%
```

## zipnote {}

```diff
@@ -12,17 +12,14 @@
 
 Filename: attacus/attacus.pyd
 Comment: 
 
 Filename: attacus/build.py
 Comment: 
 
-Filename: attacus/ensure.py
-Comment: 
-
 Filename: attacus/flutter_config.py
 Comment: 
 
 Filename: attacus/flutter_view.py
 Comment: 
 
 Filename: attacus/install.py
@@ -30,23 +27,23 @@
 
 Filename: attacus/post_build.py
 Comment: 
 
 Filename: attacus/uninstall.py
 Comment: 
 
-Filename: attacus-0.1.2.dist-info/LICENSE
+Filename: attacus-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: attacus-0.1.2.dist-info/METADATA
+Filename: attacus-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: attacus-0.1.2.dist-info/WHEEL
+Filename: attacus-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: attacus-0.1.2.dist-info/top_level.txt
+Filename: attacus-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: attacus-0.1.2.dist-info/RECORD
+Filename: attacus-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## attacus/artifacts.py

```diff
@@ -1,11 +1,12 @@
 import os
 import requests
 import tempfile
 import zipfile
+import json
 
 from loguru import logger
 
 from pathlib import Path
 from platformdirs import user_cache_dir
 
 appname = "Attacus"
@@ -36,23 +37,31 @@
     if not path.exists():
         url = f'https://storage.googleapis.com/flutter_infra_release/flutter/{version}/windows-x64/artifacts.zip'
         zip_file = download_file(url)
         extract_zip(zip_file, path)
 
 def get_engine_version() -> str:
     #version = '90fa3ae28fe6ddaee1af2c120f01e50201c1401b'
-    version = os.environ.get('FLUTTER_ENGINE_VERSION')
-    if not version:
+    version = None
+    flutter_assets = os.environ.get('FLUTTER_ASSETS')
+    if flutter_assets:
+        logger.debug(f'loading engine version from {flutter_assets}')
+        engine_data_path = Path(flutter_assets) / 'Engine.json'
+        with open(engine_data_path, 'r') as f:
+            engine_data = json.load(f)
+            version = engine_data['version']
+    else:
         flutter_root = os.environ.get('FLUTTER_ROOT')
         if not flutter_root:
             return None
+        logger.debug(f'loading engine version from sdk')
         version_path = flutter_root / Path('bin/internal/engine.version')
         with open(version_path, 'r') as file:
             version = file.readline().rstrip()
-    #logger.debug(version)
+    logger.debug(version)
     return version
 
 def download_file(url: str):
     response = requests.get(url, stream=True)
     temp_file = tempfile.TemporaryFile()
     for chunk in response.iter_content(chunk_size=128):
         temp_file.write(chunk)
```

## attacus/post_build.py

```diff
@@ -1,15 +1,23 @@
 import shutil
 from pathlib import Path
+import json
 
 from rich import print
 
-from .artifacts import get_icu_data_path
+from .artifacts import get_icu_data_path, get_engine_version
 
 def post_build():
+    engine_data =  {
+        "version": get_engine_version()
+    }
+    engine_data_path = Path.cwd() / 'build' / 'flutter_assets' / 'Engine.json'
+    with open(engine_data_path, 'w') as f:
+        json.dump(engine_data, f)
+
     # Copy icudtl.dat to the build folder so c++ tests and examples can find it
     from_path = get_icu_data_path()
     to_path = Path.cwd() / 'build'
     shutil.copy2(from_path, to_path)
 
 if __name__ == "__main__":
     post_build()
```

## Comparing `attacus-0.1.2.dist-info/LICENSE` & `attacus-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `attacus-0.1.2.dist-info/METADATA` & `attacus-0.1.3.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attacus
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python Flutter Extension
 Author-email: Kurtis Fields <kurtisfields@gmail.com>
 License: MIT License        
         Copyright (c) 2023 Kurtis Fields        
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -36,14 +36,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: loguru (~=0.7.0)
 Requires-Dist: platformdirs (~=3.5.1)
 Requires-Dist: requests (~=2.31.0)
 Requires-Dist: rich (~=13.3.5)
 Provides-Extra: dev
+Requires-Dist: cxbuild (==0.1.0) ; extra == 'dev'
 Requires-Dist: black (~=22.12.0) ; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest (~=7.2.1) ; extra == 'test'
 
 # Attacus :snake: :butterfly:
 
 Flutter Python Extension
```

