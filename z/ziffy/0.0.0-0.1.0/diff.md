# Comparing `tmp/ziffy-0.0.0.tar.gz` & `tmp/ziffy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziffy-0.0.0.tar", last modified: Tue Apr 25 10:57:58 2023, max compression
+gzip compressed data, was "ziffy-0.1.0.tar", max compression
```

## Comparing `ziffy-0.0.0.tar` & `ziffy-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 federico   (501) staff       (20)        0 2023-04-25 10:57:58.346484 ziffy-0.0.0/
--rw-r--r--   0 federico   (501) staff       (20)       49 2023-04-25 10:57:58.345881 ziffy-0.0.0/PKG-INFO
--rw-r--r--   0 federico   (501) staff       (20)        7 2023-04-25 10:51:53.000000 ziffy-0.0.0/README.md
--rw-r--r--   0 federico   (501) staff       (20)        0 2023-04-25 10:57:33.000000 ziffy-0.0.0/pyproject.toml
--rw-r--r--   0 federico   (501) staff       (20)       38 2023-04-25 10:57:58.346661 ziffy-0.0.0/setup.cfg
-drwxr-xr-x   0 federico   (501) staff       (20)        0 2023-04-25 10:57:58.340953 ziffy-0.0.0/ziffy/
--rw-r--r--   0 federico   (501) staff       (20)        0 2023-04-25 10:57:33.000000 ziffy-0.0.0/ziffy/__init__.py
--rw-r--r--   0 federico   (501) staff       (20)     1140 2023-04-25 10:51:53.000000 ziffy-0.0.0/ziffy/main.py
-drwxr-xr-x   0 federico   (501) staff       (20)        0 2023-04-25 10:57:58.345022 ziffy-0.0.0/ziffy.egg-info/
--rw-r--r--   0 federico   (501) staff       (20)       49 2023-04-25 10:57:58.000000 ziffy-0.0.0/ziffy.egg-info/PKG-INFO
--rw-r--r--   0 federico   (501) staff       (20)      172 2023-04-25 10:57:58.000000 ziffy-0.0.0/ziffy.egg-info/SOURCES.txt
--rw-r--r--   0 federico   (501) staff       (20)        1 2023-04-25 10:57:58.000000 ziffy-0.0.0/ziffy.egg-info/dependency_links.txt
--rw-r--r--   0 federico   (501) staff       (20)        6 2023-04-25 10:57:58.000000 ziffy-0.0.0/ziffy.egg-info/top_level.txt
+-rw-r--r--   0        0        0      274 2023-05-28 11:16:06.386677 ziffy-0.1.0/README.md
+-rw-r--r--   0        0        0      472 2023-05-28 08:54:09.726238 ziffy-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-28 09:43:08.507353 ziffy-0.1.0/ziffy/__init__.py
+-rw-r--r--   0        0        0      507 2023-05-28 10:22:54.367065 ziffy-0.1.0/ziffy/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:51:45.681346 ziffy-0.1.0/ziffy/cli/__init__.py
+-rw-r--r--   0        0        0      597 2023-05-28 11:28:52.911742 ziffy-0.1.0/ziffy/cli/datasets.py
+-rw-r--r--   0        0        0      713 2023-05-28 11:31:46.620844 ziffy-0.1.0/ziffy/datasets.py
+-rw-r--r--   0        0        0        0 2023-05-28 08:51:44.049342 ziffy-0.1.0/ziffy/db/__init__.py
+-rw-r--r--   0        0        0      811 2023-05-28 11:02:54.600169 ziffy-0.1.0/ziffy/db/datasets.py
+-rw-r--r--   0        0        0      963 2023-04-26 20:10:03.201603 ziffy-0.1.0/ziffy/db.py
+-rw-r--r--   0        0        0     6092 2023-05-27 16:08:47.497063 ziffy-0.1.0/ziffy/oldmain.py
+-rw-r--r--   0        0        0      714 2023-04-26 20:10:03.201603 ziffy-0.1.0/ziffy/regex.py
+-rw-r--r--   0        0        0      540 2023-05-28 10:43:33.325691 ziffy-0.1.0/ziffy/tree.py
+-rw-r--r--   0        0        0      924 2023-05-28 11:14:10.658040 ziffy-0.1.0/ziffy/utils.py
+-rw-r--r--   0        0        0      728 1970-01-01 00:00:00.000000 ziffy-0.1.0/PKG-INFO
```

