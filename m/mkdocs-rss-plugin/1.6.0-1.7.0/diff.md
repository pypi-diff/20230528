# Comparing `tmp/mkdocs-rss-plugin-1.6.0.tar.gz` & `tmp/mkdocs-rss-plugin-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-rss-plugin-1.6.0.tar", last modified: Tue Feb 21 22:10:30 2023, max compression
+gzip compressed data, was "mkdocs-rss-plugin-1.7.0.tar", last modified: Sun May 28 15:15:13 2023, max compression
```

## Comparing `mkdocs-rss-plugin-1.6.0.tar` & `mkdocs-rss-plugin-1.7.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 22:10:30.651740 mkdocs-rss-plugin-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-02-21 22:10:09.000000 mkdocs-rss-plugin-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-21 22:10:09.000000 mkdocs-rss-plugin-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-02-21 22:10:30.651740 mkdocs-rss-plugin-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-02-21 22:10:09.000000 mkdocs-rss-plugin-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 22:10:30.643740 mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-02-21 22:10:09.000000 mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 22:10:09.000000 mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-02-21 22:10:09.000000 mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin/customtypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 22:10:30.647740 mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin/git_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 22:10:09.000000 mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin/git_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-02-21 22:10:09.000000 mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin/git_manager/ci.py
--rw-r--r--   0 runner    (1001) docker     (123)    13949 2023-02-21 22:10:09.000000 mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 22:10:30.647740 mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-02-21 22:10:09.000000 mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin/templates/rss.xml.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-02-21 22:10:09.000000 mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin/timezoner_pre39.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-02-21 22:10:09.000000 mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin/timezoner_py39.py
--rw-r--r--   0 runner    (1001) docker     (123)    23261 2023-02-21 22:10:09.000000 mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 22:10:30.647740 mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-02-21 22:10:30.000000 mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-02-21 22:10:30.000000 mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 22:10:30.000000 mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-21 22:10:30.000000 mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-02-21 22:10:30.000000 mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-21 22:10:30.000000 mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-02-21 22:10:30.651740 mkdocs-rss-plugin-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-02-21 22:10:09.000000 mkdocs-rss-plugin-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 22:10:30.651740 mkdocs-rss-plugin-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    19935 2023-02-21 22:10:09.000000 mkdocs-rss-plugin-1.6.0/tests/test_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-02-21 22:10:09.000000 mkdocs-rss-plugin-1.6.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-02-21 22:10:09.000000 mkdocs-rss-plugin-1.6.0/tests/test_rss_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-02-21 22:10:09.000000 mkdocs-rss-plugin-1.6.0/tests/test_timezoner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:15:13.102958 mkdocs-rss-plugin-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-05-28 15:15:13.102958 mkdocs-rss-plugin-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:15:13.102958 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/customtypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:15:13.102958 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/git_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/git_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/git_manager/ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13939 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:15:13.102958 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/templates/rss.xml.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/timezoner_pre39.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/timezoner_py39.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23320 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:15:13.102958 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-05-28 15:15:13.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-28 15:15:13.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 15:15:13.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-28 15:15:13.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-28 15:15:13.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-28 15:15:13.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-28 15:15:13.102958 mkdocs-rss-plugin-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:15:13.102958 mkdocs-rss-plugin-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21020 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/tests/test_rss_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/tests/test_timezoner.py
```

### Comparing `mkdocs-rss-plugin-1.6.0/LICENSE` & `mkdocs-rss-plugin-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-rss-plugin-1.6.0/PKG-INFO` & `mkdocs-rss-plugin-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-rss-plugin
-Version: 1.6.0
+Version: 1.7.0
 Summary: MkDocs plugin which generates a static RSS feed using git log and page.meta.
 Author: Julien Moura
 Author-email: dev@ingeoveritas.com
 License: MIT
 Project-URL: Docs, https://guts.github.io/mkdocs-rss-plugin/
 Project-URL: Bug Reports, https://github.com/Guts/mkdocs-rss-plugin/issues/
 Project-URL: Source, https://github.com/Guts/mkdocs-rss-plugin/
@@ -63,14 +63,15 @@
 
 Full options:
 
 ```yaml
 plugins:
   - rss:
       abstract_chars_count: 160  # -1 for full content
+      abstract_delimiter: <!-- more -->
       categories:
         - tags
       comments_path: "#__comments"
       date_from_meta:
         as_creation: "date"
         as_update: false
         datetime_format: "%Y-%m-%d %H:%M"
```

### Comparing `mkdocs-rss-plugin-1.6.0/README.md` & `mkdocs-rss-plugin-1.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
 Full options:
 
 ```yaml
 plugins:
   - rss:
       abstract_chars_count: 160  # -1 for full content
+      abstract_delimiter: <!-- more -->
       categories:
         - tags
       comments_path: "#__comments"
       date_from_meta:
         as_creation: "date"
         as_update: false
         datetime_format: "%Y-%m-%d %H:%M"
```

### Comparing `mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin/__about__.py` & `mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/__about__.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,24 +26,24 @@
     "__title_clean__",
     "__uri__",
     "__version__",
     "__version_info__",
 ]
 
 __author__ = "Julien Moura"
-__copyright__ = "2020 - {0}, {1}".format(date.today().year, __author__)
+__copyright__ = f"2020 - {date.today().year}, {__author__}"
 __email__ = "dev@ingeoveritas.com"
 __license__ = "MIT"
 __summary__ = (
     "MkDocs plugin which generates a static RSS feed using git log and page.meta."
 )
 __title__ = "MkDocs RSS plugin"
 __title_clean__ = "".join(e for e in __title__ if e.isalnum())
 __uri__ = "https://github.com/Guts/mkdocs-rss-plugin/"
 
-__version__ = "1.6.0"
+__version__ = "1.7.0"
 __version_info__ = tuple(
     [
         int(num) if num.isdigit() else num
         for num in __version__.replace("-", ".", 1).split(".")
     ]
 )
```

### Comparing `mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin/customtypes.py` & `mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/customtypes.py`

 * *Files identical despite different names*

### Comparing `mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin/git_manager/ci.py` & `mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/git_manager/ci.py`

 * *Files identical despite different names*

### Comparing `mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin/plugin.py` & `mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         # start a feed dictionary using global config vars
         base_feed = {
             "author": config.get("site_author", None),
             "buildDate": formatdate(get_build_timestamp()),
             "copyright": config.get("copyright", None),
             "description": config.get("site_description", None),
             "entries": [],
-            "generator": "{} - v{}".format(__title__, __version__),
+            "generator": f"{__title__} - v{__version__}",
             "html_url": self.util.get_site_url(config),
             "language": self.util.guess_locale(config),
             "pubDate": formatdate(get_build_timestamp()),
             "repo_url": config.get("repo_url", config.get("site_url", None)),
             "title": config.get("site_name", None),
             "ttl": self.config.get("feed_ttl", None),
         }
```

### Comparing `mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin/templates/rss.xml.jinja2` & `mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/templates/rss.xml.jinja2`

 * *Files identical despite different names*

### Comparing `mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin/timezoner_pre39.py` & `mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/timezoner_pre39.py`

 * *Files identical despite different names*

### Comparing `mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin/timezoner_py39.py` & `mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/timezoner_py39.py`

 * *Files identical despite different names*

### Comparing `mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin/util.py` & `mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 # ############################################################################
 # ########## Globals #############
 # ################################
 
 REMOTE_REQUEST_HEADERS = {
     "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8",
-    "User-Agent": "{}/{}".format(__about__.__title__, __about__.__version__),
+    "User-Agent": f"{__about__.__title__}/{__about__.__version__}",
 }
 
 logger = logging.getLogger("mkdocs.mkdocs_rss_plugin")
 
 
 # ############################################################################
 # ########## Classes #############
@@ -397,15 +397,15 @@
         elif in_page.markdown:
             if chars_count is None or len(in_page.markdown) < chars_count:
                 return markdown.markdown(
                     in_page.markdown[:chars_count], output_format="html5"
                 )
             else:
                 return markdown.markdown(
-                    "{}...".format(in_page.markdown[: chars_count - 3]),
+                    f"{in_page.markdown[: chars_count - 3]}...",
                     output_format="html5",
                 )
         # Unlimited chars_count but no content is found, then return the description.
         else:
             return description if description else ""
 
     def get_image(self, in_page: Page, base_url: str) -> tuple:
@@ -416,17 +416,17 @@
         :param base_url: website URL to resolve absolute URLs for images referenced with local path.
         :type base_url: str
 
         :return: (image url, mime type, image length)
         :rtype: tuple
         """
         if in_page.meta.get("image"):
-            img_url = in_page.meta.get("image")
+            img_url = in_page.meta.get("image").strip()
         elif in_page.meta.get("illustration"):
-            img_url = in_page.meta.get("illustration")
+            img_url = in_page.meta.get("illustration").strip()
         else:
             return None
 
         # guess mimetype
         mime_type = guess_type(url=img_url, strict=False)[0]
 
         # if path, resolve absolute url
@@ -556,15 +556,16 @@
         # MkDocs locale settings - might be added in future mkdocs versions
         # see: https://github.com/timvink/mkdocs-git-revision-date-localized-plugin/issues/24
         if mkdocs_config.get("locale"):
             return mkdocs_config.get("locale")
 
         # Some themes implement a locale or a language setting
         if "theme" in mkdocs_config and "locale" in mkdocs_config.get("theme"):
-            return mkdocs_config.get("theme")._vars.get("locale")
+            locale = mkdocs_config.get("theme")._vars.get("locale")
+            return f"{locale.language}-{locale.territory}"
         elif "theme" in mkdocs_config and "language" in mkdocs_config.get("theme"):
             return mkdocs_config.get("theme")._vars.get("language")
         else:
             return None
 
     @staticmethod
     def filter_pages(pages: list, attribute: str, length: int) -> list:
```

### Comparing `mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin.egg-info/PKG-INFO` & `mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-rss-plugin
-Version: 1.6.0
+Version: 1.7.0
 Summary: MkDocs plugin which generates a static RSS feed using git log and page.meta.
 Author: Julien Moura
 Author-email: dev@ingeoveritas.com
 License: MIT
 Project-URL: Docs, https://guts.github.io/mkdocs-rss-plugin/
 Project-URL: Bug Reports, https://github.com/Guts/mkdocs-rss-plugin/issues/
 Project-URL: Source, https://github.com/Guts/mkdocs-rss-plugin/
@@ -63,14 +63,15 @@
 
 Full options:
 
 ```yaml
 plugins:
   - rss:
       abstract_chars_count: 160  # -1 for full content
+      abstract_delimiter: <!-- more -->
       categories:
         - tags
       comments_path: "#__comments"
       date_from_meta:
         as_creation: "date"
         as_update: false
         datetime_format: "%Y-%m-%d %H:%M"
```

### Comparing `mkdocs-rss-plugin-1.6.0/mkdocs_rss_plugin.egg-info/SOURCES.txt` & `mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-rss-plugin-1.6.0/setup.cfg` & `mkdocs-rss-plugin-1.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `mkdocs-rss-plugin-1.6.0/setup.py` & `mkdocs-rss-plugin-1.7.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     author_email=__about__.__email__,
     description=__about__.__summary__,
     license=__about__.__license__,
     long_description=README,
     long_description_content_type="text/markdown",
     project_urls={
         "Docs": "https://guts.github.io/mkdocs-rss-plugin/",
-        "Bug Reports": "{}issues/".format(__about__.__uri__),
+        "Bug Reports": f"{__about__.__uri__}issues/",
         "Source": __about__.__uri__,
     },
     # packaging
     packages=find_packages(
         exclude=["contrib", "docs", "*.tests", "*.tests.*", "tests.*", "tests"]
     ),
     include_package_data=True,
```

### Comparing `mkdocs-rss-plugin-1.6.0/tests/test_build.py` & `mkdocs-rss-plugin-1.7.0/tests/test_build.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,28 +54,28 @@
         """Executed after each test."""
         pass
 
     @classmethod
     def tearDownClass(cls):
         """Executed after the last test."""
         # In case of some tests failure, ensure that everything is cleaned up
-        temp_page = Path("tests/fixtures/docs/temp_page_not_in_git_log.md")
+        # temp_page = Path("tests/fixtures/docs/temp_page_not_in_git_log.md")
         # if temp_page.exists():
         #     temp_page.unlink()
 
         git_dir = Path("_git")
         if git_dir.exists():
             git_dir.replace(git_dir.with_name(".git"))
 
     # -- TESTS ---------------------------------------------------------
     def test_simple_build(self):
         with tempfile.TemporaryDirectory() as tmpdirname:
             cli_result = self.build_docs_setup(
                 testproject_path="docs",
-                mkdocs_yml_filepath=Path("mkdocs.yml"),
+                mkdocs_yml_filepath=Path("tests/fixtures/mkdocs_simple.yml"),
                 output_path=tmpdirname,
                 strict=False,
             )
 
             if cli_result.exception is not None:
                 e = cli_result.exception
                 logger.debug(format_exception(type(e), e, e.__traceback__))
@@ -326,14 +326,40 @@
                     "Page without meta with short text",
                     "Blog sample",
                 ):
                     self.assertGreaterEqual(
                         len(feed_item.description), 150, feed_item.title
                     )
 
+    def test_simple_build_lang_with_territory(self):
+        with tempfile.TemporaryDirectory() as tmpdirname:
+            cli_result = self.build_docs_setup(
+                testproject_path="docs",
+                mkdocs_yml_filepath=Path(
+                    "tests/fixtures/mkdocs_lang_with_territory.yml"
+                ),
+                output_path=tmpdirname,
+                strict=True,
+            )
+
+            if cli_result.exception is not None:
+                e = cli_result.exception
+                logger.debug(format_exception(type(e), e, e.__traceback__))
+
+            self.assertEqual(cli_result.exit_code, 0)
+            self.assertIsNone(cli_result.exception)
+
+            # created items
+            feed_parsed = feedparser.parse(Path(tmpdirname) / "feed_rss_created.xml")
+            self.assertEqual(feed_parsed.feed.get("language"), "en-US")
+
+            # updated items
+            feed_parsed = feedparser.parse(Path(tmpdirname) / "feed_rss_updated.xml")
+            self.assertEqual(feed_parsed.feed.get("language"), "en-US")
+
     def test_simple_build_pretty_print_enabled(self):
         with tempfile.TemporaryDirectory() as tmpdirname:
             cli_result = self.build_docs_setup(
                 testproject_path="docs",
                 mkdocs_yml_filepath=Path(
                     "tests/fixtures/mkdocs_pretty_print_enabled.yml"
                 ),
```

### Comparing `mkdocs-rss-plugin-1.6.0/tests/test_config.py` & `mkdocs-rss-plugin-1.7.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mkdocs-rss-plugin-1.6.0/tests/test_rss_util.py` & `mkdocs-rss-plugin-1.7.0/tests/test_rss_util.py`

 * *Files identical despite different names*

### Comparing `mkdocs-rss-plugin-1.6.0/tests/test_timezoner.py` & `mkdocs-rss-plugin-1.7.0/tests/test_timezoner.py`

 * *Files identical despite different names*

