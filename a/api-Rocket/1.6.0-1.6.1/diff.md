# Comparing `tmp/api-Rocket-1.6.0.tar.gz` & `tmp/api-Rocket-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\api-Rocket-1.6.0.tar", last modified: Sun May 28 19:01:55 2023, max compression
+gzip compressed data, was "dist\api-Rocket-1.6.1.tar", last modified: Sun May 28 19:09:09 2023, max compression
```

## Comparing `api-Rocket-1.6.0.tar` & `api-Rocket-1.6.1.tar`

### file list

```diff
@@ -1,12 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 19:01:55.204625 api-Rocket-1.6.0/
--rw-rw-rw-   0        0        0       20 2023-05-28 19:01:53.000000 api-Rocket-1.6.0/MANIFEST.in
--rw-rw-rw-   0        0        0      390 2023-05-28 19:01:55.205601 api-Rocket-1.6.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-28 19:01:55.195836 api-Rocket-1.6.0/api_Rocket/
--rw-rw-rw-   0        0        0      685 2023-05-28 18:53:58.000000 api-Rocket-1.6.0/api_Rocket/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:01:55.203648 api-Rocket-1.6.0/api_Rocket.egg-info/
--rw-rw-rw-   0        0        0      390 2023-05-28 19:01:54.000000 api-Rocket-1.6.0/api_Rocket.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-05-28 19:01:55.000000 api-Rocket-1.6.0/api_Rocket.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 19:01:54.000000 api-Rocket-1.6.0/api_Rocket.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-28 19:01:54.000000 api-Rocket-1.6.0/api_Rocket.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 19:01:55.206578 api-Rocket-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0      378 2023-05-28 19:01:53.000000 api-Rocket-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:09:09.403843 api-Rocket-1.6.1/
+-rw-rw-rw-   0        0        0       20 2023-05-28 19:09:08.000000 api-Rocket-1.6.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      390 2023-05-28 19:09:09.404820 api-Rocket-1.6.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-28 19:09:09.365758 api-Rocket-1.6.1/api_Rocket/
+-rw-rw-rw-   0        0        0      685 2023-05-28 18:53:58.000000 api-Rocket-1.6.1/api_Rocket/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:09:09.284703 api-Rocket-1.6.1/api_Rocket/lib/
+drwxrwxrwx   0        0        0        0 2023-05-28 19:09:09.389195 api-Rocket-1.6.1/api_Rocket/lib/clients/
+-rw-rw-rw-   0        0        0      418 2023-03-20 11:34:29.000000 api-Rocket-1.6.1/api_Rocket/lib/clients/async_client.py
+-rw-rw-rw-   0        0        0    10920 2023-05-26 14:58:16.000000 api-Rocket-1.6.1/api_Rocket/lib/clients/client.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:09:09.392125 api-Rocket-1.6.1/api_Rocket/lib/clients/exception/
+-rw-rw-rw-   0        0        0     1718 2023-03-24 14:12:55.000000 api-Rocket-1.6.1/api_Rocket/lib/clients/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:09:09.381383 api-Rocket-1.6.1/api_Rocket.egg-info/
+-rw-rw-rw-   0        0        0      390 2023-05-28 19:09:09.000000 api-Rocket-1.6.1/api_Rocket.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-05-28 19:09:09.000000 api-Rocket-1.6.1/api_Rocket.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 19:09:09.000000 api-Rocket-1.6.1/api_Rocket.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-28 19:09:09.000000 api-Rocket-1.6.1/api_Rocket.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 19:09:09.407750 api-Rocket-1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      378 2023-05-28 19:09:08.000000 api-Rocket-1.6.1/setup.py
```

### Comparing `api-Rocket-1.6.0/api_Rocket/__init__.py` & `api-Rocket-1.6.1/api_Rocket/__init__.py`

 * *Files identical despite different names*

