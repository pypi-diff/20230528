# Comparing `tmp/tensorPak-0.2.tar.gz` & `tmp/tensorPak-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorPak-0.2.tar", last modified: Sun May 28 19:05:02 2023, max compression
+gzip compressed data, was "tensorPak-1.0.tar", last modified: Sun May 28 20:37:30 2023, max compression
```

## Comparing `tensorPak-0.2.tar` & `tensorPak-1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 19:05:02.612527 tensorPak-0.2/
--rw-rw-rw-   0        0        0      161 2023-05-28 19:05:02.607526 tensorPak-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-28 19:05:02.613509 tensorPak-0.2/setup.cfg
--rw-rw-rw-   0        0        0      494 2023-05-28 19:04:50.000000 tensorPak-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:05:02.598531 tensorPak-0.2/tensorPak/
--rw-rw-rw-   0        0        0     4089 2023-05-28 17:30:49.000000 tensorPak-0.2/tensorPak/1.txt
--rw-rw-rw-   0        0        0     4079 2023-05-28 17:33:57.000000 tensorPak-0.2/tensorPak/11.txt
--rw-rw-rw-   0        0        0     5964 2023-05-28 17:34:39.000000 tensorPak-0.2/tensorPak/12.txt
--rw-rw-rw-   0        0        0     2790 2023-05-28 17:34:58.000000 tensorPak-0.2/tensorPak/13.txt
--rw-rw-rw-   0        0        0     4356 2023-05-28 17:35:15.000000 tensorPak-0.2/tensorPak/14.txt
--rw-rw-rw-   0        0        0      869 2023-05-28 17:35:30.000000 tensorPak-0.2/tensorPak/15.txt
--rw-rw-rw-   0        0        0     2315 2023-05-28 17:35:41.000000 tensorPak-0.2/tensorPak/16.txt
--rw-rw-rw-   0        0        0     2954 2023-05-28 17:36:05.000000 tensorPak-0.2/tensorPak/17.txt
--rw-rw-rw-   0        0        0     5831 2023-05-28 17:36:23.000000 tensorPak-0.2/tensorPak/18.txt
--rw-rw-rw-   0        0        0     1438 2023-05-28 17:36:41.000000 tensorPak-0.2/tensorPak/19.txt
--rw-rw-rw-   0        0        0     6452 2023-05-28 17:31:44.000000 tensorPak-0.2/tensorPak/2.txt
--rw-rw-rw-   0        0        0     2619 2023-05-28 17:36:53.000000 tensorPak-0.2/tensorPak/20.txt
--rw-rw-rw-   0        0        0     2189 2023-05-28 17:32:00.000000 tensorPak-0.2/tensorPak/3.txt
--rw-rw-rw-   0        0        0     4135 2023-05-28 17:32:28.000000 tensorPak-0.2/tensorPak/4.txt
--rw-rw-rw-   0        0        0     2536 2023-05-28 17:32:57.000000 tensorPak-0.2/tensorPak/5.txt
--rw-rw-rw-   0        0        0      127 2023-05-28 19:04:48.000000 tensorPak-0.2/tensorPak/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:05:02.606521 tensorPak-0.2/tensorPak.egg-info/
--rw-rw-rw-   0        0        0      161 2023-05-28 19:05:02.000000 tensorPak-0.2/tensorPak.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      412 2023-05-28 19:05:02.000000 tensorPak-0.2/tensorPak.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 19:05:02.000000 tensorPak-0.2/tensorPak.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-28 19:05:02.000000 tensorPak-0.2/tensorPak.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 20:37:30.327376 tensorPak-1.0/
+-rw-rw-rw-   0        0        0      161 2023-05-28 20:37:30.326390 tensorPak-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-28 20:37:30.328377 tensorPak-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      494 2023-05-28 20:37:26.000000 tensorPak-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 20:37:30.282144 tensorPak-1.0/tensorPak/
+-rw-rw-rw-   0        0        0     4089 2023-05-28 17:30:49.000000 tensorPak-1.0/tensorPak/1.txt
+-rw-rw-rw-   0        0        0     4079 2023-05-28 17:33:57.000000 tensorPak-1.0/tensorPak/11.txt
+-rw-rw-rw-   0        0        0     5964 2023-05-28 17:34:39.000000 tensorPak-1.0/tensorPak/12.txt
+-rw-rw-rw-   0        0        0     2790 2023-05-28 17:34:58.000000 tensorPak-1.0/tensorPak/13.txt
+-rw-rw-rw-   0        0        0     4356 2023-05-28 17:35:15.000000 tensorPak-1.0/tensorPak/14.txt
+-rw-rw-rw-   0        0        0      869 2023-05-28 17:35:30.000000 tensorPak-1.0/tensorPak/15.txt
+-rw-rw-rw-   0        0        0     2315 2023-05-28 17:35:41.000000 tensorPak-1.0/tensorPak/16.txt
+-rw-rw-rw-   0        0        0     2954 2023-05-28 17:36:05.000000 tensorPak-1.0/tensorPak/17.txt
+-rw-rw-rw-   0        0        0     5831 2023-05-28 17:36:23.000000 tensorPak-1.0/tensorPak/18.txt
+-rw-rw-rw-   0        0        0     1438 2023-05-28 17:36:41.000000 tensorPak-1.0/tensorPak/19.txt
+-rw-rw-rw-   0        0        0     6452 2023-05-28 17:31:44.000000 tensorPak-1.0/tensorPak/2.txt
+-rw-rw-rw-   0        0        0     2619 2023-05-28 17:36:53.000000 tensorPak-1.0/tensorPak/20.txt
+-rw-rw-rw-   0        0        0     2189 2023-05-28 17:32:00.000000 tensorPak-1.0/tensorPak/3.txt
+-rw-rw-rw-   0        0        0     4135 2023-05-28 17:32:28.000000 tensorPak-1.0/tensorPak/4.txt
+-rw-rw-rw-   0        0        0     2536 2023-05-28 17:32:57.000000 tensorPak-1.0/tensorPak/5.txt
+-rw-rw-rw-   0        0        0      225 2023-05-28 20:36:10.000000 tensorPak-1.0/tensorPak/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 20:37:30.295142 tensorPak-1.0/tensorPak.egg-info/
+-rw-rw-rw-   0        0        0      161 2023-05-28 20:37:29.000000 tensorPak-1.0/tensorPak.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2023-05-28 20:37:29.000000 tensorPak-1.0/tensorPak.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 20:37:29.000000 tensorPak-1.0/tensorPak.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-28 20:37:29.000000 tensorPak-1.0/tensorPak.egg-info/top_level.txt
```

### Comparing `tensorPak-0.2/tensorPak/1.txt` & `tensorPak-1.0/tensorPak/1.txt`

 * *Files identical despite different names*

### Comparing `tensorPak-0.2/tensorPak/11.txt` & `tensorPak-1.0/tensorPak/11.txt`

 * *Files identical despite different names*

### Comparing `tensorPak-0.2/tensorPak/12.txt` & `tensorPak-1.0/tensorPak/12.txt`

 * *Files identical despite different names*

### Comparing `tensorPak-0.2/tensorPak/13.txt` & `tensorPak-1.0/tensorPak/13.txt`

 * *Files identical despite different names*

### Comparing `tensorPak-0.2/tensorPak/14.txt` & `tensorPak-1.0/tensorPak/14.txt`

 * *Files identical despite different names*

### Comparing `tensorPak-0.2/tensorPak/15.txt` & `tensorPak-1.0/tensorPak/15.txt`

 * *Files identical despite different names*

### Comparing `tensorPak-0.2/tensorPak/16.txt` & `tensorPak-1.0/tensorPak/16.txt`

 * *Files identical despite different names*

### Comparing `tensorPak-0.2/tensorPak/17.txt` & `tensorPak-1.0/tensorPak/17.txt`

 * *Files identical despite different names*

### Comparing `tensorPak-0.2/tensorPak/18.txt` & `tensorPak-1.0/tensorPak/18.txt`

 * *Files identical despite different names*

### Comparing `tensorPak-0.2/tensorPak/19.txt` & `tensorPak-1.0/tensorPak/19.txt`

 * *Files identical despite different names*

### Comparing `tensorPak-0.2/tensorPak/2.txt` & `tensorPak-1.0/tensorPak/2.txt`

 * *Files identical despite different names*

### Comparing `tensorPak-0.2/tensorPak/20.txt` & `tensorPak-1.0/tensorPak/20.txt`

 * *Files identical despite different names*

### Comparing `tensorPak-0.2/tensorPak/3.txt` & `tensorPak-1.0/tensorPak/3.txt`

 * *Files identical despite different names*

### Comparing `tensorPak-0.2/tensorPak/4.txt` & `tensorPak-1.0/tensorPak/4.txt`

 * *Files identical despite different names*

### Comparing `tensorPak-0.2/tensorPak/5.txt` & `tensorPak-1.0/tensorPak/5.txt`

 * *Files identical despite different names*

