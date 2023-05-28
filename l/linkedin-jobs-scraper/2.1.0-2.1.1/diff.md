# Comparing `tmp/linkedin-jobs-scraper-2.1.0.tar.gz` & `tmp/linkedin-jobs-scraper-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/linkedin-jobs-scraper-2.1.0.tar", last modified: Sun Apr 23 15:33:50 2023, max compression
+gzip compressed data, was "dist/linkedin-jobs-scraper-2.1.1.tar", last modified: Sun May 28 17:54:42 2023, max compression
```

## Comparing `linkedin-jobs-scraper-2.1.0.tar` & `linkedin-jobs-scraper-2.1.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:33:50.000000 linkedin-jobs-scraper-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    13367 2023-04-23 15:33:50.000000 linkedin-jobs-scraper-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:33:50.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:33:50.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/chrome_cdp/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/chrome_cdp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/chrome_cdp/cdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/chrome_cdp/cookie.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/chrome_cdp/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/chrome_cdp/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/chrome_cdp/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/chrome_cdp/target_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/chrome_cdp/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:33:50.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/events/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/events/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:33:50.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:33:50.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/filters/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    18234 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/linkedin_scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:33:50.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/query/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/query/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:33:50.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13870 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/strategies/anonymous_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    23067 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/strategies/authenticated_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/strategies/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:33:50.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/utils/chrome_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/utils/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/utils/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/utils/user_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:33:50.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13367 2023-04-23 15:33:49.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-23 15:33:50.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 15:33:49.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-23 15:33:49.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-23 15:33:49.000000 linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 15:33:50.000000 linkedin-jobs-scraper-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-23 15:30:30.000000 linkedin-jobs-scraper-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:54:42.000000 linkedin-jobs-scraper-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    13367 2023-05-28 17:54:42.000000 linkedin-jobs-scraper-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-05-28 17:51:37.000000 linkedin-jobs-scraper-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:54:42.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:54:42.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/chrome_cdp/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/chrome_cdp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/chrome_cdp/cdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/chrome_cdp/cookie.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/chrome_cdp/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/chrome_cdp/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/chrome_cdp/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/chrome_cdp/target_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/chrome_cdp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:54:42.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/events/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:54:42.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:54:42.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/filters/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18433 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/linkedin_scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:54:42.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/query/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:54:42.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13870 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/strategies/anonymous_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23066 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/strategies/authenticated_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/strategies/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:54:42.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/utils/chrome_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/utils/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/utils/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/utils/user_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:54:42.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13367 2023-05-28 17:54:41.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-28 17:54:42.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 17:54:41.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-28 17:54:41.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-28 17:54:41.000000 linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 17:54:42.000000 linkedin-jobs-scraper-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-28 17:51:38.000000 linkedin-jobs-scraper-2.1.1/setup.py
```

### Comparing `linkedin-jobs-scraper-2.1.0/PKG-INFO` & `linkedin-jobs-scraper-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkedin-jobs-scraper
-Version: 2.1.0
+Version: 2.1.1
 Summary: Scrape public available jobs on Linkedin using headless browser
 Home-page: https://github.com/spinlud/py-linkedin-jobs-scraper.git
 Author: Ludovico Fabbri
 Author-email: ludovico.fabbri@gmail.com
 License: UNKNOWN
 Description: # linkedin-jobs-scraper
         > Scrape public available jobs on Linkedin using headless browser.
```

### Comparing `linkedin-jobs-scraper-2.1.0/README.md` & `linkedin-jobs-scraper-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/chrome_cdp/cdp.py` & `linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/chrome_cdp/cdp.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/chrome_cdp/cookie.py` & `linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/chrome_cdp/cookie.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/chrome_cdp/request.py` & `linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/chrome_cdp/request.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/chrome_cdp/response.py` & `linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/chrome_cdp/response.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/chrome_cdp/target_info.py` & `linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/chrome_cdp/target_info.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/config.py` & `linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/config.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/events/events.py` & `linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/events/events.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/filters/filters.py` & `linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/filters/filters.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/linkedin_scraper.py` & `linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/linkedin_scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,17 +180,19 @@
                     # Block tracking and other stuff not useful
                     to_block = [
                         'li/track',
                         'realtime.www.linkedin.com/realtime',
                         'platform.linkedin.com/litms',
                         'linkedin.com/sensorCollect',
                         'linkedin.com/pixel/tracking',
+                        'linkedin.com/li/track',
                     ]
 
                     if any([e in request.url for e in to_block]):
+                        debug('[CDP]', 'Aborting request', str(request))
                         return request.abort()
 
                     # Block 3rd part domains requests
                     if domain not in {'linkedin.com', 'licdn.com'}:
                         return request.abort()
 
                     # If optimize is enabled, block other resource types
@@ -200,14 +202,15 @@
                             'stylesheet',
                             'media',
                             'font',
                             'imageset',
                         }
 
                         if request.resource_type.lower() in types_to_block:
+                            debug('[CDP]', 'Aborting request', str(request))
                             return request.abort()
 
                     # TODO: rotating proxy mode, only "working" in anonymous mode (discontinued)
                     if len(self._proxies) > 0 and not Config.LI_AT_COOKIE:
                         # Do not proxy request with non http(s) scheme
                         if 'http' not in urlparse(request.url).scheme.lower():
                             return request.resume()
```

### Comparing `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/query/query.py` & `linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/query/query.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/strategies/anonymous_strategy.py` & `linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/strategies/anonymous_strategy.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/strategies/authenticated_strategy.py` & `linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/strategies/authenticated_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 class Selectors(NamedTuple):
     container = '.jobs-search-results-list'
     chatPanel = '.msg-overlay-list-bubble'
     jobs = 'div.job-card-container'
     link = 'a.job-card-container__link'
     applyBtn = 'button.jobs-apply-button[role="link"]'
     title = '.artdeco-entity-lockup__title'
-    company = '.job-card-container__company-name'
+    company = '.artdeco-entity-lockup__subtitle'
     place = '.artdeco-entity-lockup__caption'
     date = 'time'
     description = '.jobs-description'
     detailsPanel = '.jobs-search__job-details--container'
     detailsTop = '.jobs-details-top-card'
     details = '.jobs-details__main-content'
     insights = '[class=jobs-unified-top-card__job-insight]'  # only one class
```

### Comparing `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/utils/chrome_driver.py` & `linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/utils/chrome_driver.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/utils/logger.py` & `linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/utils/logger.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/utils/url.py` & `linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/utils/url.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper/utils/user_agent.py` & `linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper/utils/user_agent.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper.egg-info/PKG-INFO` & `linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkedin-jobs-scraper
-Version: 2.1.0
+Version: 2.1.1
 Summary: Scrape public available jobs on Linkedin using headless browser
 Home-page: https://github.com/spinlud/py-linkedin-jobs-scraper.git
 Author: Ludovico Fabbri
 Author-email: ludovico.fabbri@gmail.com
 License: UNKNOWN
 Description: # linkedin-jobs-scraper
         > Scrape public available jobs on Linkedin using headless browser.
```

### Comparing `linkedin-jobs-scraper-2.1.0/linkedin_jobs_scraper.egg-info/SOURCES.txt` & `linkedin-jobs-scraper-2.1.1/linkedin_jobs_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-2.1.0/setup.py` & `linkedin-jobs-scraper-2.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='linkedin-jobs-scraper',
-    version='2.1.0',
+    version='2.1.1',
     author='Ludovico Fabbri',
     author_email='ludovico.fabbri@gmail.com',
     description='Scrape public available jobs on Linkedin using headless browser',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/spinlud/py-linkedin-jobs-scraper.git',
     packages=[
```

