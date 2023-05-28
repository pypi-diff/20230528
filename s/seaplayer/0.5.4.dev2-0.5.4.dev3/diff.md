# Comparing `tmp/seaplayer-0.5.4.dev2.tar.gz` & `tmp/seaplayer-0.5.4.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaplayer-0.5.4.dev2.tar", max compression
+gzip compressed data, was "seaplayer-0.5.4.dev3.tar", max compression
```

## Comparing `seaplayer-0.5.4.dev2.tar` & `seaplayer-0.5.4.dev3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1085 2023-05-23 03:20:59.344210 seaplayer-0.5.4.dev2/LICENSE
--rw-r--r--   0        0        0     1652 2023-05-27 12:20:18.053841 seaplayer-0.5.4.dev2/pyproject.toml
--rw-r--r--   0        0        0     1336 2023-05-23 03:20:59.345209 seaplayer-0.5.4.dev2/README.md
--rw-r--r--   0        0        0        0 2023-05-23 03:20:59.348294 seaplayer-0.5.4.dev2/seaplayer/__init__.py
--rw-r--r--   0        0        0      347 2023-05-23 03:20:59.348294 seaplayer-0.5.4.dev2/seaplayer/__main__.py
--rw-r--r--   0        0        0    14705 2023-05-23 03:20:59.348294 seaplayer-0.5.4.dev2/seaplayer/assets/image-not-found.png
--rw-r--r--   0        0        0      264 2023-05-25 07:17:50.820137 seaplayer-0.5.4.dev2/seaplayer/codecs/__init__.py
--rw-r--r--   0        0        0     2486 2023-05-25 07:17:50.819139 seaplayer-0.5.4.dev2/seaplayer/codecs/Any.py
--rw-r--r--   0        0        0      477 2023-05-23 03:20:59.349294 seaplayer-0.5.4.dev2/seaplayer/codecs/FLAC.py
--rw-r--r--   0        0        0     2946 2023-05-25 07:17:50.819139 seaplayer-0.5.4.dev2/seaplayer/codecs/MIDI.py
--rw-r--r--   0        0        0      473 2023-05-23 03:20:59.349294 seaplayer-0.5.4.dev2/seaplayer/codecs/MP3.py
--rw-r--r--   0        0        0      475 2023-05-23 03:20:59.349294 seaplayer-0.5.4.dev2/seaplayer/codecs/OGG.py
--rw-r--r--   0        0        0      593 2023-05-23 03:20:59.349294 seaplayer-0.5.4.dev2/seaplayer/codecs/WAV.py
--rw-r--r--   0        0        0     1924 2023-05-23 03:20:59.350294 seaplayer-0.5.4.dev2/seaplayer/codeсbase.py
--rw-r--r--   0        0        0     6188 2023-05-25 07:17:50.820137 seaplayer-0.5.4.dev2/seaplayer/config.py
--rw-r--r--   0        0        0        0 2023-05-23 03:20:59.350294 seaplayer-0.5.4.dev2/seaplayer/css/configurate.css
--rw-r--r--   0        0        0     1585 2023-05-23 03:20:59.351294 seaplayer-0.5.4.dev2/seaplayer/css/objects.css
--rw-r--r--   0        0        0      595 2023-05-23 03:20:59.351294 seaplayer-0.5.4.dev2/seaplayer/css/seaplayer.css
--rw-r--r--   0        0        0      278 2023-05-23 03:20:59.351294 seaplayer-0.5.4.dev2/seaplayer/css/unknown.css
--rw-r--r--   0        0        0      382 2023-05-23 03:20:59.351294 seaplayer-0.5.4.dev2/seaplayer/exceptions.py
--rw-r--r--   0        0        0     1413 2023-05-23 03:20:59.353307 seaplayer-0.5.4.dev2/seaplayer/functions.py
--rw-r--r--   0        0        0        0 2023-05-23 03:20:59.353307 seaplayer-0.5.4.dev2/seaplayer/modules/__init__.py
--rw-r--r--   0        0        0     2036 2023-05-23 03:20:59.354294 seaplayer-0.5.4.dev2/seaplayer/modules/colorizer.py
--rw-r--r--   0        0        0      376 2023-05-25 17:39:02.081110 seaplayer-0.5.4.dev2/seaplayer/objects/__init__.py
--rw-r--r--   0        0        0     1052 2023-05-25 07:17:50.820137 seaplayer-0.5.4.dev2/seaplayer/objects/Configurate.py
--rw-r--r--   0        0        0     1421 2023-05-25 17:39:02.081110 seaplayer-0.5.4.dev2/seaplayer/objects/DataOptions.py
--rw-r--r--   0        0        0     3006 2023-05-23 03:20:59.354294 seaplayer-0.5.4.dev2/seaplayer/objects/Image.py
--rw-r--r--   0        0        0     1126 2023-05-23 03:20:59.354294 seaplayer-0.5.4.dev2/seaplayer/objects/Input.py
--rw-r--r--   0        0        0     1287 2023-05-26 21:36:55.785380 seaplayer-0.5.4.dev2/seaplayer/objects/Log.py
--rw-r--r--   0        0        0     5562 2023-05-27 11:40:26.374121 seaplayer-0.5.4.dev2/seaplayer/objects/MusicList.py
--rw-r--r--   0        0        0      787 2023-05-23 03:20:59.355309 seaplayer-0.5.4.dev2/seaplayer/objects/Notification.py
--rw-r--r--   0        0        0     1269 2023-05-23 03:20:59.355309 seaplayer-0.5.4.dev2/seaplayer/objects/ProgressBar.py
--rw-r--r--   0        0        0       86 2023-05-23 03:20:59.355309 seaplayer-0.5.4.dev2/seaplayer/plug/__init__.py
--rw-r--r--   0        0        0      123 2023-05-26 18:16:55.016730 seaplayer-0.5.4.dev2/seaplayer/plug/__main__.py
--rw-r--r--   0        0        0       21 2023-05-26 19:51:28.701684 seaplayer-0.5.4.dev2/seaplayer/plug/cli/__init__.py
--rw-r--r--   0        0        0     5259 2023-05-27 12:11:55.197047 seaplayer-0.5.4.dev2/seaplayer/plug/cli/cli.py
--rw-r--r--   0        0        0      582 2023-05-26 20:10:17.518991 seaplayer-0.5.4.dev2/seaplayer/plug/cli/exceptions.py
--rw-r--r--   0        0        0     1937 2023-05-26 18:16:55.018728 seaplayer-0.5.4.dev2/seaplayer/plug/cli/functions.py
--rw-r--r--   0        0        0      133 2023-05-26 19:55:28.316980 seaplayer-0.5.4.dev2/seaplayer/plug/cli/vars.py
--rw-r--r--   0        0        0      817 2023-05-26 22:40:27.692911 seaplayer-0.5.4.dev2/seaplayer/plug/pluginbase.py
--rw-r--r--   0        0        0      759 2023-05-26 18:16:55.019724 seaplayer-0.5.4.dev2/seaplayer/plug/pluginbase.pyi
--rw-r--r--   0        0        0     8688 2023-05-26 22:50:40.897429 seaplayer-0.5.4.dev2/seaplayer/plug/pluginloader.py
--rw-r--r--   0        0        0     2692 2023-05-26 18:16:55.020726 seaplayer-0.5.4.dev2/seaplayer/plug/pluginloader.pyi
--rw-r--r--   0        0        0       84 2023-05-23 03:20:59.356797 seaplayer-0.5.4.dev2/seaplayer/screens/__init__.py
--rw-r--r--   0        0        0     8542 2023-05-25 17:39:02.083097 seaplayer-0.5.4.dev2/seaplayer/screens/Configurate.py
--rw-r--r--   0        0        0     1002 2023-05-23 03:20:59.356797 seaplayer-0.5.4.dev2/seaplayer/screens/Unknown.py
--rw-r--r--   0        0        0    19765 2023-05-27 12:08:26.337289 seaplayer-0.5.4.dev2/seaplayer/seaplayer.py
--rw-r--r--   0        0        0       91 2023-05-27 09:37:18.022755 seaplayer-0.5.4.dev2/seaplayer/types/__init__.py
--rw-r--r--   0        0        0     1576 2023-05-27 12:03:27.045912 seaplayer-0.5.4.dev2/seaplayer/types/Cache.py
--rw-r--r--   0        0        0     2624 2023-05-23 03:20:59.357805 seaplayer-0.5.4.dev2/seaplayer/types/Convert.py
--rw-r--r--   0        0        0     1589 2023-05-23 03:20:59.357805 seaplayer-0.5.4.dev2/seaplayer/types/MusicList.py
--rw-r--r--   0        0        0     1525 2023-05-27 12:13:15.760303 seaplayer-0.5.4.dev2/seaplayer/units.py
--rw-r--r--   0        0        0     2836 1970-01-01 00:00:00.000000 seaplayer-0.5.4.dev2/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-05-23 03:20:59.344210 seaplayer-0.5.4.dev3/LICENSE
+-rw-r--r--   0        0        0     1652 2023-05-27 17:07:14.285094 seaplayer-0.5.4.dev3/pyproject.toml
+-rw-r--r--   0        0        0     1336 2023-05-23 03:20:59.345209 seaplayer-0.5.4.dev3/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 03:20:59.348294 seaplayer-0.5.4.dev3/seaplayer/__init__.py
+-rw-r--r--   0        0        0      347 2023-05-23 03:20:59.348294 seaplayer-0.5.4.dev3/seaplayer/__main__.py
+-rw-r--r--   0        0        0    14705 2023-05-23 03:20:59.348294 seaplayer-0.5.4.dev3/seaplayer/assets/image-not-found.png
+-rw-r--r--   0        0        0      264 2023-05-25 07:17:50.820137 seaplayer-0.5.4.dev3/seaplayer/codecs/__init__.py
+-rw-r--r--   0        0        0     2486 2023-05-25 07:17:50.819139 seaplayer-0.5.4.dev3/seaplayer/codecs/Any.py
+-rw-r--r--   0        0        0      477 2023-05-23 03:20:59.349294 seaplayer-0.5.4.dev3/seaplayer/codecs/FLAC.py
+-rw-r--r--   0        0        0     2946 2023-05-25 07:17:50.819139 seaplayer-0.5.4.dev3/seaplayer/codecs/MIDI.py
+-rw-r--r--   0        0        0      473 2023-05-23 03:20:59.349294 seaplayer-0.5.4.dev3/seaplayer/codecs/MP3.py
+-rw-r--r--   0        0        0      475 2023-05-23 03:20:59.349294 seaplayer-0.5.4.dev3/seaplayer/codecs/OGG.py
+-rw-r--r--   0        0        0      593 2023-05-23 03:20:59.349294 seaplayer-0.5.4.dev3/seaplayer/codecs/WAV.py
+-rw-r--r--   0        0        0     1924 2023-05-23 03:20:59.350294 seaplayer-0.5.4.dev3/seaplayer/codeсbase.py
+-rw-r--r--   0        0        0     6188 2023-05-27 18:01:34.042639 seaplayer-0.5.4.dev3/seaplayer/config.py
+-rw-r--r--   0        0        0        0 2023-05-23 03:20:59.350294 seaplayer-0.5.4.dev3/seaplayer/css/configurate.css
+-rw-r--r--   0        0        0     1585 2023-05-23 03:20:59.351294 seaplayer-0.5.4.dev3/seaplayer/css/objects.css
+-rw-r--r--   0        0        0      595 2023-05-23 03:20:59.351294 seaplayer-0.5.4.dev3/seaplayer/css/seaplayer.css
+-rw-r--r--   0        0        0      278 2023-05-23 03:20:59.351294 seaplayer-0.5.4.dev3/seaplayer/css/unknown.css
+-rw-r--r--   0        0        0      382 2023-05-23 03:20:59.351294 seaplayer-0.5.4.dev3/seaplayer/exceptions.py
+-rw-r--r--   0        0        0     1413 2023-05-23 03:20:59.353307 seaplayer-0.5.4.dev3/seaplayer/functions.py
+-rw-r--r--   0        0        0        0 2023-05-23 03:20:59.353307 seaplayer-0.5.4.dev3/seaplayer/modules/__init__.py
+-rw-r--r--   0        0        0     2128 2023-05-27 17:36:06.594476 seaplayer-0.5.4.dev3/seaplayer/modules/colorizer.py
+-rw-r--r--   0        0        0      376 2023-05-25 17:39:02.081110 seaplayer-0.5.4.dev3/seaplayer/objects/__init__.py
+-rw-r--r--   0        0        0     1052 2023-05-25 07:17:50.820137 seaplayer-0.5.4.dev3/seaplayer/objects/Configurate.py
+-rw-r--r--   0        0        0     1421 2023-05-25 17:39:02.081110 seaplayer-0.5.4.dev3/seaplayer/objects/DataOptions.py
+-rw-r--r--   0        0        0     3006 2023-05-23 03:20:59.354294 seaplayer-0.5.4.dev3/seaplayer/objects/Image.py
+-rw-r--r--   0        0        0     1126 2023-05-23 03:20:59.354294 seaplayer-0.5.4.dev3/seaplayer/objects/Input.py
+-rw-r--r--   0        0        0     1287 2023-05-26 21:36:55.785380 seaplayer-0.5.4.dev3/seaplayer/objects/Log.py
+-rw-r--r--   0        0        0     5701 2023-05-27 17:49:37.836036 seaplayer-0.5.4.dev3/seaplayer/objects/MusicList.py
+-rw-r--r--   0        0        0      787 2023-05-23 03:20:59.355309 seaplayer-0.5.4.dev3/seaplayer/objects/Notification.py
+-rw-r--r--   0        0        0     1269 2023-05-23 03:20:59.355309 seaplayer-0.5.4.dev3/seaplayer/objects/ProgressBar.py
+-rw-r--r--   0        0        0       86 2023-05-23 03:20:59.355309 seaplayer-0.5.4.dev3/seaplayer/plug/__init__.py
+-rw-r--r--   0        0        0      123 2023-05-26 18:16:55.016730 seaplayer-0.5.4.dev3/seaplayer/plug/__main__.py
+-rw-r--r--   0        0        0       21 2023-05-26 19:51:28.701684 seaplayer-0.5.4.dev3/seaplayer/plug/cli/__init__.py
+-rw-r--r--   0        0        0     5259 2023-05-27 12:11:55.197047 seaplayer-0.5.4.dev3/seaplayer/plug/cli/cli.py
+-rw-r--r--   0        0        0      582 2023-05-26 20:10:17.518991 seaplayer-0.5.4.dev3/seaplayer/plug/cli/exceptions.py
+-rw-r--r--   0        0        0     1937 2023-05-26 18:16:55.018728 seaplayer-0.5.4.dev3/seaplayer/plug/cli/functions.py
+-rw-r--r--   0        0        0      133 2023-05-26 19:55:28.316980 seaplayer-0.5.4.dev3/seaplayer/plug/cli/vars.py
+-rw-r--r--   0        0        0      817 2023-05-26 22:40:27.692911 seaplayer-0.5.4.dev3/seaplayer/plug/pluginbase.py
+-rw-r--r--   0        0        0      759 2023-05-26 18:16:55.019724 seaplayer-0.5.4.dev3/seaplayer/plug/pluginbase.pyi
+-rw-r--r--   0        0        0     8688 2023-05-26 22:50:40.897429 seaplayer-0.5.4.dev3/seaplayer/plug/pluginloader.py
+-rw-r--r--   0        0        0     2692 2023-05-26 18:16:55.020726 seaplayer-0.5.4.dev3/seaplayer/plug/pluginloader.pyi
+-rw-r--r--   0        0        0       84 2023-05-23 03:20:59.356797 seaplayer-0.5.4.dev3/seaplayer/screens/__init__.py
+-rw-r--r--   0        0        0     8542 2023-05-25 17:39:02.083097 seaplayer-0.5.4.dev3/seaplayer/screens/Configurate.py
+-rw-r--r--   0        0        0     1002 2023-05-23 03:20:59.356797 seaplayer-0.5.4.dev3/seaplayer/screens/Unknown.py
+-rw-r--r--   0        0        0    20323 2023-05-27 19:52:25.382634 seaplayer-0.5.4.dev3/seaplayer/seaplayer.py
+-rw-r--r--   0        0        0       91 2023-05-27 09:37:18.022755 seaplayer-0.5.4.dev3/seaplayer/types/__init__.py
+-rw-r--r--   0        0        0     1576 2023-05-27 12:03:27.045912 seaplayer-0.5.4.dev3/seaplayer/types/Cache.py
+-rw-r--r--   0        0        0     2624 2023-05-23 03:20:59.357805 seaplayer-0.5.4.dev3/seaplayer/types/Convert.py
+-rw-r--r--   0        0        0     1589 2023-05-23 03:20:59.357805 seaplayer-0.5.4.dev3/seaplayer/types/MusicList.py
+-rw-r--r--   0        0        0     1525 2023-05-27 17:07:22.141538 seaplayer-0.5.4.dev3/seaplayer/units.py
+-rw-r--r--   0        0        0     2836 1970-01-01 00:00:00.000000 seaplayer-0.5.4.dev3/PKG-INFO
```

### Comparing `seaplayer-0.5.4.dev2/LICENSE` & `seaplayer-0.5.4.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/pyproject.toml` & `seaplayer-0.5.4.dev3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SeaPlayer"
-version = "0.5.4.dev2"
+version = "0.5.4.dev3"
 description = "SeaPlayer is a player that works in the terminal."
 repository = "https://github.com/romanin-rf/SeaPlayer"
 authors = ["Romanin <semina054@gmail.com>"]
 keywords = ["tui", "player", "seaplayer", "wav", "mp3", "ogg", "midi"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
```

### Comparing `seaplayer-0.5.4.dev2/README.md` & `seaplayer-0.5.4.dev3/README.md`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/seaplayer/assets/image-not-found.png` & `seaplayer-0.5.4.dev3/seaplayer/assets/image-not-found.png`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/seaplayer/codecs/Any.py` & `seaplayer-0.5.4.dev3/seaplayer/codecs/Any.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/seaplayer/codecs/MIDI.py` & `seaplayer-0.5.4.dev3/seaplayer/codecs/MIDI.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/seaplayer/codecs/WAV.py` & `seaplayer-0.5.4.dev3/seaplayer/codecs/WAV.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/seaplayer/codeсbase.py` & `seaplayer-0.5.4.dev3/seaplayer/codeсbase.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/seaplayer/config.py` & `seaplayer-0.5.4.dev3/seaplayer/config.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/seaplayer/css/objects.css` & `seaplayer-0.5.4.dev3/seaplayer/css/objects.css`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/seaplayer/css/seaplayer.css` & `seaplayer-0.5.4.dev3/seaplayer/css/seaplayer.css`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/seaplayer/functions.py` & `seaplayer-0.5.4.dev3/seaplayer/functions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/seaplayer/modules/colorizer.py` & `seaplayer-0.5.4.dev3/seaplayer/modules/colorizer.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,48 +6,48 @@
     is_tuple_type,
     get_args,
     get_origin
 )
 
 # ! Vars
 REPLACE_TYPES = {
-    "str": "[green]str[/]",
-    "bool": "[green]bool[/]",
-    "int": "[green]int[/]",
-    "float": "[green]float[/]",
-    "bytes": "[green]bytes[/]",
-    "bytearray": "[green]bytearray[/]",
-    "complex": "[green]complex[/]",
-    "list": "[green]list[/]",
-    "tuple": "[green]tuple[/]",
-    "dict": "[green]dict[/]",
-    "None": "[cyan]None[/]",
-    "Tuple": "[green]Tuple[/]",
-    "Dict": "[green]Dict[/]",
-    "List": "[green]List[/]",
-    "Any": "[white]Any[/]",
-    "Literal": "[green]Literal[/]",
+    "str": "[green]str[/green]",
+    "bool": "[green]bool[/green]",
+    "int": "[green]int[/green]",
+    "float": "[green]float[/green]",
+    "bytes": "[green]bytes[/green]",
+    "bytearray": "[green]bytearray[/green]",
+    "complex": "[green]complex[/green]",
+    "list": "[green]list[/green]",
+    "tuple": "[green]tuple[/green]",
+    "dict": "[green]dict[/green]",
+    "None": "[cyan]None[/cyan]",
+    "Tuple": "[green]Tuple[/green]",
+    "Dict": "[green]Dict[/green]",
+    "List": "[green]List[/green]",
+    "Any": "[white]Any[/white]",
+    "Literal": "[green]Literal[/green]",
     "['": "[[yellow]'",
     ", '": ", [yellow]'",
-    "']": "'[/]]",
-    "', ": "'[/], "
+    "']": "'[/yellow]]",
+    "', ": "'[/yellow], "
 }
 
 # ! Other Functions
 def is_list_type(tp) -> bool: return get_origin(tp) == list
 def is_dict_type(tp) -> bool: return get_origin(tp) == dict
 def replaces(string: str, replacement: Dict[str, str]) -> str:
     for _old, _new in replacement.items(): string = string.replace(_old, _new)
     return string
 
 # ! Functions
 def pullyper(tp: type) -> str:
     if tp is None: return "None"
     elif is_optional_type(tp):
-       return f"{pullyper(get_args(tp)[0])} | None"
+        return f"{pullyper(get_args(tp)[0])} | None"
     elif is_union_type(tp):
         return " | ".join(pullyper(arg) for arg in get_args(tp))
     elif is_literal_type(tp):
         return f"Literal[{', '.join(repr(arg) for arg in get_args(tp))}]"
     elif is_tuple_type(tp):
         if len(args:=get_args(tp)) > 0: return f"Tuple[{', '.join(pullyper(arg) for arg in args)}]"
         return "Tuple"
```

### Comparing `seaplayer-0.5.4.dev2/seaplayer/objects/Configurate.py` & `seaplayer-0.5.4.dev3/seaplayer/objects/Configurate.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/seaplayer/objects/DataOptions.py` & `seaplayer-0.5.4.dev3/seaplayer/objects/DataOptions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/seaplayer/objects/Image.py` & `seaplayer-0.5.4.dev3/seaplayer/objects/Image.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/seaplayer/objects/Input.py` & `seaplayer-0.5.4.dev3/seaplayer/objects/Input.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/seaplayer/objects/Log.py` & `seaplayer-0.5.4.dev3/seaplayer/objects/Log.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/seaplayer/objects/MusicList.py` & `seaplayer-0.5.4.dev3/seaplayer/objects/MusicList.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,19 @@
                 ),
                 sound.name,
                 sound_uuid
             )
         )
         return sound_uuid
     
-    def get_sound(self, sound_uuid: str) -> Optional[CodecBase]: return self.music_list.get(sound_uuid)
+    def get_sound(self, sound_uuid: str) -> Optional[CodecBase]:
+        return self.music_list.get(sound_uuid)
+    
+    async def aio_get_sound(self, sound_uuid: str) -> Optional[CodecBase]:
+        return self.music_list.get(sound_uuid)
     
     async def aio_add_sound(self, sound: CodecBase):
         sound_uuid = await self.music_list.aio_add(sound)
         await self.append(
             MusicListViewItem(
                 f"{get_sound_basename(sound)}",
                 "{duration} sec, {channel_mode}, {samplerate} Hz, {bitrate} kbps, {codec_name}".format(
```

### Comparing `seaplayer-0.5.4.dev2/seaplayer/objects/Notification.py` & `seaplayer-0.5.4.dev3/seaplayer/objects/Notification.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/seaplayer/objects/ProgressBar.py` & `seaplayer-0.5.4.dev3/seaplayer/objects/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/seaplayer/plug/cli/cli.py` & `seaplayer-0.5.4.dev3/seaplayer/plug/cli/cli.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/seaplayer/plug/cli/exceptions.py` & `seaplayer-0.5.4.dev3/seaplayer/plug/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/seaplayer/plug/cli/functions.py` & `seaplayer-0.5.4.dev3/seaplayer/plug/cli/functions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/seaplayer/plug/pluginbase.py` & `seaplayer-0.5.4.dev3/seaplayer/plug/pluginbase.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/seaplayer/plug/pluginbase.pyi` & `seaplayer-0.5.4.dev3/seaplayer/plug/pluginbase.pyi`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/seaplayer/plug/pluginloader.py` & `seaplayer-0.5.4.dev3/seaplayer/plug/pluginloader.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/seaplayer/plug/pluginloader.pyi` & `seaplayer-0.5.4.dev3/seaplayer/plug/pluginloader.pyi`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/seaplayer/screens/Configurate.py` & `seaplayer-0.5.4.dev3/seaplayer/screens/Configurate.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/seaplayer/screens/Unknown.py` & `seaplayer-0.5.4.dev3/seaplayer/screens/Unknown.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/seaplayer/seaplayer.py` & `seaplayer-0.5.4.dev3/seaplayer/seaplayer.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,15 +103,18 @@
     CODECS: List[Type[CodecBase]] = [ *codecs ]
     CODECS_KWARGS: Dict[str, Any] = {
         "sound_fonts_path": config.sound_font_path,
         "sound_device_id": config.output_sound_device_id
     }
     
     # ! Init Objects
-    log_menu = LogMenu(enable_logging=config.log_menu_enable, wrap=True, highlight=True, markup=True)
+    log_menu = LogMenu(
+        enable_logging=config.log_menu_enable,
+        wrap=True, highlight=True, markup=True
+    )
     
     # ! Log Functions
     info = log_menu.info
     error = log_menu.error
     warn = log_menu.warn
     exception = log_menu.exception
 
@@ -176,42 +179,54 @@
     async def get_sound_seek(self) -> Tuple[str, Optional[float], Optional[float]]:
         if (sound:=await self.aio_gcs()) is not None:
             pos = sound.get_pos()
             minutes, seconds = round(pos // 60), round(pos % 60)
             return f"{minutes}:{str(seconds).rjust(2,'0')} | {str(round(sound.get_volume()*100)).rjust(3)}%", pos, sound.duration
         return "0:00 |   0%", None, None
     
-    def get_sound_selected_label_text(self) -> str:
-        if (sound:=self.gcs()) is not None:
+    def get_sound_selected_label_text(self, sound: Optional[CodecBase]=None) -> str:
+        if sound is None:
+            sound = self.gcs()
+        if sound is not None:
             return f"({check_status(sound)}): {get_sound_basename(sound)}"
         return "<sound not selected>"
     
-    async def aio_get_sound_selected_label_text(self) -> str:
-        if (sound:=await self.aio_gcs()) is not None:
+    async def aio_get_sound_selected_label_text(self, sound: Optional[CodecBase]=None) -> str:
+        if sound is None:
+            sound = await self.aio_gcs()
+        if sound is not None:
             return f"({check_status(sound)}): {get_sound_basename(sound)}"
         return "<sound not selected>"
     
+    def update_select_label(self, sound: Optional[CodecBase]=None) -> None:
+        self.music_selected_label.update(self.get_sound_selected_label_text(sound))
+    
+    async def aio_update_select_label(self, sound: Optional[CodecBase]=None) -> None:
+        self.music_selected_label.update(await self.aio_get_sound_selected_label_text(sound))
+    
     def gpms(self, modes: Tuple[str, str, str]=("(MODE): PLAY", "(MODE): REPLAY SOUND", "(MODE): REPLAY LIST")) -> str: return modes[self.playback_mode]
     def switch_playback_mode(self) -> None:
         if self.playback_mode == 2: self.playback_mode = 0
         else: self.playback_mode += 1
     
     async def update_loop_playback(self) -> None:
         while self.started:
             if (sound:=await self.aio_gcs()) is not None:
                 status = check_status(sound)
                 if (self.last_playback_status is not None) and (self.last_playback_status != status):
-                    self.music_selected_label.update(await self.aio_get_sound_selected_label_text())
+                    await self.aio_update_select_label(sound)
                 
                 if (status == "Stoped") and (self.last_playback_status == "Playing"):
                     if self.playback_mode == 1:
                         sound.play()
                         self.info(f"Replay sound: {repr(sound)}")
                     elif self.playback_mode == 2:
-                        if (sound:=await self.set_sound_for_playback(sound_uuid:=await self.music_list_view.aio_get_next_sound_uuid(self.currect_sound_uuid), True)) is not None:
+                        sound_uuid = await self.music_list_view.aio_get_next_sound_uuid(self.currect_sound_uuid)
+                        sound = await self.set_sound_for_playback(sound_uuid, True)
+                        if sound is not None:
                             self.playback_mode_blocked = True
                             await self.music_list_view.aio_select_list_item_from_sound_uuid(sound_uuid)
                             sound.play()
                             self.info(f"Playing the next sound: {repr(sound)}")
                 
                 self.last_playback_status = status
             await asyncio.sleep(0.2)
@@ -222,16 +237,14 @@
         self.info(f"{__title__} v{__version__} from {__author__} ({__email__})")
         self.info(f"Source          : {__url__}")
         self.info(f"Codecs          : {repr(self.CODECS)}")
         self.info(f"Config Path     : {repr(self.config.filepath)}")
         self.info(f"CSS Dirpath     : {repr(CSS_LOCALDIR)}")
         self.info(f"Assets Dirpath  : {repr(ASSETS_DIRPATH)}")
         self.info(f"Codecs Kwargs   : {repr(self.CODECS_KWARGS)}")
-        self.info(f"Sound Device ID : {repr(self.config.output_sound_device_id)}")
-        
         
         # * Play Screen
         self.music_play_screen = Static(classes="screen-box")
         self.music_play_screen.border_title = "Player"
         
         # * Image Object Init
         self.music_selected_label = Label(self.get_sound_selected_label_text(), classes="music-selected-label")
@@ -258,17 +271,17 @@
             with Vertical():
                 with Static(classes="player-visual-panel"):
                     yield self.music_image
                 with Static(classes="player-contol-panel"):
                     yield self.music_selected_label
                     yield IndeterminateProgress(getfunc=self.get_sound_seek)
                     with Horizontal(classes="box-buttons-sound-control"):
-                        yield Button("Play/Stop", id="button-play-stop", variant="warning", classes="button-sound-control")
+                        yield Button("Pause", id="button-pause", variant="success", classes="button-sound-control")
                         yield Static(classes="pass-one-width")
-                        yield Button("Pause/Unpause", id="button-pause-unpause", variant="success", classes="button-sound-control")
+                        yield Button("Play/Stop/Unpause", id="button-play-stop", variant="warning", classes="button-sound-control")
                         yield Static(classes="pass-one-width")
                         yield Button(self.gpms(), id="switch-playback-mode", variant="primary", classes="button-sound-control")
         with self.music_list_screen:
             yield self.music_list_view
             yield self.music_list_add_input
         if self.config.log_menu_enable:
             yield self.log_menu
@@ -353,28 +366,31 @@
             sound.unpause()
     
     async def on_button_pressed(self, event: Button.Pressed) -> None:
         if event.button.id == "switch-playback-mode":
             self.switch_playback_mode()
             event.button.label = self.gpms()
     
-    @on(Button.Pressed, "#button-pause-unpause")
+    @on(Button.Pressed, "#button-pause")
     async def bp_pause_unpause(self) -> None:
         if (sound:=await self.aio_gcs()) is not None:
-            if sound.playing:
-                if sound.paused: await self.currect_sound_unpause(sound)
-                else: await self.currect_sound_pause(sound)
-            self.music_selected_label.update(await self.aio_get_sound_selected_label_text())
+            if sound.playing: await self.currect_sound_pause(sound)
+            await self.aio_update_select_label(sound)
     
     @on(Button.Pressed, "#button-play-stop")
     async def bp_play_stop(self) -> None:
         if (sound:=await self.aio_gcs()) is not None:
-            if sound.playing: await self.currect_sound_stop(sound)
-            else: await self.currect_sound_play(sound)
-            self.music_selected_label.update(await self.aio_get_sound_selected_label_text())
+            if sound.playing:
+                if sound.paused:
+                    await self.currect_sound_unpause(sound)
+                else:
+                    await self.currect_sound_stop(sound)
+            else:
+                await self.currect_sound_play(sound)
+            await self.aio_update_select_label(sound)
     
     async def submit_plus_sound(self, value: str) -> None:
         if value.replace(" ", "") != "":
             try: self.last_paths_globalized = glob.glob(value, recursive=self.config.recursive_search)
             except: self.last_paths_globalized = [ value ]
             self.info(f"Submit 'plus_sound' values: {repr(self.last_paths_globalized)}")
             if len(self.last_paths_globalized) > 0:
@@ -390,31 +406,35 @@
         sound_uuid: Optional[str],
         playback_mode_blocked: Optional[bool]=None
     ) -> Optional[CodecBase]:
         if playback_mode_blocked is not None:
             self.playback_mode_blocked = playback_mode_blocked
         if sound_uuid is not None:
             if not self.playback_mode_blocked:
-                if (sound:=await self.aio_gcs()) is not None:
-                    self.last_playback_status = "Stoped"
-                    sound.stop()
+                sound = await self.aio_gcs()
+                await self.currect_sound_stop(sound)
             self.playback_mode_blocked = False
             
-            self.currect_sound_uuid = sound_uuid
-            if (sound:=self.music_list_view.get_sound(self.currect_sound_uuid)) is not None:
+            sound = await self.music_list_view.aio_get_sound(sound_uuid)
+            if sound is not None:
                 sound.set_volume(self.currect_volume)
                 await self.music_image.update_image(image_from_bytes(sound.icon_data))
                 self.info(f"A new sound has been selected: {repr(sound)}")
+            
             self.currect_sound = sound
-            self.music_selected_label.update(await self.aio_get_sound_selected_label_text())
+            self.currect_sound_uuid = sound_uuid if self.currect_sound is not None else None
+            
+            await self.aio_update_select_label(sound)
             return sound
     
     async def on_list_view_selected(self, selected: MusicListView.Selected):
         if isinstance(selected.item, MusicListViewItem):
-            await self.set_sound_for_playback(getattr(selected.item, "sound_uuid", None))
+            sound_uuid = getattr(selected.item, "sound_uuid", None)
+            if (sound_uuid != self.currect_sound_uuid) or (self.currect_sound_uuid is None):
+                await self.set_sound_for_playback(sound_uuid)
     
     async def action_plus_rewind(self):
         if (sound:=await self.aio_gcs()) is not None:
             sound.set_pos(sound.get_pos()+self.config.rewind_count_seconds)
     
     async def action_minus_rewind(self):
         if (sound:=await self.aio_gcs()) is not None:
@@ -435,18 +455,19 @@
     async def action_screenshot(self) -> None:
         path = self.save_screenshot(path=LOCALDIR)
         self.info(f"Screenshot saved to: {repr(path)}")
         await self.aio_nofy(f"Screenshot saved to: [green]{repr(path)}[/]")
     
     async def action_quit(self):
         self.started = False
+        if ENABLE_PLUGIN_SYSTEM:
+            await self.plugin_loader.on_quit()
         if (sound:=await self.aio_gcs()) is not None:
             sound.unpause()
             sound.stop()
-            if ENABLE_PLUGIN_SYSTEM:
-                await self.plugin_loader.on_quit()
         return await super().action_quit()
 
     def run(self, *args, **kwargs):
         if ENABLE_PLUGIN_SYSTEM:
             self.plugin_loader.on_run()
         super().run(*args, **kwargs)
+
```

### Comparing `seaplayer-0.5.4.dev2/seaplayer/types/Cache.py` & `seaplayer-0.5.4.dev3/seaplayer/types/Cache.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/seaplayer/types/Convert.py` & `seaplayer-0.5.4.dev3/seaplayer/types/Convert.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/seaplayer/types/MusicList.py` & `seaplayer-0.5.4.dev3/seaplayer/types/MusicList.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev2/seaplayer/units.py` & `seaplayer-0.5.4.dev3/seaplayer/units.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 from platformdirs import user_config_dir
 # > Image Works
 from PIL.Image import Resampling
 
 # ! Metadata
 __title__ = "SeaPlayer"
-__version__ = "0.5.4.dev2"
+__version__ = "0.5.4.dev3"
 __author__ = "Romanin"
 __email__ = "semina054@gmail.com"
 __url__ = "https://github.com/romanin-rf/SeaPlayer"
 
 # ! Paths
 if getattr(sys, 'frozen', False) and hasattr(sys, '_MEIPASS'):
     LOCALDIR = os.path.dirname(sys.executable)
```

### Comparing `seaplayer-0.5.4.dev2/PKG-INFO` & `seaplayer-0.5.4.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaplayer
-Version: 0.5.4.dev2
+Version: 0.5.4.dev3
 Summary: SeaPlayer is a player that works in the terminal.
 Home-page: https://github.com/romanin-rf/SeaPlayer
 License: MIT
 Keywords: tui,player,seaplayer,wav,mp3,ogg,midi
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<3.12
```

