# Comparing `tmp/stream-unzip-0.0.86.tar.gz` & `tmp/stream-unzip-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stream-unzip-0.0.86.tar", last modified: Sun May 28 19:14:45 2023, max compression
+gzip compressed data, was "/Users/dituser/dev/stream-unzip/dist/tmp74d7pg01/stream-unzip-0.0.9.tar", last modified: Tue May 18 03:10:27 2021, max compression
```

## Comparing `stream-unzip-0.0.86.tar` & `stream-unzip-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 19:14:45.660119 stream-unzip-0.0.86/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-28 19:14:37.000000 stream-unzip-0.0.86/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-28 19:14:45.660119 stream-unzip-0.0.86/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-28 19:14:37.000000 stream-unzip-0.0.86/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 19:14:45.660119 stream-unzip-0.0.86/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-28 19:14:37.000000 stream-unzip-0.0.86/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 19:14:45.660119 stream-unzip-0.0.86/stream_unzip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-28 19:14:45.000000 stream-unzip-0.0.86/stream_unzip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-28 19:14:45.000000 stream-unzip-0.0.86/stream_unzip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 19:14:45.000000 stream-unzip-0.0.86/stream_unzip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-28 19:14:45.000000 stream-unzip-0.0.86/stream_unzip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-28 19:14:45.000000 stream-unzip-0.0.86/stream_unzip.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20342 2023-05-28 19:14:37.000000 stream-unzip-0.0.86/stream_unzip.py
+drwxr-xr-x   0 dituser    (501) staff       (20)        0 2021-05-18 03:10:27.987233 stream-unzip-0.0.9/
+-rw-r--r--   0 dituser    (501) staff       (20)     1091 2021-05-16 14:23:12.000000 stream-unzip-0.0.9/LICENSE
+-rw-r--r--   0 dituser    (501) staff       (20)     2521 2021-05-18 03:10:27.986728 stream-unzip-0.0.9/PKG-INFO
+-rw-r--r--   0 dituser    (501) staff       (20)     1701 2021-05-17 09:27:01.000000 stream-unzip-0.0.9/README.md
+-rw-r--r--   0 dituser    (501) staff       (20)       38 2021-05-18 03:10:27.987368 stream-unzip-0.0.9/setup.cfg
+-rw-r--r--   0 dituser    (501) staff       (20)      782 2021-05-18 03:09:44.000000 stream-unzip-0.0.9/setup.py
+drwxr-xr-x   0 dituser    (501) staff       (20)        0 2021-05-18 03:10:27.986064 stream-unzip-0.0.9/stream_unzip.egg-info/
+-rw-r--r--   0 dituser    (501) staff       (20)     2521 2021-05-18 03:10:27.000000 stream-unzip-0.0.9/stream_unzip.egg-info/PKG-INFO
+-rw-r--r--   0 dituser    (501) staff       (20)      186 2021-05-18 03:10:27.000000 stream-unzip-0.0.9/stream_unzip.egg-info/SOURCES.txt
+-rw-r--r--   0 dituser    (501) staff       (20)        1 2021-05-18 03:10:27.000000 stream-unzip-0.0.9/stream_unzip.egg-info/dependency_links.txt
+-rw-r--r--   0 dituser    (501) staff       (20)       13 2021-05-18 03:10:27.000000 stream-unzip-0.0.9/stream_unzip.egg-info/top_level.txt
+-rw-r--r--   0 dituser    (501) staff       (20)     5497 2021-05-18 03:09:34.000000 stream-unzip-0.0.9/stream_unzip.py
```

### Comparing `stream-unzip-0.0.86/LICENSE` & `stream-unzip-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stream-unzip-0.0.86/setup.py` & `stream-unzip-0.0.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,31 +4,23 @@
 def long_description():
     with open('README.md', 'r') as file:
         return file.read()
 
 
 setuptools.setup(
     name='stream-unzip',
-    version='0.0.86',
+    version='0.0.9',
     author='Department for International Trade',
     author_email='sre@digital.trade.gov.uk',
     description='Python function to stream unzip all the files in a ZIP archive, without loading the entire ZIP file into memory or any of its uncompressed files',
     long_description=long_description(),
     long_description_content_type='text/markdown',
-    project_urls={
-        'Documentation': 'https://stream-unzip.docs.trade.gov.uk/',
-        'Source': 'https://github.com/uktrade/stream-unzip',
-    },
+    url='https://github.com/uktrade/stream-unzip',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
-        'Topic :: System :: Archiving :: Compression',
-    ],
-    python_requires='>=3.5.1',
-    install_requires=[
-        'pycryptodome>=3.10.1',
-        'stream-inflate>=0.0.12',
     ],
+    python_requires='>=3.6.0',
     py_modules=[
         'stream_unzip',
     ],
 )
```

