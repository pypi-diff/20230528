# Comparing `tmp/alpha-filter-0.9.tar.gz` & `tmp/alpha-filter-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpha-filter-0.9.tar", last modified: Sun Apr 30 11:19:15 2023, max compression
+gzip compressed data, was "alpha-filter-0.9.1.tar", last modified: Sun May 28 13:17:45 2023, max compression
```

## Comparing `alpha-filter-0.9.tar` & `alpha-filter-0.9.1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 11:19:15.605029 alpha-filter-0.9/
--rw-rw-rw-   0        0        0     1607 2023-04-30 11:19:15.604031 alpha-filter-0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1453 2023-04-29 23:39:58.000000 alpha-filter-0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 11:19:15.603030 alpha-filter-0.9/alpha_filter.egg-info/
--rw-rw-rw-   0        0        0     1607 2023-04-30 11:19:15.000000 alpha-filter-0.9/alpha_filter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-04-30 11:19:15.000000 alpha-filter-0.9/alpha_filter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 11:19:15.000000 alpha-filter-0.9/alpha_filter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-30 11:19:15.000000 alpha-filter-0.9/alpha_filter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4683 2023-04-29 23:05:36.000000 alpha-filter-0.9/alphafilter.py
--rw-rw-rw-   0        0        0       42 2023-04-30 11:19:15.605029 alpha-filter-0.9/setup.cfg
--rw-rw-rw-   0        0        0      353 2023-04-30 11:18:54.000000 alpha-filter-0.9/setup.py
+drwxrwxr-x   0 yllen     (1000) yllen     (1000)        0 2023-05-28 13:17:45.423551 alpha-filter-0.9.1/
+-rw-rw-r--   0 yllen     (1000) yllen     (1000)      172 2023-05-28 13:17:45.423551 alpha-filter-0.9.1/PKG-INFO
+-rw-rw-r--   0 yllen     (1000) yllen     (1000)     1764 2023-05-28 13:10:31.000000 alpha-filter-0.9.1/README.md
+drwxrwxr-x   0 yllen     (1000) yllen     (1000)        0 2023-05-28 13:17:45.423551 alpha-filter-0.9.1/alpha_filter.egg-info/
+-rw-rw-r--   0 yllen     (1000) yllen     (1000)      172 2023-05-28 13:17:45.000000 alpha-filter-0.9.1/alpha_filter.egg-info/PKG-INFO
+-rw-rw-r--   0 yllen     (1000) yllen     (1000)      162 2023-05-28 13:17:45.000000 alpha-filter-0.9.1/alpha_filter.egg-info/SOURCES.txt
+-rw-rw-r--   0 yllen     (1000) yllen     (1000)        1 2023-05-28 13:17:45.000000 alpha-filter-0.9.1/alpha_filter.egg-info/dependency_links.txt
+-rw-rw-r--   0 yllen     (1000) yllen     (1000)       13 2023-05-28 13:17:45.000000 alpha-filter-0.9.1/alpha_filter.egg-info/top_level.txt
+-rw-rw-r--   0 yllen     (1000) yllen     (1000)       38 2023-05-28 13:17:45.423551 alpha-filter-0.9.1/setup.cfg
+-rw-rw-r--   0 yllen     (1000) yllen     (1000)      184 2023-05-28 11:52:34.000000 alpha-filter-0.9.1/setup.py
```

### Comparing `alpha-filter-0.9/PKG-INFO` & `alpha-filter-0.9.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,55 @@
-Metadata-Version: 2.1
-Name: alpha-filter
-Version: 0.9
-Summary: differential filter
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
-[![Python 3.6](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-360/) _and greater_
-
-# alpha-filter
-
-When parsing, sometimes it is necessary to reduce the number of requests to the server, for example, our script collects links from pagination to the product every day, and then parses each product separately. But what to do if some time ago we already parsed these goods, why do it twice. alpha-filter will help filter out those ads that have already been read, and will return only new ones.
- 
-## Getting starting
-```sh
-pip install alpha-filter
-```
-
-### Usage
-
-```python
-from alphafilter import filter_ads
-
-first_parsing_urls = ["https://www.example.com/1", "https://www.example.com/2"]
-new, old = filter_ads(first_parsing_urls)
-new = ["https://www.example.com/1", "https://www.example.com/2"]
-old = []
-
-second_parsing_urls = first_parsing_urls # second parsing same with first
-
-new, old = filter_ads(second_parsing_urls)
-new = []
-old = []
-
-third_parsing_urls = ["https://www.example.com/2", "https://www.example.com/3"]
-
-new, old = filter_ads(third_parsing_urls)
-new = ["https://www.example.com/3"]
-old = ["https://www.example.com/2"]
-```
-It uses a fast sqlite database to store urls. The database file ('ads.db') will be created in the root directory
-
-__Warning!!! this package has no protection against sql injection, do not use it for the external interface__
+[![Python 3.6](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-360/) _and greater_
+
+# alpha-filter
+
+When parsing, sometimes it is necessary to reduce the number of requests to the server, for example, our script collects links from pagination to the product every day, and then parses each product separately. But what to do if some time ago we already parsed these goods, why do it twice. alpha-filter will help filter out those ads that have already been read, and will return only new ones.
+ 
+## Getting starting
+```sh
+pip install alpha-filter
+```
+
+### Usage
+
+```python
+from alphafilter import filter_ads, mark_as_processed, is_processed
+
+>>> first_parsing_urls = ["https://www.example.com/1", "https://www.example.com/2"]
+>>> new, old = filter_ads(first_parsing_urls)
+>>> new
+["https://www.example.com/1", "https://www.example.com/2"]
+>>> old
+[]
+
+second_parsing_urls = first_parsing_urls # second parsing same with first
+
+>>> new, old = filter_ads(second_parsing_urls)
+>>> new
+[]
+>>> old
+[]
+
+>>>third_parsing_urls = ["https://www.example.com/2", "https://www.example.com/3"]
+
+>>> new, old = filter_ads(third_parsing_urls)
+>>> new
+["https://www.example.com/3"]
+>>> old
+["https://www.example.com/1"]
+```
+Also you can mark your urls for some purposes
+
+
+```python
+>>> urls_for_mark = ["https://www.example.com/2", "https://www.example.com/3"]
+>>> mark_as_processed(urls_for_mark)
+>>> is_processed("https://www.example.com/2")
+True
+>>> is_processed("https://www.example.com/4")
+False
+```
+
+
+It uses a fast sqlite database to store urls. The database file ('ads.db') will be created in the root directory
+
+__Warning!!! this package has no protection against sql injection, do not use it for the external interface__
```

