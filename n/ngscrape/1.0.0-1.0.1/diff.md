# Comparing `tmp/ngscrape-1.0.0.tar.gz` & `tmp/ngscrape-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngscrape-1.0.0.tar", last modified: Sun May 28 19:48:16 2023, max compression
+gzip compressed data, was "ngscrape-1.0.1.tar", last modified: Sun May 28 19:55:05 2023, max compression
```

## Comparing `ngscrape-1.0.0.tar` & `ngscrape-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 19:48:16.296464 ngscrape-1.0.0/
--rw-rw-rw-   0        0        0    35184 2023-05-27 22:41:04.000000 ngscrape-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    42283 2023-05-28 19:48:16.295466 ngscrape-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      687 2023-05-28 19:47:57.000000 ngscrape-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0     1291 2023-05-28 00:12:10.000000 ngscrape-1.0.0/readme.md
--rw-rw-rw-   0        0        0       42 2023-05-28 19:48:16.297465 ngscrape-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-28 19:48:16.255458 ngscrape-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-28 19:48:16.262457 ngscrape-1.0.0/src/ngscrape/
--rw-rw-rw-   0        0        0     3663 2023-05-28 00:08:55.000000 ngscrape-1.0.0/src/ngscrape/ngscrape.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:48:16.292462 ngscrape-1.0.0/src/ngscrape.egg-info/
--rw-rw-rw-   0        0        0    42283 2023-05-28 19:48:16.000000 ngscrape-1.0.0/src/ngscrape.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-05-28 19:48:16.000000 ngscrape-1.0.0/src/ngscrape.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 19:48:16.000000 ngscrape-1.0.0/src/ngscrape.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-28 19:48:16.000000 ngscrape-1.0.0/src/ngscrape.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-28 19:48:16.000000 ngscrape-1.0.0/src/ngscrape.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 19:55:05.935881 ngscrape-1.0.1/
+-rw-rw-rw-   0        0        0    35184 2023-05-27 22:41:04.000000 ngscrape-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0    42296 2023-05-28 19:55:05.933879 ngscrape-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      738 2023-05-28 19:54:46.000000 ngscrape-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1259 2023-05-28 19:51:04.000000 ngscrape-1.0.1/readme.md
+-rw-rw-rw-   0        0        0       42 2023-05-28 19:55:05.936897 ngscrape-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 19:55:05.894883 ngscrape-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-28 19:55:05.900879 ngscrape-1.0.1/src/ngscrape/
+-rw-rw-rw-   0        0        0     3663 2023-05-28 19:51:27.000000 ngscrape-1.0.1/src/ngscrape/ngscrape.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:55:05.931874 ngscrape-1.0.1/src/ngscrape.egg-info/
+-rw-rw-rw-   0        0        0    42296 2023-05-28 19:55:05.000000 ngscrape-1.0.1/src/ngscrape.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-05-28 19:55:05.000000 ngscrape-1.0.1/src/ngscrape.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 19:55:05.000000 ngscrape-1.0.1/src/ngscrape.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-28 19:55:05.000000 ngscrape-1.0.1/src/ngscrape.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-28 19:55:05.000000 ngscrape-1.0.1/src/ngscrape.egg-info/top_level.txt
```

### Comparing `ngscrape-1.0.0/LICENSE` & `ngscrape-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ngscrape-1.0.0/PKG-INFO` & `ngscrape-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ngscrape
-Version: 1.0.0
-Summary: Newgrounds flash game scraper
+Version: 1.0.1
+Summary: Newgrounds flash game scraper powered by bs4 and requests
 Author-email: aeiea <dpthn@proton.me>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -662,15 +662,15 @@
         
           You should also get your employer (if you work as a programmer) or school,
         if any, to sign a "copyright disclaimer" for the program, if necessary.
         For more information on this, and how to apply and follow the GNU AGPL, see
         <https://www.gnu.org/licenses/>.
         
 Project-URL: Homepage, https://github.com/aeiea/ngscrape
-Keywords: flash,newgrounds,scraper
+Keywords: flash,newgrounds,scraper,games,opensource
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -678,23 +678,23 @@
 Newgrounds game scraper made with beautifulsoup4 and requestslib.
 
 NGScrape is licensed under the GNU Affero General Public License v3.0. If a copy is not included with this file, you can find one at https://www.gnu.org/licenses/agpl-3.0.en.html.
 
 Please star is this was useful!
 
 Functions:
-    `__init__(debug: bool = False) -> None`
-        Start a new NGScrape Instance.
-    `scrape_game_by_url(url: str, download: str, filename: str) -> None`
-        Scrape a flash game by url.
-        Parameters:
-            url (str): The URL of the flash game. For example, the URL for Alien Homonid is https://www.newgrounds.com/portal/view/59593.
-            download (str): The directory to download the file to.
-            filename (str): The name of the downloaded file.
-        Example parameters:
-            url = 'https://www.newgrounds.com/portal/view/59593'
-            download = 'testdir'
-            filename = 'game.swf'
-        Example output with debug mode:
-            NGScrape: Made request to https://www.newgrounds.com/portal/view/59593 and got status code 200
-            NGScrape: Found flash game link https:\/\/uploads.ungrounded.net\/59000\/59593_alien_booya.swf?f1101313499
-            NGScrape: Downloaded swf file to testdir/game.swf
+- `__init__(debug: bool = False) -> None`
+    - Start a new NGScrape Instance.
+- `scrape_game_by_url(url: str, download: str, filename: str) -> None`
+    - Scrape a flash game by url.
+    - Parameters:
+        - url (str): The URL of the flash game. For example, the URL for Alien Homonid is https://www.newgrounds.com/portal/view/59593.
+        - download (str): The directory to download the file to.
+        - filename (str): The name of the downloaded file.
+    - Example parameters:
+        - url = 'https://www.newgrounds.com/portal/view/59593'
+        - download = 'testdir'
+        - filename = 'game.swf'
+    - Example output with debug mode:
+        - NGScrape: Made request to https://www.newgrounds.com/portal/view/59593 and got status code 200
+        - NGScrape: Found flash game link https:\/\/uploads.ungrounded.net\/59000\/59593_alien_booya.swf?f1101313499
+        - NGScrape: Downloaded swf file to testdir/game.swf
```

### Comparing `ngscrape-1.0.0/pyproject.toml` & `ngscrape-1.0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ngscrape"
-version = "1.0.0"
-description = "Newgrounds flash game scraper"
+version = "1.0.1"
+description = "Newgrounds flash game scraper powered by bs4 and requests"
 readme = "readme.md"
 authors = [{ name = "aeiea", email = "dpthn@proton.me" }]
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
-keywords = ["flash", "newgrounds", "scraper"]
+keywords = ["flash", "newgrounds", "scraper", "games", "opensource"]
 dependencies = ["beautifulsoup4", "requests"]
 requires-python = ">=3.7"
 [project.urls]
 Homepage = "https://github.com/aeiea/ngscrape"
```

### Comparing `ngscrape-1.0.0/readme.md` & `ngscrape-1.0.1/readme.md`

 * *Files 23% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 Newgrounds game scraper made with beautifulsoup4 and requestslib.
 
 NGScrape is licensed under the GNU Affero General Public License v3.0. If a copy is not included with this file, you can find one at https://www.gnu.org/licenses/agpl-3.0.en.html.
 
 Please star is this was useful!
 
 Functions:
-    `__init__(debug: bool = False) -> None`
-        Start a new NGScrape Instance.
-    `scrape_game_by_url(url: str, download: str, filename: str) -> None`
-        Scrape a flash game by url.
-        Parameters:
-            url (str): The URL of the flash game. For example, the URL for Alien Homonid is https://www.newgrounds.com/portal/view/59593.
-            download (str): The directory to download the file to.
-            filename (str): The name of the downloaded file.
-        Example parameters:
-            url = 'https://www.newgrounds.com/portal/view/59593'
-            download = 'testdir'
-            filename = 'game.swf'
-        Example output with debug mode:
-            NGScrape: Made request to https://www.newgrounds.com/portal/view/59593 and got status code 200
-            NGScrape: Found flash game link https:\/\/uploads.ungrounded.net\/59000\/59593_alien_booya.swf?f1101313499
-            NGScrape: Downloaded swf file to testdir/game.swf
+- `__init__(debug: bool = False) -> None`
+    - Start a new NGScrape Instance.
+- `scrape_game_by_url(url: str, download: str, filename: str) -> None`
+    - Scrape a flash game by url.
+    - Parameters:
+        - url (str): The URL of the flash game. For example, the URL for Alien Homonid is https://www.newgrounds.com/portal/view/59593.
+        - download (str): The directory to download the file to.
+        - filename (str): The name of the downloaded file.
+    - Example parameters:
+        - url = 'https://www.newgrounds.com/portal/view/59593'
+        - download = 'testdir'
+        - filename = 'game.swf'
+    - Example output with debug mode:
+        - NGScrape: Made request to https://www.newgrounds.com/portal/view/59593 and got status code 200
+        - NGScrape: Found flash game link https:\/\/uploads.ungrounded.net\/59000\/59593_alien_booya.swf?f1101313499
+        - NGScrape: Downloaded swf file to testdir/game.swf
```

### Comparing `ngscrape-1.0.0/src/ngscrape/ngscrape.py` & `ngscrape-1.0.1/src/ngscrape/ngscrape.py`

 * *Files identical despite different names*

### Comparing `ngscrape-1.0.0/src/ngscrape.egg-info/PKG-INFO` & `ngscrape-1.0.1/src/ngscrape.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ngscrape
-Version: 1.0.0
-Summary: Newgrounds flash game scraper
+Version: 1.0.1
+Summary: Newgrounds flash game scraper powered by bs4 and requests
 Author-email: aeiea <dpthn@proton.me>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -662,15 +662,15 @@
         
           You should also get your employer (if you work as a programmer) or school,
         if any, to sign a "copyright disclaimer" for the program, if necessary.
         For more information on this, and how to apply and follow the GNU AGPL, see
         <https://www.gnu.org/licenses/>.
         
 Project-URL: Homepage, https://github.com/aeiea/ngscrape
-Keywords: flash,newgrounds,scraper
+Keywords: flash,newgrounds,scraper,games,opensource
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -678,23 +678,23 @@
 Newgrounds game scraper made with beautifulsoup4 and requestslib.
 
 NGScrape is licensed under the GNU Affero General Public License v3.0. If a copy is not included with this file, you can find one at https://www.gnu.org/licenses/agpl-3.0.en.html.
 
 Please star is this was useful!
 
 Functions:
-    `__init__(debug: bool = False) -> None`
-        Start a new NGScrape Instance.
-    `scrape_game_by_url(url: str, download: str, filename: str) -> None`
-        Scrape a flash game by url.
-        Parameters:
-            url (str): The URL of the flash game. For example, the URL for Alien Homonid is https://www.newgrounds.com/portal/view/59593.
-            download (str): The directory to download the file to.
-            filename (str): The name of the downloaded file.
-        Example parameters:
-            url = 'https://www.newgrounds.com/portal/view/59593'
-            download = 'testdir'
-            filename = 'game.swf'
-        Example output with debug mode:
-            NGScrape: Made request to https://www.newgrounds.com/portal/view/59593 and got status code 200
-            NGScrape: Found flash game link https:\/\/uploads.ungrounded.net\/59000\/59593_alien_booya.swf?f1101313499
-            NGScrape: Downloaded swf file to testdir/game.swf
+- `__init__(debug: bool = False) -> None`
+    - Start a new NGScrape Instance.
+- `scrape_game_by_url(url: str, download: str, filename: str) -> None`
+    - Scrape a flash game by url.
+    - Parameters:
+        - url (str): The URL of the flash game. For example, the URL for Alien Homonid is https://www.newgrounds.com/portal/view/59593.
+        - download (str): The directory to download the file to.
+        - filename (str): The name of the downloaded file.
+    - Example parameters:
+        - url = 'https://www.newgrounds.com/portal/view/59593'
+        - download = 'testdir'
+        - filename = 'game.swf'
+    - Example output with debug mode:
+        - NGScrape: Made request to https://www.newgrounds.com/portal/view/59593 and got status code 200
+        - NGScrape: Found flash game link https:\/\/uploads.ungrounded.net\/59000\/59593_alien_booya.swf?f1101313499
+        - NGScrape: Downloaded swf file to testdir/game.swf
```

