# Comparing `tmp/TMDBTraktSyncer-1.1.7.tar.gz` & `tmp/TMDBTraktSyncer-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TMDBTraktSyncer-1.1.7.tar", last modified: Wed May 24 01:35:14 2023, max compression
+gzip compressed data, was "TMDBTraktSyncer-1.1.8.tar", last modified: Sun May 28 13:00:48 2023, max compression
```

## Comparing `TMDBTraktSyncer-1.1.7.tar` & `TMDBTraktSyncer-1.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 01:35:14.424027 TMDBTraktSyncer-1.1.7/
--rw-rw-rw-   0        0        0     1079 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.1.7/LICENSE
--rw-rw-rw-   0        0        0     7257 2023-05-24 01:35:14.423026 TMDBTraktSyncer-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     6555 2023-05-24 01:34:43.000000 TMDBTraktSyncer-1.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 01:35:14.394903 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer/
--rw-rw-rw-   0        0        0    10142 2023-05-24 01:26:25.000000 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer/TMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1928 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     8916 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     3952 2023-05-24 00:42:48.000000 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer/tmdbData.py
--rw-rw-rw-   0        0        0     3037 2023-05-24 00:45:06.000000 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0     3325 2023-05-24 00:34:12.000000 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-24 01:35:14.421027 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     7257 2023-05-24 01:35:14.000000 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      481 2023-05-24 01:35:14.000000 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 01:35:14.000000 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-24 01:35:14.000000 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-05-24 01:35:14.000000 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-24 01:35:14.000000 TMDBTraktSyncer-1.1.7/TMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 01:35:14.424027 TMDBTraktSyncer-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1311 2023-05-24 01:30:39.000000 TMDBTraktSyncer-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 13:00:48.429756 TMDBTraktSyncer-1.1.8/
+-rw-rw-rw-   0        0        0     1079 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.1.8/LICENSE
+-rw-rw-rw-   0        0        0    10672 2023-05-28 13:00:48.429756 TMDBTraktSyncer-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     9927 2023-05-28 12:50:14.000000 TMDBTraktSyncer-1.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 13:00:48.395757 TMDBTraktSyncer-1.1.8/TMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    10142 2023-05-24 01:26:25.000000 TMDBTraktSyncer-1.1.8/TMDBTraktSyncer/TMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.1.8/TMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     4840 2023-05-28 12:58:18.000000 TMDBTraktSyncer-1.1.8/TMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     8916 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.1.8/TMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     3952 2023-05-24 00:42:48.000000 TMDBTraktSyncer-1.1.8/TMDBTraktSyncer/tmdbData.py
+-rw-rw-rw-   0        0        0     3037 2023-05-24 00:45:06.000000 TMDBTraktSyncer-1.1.8/TMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0     3325 2023-05-24 00:34:12.000000 TMDBTraktSyncer-1.1.8/TMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-28 13:00:48.426756 TMDBTraktSyncer-1.1.8/TMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0    10672 2023-05-28 13:00:48.000000 TMDBTraktSyncer-1.1.8/TMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      481 2023-05-28 13:00:48.000000 TMDBTraktSyncer-1.1.8/TMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 13:00:48.000000 TMDBTraktSyncer-1.1.8/TMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-28 13:00:48.000000 TMDBTraktSyncer-1.1.8/TMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-05-28 13:00:48.000000 TMDBTraktSyncer-1.1.8/TMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-28 13:00:48.000000 TMDBTraktSyncer-1.1.8/TMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 13:00:48.430757 TMDBTraktSyncer-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1334 2023-05-28 12:50:04.000000 TMDBTraktSyncer-1.1.8/setup.py
```

### Comparing `TMDBTraktSyncer-1.1.7/LICENSE` & `TMDBTraktSyncer-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.7/PKG-INFO` & `TMDBTraktSyncer-1.1.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.1.7
+Version: 1.1.8
 Summary: This python script syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
+Author: RileyXX
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # TMDB-Trakt-Syncer
 
 This Python script syncs user watchlist and ratings for Movies, TV Shows, and Episodes both ways between [Trakt](https://trakt.tv/) and [TMDB](https://www.themoviedb.org/). Data already set will not be overwritten. Ratings are synced by default and watchlist sync is optional. The user will be prompted to enter their preferences and api keys on first run. 
 
-The script is compatible on any operating system that supports Python v3.6 or later, including Windows, Linux, Mac, and ChromeOS. If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
+The script is compatible on any operating system that supports Python v3.6 or later, including Windows, Linux, Mac, and ChromeOS. If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer). See below for my other [recommended projects](https://github.com/RileyXX/TMDB-Trakt-Syncer#other-recommended-projects).
 
 ## Installation Instructions:
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
 2. Install the script by running `python -m pip install TMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDbTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
    - Type of use: `Personal`
@@ -100,7 +101,33 @@
 ## Also Posted on:
 * [PyPi](https://pypi.org/project/TMDBTraktSyncer/)
 * [Reddit](https://www.reddit.com/r/trakt/comments/13jlu4r/tmdb_trakt_rating_syncer_tool_2_way_sync/)
 
 <br>
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+## Other Recommended Projects:
+
+| Project Name | Description |
+|--------------|-------------|
+| [PlexTraktSync](https://github.com/Taxel/PlexTraktSync) | A script that syncs user watch history and ratings between Trakt and Plex (without needing a PlexPass or Trakt VIP subscription). |
+| [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer) | A script that syncs user watchlist, ratings, and comments both ways between Trakt and IMDB. |
+| [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer) | A script that syncs user watchlist and ratings both ways between Trakt and TMDB. |
+| [PlexPreferNonForcedSubs](https://github.com/RileyXX/PlexPreferNonForcedSubs) | A script that sets all movies and shows in your local Plex library to English non-forced subtitles by default. |
+| [Casvt / PlexAutoDelete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py) | A script for automatically deleting watched content from Plex. |
+| [Netflix-to-Trakt-Import](https://github.com/jensb89/Netflix-to-Trakt-Import) | A tool to import your Netflix viewing history into Trakt. |
+| [trakt-tv-backup](https://darekkay.com/blog/trakt-tv-backup/) | A command-line tool for backing up your Trakt.tv data. |
+| [blacktwin / JBOPS](https://github.com/blacktwin/JBOPS) | A collection of scripts and tools for enhancing and automating tasks in Plex. |
+| [Casvt / Plex-scripts](https://github.com/Casvt/Plex-scripts) | A collection of useful scripts for Plex automation and management. |
+| [trakt---letterboxd-import](https://github.com/jensb89/trakt---letterboxd-import) | A tool to import your Letterboxd ratings and watchlist into Trakt. |
+| [TraktRater](https://github.com/damienhaynes/TraktRater/) | A tool to help users transfer user episode, show, and movie user ratings and watchlists from multiple media database sites around the web. |
+| [TvTimeToTrakt](https://github.com/lukearran/TvTimeToTrakt) | A tool to sync your TV Time watch history with Trakt.tv. |
+| [Plex Media Server](https://www.plex.tv/media-server-downloads/#plex-app) | A media server software to organize and stream your personal media collection. |
+| [Radarr](https://github.com/Radarr/Radarr) | A movie collection manager and downloader for various platforms. |
+| [Sonarr](https://github.com/Sonarr/Sonarr) | A TV show collection manager and downloader for various platforms. |
+| [Jackett](https://github.com/Jackett/Jackett) | A proxy server that provides API support for various torrent trackers commonly used with Radarr and Sonarr. |
+| [qBittorrent](https://github.com/qbittorrent/qBittorrent) | A free and open-source BitTorrent client. |
+| [Mullvad VPN](https://github.com/mullvad/mullvadvpn-app) | An open-source VPN client for Mullvad VPN service with port forwarding support. Great VPN for torrents. |
+| [Overseerr](https://github.com/sct/overseerr) | A request management and media discovery tool for your home media server. |
+| [FlareSolverr](https://github.com/FlareSolverr/FlareSolverr) | A reverse proxy solution to bypass Cloudflare protection and access websites commonly used with Jackett. |
+| [youtube-dl](https://github.com/ytdl-org/youtube-dl) | A command-line program to download videos from YouTube and other sites. |
```

### Comparing `TMDBTraktSyncer-1.1.7/README.md` & `TMDBTraktSyncer-1.1.8/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # TMDB-Trakt-Syncer
 
 This Python script syncs user watchlist and ratings for Movies, TV Shows, and Episodes both ways between [Trakt](https://trakt.tv/) and [TMDB](https://www.themoviedb.org/). Data already set will not be overwritten. Ratings are synced by default and watchlist sync is optional. The user will be prompted to enter their preferences and api keys on first run. 
 
-The script is compatible on any operating system that supports Python v3.6 or later, including Windows, Linux, Mac, and ChromeOS. If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
+The script is compatible on any operating system that supports Python v3.6 or later, including Windows, Linux, Mac, and ChromeOS. If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer). See below for my other [recommended projects](https://github.com/RileyXX/TMDB-Trakt-Syncer#other-recommended-projects).
 
 ## Installation Instructions:
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
 2. Install the script by running `python -m pip install TMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDbTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
    - Type of use: `Personal`
@@ -85,7 +85,33 @@
 ## Also Posted on:
 * [PyPi](https://pypi.org/project/TMDBTraktSyncer/)
 * [Reddit](https://www.reddit.com/r/trakt/comments/13jlu4r/tmdb_trakt_rating_syncer_tool_2_way_sync/)
 
 <br>
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+## Other Recommended Projects:
+
+| Project Name | Description |
+|--------------|-------------|
+| [PlexTraktSync](https://github.com/Taxel/PlexTraktSync) | A script that syncs user watch history and ratings between Trakt and Plex (without needing a PlexPass or Trakt VIP subscription). |
+| [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer) | A script that syncs user watchlist, ratings, and comments both ways between Trakt and IMDB. |
+| [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer) | A script that syncs user watchlist and ratings both ways between Trakt and TMDB. |
+| [PlexPreferNonForcedSubs](https://github.com/RileyXX/PlexPreferNonForcedSubs) | A script that sets all movies and shows in your local Plex library to English non-forced subtitles by default. |
+| [Casvt / PlexAutoDelete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py) | A script for automatically deleting watched content from Plex. |
+| [Netflix-to-Trakt-Import](https://github.com/jensb89/Netflix-to-Trakt-Import) | A tool to import your Netflix viewing history into Trakt. |
+| [trakt-tv-backup](https://darekkay.com/blog/trakt-tv-backup/) | A command-line tool for backing up your Trakt.tv data. |
+| [blacktwin / JBOPS](https://github.com/blacktwin/JBOPS) | A collection of scripts and tools for enhancing and automating tasks in Plex. |
+| [Casvt / Plex-scripts](https://github.com/Casvt/Plex-scripts) | A collection of useful scripts for Plex automation and management. |
+| [trakt---letterboxd-import](https://github.com/jensb89/trakt---letterboxd-import) | A tool to import your Letterboxd ratings and watchlist into Trakt. |
+| [TraktRater](https://github.com/damienhaynes/TraktRater/) | A tool to help users transfer user episode, show, and movie user ratings and watchlists from multiple media database sites around the web. |
+| [TvTimeToTrakt](https://github.com/lukearran/TvTimeToTrakt) | A tool to sync your TV Time watch history with Trakt.tv. |
+| [Plex Media Server](https://www.plex.tv/media-server-downloads/#plex-app) | A media server software to organize and stream your personal media collection. |
+| [Radarr](https://github.com/Radarr/Radarr) | A movie collection manager and downloader for various platforms. |
+| [Sonarr](https://github.com/Sonarr/Sonarr) | A TV show collection manager and downloader for various platforms. |
+| [Jackett](https://github.com/Jackett/Jackett) | A proxy server that provides API support for various torrent trackers commonly used with Radarr and Sonarr. |
+| [qBittorrent](https://github.com/qbittorrent/qBittorrent) | A free and open-source BitTorrent client. |
+| [Mullvad VPN](https://github.com/mullvad/mullvadvpn-app) | An open-source VPN client for Mullvad VPN service with port forwarding support. Great VPN for torrents. |
+| [Overseerr](https://github.com/sct/overseerr) | A request management and media discovery tool for your home media server. |
+| [FlareSolverr](https://github.com/FlareSolverr/FlareSolverr) | A reverse proxy solution to bypass Cloudflare protection and access websites commonly used with Jackett. |
+| [youtube-dl](https://github.com/ytdl-org/youtube-dl) | A command-line program to download videos from YouTube and other sites. |
```

### Comparing `TMDBTraktSyncer-1.1.7/TMDBTraktSyncer/TMDBTraktSyncer.py` & `TMDBTraktSyncer-1.1.8/TMDBTraktSyncer/TMDBTraktSyncer.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.7/TMDBTraktSyncer/errorHandling.py` & `TMDBTraktSyncer-1.1.8/TMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.7/TMDBTraktSyncer/tmdbData.py` & `TMDBTraktSyncer-1.1.8/TMDBTraktSyncer/tmdbData.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.7/TMDBTraktSyncer/traktData.py` & `TMDBTraktSyncer-1.1.8/TMDBTraktSyncer/traktData.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.7/TMDBTraktSyncer/verifyCredentials.py` & `TMDBTraktSyncer-1.1.8/TMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.7/TMDBTraktSyncer.egg-info/PKG-INFO` & `TMDBTraktSyncer-1.1.8/TMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.1.7
+Version: 1.1.8
 Summary: This python script syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
+Author: RileyXX
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # TMDB-Trakt-Syncer
 
 This Python script syncs user watchlist and ratings for Movies, TV Shows, and Episodes both ways between [Trakt](https://trakt.tv/) and [TMDB](https://www.themoviedb.org/). Data already set will not be overwritten. Ratings are synced by default and watchlist sync is optional. The user will be prompted to enter their preferences and api keys on first run. 
 
-The script is compatible on any operating system that supports Python v3.6 or later, including Windows, Linux, Mac, and ChromeOS. If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
+The script is compatible on any operating system that supports Python v3.6 or later, including Windows, Linux, Mac, and ChromeOS. If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer). See below for my other [recommended projects](https://github.com/RileyXX/TMDB-Trakt-Syncer#other-recommended-projects).
 
 ## Installation Instructions:
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
 2. Install the script by running `python -m pip install TMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDbTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
    - Type of use: `Personal`
@@ -100,7 +101,33 @@
 ## Also Posted on:
 * [PyPi](https://pypi.org/project/TMDBTraktSyncer/)
 * [Reddit](https://www.reddit.com/r/trakt/comments/13jlu4r/tmdb_trakt_rating_syncer_tool_2_way_sync/)
 
 <br>
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+## Other Recommended Projects:
+
+| Project Name | Description |
+|--------------|-------------|
+| [PlexTraktSync](https://github.com/Taxel/PlexTraktSync) | A script that syncs user watch history and ratings between Trakt and Plex (without needing a PlexPass or Trakt VIP subscription). |
+| [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer) | A script that syncs user watchlist, ratings, and comments both ways between Trakt and IMDB. |
+| [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer) | A script that syncs user watchlist and ratings both ways between Trakt and TMDB. |
+| [PlexPreferNonForcedSubs](https://github.com/RileyXX/PlexPreferNonForcedSubs) | A script that sets all movies and shows in your local Plex library to English non-forced subtitles by default. |
+| [Casvt / PlexAutoDelete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py) | A script for automatically deleting watched content from Plex. |
+| [Netflix-to-Trakt-Import](https://github.com/jensb89/Netflix-to-Trakt-Import) | A tool to import your Netflix viewing history into Trakt. |
+| [trakt-tv-backup](https://darekkay.com/blog/trakt-tv-backup/) | A command-line tool for backing up your Trakt.tv data. |
+| [blacktwin / JBOPS](https://github.com/blacktwin/JBOPS) | A collection of scripts and tools for enhancing and automating tasks in Plex. |
+| [Casvt / Plex-scripts](https://github.com/Casvt/Plex-scripts) | A collection of useful scripts for Plex automation and management. |
+| [trakt---letterboxd-import](https://github.com/jensb89/trakt---letterboxd-import) | A tool to import your Letterboxd ratings and watchlist into Trakt. |
+| [TraktRater](https://github.com/damienhaynes/TraktRater/) | A tool to help users transfer user episode, show, and movie user ratings and watchlists from multiple media database sites around the web. |
+| [TvTimeToTrakt](https://github.com/lukearran/TvTimeToTrakt) | A tool to sync your TV Time watch history with Trakt.tv. |
+| [Plex Media Server](https://www.plex.tv/media-server-downloads/#plex-app) | A media server software to organize and stream your personal media collection. |
+| [Radarr](https://github.com/Radarr/Radarr) | A movie collection manager and downloader for various platforms. |
+| [Sonarr](https://github.com/Sonarr/Sonarr) | A TV show collection manager and downloader for various platforms. |
+| [Jackett](https://github.com/Jackett/Jackett) | A proxy server that provides API support for various torrent trackers commonly used with Radarr and Sonarr. |
+| [qBittorrent](https://github.com/qbittorrent/qBittorrent) | A free and open-source BitTorrent client. |
+| [Mullvad VPN](https://github.com/mullvad/mullvadvpn-app) | An open-source VPN client for Mullvad VPN service with port forwarding support. Great VPN for torrents. |
+| [Overseerr](https://github.com/sct/overseerr) | A request management and media discovery tool for your home media server. |
+| [FlareSolverr](https://github.com/FlareSolverr/FlareSolverr) | A reverse proxy solution to bypass Cloudflare protection and access websites commonly used with Jackett. |
+| [youtube-dl](https://github.com/ytdl-org/youtube-dl) | A command-line program to download videos from YouTube and other sites. |
```

### Comparing `TMDBTraktSyncer-1.1.7/setup.py` & `TMDBTraktSyncer-1.1.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.1.7'
+VERSION = '1.1.8'
 DESCRIPTION = 'This python script syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.'
 
 # Setting up
 setup(
     name="TMDBTraktSyncer",
     version=VERSION,
+    author="RileyXX",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://github.com/RileyXX/TMDB-Trakt-Syncer",
     packages=find_packages(),
     install_requires=['requests'],
     keywords=['python', 'video', 'trakt', 'tmdb', 'ratings', 'sync', 'movies', 'tv shows'],
```

