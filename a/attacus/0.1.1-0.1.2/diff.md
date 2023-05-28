# Comparing `tmp/attacus-0.1.1-cp310-cp310-win_amd64.whl.zip` & `tmp/attacus-0.1.2-cp310-cp310-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,19 @@
-Zip file size: 899932 bytes, number of entries: 13
+Zip file size: 901123 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat       23 b- defN 23-May-26 10:35 attacus/__about__.py
 -rw-rw-rw-  2.0 fat      165 b- defN 23-May-27 06:52 attacus/__init__.py
 -rw-rw-rw-  2.0 fat      189 b- defN 23-May-26 08:44 attacus/app.py
--rw-rw-rw-  2.0 fat     2395 b- defN 23-May-27 06:55 attacus/artifacts.py
--rw-rw-rw-  2.0 fat  2275328 b- defN 23-May-27 08:20 attacus/attacus.pyd
+-rw-rw-rw-  2.0 fat     2398 b- defN 23-May-28 01:19 attacus/artifacts.py
+-rw-rw-rw-  2.0 fat  2275328 b- defN 23-May-28 07:29 attacus/attacus.pyd
+-rw-rw-rw-  2.0 fat      412 b- defN 23-May-28 06:53 attacus/build.py
 -rw-rw-rw-  2.0 fat     1650 b- defN 23-May-26 09:47 attacus/ensure.py
--rw-rw-rw-  2.0 fat      365 b- defN 23-May-27 08:25 attacus/flutter_config.py
+-rw-rw-rw-  2.0 fat      429 b- defN 23-May-28 01:20 attacus/flutter_config.py
 -rw-rw-rw-  2.0 fat      355 b- defN 23-May-27 08:23 attacus/flutter_view.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-May-27 08:52 attacus-0.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     5082 b- defN 23-May-27 08:52 attacus-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-May-27 08:52 attacus-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-27 08:52 attacus-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      996 b- defN 23-May-27 08:52 attacus-0.1.1.dist-info/RECORD
-13 files, 2287749 bytes uncompressed, 898290 bytes compressed:  60.8%
+-rw-rw-rw-  2.0 fat      480 b- defN 23-May-28 06:31 attacus/install.py
+-rw-rw-rw-  2.0 fat      372 b- defN 23-May-28 06:52 attacus/post_build.py
+-rw-rw-rw-  2.0 fat      186 b- defN 23-May-28 06:30 attacus/uninstall.py
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-May-28 07:30 attacus-0.1.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4221 b- defN 23-May-28 07:30 attacus-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-May-28 07:30 attacus-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-28 07:30 attacus-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1295 b- defN 23-May-28 07:30 attacus-0.1.2.dist-info/RECORD
+17 files, 2288704 bytes uncompressed, 899027 bytes compressed:  60.7%
```

## zipnote {}

```diff
@@ -9,32 +9,44 @@
 
 Filename: attacus/artifacts.py
 Comment: 
 
 Filename: attacus/attacus.pyd
 Comment: 
 
+Filename: attacus/build.py
+Comment: 
+
 Filename: attacus/ensure.py
 Comment: 
 
 Filename: attacus/flutter_config.py
 Comment: 
 
 Filename: attacus/flutter_view.py
 Comment: 
 
-Filename: attacus-0.1.1.dist-info/LICENSE
+Filename: attacus/install.py
+Comment: 
+
+Filename: attacus/post_build.py
+Comment: 
+
+Filename: attacus/uninstall.py
+Comment: 
+
+Filename: attacus-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: attacus-0.1.1.dist-info/METADATA
+Filename: attacus-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: attacus-0.1.1.dist-info/WHEEL
+Filename: attacus-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: attacus-0.1.1.dist-info/top_level.txt
+Filename: attacus-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: attacus-0.1.1.dist-info/RECORD
+Filename: attacus-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## attacus/artifacts.py

```diff
@@ -17,26 +17,26 @@
     if not version:
         raise RuntimeError('Flutter Engine Version not found')
     ensure_engine(version)
     ensure_artifacts(version)
 
 def ensure_engine(version: str) -> None:
     path = Path(user_cache_dir(appname, appauthor)) / 'flutter' / version / 'engine'
-    logger.debug(path)
+    #logger.debug(path)
     if not path.exists():
         url = f'https://storage.googleapis.com/flutter_infra_release/flutter/{version}/windows-x64/windows-x64-embedder.zip'
         zip_file = download_file(url)
         extract_zip(zip_file, path)
 
     #os.environ["PATH"] = f"{path}{os.pathsep}{os.environ['PATH']}"
     os.add_dll_directory(path)
 
 def ensure_artifacts(version: str) -> None:
     path = Path(user_cache_dir(appname, appauthor)) / 'flutter' / version / 'artifacts'
-    logger.debug(path)
+    #logger.debug(path)
     if not path.exists():
         url = f'https://storage.googleapis.com/flutter_infra_release/flutter/{version}/windows-x64/artifacts.zip'
         zip_file = download_file(url)
         extract_zip(zip_file, path)
 
 def get_engine_version() -> str:
     #version = '90fa3ae28fe6ddaee1af2c120f01e50201c1401b'
@@ -44,15 +44,15 @@
     if not version:
         flutter_root = os.environ.get('FLUTTER_ROOT')
         if not flutter_root:
             return None
         version_path = flutter_root / Path('bin/internal/engine.version')
         with open(version_path, 'r') as file:
             version = file.readline().rstrip()
-    logger.debug(version)
+    #logger.debug(version)
     return version
 
 def download_file(url: str):
     response = requests.get(url, stream=True)
     temp_file = tempfile.TemporaryFile()
     for chunk in response.iter_content(chunk_size=128):
         temp_file.write(chunk)
```

## attacus/flutter_config.py

```diff
@@ -5,9 +5,10 @@
 
 from . import attacus as core
 from .artifacts import get_icu_data_path
 
 class FlutterConfig(core.FlutterConfig):
     def __init__(self) -> None:
         super().__init__()
+        self.assets_path = str(Path.cwd() / 'flutter_assets')
         self.icu_data_path = str(get_icu_data_path())
-        logger.debug(self.icu_data_path)
+        #logger.debug(self.icu_data_path)
```

## Comparing `attacus-0.1.1.dist-info/LICENSE` & `attacus-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `attacus-0.1.1.dist-info/METADATA` & `attacus-0.1.2.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attacus
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Flutter Extension
 Author-email: Kurtis Fields <kurtisfields@gmail.com>
 License: MIT License        
         Copyright (c) 2023 Kurtis Fields        
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -31,109 +31,75 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: loguru (==0.7.0)
-Requires-Dist: platformdirs (==3.5.1)
-Requires-Dist: requests (==2.31.0)
+Requires-Dist: loguru (~=0.7.0)
+Requires-Dist: platformdirs (~=3.5.1)
+Requires-Dist: requests (~=2.31.0)
+Requires-Dist: rich (~=13.3.5)
 Provides-Extra: dev
 Requires-Dist: black (~=22.12.0) ; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest (~=7.2.1) ; extra == 'test'
 
-# Attacus :butterfly: :snake:
+# Attacus :snake: :butterfly:
 
-Flutter SDL Python
+Flutter Python Extension
 
 [Flutter](https://flutter.dev/)
 
+[Flutter Embedder](https://github.com/flutter/flutter/wiki/Custom-Flutter-Engine-Embedders)
+
 [SDL](https://github.com/libsdl-org/SDL/)
 
-## Required
+## Development
+
+### Required
 
 * [Hatch](https://hatch.pypa.io/)
 
-## Optional
+### Optional
 
 * [Ninja](https://ninja-build.org/)
 
-## Clone
+### Clone
 
 ```bash
 git clone https://github.com/crungelab/attacus
 cd attacus
 ```
 
-## Extra Steps
-
-You need to download the Flutter engine binaries from: [Custom-Flutter-Engine-Embedders](https://github.com/flutter/flutter/wiki/Custom-Flutter-Engine-Embedders)
-
-Extract to: [project-root]/binaries/flutter
-
-# Development
-
-## Tool Chain
+### Tool Chain
 
 [cxbuild](https://github.com/crungelab/cxbuild)
 
 [pybind11](https://github.com/pybind/pybind11)
 
-## Develop
+### Develop
 ```bash
 hatch shell
 procure
 cxbuild develop
 ```
 
-### Release
+### Build
 ```bash
 cxbuild
 ```
 
-## Quick Start
-```bash
-git clone --recursive https://github.com/kfields/attacus
-cd attacus
-mkdir build
-cd build
-cmake ..
-```
-### Or
-```bash
-mkdir build-debug
-cd build-debug
-cmake -DCMAKE_BUILD_TYPE=Debug ..
-```
-## Wayland
-```bash
-sudo apt install libwayland-dev
-sudo apt install libxkbcommon-dev
-sudo add-apt-repository ppa:christianrauch/libdecoration
-
-cmake -DATT_WM_WAYLAND=ON -DCMAKE_BUILD_TYPE=Debug ..
-```
-
-## Glad
-    v1
-    glad --generator c --no-loader --out-path src
-    
-    v2
-    glad --api gl:core --out-path src/glad c
-
-
-## [Flutter Custom Devices](https://github.com/flutter/flutter/wiki/Using-custom-embedders-with-the-Flutter-CLI)
+### [Flutter Custom Devices](https://github.com/flutter/flutter/wiki/Using-custom-embedders-with-the-Flutter-CLI)
+This will enable and display the location of your .flutter_custom_devices.json file
 ```
-flutter channel master
 flutter config --enable-custom-devices
 flutter custom-devices
 ```
-C:\Users\kurti\AppData\Roaming\.flutter_custom_devices.json
+Add this to your .flutter_custom_devices.json file
 
 ``` json
     {
       "id": "attacus",
       "label": "Attacus",
       "sdkNameAndVersion": "Attacus 0.1",
       "platform": null,
@@ -143,50 +109,41 @@
         "-n",
         "1",
         "-w",
         "500",
         "localhost"
       ],
       "pingSuccessRegex": "[<=]\\d+ms",
-      "postBuild": null,
+      "postBuild": [
+        "python",
+        "-m",
+        "attacus.post_build"
+      ],
       "install": [
         "python",
-        "--version"
+        "-m",
+        "attacus.install"
       ],
       "uninstall": [
         "python",
-        "--version"
+        "-m",
+        "attacus.uninstall"
       ],
       "runDebug": [
         "python",
         "main.py"
       ],
       "forwardPort": null,
       "forwardPortSuccessRegex": null,
       "screenshot": null
     }
 ```
 
-## [Flutter Embedder](https://github.com/flutter/flutter/wiki/Custom-Flutter-Engine-Embedders)
-Get the SHA of the Flutter engine you wish to use
-```bash
-cd flutter/bin/internal
-cat engine.version
-```
-
-## Flutter Examples
+## Examples
 ```bash
 flutter build bundle
 python main.py
 ```
 or
 ```bash
 flutter run
 ```
-
-
-## icudtl.dat
-```
-flutter\bin\cache\artifacts\engine\windows-x64\icudtl.dat
-```
-I'm manually copying this into the build directory.  Not good.
-It needs to be copied over automatically
```

## Comparing `attacus-0.1.1.dist-info/RECORD` & `attacus-0.1.2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 attacus/__about__.py,sha256=ryAfvAaW7VM8g1gnCrFCPrXmcbbm99Xw44aLkwGZzaI,23
 attacus/__init__.py,sha256=aJCUEMMOC7CoN0HXU20S5egMwzY1teojhDwcDsSWfCU,165
 attacus/app.py,sha256=qdfUm8sRao1JsrGJplAVsa5xVeqco2LRQO0PzbBuFHU,189
-attacus/artifacts.py,sha256=EuYkYmytD5ol7KPYiUUoWS5nN7iQv-Zjm8HUzJ0bnkQ,2395
-attacus/attacus.pyd,sha256=Nh2i7mj56vWCv9SA68CNMhTG47XenHGqYxT2zNbuvtc,2275328
+attacus/artifacts.py,sha256=dCXrBem4m1bPxTJV5wxqb9IGkipZFzM80RZ_iW38yIc,2398
+attacus/attacus.pyd,sha256=MJznWxvk9ULuLhpxsAt5GBVdmoKkomOnupgtggW3UmA,2275328
+attacus/build.py,sha256=Zdre-h0ZqCdSrWOTsY6V44Jnam7FG5RKaw4L_EpKJMw,412
 attacus/ensure.py,sha256=ZvRjcirqcu6us-WqDGTWqY314_j31xsb4K-5_P3c0iM,1650
-attacus/flutter_config.py,sha256=0ERLbiaKTHwliVQAxdoNRY_-YnzeAjlhPU4cxIc-wQs,365
+attacus/flutter_config.py,sha256=FStJTXK27hzwSOsp23VMW0K0R9xS_Aw2-5Jwdmad-Os,429
 attacus/flutter_view.py,sha256=lFA-0N8qlBcyogR_aHvVUETf_F6YBIboYSW5b8UXBQU,355
-attacus-0.1.1.dist-info/LICENSE,sha256=_66BWzWzllOL6nPR0Jn9JDr5IFHvfOCeTUBcY-IAOR8,1091
-attacus-0.1.1.dist-info/METADATA,sha256=23E1qx_hWE3_tYbohIbsWhA2X6jUt3fruAgl8b_Vc6M,5082
-attacus-0.1.1.dist-info/WHEEL,sha256=W26pYN7HLsBT1jrDSL9udgf_mdNKJmYmL23sIP-FcgM,102
-attacus-0.1.1.dist-info/top_level.txt,sha256=MzO2IQ9x5yLfi1noaf99pmzxRu3h7OczbuZKytaFjUI,8
-attacus-0.1.1.dist-info/RECORD,,
+attacus/install.py,sha256=vAL4dBvUdakLQ1g2M6I1PtRG6be7_ZCQXESiPbHXa94,480
+attacus/post_build.py,sha256=1i6lDdxRBdQ5mh00s_AXX88d94Z2wGDOzTK9uDF05zA,372
+attacus/uninstall.py,sha256=lSIo76H7g5Bb33Nva8nIzua-yqhXAwpQEa_kG3-dI_4,186
+attacus-0.1.2.dist-info/LICENSE,sha256=_66BWzWzllOL6nPR0Jn9JDr5IFHvfOCeTUBcY-IAOR8,1091
+attacus-0.1.2.dist-info/METADATA,sha256=bveMAyYXN5lC4ogJDvWMVcvUGlsmnHusd8PHsQtu3wE,4221
+attacus-0.1.2.dist-info/WHEEL,sha256=W26pYN7HLsBT1jrDSL9udgf_mdNKJmYmL23sIP-FcgM,102
+attacus-0.1.2.dist-info/top_level.txt,sha256=MzO2IQ9x5yLfi1noaf99pmzxRu3h7OczbuZKytaFjUI,8
+attacus-0.1.2.dist-info/RECORD,,
```

