# Comparing `tmp/sendgrify-2.0.0.macosx-11.6-arm64.tar.gz` & `tmp/sendgrify-2.0.1.macosx-11.6-arm64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sendgrify-2.0.0.macosx-11.6-arm64.tar", last modified: Sat May 27 23:26:27 2023, max compression
+gzip compressed data, was "sendgrify-2.0.1.macosx-11.6-arm64.tar", last modified: Sat May 27 23:32:00 2023, max compression
```

## Comparing `sendgrify-2.0.0.macosx-11.6-arm64.tar` & `sendgrify-2.0.1.macosx-11.6-arm64.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:26:27.412436 ./
-drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:26:27.412478 ./Users/
-drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:26:27.412516 ./Users/sdelquin/
-drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:26:27.412553 ./Users/sdelquin/.pyenv/
-drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:26:27.412591 ./Users/sdelquin/.pyenv/versions/
-drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:26:27.412628 ./Users/sdelquin/.pyenv/versions/sendgrify/
-drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:26:27.412667 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/
-drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:26:27.412707 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/
-drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:26:27.425413 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/
-drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:26:27.413537 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify/
+drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:32:00.336617 ./
+drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:32:00.336655 ./Users/
+drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:32:00.336693 ./Users/sdelquin/
+drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:32:00.336731 ./Users/sdelquin/.pyenv/
+drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:32:00.336769 ./Users/sdelquin/.pyenv/versions/
+drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:32:00.336807 ./Users/sdelquin/.pyenv/versions/sendgrify/
+drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:32:00.336845 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/
+drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:32:00.336884 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/
+drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:32:00.340887 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/
+drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:32:00.337695 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify/
 -rw-r--r--   0 sdelquin   (501) staff       (20)       27 2023-05-27 23:11:19.000000 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify/__init__.py
-drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:26:27.414307 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify/__pycache__/
--rw-r--r--   0 sdelquin   (501) staff       (20)      252 2023-05-27 23:26:27.413615 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 sdelquin   (501) staff       (20)     4772 2023-05-27 23:26:27.414259 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify/__pycache__/core.cpython-311.pyc
+drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:32:00.338461 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify/__pycache__/
+-rw-r--r--   0 sdelquin   (501) staff       (20)      252 2023-05-27 23:32:00.337770 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 sdelquin   (501) staff       (20)     4772 2023-05-27 23:32:00.338416 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify/__pycache__/core.cpython-311.pyc
 -rw-r--r--   0 sdelquin   (501) staff       (20)     2795 2023-05-27 23:11:26.000000 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify/core.py
-drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:26:27.426174 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify-2.0.0-py3.11.egg-info/
--rw-r--r--   0 sdelquin   (501) staff       (20)     1432 2023-05-27 23:26:27.422863 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify-2.0.0-py3.11.egg-info/PKG-INFO
--rw-r--r--   0 sdelquin   (501) staff       (20)      230 2023-05-27 23:26:27.425307 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify-2.0.0-py3.11.egg-info/SOURCES.txt
--rw-r--r--   0 sdelquin   (501) staff       (20)        1 2023-05-27 23:26:27.422944 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify-2.0.0-py3.11.egg-info/dependency_links.txt
--rw-r--r--   0 sdelquin   (501) staff       (20)       32 2023-05-27 23:26:27.423048 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify-2.0.0-py3.11.egg-info/requires.txt
--rw-r--r--   0 sdelquin   (501) staff       (20)       10 2023-05-27 23:26:27.423108 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify-2.0.0-py3.11.egg-info/top_level.txt
+drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2023-05-27 23:32:00.341850 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify-2.0.1-py3.11.egg-info/
+-rw-r--r--   0 sdelquin   (501) staff       (20)     1432 2023-05-27 23:32:00.294371 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify-2.0.1-py3.11.egg-info/PKG-INFO
+-rw-r--r--   0 sdelquin   (501) staff       (20)      230 2023-05-27 23:32:00.300420 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify-2.0.1-py3.11.egg-info/SOURCES.txt
+-rw-r--r--   0 sdelquin   (501) staff       (20)        1 2023-05-27 23:32:00.294460 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify-2.0.1-py3.11.egg-info/dependency_links.txt
+-rw-r--r--   0 sdelquin   (501) staff       (20)       32 2023-05-27 23:32:00.294567 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify-2.0.1-py3.11.egg-info/requires.txt
+-rw-r--r--   0 sdelquin   (501) staff       (20)       10 2023-05-27 23:32:00.294628 ./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify-2.0.1-py3.11.egg-info/top_level.txt
```

### Comparing `./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify-2.0.0-py3.11.egg-info/PKG-INFO` & `./Users/sdelquin/.pyenv/versions/sendgrify/lib/python3.11/site-packages/sendgrify-2.0.1-py3.11.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sendgrify
-Version: 2.0.0
+Version: 2.0.1
 Summary: SendGrid for Humans
 Home-page: https://github.com/sdelquin/sendgrify.git
 Author: Sergio Delgado Quintero
 Author-email: sdelquin@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

