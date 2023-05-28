# Comparing `tmp/scrobblez-0.1.0.tar.gz` & `tmp/scrobblez-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scrobblez-0.1.0.tar", last modified: Mon Oct  5 05:49:34 2020, max compression
+gzip compressed data, was "scrobblez-0.1.1.tar", last modified: Sun May 28 04:29:05 2023, max compression
```

## Comparing `scrobblez-0.1.0.tar` & `scrobblez-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,23 @@
-drwxr-xr-x   0 mulhaq    (1000) users      (100)        0 2020-10-05 05:49:34.622123 scrobblez-0.1.0/
--rw-r--r--   0 mulhaq    (1000) users      (100)       56 2020-10-05 05:40:58.000000 scrobblez-0.1.0/.gitignore
--rw-r--r--   0 mulhaq    (1000) users      (100)     1069 2020-10-05 05:40:58.000000 scrobblez-0.1.0/LICENSE
--rw-r--r--   0 mulhaq    (1000) users      (100)     3393 2020-10-05 05:49:34.622123 scrobblez-0.1.0/PKG-INFO
--rw-r--r--   0 mulhaq    (1000) users      (100)     2327 2020-10-05 05:40:58.000000 scrobblez-0.1.0/README.md
--rw-r--r--   0 mulhaq    (1000) users      (100)       36 2020-10-05 05:40:58.000000 scrobblez-0.1.0/requirements.txt
-drwxr-xr-x   0 mulhaq    (1000) users      (100)        0 2020-10-05 05:49:34.622123 scrobblez-0.1.0/scrobblez/
--rw-r--r--   0 mulhaq    (1000) users      (100)        0 2020-10-05 05:40:58.000000 scrobblez-0.1.0/scrobblez/__init__.py
--rw-r--r--   0 mulhaq    (1000) users      (100)     1519 2020-10-05 05:40:58.000000 scrobblez-0.1.0/scrobblez/__main__.py
--rw-r--r--   0 mulhaq    (1000) users      (100)     4200 2020-10-05 05:40:58.000000 scrobblez-0.1.0/scrobblez/cli.py
--rw-r--r--   0 mulhaq    (1000) users      (100)     4514 2020-10-05 05:40:58.000000 scrobblez-0.1.0/scrobblez/looper.py
-drwxr-xr-x   0 mulhaq    (1000) users      (100)        0 2020-10-05 05:49:34.622123 scrobblez-0.1.0/scrobblez/metadata_filter/
--rw-r--r--   0 mulhaq    (1000) users      (100)       30 2020-10-05 05:40:58.000000 scrobblez-0.1.0/scrobblez/metadata_filter/__init__.py
--rw-r--r--   0 mulhaq    (1000) users      (100)     3381 2020-10-05 05:40:58.000000 scrobblez-0.1.0/scrobblez/scrobblers.py
--rw-r--r--   0 mulhaq    (1000) users      (100)      173 2020-10-05 05:40:58.000000 scrobblez-0.1.0/scrobblez/types.py
-drwxr-xr-x   0 mulhaq    (1000) users      (100)        0 2020-10-05 05:49:34.622123 scrobblez-0.1.0/scrobblez.egg-info/
--rw-r--r--   0 mulhaq    (1000) users      (100)     3393 2020-10-05 05:49:34.000000 scrobblez-0.1.0/scrobblez.egg-info/PKG-INFO
--rw-r--r--   0 mulhaq    (1000) users      (100)      448 2020-10-05 05:49:34.000000 scrobblez-0.1.0/scrobblez.egg-info/SOURCES.txt
--rw-r--r--   0 mulhaq    (1000) users      (100)        1 2020-10-05 05:49:34.000000 scrobblez-0.1.0/scrobblez.egg-info/dependency_links.txt
--rw-r--r--   0 mulhaq    (1000) users      (100)       55 2020-10-05 05:49:34.000000 scrobblez-0.1.0/scrobblez.egg-info/entry_points.txt
--rw-r--r--   0 mulhaq    (1000) users      (100)        1 2020-10-05 05:49:34.000000 scrobblez-0.1.0/scrobblez.egg-info/not-zip-safe
--rw-r--r--   0 mulhaq    (1000) users      (100)       36 2020-10-05 05:49:34.000000 scrobblez-0.1.0/scrobblez.egg-info/requires.txt
--rw-r--r--   0 mulhaq    (1000) users      (100)       10 2020-10-05 05:49:34.000000 scrobblez-0.1.0/scrobblez.egg-info/top_level.txt
--rw-r--r--   0 mulhaq    (1000) users      (100)       38 2020-10-05 05:49:34.622123 scrobblez-0.1.0/setup.cfg
--rw-r--r--   0 mulhaq    (1000) users      (100)      857 2020-10-05 05:40:58.000000 scrobblez-0.1.0/setup.py
+drwxr-xr-x   0 mulhaq    (1000) users      (100)        0 2023-05-28 04:29:05.724048 scrobblez-0.1.1/
+-rw-r--r--   0 mulhaq    (1000) users      (100)     1069 2020-10-05 05:40:58.000000 scrobblez-0.1.1/LICENSE
+-rw-r--r--   0 mulhaq    (1000) users      (100)     2616 2023-05-28 04:29:05.724048 scrobblez-0.1.1/PKG-INFO
+-rw-r--r--   0 mulhaq    (1000) users      (100)     2327 2020-10-05 05:40:58.000000 scrobblez-0.1.1/README.md
+drwxr-xr-x   0 mulhaq    (1000) users      (100)        0 2023-05-28 04:29:05.720715 scrobblez-0.1.1/scrobblez/
+-rw-r--r--   0 mulhaq    (1000) users      (100)        0 2020-10-05 05:40:58.000000 scrobblez-0.1.1/scrobblez/__init__.py
+-rw-r--r--   0 mulhaq    (1000) users      (100)     1519 2023-05-28 04:28:52.000000 scrobblez-0.1.1/scrobblez/__main__.py
+-rw-r--r--   0 mulhaq    (1000) users      (100)     4200 2020-10-05 05:40:58.000000 scrobblez-0.1.1/scrobblez/cli.py
+-rw-r--r--   0 mulhaq    (1000) users      (100)     4872 2023-05-28 04:28:52.000000 scrobblez-0.1.1/scrobblez/looper.py
+drwxr-xr-x   0 mulhaq    (1000) users      (100)        0 2023-05-28 04:29:05.724048 scrobblez-0.1.1/scrobblez/metadata_filter/
+-rw-r--r--   0 mulhaq    (1000) users      (100)       30 2020-10-05 05:40:58.000000 scrobblez-0.1.1/scrobblez/metadata_filter/__init__.py
+-rw-r--r--   0 mulhaq    (1000) users      (100)     3502 2021-01-12 23:14:05.000000 scrobblez-0.1.1/scrobblez/scrobblers.py
+-rw-r--r--   0 mulhaq    (1000) users      (100)      173 2020-10-05 05:40:58.000000 scrobblez-0.1.1/scrobblez/types.py
+drwxr-xr-x   0 mulhaq    (1000) users      (100)        0 2023-05-28 04:29:05.724048 scrobblez-0.1.1/scrobblez.egg-info/
+-rw-r--r--   0 mulhaq    (1000) users      (100)     2616 2023-05-28 04:29:05.000000 scrobblez-0.1.1/scrobblez.egg-info/PKG-INFO
+-rw-r--r--   0 mulhaq    (1000) users      (100)      420 2023-05-28 04:29:05.000000 scrobblez-0.1.1/scrobblez.egg-info/SOURCES.txt
+-rw-r--r--   0 mulhaq    (1000) users      (100)        1 2023-05-28 04:29:05.000000 scrobblez-0.1.1/scrobblez.egg-info/dependency_links.txt
+-rw-r--r--   0 mulhaq    (1000) users      (100)       54 2023-05-28 04:29:05.000000 scrobblez-0.1.1/scrobblez.egg-info/entry_points.txt
+-rw-r--r--   0 mulhaq    (1000) users      (100)        1 2023-05-28 04:29:05.000000 scrobblez-0.1.1/scrobblez.egg-info/not-zip-safe
+-rw-r--r--   0 mulhaq    (1000) users      (100)       36 2023-05-28 04:29:05.000000 scrobblez-0.1.1/scrobblez.egg-info/requires.txt
+-rw-r--r--   0 mulhaq    (1000) users      (100)       10 2023-05-28 04:29:05.000000 scrobblez-0.1.1/scrobblez.egg-info/top_level.txt
+-rw-r--r--   0 mulhaq    (1000) users      (100)       38 2023-05-28 04:29:05.724048 scrobblez-0.1.1/setup.cfg
+-rw-r--r--   0 mulhaq    (1000) users      (100)      857 2021-01-12 23:11:34.000000 scrobblez-0.1.1/setup.py
```

### Comparing `scrobblez-0.1.0/LICENSE` & `scrobblez-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scrobblez-0.1.0/PKG-INFO` & `scrobblez-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,107 +1,96 @@
-Metadata-Version: 2.1
-Name: scrobblez
-Version: 0.1.0
-Summary: Scrobbler for MPRIS 2 compatible clients
-Home-page: https://github.com/YodaEmbedding/scrobblez
-Author: Mateen Ulhaq
-Author-email: mulhaq2005@gmail.com
-License: MIT
-Description: # scrobblez
-        
-        [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-        
-        User-customizable scrobbler for Last.fm and MPRIS 2.
-        
-        This scrobbler cleans up metadata (e.g. artist, album, track titles) produced
-        by services with non-standard tagging schemes (e.g. Spotify). The cleaning
-        process is extensible and can be customized to a user's particular needs.
-        
-        ## Install
-        
-        Install from PyPI:
-        
-        ```bash
-        pip install scrobblez
-        ```
-        
-        Or install from source:
-        
-        ```bash
-        git clone https://github.com/YodaEmbedding/scrobblez
-        cd scrobblez
-        pip install .
-        ```
-        
-        ## Usage
-        
-        Simply run the following command:
-        
-        ```bash
-        scrobblez
-        ```
-        
-        ## Configuration
-        
-        Within `~/.config/scrobblez/config.py`, you may specify a whitelist of valid
-        player names:
-        
-        ```python
-        whitelist = ["spotify"]
-        ```
-        
-        Optionally, you can also customize the metadata cleaning process:
-        
-        ```python
-        from scrobblez.metadata_filter import *
-        from scrobblez.types import Metadata
-        
-        def fix_metadata(metadata: Metadata) -> Metadata:
-            m = dict(metadata)
-        
-            # Keep first artist only in list of artists
-            m["artist"] = m["artist"][0]
-            m["album_artist"] = m["album_artist"][0]
-        
-            # Specify which filter rules to use
-            rules = (
-                REMASTERED_FILTER_RULES
-                + SUFFIX_FILTER_RULES
-                + VERSION_FILTER_RULES
-                + ORIGIN_FILTER_RULES
-                + FEATURE_FILTER_RULES
-                + CLEAN_EXPLICIT_FILTER_RULES
-                + LIVE_FILTER_RULES
-                + TRIM_WHITESPACE_FILTER_RULES
-            )
-        
-            # Specify manual artist/album/title overrides
-            artist_overrides = {
-                "Yusuf": "Cat Stevens",
-                "Yusuf / Cat Stevens": "Cat Stevens",
-            }
-        
-            album_overrides = {
-                "The Lord of the Rings - The Return of the King - "
-                "The Complete Recordings (Limited Edition)":
-                "The Lord of the Rings: Return of the King - the Complete Recordings",
-            }
-        
-            title_overrides = {
-                "Better Get Hit In Your Soul - Instrumental":
-                "Better Git It in Your Soul",
-            }
-        
-            def fix(k, overrides, f=lambda x: x):
-                m[k] = overrides.get(m[k], f(m[k]))
-        
-            # Apply fixes
-            fix("artist", artist_overrides)
-            fix("album_artist", artist_overrides)
-            fix("album", album_overrides, lambda x: apply_filters(rules, x))
-            fix("title", title_overrides, lambda x: apply_filters(rules, x))
-        
-            return m
-        ```
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+# scrobblez
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+User-customizable scrobbler for Last.fm and MPRIS 2.
+
+This scrobbler cleans up metadata (e.g. artist, album, track titles) produced
+by services with non-standard tagging schemes (e.g. Spotify). The cleaning
+process is extensible and can be customized to a user's particular needs.
+
+## Install
+
+Install from PyPI:
+
+```bash
+pip install scrobblez
+```
+
+Or install from source:
+
+```bash
+git clone https://github.com/YodaEmbedding/scrobblez
+cd scrobblez
+pip install .
+```
+
+## Usage
+
+Simply run the following command:
+
+```bash
+scrobblez
+```
+
+## Configuration
+
+Within `~/.config/scrobblez/config.py`, you may specify a whitelist of valid
+player names:
+
+```python
+whitelist = ["spotify"]
+```
+
+Optionally, you can also customize the metadata cleaning process:
+
+```python
+from scrobblez.metadata_filter import *
+from scrobblez.types import Metadata
+
+def fix_metadata(metadata: Metadata) -> Metadata:
+    m = dict(metadata)
+
+    # Keep first artist only in list of artists
+    m["artist"] = m["artist"][0]
+    m["album_artist"] = m["album_artist"][0]
+
+    # Specify which filter rules to use
+    rules = (
+        REMASTERED_FILTER_RULES
+        + SUFFIX_FILTER_RULES
+        + VERSION_FILTER_RULES
+        + ORIGIN_FILTER_RULES
+        + FEATURE_FILTER_RULES
+        + CLEAN_EXPLICIT_FILTER_RULES
+        + LIVE_FILTER_RULES
+        + TRIM_WHITESPACE_FILTER_RULES
+    )
+
+    # Specify manual artist/album/title overrides
+    artist_overrides = {
+        "Yusuf": "Cat Stevens",
+        "Yusuf / Cat Stevens": "Cat Stevens",
+    }
+
+    album_overrides = {
+        "The Lord of the Rings - The Return of the King - "
+        "The Complete Recordings (Limited Edition)":
+        "The Lord of the Rings: Return of the King - the Complete Recordings",
+    }
+
+    title_overrides = {
+        "Better Get Hit In Your Soul - Instrumental":
+        "Better Git It in Your Soul",
+    }
+
+    def fix(k, overrides, f=lambda x: x):
+        m[k] = overrides.get(m[k], f(m[k]))
+
+    # Apply fixes
+    fix("artist", artist_overrides)
+    fix("album_artist", artist_overrides)
+    fix("album", album_overrides, lambda x: apply_filters(rules, x))
+    fix("title", title_overrides, lambda x: apply_filters(rules, x))
+
+    return m
+```
```

### Comparing `scrobblez-0.1.0/README.md` & `scrobblez-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: scrobblez
+Version: 0.1.1
+Summary: Scrobbler for MPRIS 2 compatible clients
+Home-page: https://github.com/YodaEmbedding/scrobblez
+Author: Mateen Ulhaq
+Author-email: mulhaq2005@gmail.com
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # scrobblez
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 User-customizable scrobbler for Last.fm and MPRIS 2.
 
 This scrobbler cleans up metadata (e.g. artist, album, track titles) produced
```

### Comparing `scrobblez-0.1.0/scrobblez/__main__.py` & `scrobblez-0.1.1/scrobblez/__main__.py`

 * *Files identical despite different names*

### Comparing `scrobblez-0.1.0/scrobblez/cli.py` & `scrobblez-0.1.1/scrobblez/cli.py`

 * *Files identical despite different names*

### Comparing `scrobblez-0.1.0/scrobblez/looper.py` & `scrobblez-0.1.1/scrobblez/looper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from datetime import datetime, timezone
 from functools import partial
 from math import isclose
 from time import sleep, time
 from typing import Callable, Dict, Tuple
 
+import dbus
 from mpris2 import Player
 
 from scrobblez.scrobblers import Scrobbler
 from scrobblez.types import Metadata, NowPlayingInfo, Scrobble
 
 POLL_INTERVAL = 1
-REL_TOL = 0.25
+REL_TOL = 0.50
 ABS_TOL = POLL_INTERVAL * 2
 
 
 class Looper:
     def __init__(
         self,
         player: Player,
@@ -28,20 +29,24 @@
         self._can_now_play: bool = False
         self._can_scrobble: bool = False
         self._elapsed: float = 0
 
     def run(self):
         self.scrobbler.flush_scrobble_cache()
 
-        while True:
-            loop_start = time()
-            self._run_step()
-            sleep(max(0, POLL_INTERVAL - (time() - loop_start)))
-            if self._is_playing:
-                self._elapsed += time() - loop_start
+        try:
+            while True:
+                loop_start = time()
+                self._run_step()
+                sleep(max(0, POLL_INTERVAL - (time() - loop_start)))
+                if self._is_playing:
+                    self._elapsed += time() - loop_start
+        except dbus.exceptions.DBusException as e:
+            self._try_scrobble(offset=self._elapsed)
+            raise e
 
     def _run_step(self):
         metadata = clean_player_metadata(self.player.Metadata)
 
         if metadata != self._metadata:
             self._try_scrobble(offset=min(self._elapsed, self._duration))
             self._new_track(metadata)
@@ -69,14 +74,18 @@
     def _try_scrobble(self, offset: float):
         near = partial(isclose, rel_tol=REL_TOL, abs_tol=ABS_TOL)
         if not self._can_scrobble or not near(self._elapsed, self._duration):
             return
         self._send_scrobble(timestamp=int(timestamp_now() - offset))
 
     def _send_now_playing(self):
+        fmt_metadata = "\n".join(
+            f"  {k}: {v}" for k, v in self._metadata.items()
+        )
+        print(f"Now playing (unfixed metadata, debug info):\n{fmt_metadata}\n")
         info = to_now_playing(self._fix_metadata(self._metadata))
         self.scrobbler.update_now_playing(info)
         self._can_now_play = False
 
     def _send_scrobble(self, timestamp: int):
         scrobble = to_scrobble(self._fix_metadata(self._metadata), timestamp)
         self.scrobbler.scrobble(scrobble)
```

### Comparing `scrobblez-0.1.0/scrobblez/scrobblers.py` & `scrobblez-0.1.1/scrobblez/scrobblers.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,18 @@
         log("Scrobble", fmt_dict(scrobble))
         self.cache.put(scrobble)
         self._log_queue.put(scrobble)
         self.flush_scrobble_cache()
 
     def update_now_playing(self, info: NowPlayingInfo):
         log("Now playing", fmt_dict(info))
-        self.network.update_now_playing(**info)
+        try:
+            self.network.update_now_playing(**info)
+        except Exception as e:
+            log("Exception when sending now playing", f"{type(e)}({e})")
 
     def flush_scrobble_cache(self):
         """Send scrobbles over network."""
         if self.cache_only:
             return
 
         while not self.cache.empty():
```

### Comparing `scrobblez-0.1.0/scrobblez.egg-info/PKG-INFO` & `scrobblez-0.1.1/scrobblez.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,107 +1,107 @@
 Metadata-Version: 2.1
 Name: scrobblez
-Version: 0.1.0
+Version: 0.1.1
 Summary: Scrobbler for MPRIS 2 compatible clients
 Home-page: https://github.com/YodaEmbedding/scrobblez
 Author: Mateen Ulhaq
 Author-email: mulhaq2005@gmail.com
 License: MIT
-Description: # scrobblez
-        
-        [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-        
-        User-customizable scrobbler for Last.fm and MPRIS 2.
-        
-        This scrobbler cleans up metadata (e.g. artist, album, track titles) produced
-        by services with non-standard tagging schemes (e.g. Spotify). The cleaning
-        process is extensible and can be customized to a user's particular needs.
-        
-        ## Install
-        
-        Install from PyPI:
-        
-        ```bash
-        pip install scrobblez
-        ```
-        
-        Or install from source:
-        
-        ```bash
-        git clone https://github.com/YodaEmbedding/scrobblez
-        cd scrobblez
-        pip install .
-        ```
-        
-        ## Usage
-        
-        Simply run the following command:
-        
-        ```bash
-        scrobblez
-        ```
-        
-        ## Configuration
-        
-        Within `~/.config/scrobblez/config.py`, you may specify a whitelist of valid
-        player names:
-        
-        ```python
-        whitelist = ["spotify"]
-        ```
-        
-        Optionally, you can also customize the metadata cleaning process:
-        
-        ```python
-        from scrobblez.metadata_filter import *
-        from scrobblez.types import Metadata
-        
-        def fix_metadata(metadata: Metadata) -> Metadata:
-            m = dict(metadata)
-        
-            # Keep first artist only in list of artists
-            m["artist"] = m["artist"][0]
-            m["album_artist"] = m["album_artist"][0]
-        
-            # Specify which filter rules to use
-            rules = (
-                REMASTERED_FILTER_RULES
-                + SUFFIX_FILTER_RULES
-                + VERSION_FILTER_RULES
-                + ORIGIN_FILTER_RULES
-                + FEATURE_FILTER_RULES
-                + CLEAN_EXPLICIT_FILTER_RULES
-                + LIVE_FILTER_RULES
-                + TRIM_WHITESPACE_FILTER_RULES
-            )
-        
-            # Specify manual artist/album/title overrides
-            artist_overrides = {
-                "Yusuf": "Cat Stevens",
-                "Yusuf / Cat Stevens": "Cat Stevens",
-            }
-        
-            album_overrides = {
-                "The Lord of the Rings - The Return of the King - "
-                "The Complete Recordings (Limited Edition)":
-                "The Lord of the Rings: Return of the King - the Complete Recordings",
-            }
-        
-            title_overrides = {
-                "Better Get Hit In Your Soul - Instrumental":
-                "Better Git It in Your Soul",
-            }
-        
-            def fix(k, overrides, f=lambda x: x):
-                m[k] = overrides.get(m[k], f(m[k]))
-        
-            # Apply fixes
-            fix("artist", artist_overrides)
-            fix("album_artist", artist_overrides)
-            fix("album", album_overrides, lambda x: apply_filters(rules, x))
-            fix("title", title_overrides, lambda x: apply_filters(rules, x))
-        
-            return m
-        ```
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# scrobblez
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+User-customizable scrobbler for Last.fm and MPRIS 2.
+
+This scrobbler cleans up metadata (e.g. artist, album, track titles) produced
+by services with non-standard tagging schemes (e.g. Spotify). The cleaning
+process is extensible and can be customized to a user's particular needs.
+
+## Install
+
+Install from PyPI:
+
+```bash
+pip install scrobblez
+```
+
+Or install from source:
+
+```bash
+git clone https://github.com/YodaEmbedding/scrobblez
+cd scrobblez
+pip install .
+```
+
+## Usage
+
+Simply run the following command:
+
+```bash
+scrobblez
+```
+
+## Configuration
+
+Within `~/.config/scrobblez/config.py`, you may specify a whitelist of valid
+player names:
+
+```python
+whitelist = ["spotify"]
+```
+
+Optionally, you can also customize the metadata cleaning process:
+
+```python
+from scrobblez.metadata_filter import *
+from scrobblez.types import Metadata
+
+def fix_metadata(metadata: Metadata) -> Metadata:
+    m = dict(metadata)
+
+    # Keep first artist only in list of artists
+    m["artist"] = m["artist"][0]
+    m["album_artist"] = m["album_artist"][0]
+
+    # Specify which filter rules to use
+    rules = (
+        REMASTERED_FILTER_RULES
+        + SUFFIX_FILTER_RULES
+        + VERSION_FILTER_RULES
+        + ORIGIN_FILTER_RULES
+        + FEATURE_FILTER_RULES
+        + CLEAN_EXPLICIT_FILTER_RULES
+        + LIVE_FILTER_RULES
+        + TRIM_WHITESPACE_FILTER_RULES
+    )
+
+    # Specify manual artist/album/title overrides
+    artist_overrides = {
+        "Yusuf": "Cat Stevens",
+        "Yusuf / Cat Stevens": "Cat Stevens",
+    }
+
+    album_overrides = {
+        "The Lord of the Rings - The Return of the King - "
+        "The Complete Recordings (Limited Edition)":
+        "The Lord of the Rings: Return of the King - the Complete Recordings",
+    }
+
+    title_overrides = {
+        "Better Get Hit In Your Soul - Instrumental":
+        "Better Git It in Your Soul",
+    }
+
+    def fix(k, overrides, f=lambda x: x):
+        m[k] = overrides.get(m[k], f(m[k]))
+
+    # Apply fixes
+    fix("artist", artist_overrides)
+    fix("album_artist", artist_overrides)
+    fix("album", album_overrides, lambda x: apply_filters(rules, x))
+    fix("title", title_overrides, lambda x: apply_filters(rules, x))
+
+    return m
+```
```

### Comparing `scrobblez-0.1.0/setup.py` & `scrobblez-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 root = path.abspath(path.dirname(__file__))
 with open(path.join(root, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="scrobblez",
-    version="0.1.0",
+    version="0.1.1",
     description="Scrobbler for MPRIS 2 compatible clients",
     url="https://github.com/YodaEmbedding/scrobblez",
     author="Mateen Ulhaq",
     author_email="mulhaq2005@gmail.com",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

