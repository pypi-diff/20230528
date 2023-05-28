# Comparing `tmp/podcast_downloader-0.6.0.tar.gz` & `tmp/podcast_downloader-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podcast_downloader-0.6.0.tar", last modified: Sun May 21 16:49:31 2023, max compression
+gzip compressed data, was "podcast_downloader-0.6.1.tar", last modified: Sun May 28 07:06:07 2023, max compression
```

## Comparing `podcast_downloader-0.6.0.tar` & `podcast_downloader-0.6.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:49:31.198124 podcast_downloader-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-21 16:49:21.000000 podcast_downloader-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11282 2023-05-21 16:49:31.198124 podcast_downloader-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-05-21 16:49:21.000000 podcast_downloader-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:49:31.194124 podcast_downloader-0.6.0/podcast_downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 16:49:21.000000 podcast_downloader-0.6.0/podcast_downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-05-21 16:49:21.000000 podcast_downloader-0.6.0/podcast_downloader/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-21 16:49:21.000000 podcast_downloader-0.6.0/podcast_downloader/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-21 16:49:21.000000 podcast_downloader-0.6.0/podcast_downloader/downloaded.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-21 16:49:21.000000 podcast_downloader-0.6.0/podcast_downloader/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-21 16:49:21.000000 podcast_downloader-0.6.0/podcast_downloader/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-21 16:49:21.000000 podcast_downloader-0.6.0/podcast_downloader/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:49:31.198124 podcast_downloader-0.6.0/podcast_downloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11282 2023-05-21 16:49:31.000000 podcast_downloader-0.6.0/podcast_downloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-21 16:49:31.000000 podcast_downloader-0.6.0/podcast_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 16:49:31.000000 podcast_downloader-0.6.0/podcast_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-21 16:49:31.000000 podcast_downloader-0.6.0/podcast_downloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-21 16:49:31.000000 podcast_downloader-0.6.0/podcast_downloader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 16:49:31.198124 podcast_downloader-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-21 16:49:21.000000 podcast_downloader-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 07:06:07.251380 podcast_downloader-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-28 07:05:45.000000 podcast_downloader-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-05-28 07:06:07.251380 podcast_downloader-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-05-28 07:05:45.000000 podcast_downloader-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 07:06:07.251380 podcast_downloader-0.6.1/podcast_downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 07:05:45.000000 podcast_downloader-0.6.1/podcast_downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-05-28 07:05:45.000000 podcast_downloader-0.6.1/podcast_downloader/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-28 07:05:45.000000 podcast_downloader-0.6.1/podcast_downloader/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-28 07:05:45.000000 podcast_downloader-0.6.1/podcast_downloader/downloaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-28 07:05:45.000000 podcast_downloader-0.6.1/podcast_downloader/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-28 07:05:45.000000 podcast_downloader-0.6.1/podcast_downloader/rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-28 07:05:45.000000 podcast_downloader-0.6.1/podcast_downloader/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 07:06:07.251380 podcast_downloader-0.6.1/podcast_downloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-05-28 07:06:07.000000 podcast_downloader-0.6.1/podcast_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-28 07:06:07.000000 podcast_downloader-0.6.1/podcast_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 07:06:07.000000 podcast_downloader-0.6.1/podcast_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-28 07:06:07.000000 podcast_downloader-0.6.1/podcast_downloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-28 07:06:07.000000 podcast_downloader-0.6.1/podcast_downloader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 07:06:07.251380 podcast_downloader-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-28 07:05:45.000000 podcast_downloader-0.6.1/setup.py
```

### Comparing `podcast_downloader-0.6.0/LICENSE` & `podcast_downloader-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `podcast_downloader-0.6.0/PKG-INFO` & `podcast_downloader-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podcast_downloader
-Version: 0.6.0
+Version: 0.6.1
 Summary: The script for downloading the recent mp3 from given RSS channels
 Home-page: https://github.com/dplocki/podcast-downloader
 Author: Dawid Plocki
 Author-email: dawid.plocki@gmail.com
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
@@ -15,14 +15,15 @@
 License-File: LICENSE
 
 # Podcast Downloader
 
 ![GitHub](https://img.shields.io/github/license/dplocki/podcast-downloader)
 ![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fdplocki%2Fpodcast-downloader%2Fbadge%3Fref%3Dmaster&style=flat)
 ![PyPI](https://img.shields.io/pypi/v/podcast-downloader)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 The Python module for downloading files from given RSS feeds.
 It is not using database of any sort. It require configuration file.
 
 The script is analyzing the directory where it put the previously downloaded files.
 It is compering the last added file with the rss feed, finding the missing ones, and downloading them.
 
@@ -59,15 +60,15 @@
 
 ## Configuration
 
 ### The configuration file
 
 The configuration file is placed in home directory.
 
-The name: `.podcast_downloader_config.json`. The file is format in [JSON](https://en.wikipedia.org/wiki/JSON).
+The name: `.podcast_downloader_config.json`. The file is format in [JSON](https://en.wikipedia.org/wiki/JSON). The expected encoding is [utf-8](https://en.wikipedia.org/wiki/UTF-8).
 
 ### The settings hierarchy
 
 The script will replace default values by read from configuration file.
 Those will be cover by all values given by command line.
 
 ```
```

### Comparing `podcast_downloader-0.6.0/README.md` & `podcast_downloader-0.6.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Podcast Downloader
 
 ![GitHub](https://img.shields.io/github/license/dplocki/podcast-downloader)
 ![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fdplocki%2Fpodcast-downloader%2Fbadge%3Fref%3Dmaster&style=flat)
 ![PyPI](https://img.shields.io/pypi/v/podcast-downloader)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 The Python module for downloading files from given RSS feeds.
 It is not using database of any sort. It require configuration file.
 
 The script is analyzing the directory where it put the previously downloaded files.
 It is compering the last added file with the rss feed, finding the missing ones, and downloading them.
 
@@ -43,15 +44,15 @@
 
 ## Configuration
 
 ### The configuration file
 
 The configuration file is placed in home directory.
 
-The name: `.podcast_downloader_config.json`. The file is format in [JSON](https://en.wikipedia.org/wiki/JSON).
+The name: `.podcast_downloader_config.json`. The file is format in [JSON](https://en.wikipedia.org/wiki/JSON). The expected encoding is [utf-8](https://en.wikipedia.org/wiki/UTF-8).
 
 ### The settings hierarchy
 
 The script will replace default values by read from configuration file.
 Those will be cover by all values given by command line.
 
 ```
```

### Comparing `podcast_downloader-0.6.0/podcast_downloader/__main__.py` & `podcast_downloader-0.6.1/podcast_downloader/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from podcast_downloader.configuration import (
     configuration_verification,
     get_label_to_date,
     get_n_age_date,
     parse_day_label,
 )
-from .utils import log, compose, log_error, warning
+from .utils import ConsoleOutputFormatter, compose
 from .downloaded import get_downloaded_files, get_extensions_checker
 from .parameters import merge_parameters_collection, load_configuration_file, parse_argv
 from .rss import (
     RSSEntity,
     build_only_allowed_filter_for_link_data,
     build_only_new_entities,
     file_template_to_file_name,
@@ -42,20 +42,19 @@
     try:
         request = urllib.request.Request(rss_entity.link, headers=headers)
 
         with urllib.request.urlopen(request) as response:
             with open(path_to_file, "wb") as file:
                 file.write(response.read())
 
-    except Exception as exception:
-        log_error(
-            'The podcast file "{}" could not be saved to disk "{}" due to the following error:\n{}',
+    except Exception:
+        logger.exception(
+            'The podcast file "%s" could not be saved to disk "%s" due to the following error',
             rss_entity.link,
             path_to_file,
-            exception,
         )
 
 
 def build_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser()
 
     parser.add_argument(
@@ -119,48 +118,55 @@
         default_file_name_template_with_date = (
             "[%publish_date%] %file_name%.%file_extension%"
         )
 
         if sub_configuration[configuration.CONFIG_PODCASTS_REQUIRE_DATE]:
             configuration_value = default_file_name_template_with_date
 
-        warning(
-            'The option {} is deprecated, please replace use of it with the {} option: "{}"',
+        logger.warning(
+            'The option %s is deprecated, please replace use of it with the %s option: "%s"',
             configuration.CONFIG_PODCASTS_REQUIRE_DATE,
             configuration.CONFIG_FILE_NAME_TEMPLATE,
             default_file_name_template_with_date,
         )
 
     return partial(file_template_to_file_name, configuration_value)
 
 
 if __name__ == "__main__":
     import sys
+    from logging import getLogger, StreamHandler, INFO
+
+    logger = getLogger(__name__)
+    logger.setLevel(INFO)
+    stdout_handler = StreamHandler()
+    stdout_handler.setFormatter(ConsoleOutputFormatter())
+    logger.addHandler(stdout_handler)
 
     DEFAULT_CONFIGURATION = {
         configuration.CONFIG_DOWNLOADS_LIMIT: sys.maxsize,
         configuration.CONFIG_IF_DIRECTORY_EMPTY: "download_last",
         configuration.CONFIG_PODCAST_EXTENSIONS: {".mp3": "audio/mpeg"},
         configuration.CONFIG_FILE_NAME_TEMPLATE: "%file_name%.%file_extension%",
         configuration.CONFIG_HTTP_HEADER: {"User-Agent": "podcast-downloader"},
         configuration.CONFIG_PODCASTS: [],
     }
 
     CONFIG_FILE = "~/.podcast_downloader_config.json"
-    log('Loading configuration (from file: "{}")', CONFIG_FILE)
+    logger.info('Loading configuration (from file: "%s")', CONFIG_FILE)
 
     CONFIGURATION = merge_parameters_collection(
         DEFAULT_CONFIGURATION,
         load_configuration_file(os.path.expanduser(CONFIG_FILE)),
         parse_argv(build_parser()),
     )
 
     is_valid, error = configuration_verification(CONFIGURATION)
     if not is_valid:
-        log("There is a problem with configuration file: {}", error)
+        logger.info("There is a problem with configuration file: %s", error)
         exit(1)
 
     RSS_SOURCES = CONFIGURATION[configuration.CONFIG_PODCASTS]
     DOWNLOADS_LIMITS = CONFIGURATION[configuration.CONFIG_DOWNLOADS_LIMIT]
 
     for rss_source in RSS_SOURCES:
         file_length_limit = get_system_file_name_limit(rss_source)
@@ -184,18 +190,18 @@
         )
         rss_https_header = merge_parameters_collection(
             CONFIGURATION[configuration.CONFIG_HTTP_HEADER],
             rss_source.get(configuration.CONFIG_HTTP_HEADER, {}),
         )
 
         if rss_disable:
-            log('Skipping the "{}"', rss_source_name)
+            logger.info('Skipping the "%s"', rss_source_name)
             continue
 
-        log('Checking "{}"', rss_source_name)
+        logger.info('Checking "%s"', rss_source_name)
 
         to_name_function = configuration_to_function_rss_to_name(
             rss_file_name_template_value, rss_source
         )
         on_directory_empty = configuration_to_function_on_empty_directory(
             rss_if_directory_empty
         )
@@ -218,15 +224,15 @@
             list,
             download_limiter_function,
             partial(filter, build_only_allowed_filter_for_link_data(allow_link_types)),
             flatten_rss_links_data,
             get_raw_rss_entries_from_web,
         )(rss_source_link)
 
-        log('Last downloaded file "{}"', last_downloaded_file or "<none>")
+        logger.info('Last downloaded file "%s"', last_downloaded_file or "<none>")
 
         if missing_files_links:
             to_real_podcast_file_name = compose(
                 partial(limit_file_name, file_length_limit), to_name_function
             )
 
             download_podcast = partial(
@@ -240,27 +246,25 @@
                 if wanted_podcast_file_name in downloaded_files:
                     continue
 
                 if DOWNLOADS_LIMITS == 0:
                     continue
 
                 if len(wanted_podcast_file_name) > file_length_limit:
-                    warning(
-                        'Your system cannot support the full podcast file name "{}". The name will be shortened',
+                    logger.info(
+                        'Your system cannot support the full podcast file name "%s". The name will be shortened',
                         wanted_podcast_file_name,
                     )
 
-                log(
-                    '{}: Downloading file: "{}" saved as "{}"',
+                logger.info(
+                    '%s: Downloading file: "%s" saved as "%s"',
                     rss_source_name,
                     rss_entry.link,
                     to_real_podcast_file_name(rss_entry),
                 )
 
                 download_podcast(rss_source_path, rss_entry)
                 DOWNLOADS_LIMITS -= 1
         else:
-            log("{}: Nothing new", rss_source_name)
-
-        log("-" * 30)
+            logger.info("%s: Nothing new", rss_source_name)
 
-    log("Finished")
+    logger.info("Finished")
```

### Comparing `podcast_downloader-0.6.0/podcast_downloader/configuration.py` & `podcast_downloader-0.6.1/podcast_downloader/configuration.py`

 * *Files identical despite different names*

### Comparing `podcast_downloader-0.6.0/podcast_downloader/downloaded.py` & `podcast_downloader-0.6.1/podcast_downloader/downloaded.py`

 * *Files identical despite different names*

### Comparing `podcast_downloader-0.6.0/podcast_downloader/rss.py` & `podcast_downloader-0.6.1/podcast_downloader/rss.py`

 * *Files identical despite different names*

### Comparing `podcast_downloader-0.6.0/podcast_downloader.egg-info/PKG-INFO` & `podcast_downloader-0.6.1/podcast_downloader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podcast-downloader
-Version: 0.6.0
+Version: 0.6.1
 Summary: The script for downloading the recent mp3 from given RSS channels
 Home-page: https://github.com/dplocki/podcast-downloader
 Author: Dawid Plocki
 Author-email: dawid.plocki@gmail.com
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
@@ -15,14 +15,15 @@
 License-File: LICENSE
 
 # Podcast Downloader
 
 ![GitHub](https://img.shields.io/github/license/dplocki/podcast-downloader)
 ![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fdplocki%2Fpodcast-downloader%2Fbadge%3Fref%3Dmaster&style=flat)
 ![PyPI](https://img.shields.io/pypi/v/podcast-downloader)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 The Python module for downloading files from given RSS feeds.
 It is not using database of any sort. It require configuration file.
 
 The script is analyzing the directory where it put the previously downloaded files.
 It is compering the last added file with the rss feed, finding the missing ones, and downloading them.
 
@@ -59,15 +60,15 @@
 
 ## Configuration
 
 ### The configuration file
 
 The configuration file is placed in home directory.
 
-The name: `.podcast_downloader_config.json`. The file is format in [JSON](https://en.wikipedia.org/wiki/JSON).
+The name: `.podcast_downloader_config.json`. The file is format in [JSON](https://en.wikipedia.org/wiki/JSON). The expected encoding is [utf-8](https://en.wikipedia.org/wiki/UTF-8).
 
 ### The settings hierarchy
 
 The script will replace default values by read from configuration file.
 Those will be cover by all values given by command line.
 
 ```
```

### Comparing `podcast_downloader-0.6.0/setup.py` & `podcast_downloader-0.6.1/setup.py`

 * *Files identical despite different names*

