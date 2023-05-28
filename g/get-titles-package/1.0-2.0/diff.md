# Comparing `tmp/get-titles-package-1.0.tar.gz` & `tmp/get-titles-package-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get-titles-package-1.0.tar", last modified: Sun May 28 11:51:58 2023, max compression
+gzip compressed data, was "get-titles-package-2.0.tar", last modified: Sun May 28 12:00:49 2023, max compression
```

## Comparing `get-titles-package-1.0.tar` & `get-titles-package-2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 11:51:58.934839 get-titles-package-1.0/
--rw-rw-rw-   0        0        0      126 2023-05-28 11:51:58.932364 get-titles-package-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-28 11:51:58.932364 get-titles-package-1.0/get_titles_package.egg-info/
--rw-rw-rw-   0        0        0      126 2023-05-28 11:51:58.000000 get-titles-package-1.0/get_titles_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-05-28 11:51:58.000000 get-titles-package-1.0/get_titles_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 11:51:58.000000 get-titles-package-1.0/get_titles_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 11:51:58.000000 get-titles-package-1.0/get_titles_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 11:51:58.934839 get-titles-package-1.0/setup.cfg
--rw-rw-rw-   0        0        0      224 2023-05-28 11:35:33.000000 get-titles-package-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:00:49.237545 get-titles-package-2.0/
+-rw-rw-rw-   0        0        0      126 2023-05-28 12:00:49.237545 get-titles-package-2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-28 12:00:49.237545 get-titles-package-2.0/get_titles_package.egg-info/
+-rw-rw-rw-   0        0        0      126 2023-05-28 12:00:49.000000 get-titles-package-2.0/get_titles_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-05-28 12:00:49.000000 get-titles-package-2.0/get_titles_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 12:00:49.000000 get-titles-package-2.0/get_titles_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 12:00:49.000000 get-titles-package-2.0/get_titles_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 12:00:49.237545 get-titles-package-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      224 2023-05-28 12:00:39.000000 get-titles-package-2.0/setup.py
```

