# Comparing `tmp/sendgrify-1.0.2.tar.gz` & `tmp/sendgrify-2.0.0.macosx-11.6-arm64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sendgrify-1.0.2.tar", last modified: Mon Mar  1 13:42:02 2021, max compression
+gzip compressed data, was "sendgrify-2.0.0.macosx-11.6-arm64.tar", last modified: Sat May 27 23:26:27 2023, max compression
```

## Comparing `sendgrify-1.0.2.tar` & `sendgrify-2.0.0.macosx-11.6-arm64.tar`

### file list

```diff
@@ -1,14 +1,21 @@
-drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2021-03-01 13:42:02.074862 sendgrify-1.0.2/
--rw-r--r--   0 sdelquin   (501) staff       (20)     3711 2021-03-01 13:42:02.074705 sendgrify-1.0.2/PKG-INFO
--rw-r--r--   0 sdelquin   (501) staff       (20)     2499 2021-03-01 13:41:02.000000 sendgrify-1.0.2/README.md
-drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2021-03-01 13:42:02.073641 sendgrify-1.0.2/sendgrify/
--rw-r--r--   0 sdelquin   (501) staff       (20)        0 2021-02-27 11:51:11.000000 sendgrify-1.0.2/sendgrify/__init__.py
--rw-r--r--   0 sdelquin   (501) staff       (20)     2615 2021-02-28 13:55:34.000000 sendgrify-1.0.2/sendgrify/core.py
-drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2021-03-01 13:42:02.074473 sendgrify-1.0.2/sendgrify.egg-info/
--rw-r--r--   0 sdelquin   (501) staff       (20)     3711 2021-03-01 13:42:02.000000 sendgrify-1.0.2/sendgrify.egg-info/PKG-INFO
--rw-r--r--   0 sdelquin   (501) staff       (20)      222 2021-03-01 13:42:02.000000 sendgrify-1.0.2/sendgrify.egg-info/SOURCES.txt
--rw-r--r--   0 sdelquin   (501) staff       (20)        1 2021-03-01 13:42:02.000000 sendgrify-1.0.2/sendgrify.egg-info/dependency_links.txt
--rw-r--r--   0 sdelquin   (501) staff       (20)        9 2021-03-01 13:42:02.000000 sendgrify-1.0.2/sendgrify.egg-info/requires.txt
--rw-r--r--   0 sdelquin   (501) staff       (20)       10 2021-03-01 13:42:02.000000 sendgrify-1.0.2/sendgrify.egg-info/top_level.txt
--rw-r--r--   0 sdelquin   (501) staff       (20)       38 2021-03-01 13:42:02.074916 sendgrify-1.0.2/setup.cfg
--rw-r--r--   0 sdelquin   (501) staff       (20)      491 2021-03-01 13:41:10.000000 sendgrify-1.0.2/setup.py
+drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:26:27.412436 ./
+drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:26:27.412478 ./Users/
+drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:26:27.412516 ./Users/sdelquin/
+drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:26:27.412553 ./Users/sdelquin/.pyenv/
+drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:26:27.412591 ./Users/sdelquin/.pyenv/versions/
+drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:26:27.412628 ./Users/sdelquin/.pyenv/versions/sendgrify/
+drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:26:27.412667 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/
+drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:26:27.412707 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/
+drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:26:27.425413 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/
+drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:26:27.413537 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify/
+-rw-r--r--   0 sdelquin   (501) staff       (20)       27 2023-05-27 23:11:19.000000 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify/__init__.py
+drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:26:27.414307 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify/__pycache__/
+-rw-r--r--   0 sdelquin   (501) staff       (20)      252 2023-05-27 23:26:27.413615 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 sdelquin   (501) staff       (20)     4772 2023-05-27 23:26:27.414259 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify/__pycache__/core.cpython-311.pyc
+-rw-r--r--   0 sdelquin   (501) staff       (20)     2795 2023-05-27 23:11:26.000000 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify/core.py
+drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:26:27.426174 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify-2.0.0-py3.11.egg-info/
+-rw-r--r--   0 sdelquin   (501) staff       (20)     1432 2023-05-27 23:26:27.422863 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify-2.0.0-py3.11.egg-info/PKG-INFO
+-rw-r--r--   0 sdelquin   (501) staff       (20)      230 2023-05-27 23:26:27.425307 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify-2.0.0-py3.11.egg-info/SOURCES.txt
+-rw-r--r--   0 sdelquin   (501) staff       (20)        1 2023-05-27 23:26:27.422944 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify-2.0.0-py3.11.egg-info/dependency_links.txt
+-rw-r--r--   0 sdelquin   (501) staff       (20)       32 2023-05-27 23:26:27.423048 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify-2.0.0-py3.11.egg-info/requires.txt
+-rw-r--r--   0 sdelquin   (501) staff       (20)       10 2023-05-27 23:26:27.423108 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify-2.0.0-py3.11.egg-info/top_level.txt
```

