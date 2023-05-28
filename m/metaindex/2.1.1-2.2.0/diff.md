# Comparing `tmp/metaindex-2.1.1.tar.gz` & `tmp/metaindex-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaindex-2.1.1.tar", last modified: Fri May 19 10:57:14 2023, max compression
+gzip compressed data, was "metaindex-2.2.0.tar", last modified: Sat May 27 19:17:27 2023, max compression
```

## Comparing `metaindex-2.1.1.tar` & `metaindex-2.2.0.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-19 10:57:14.327107 metaindex-2.1.1/
--rw-r--r--   0 robert    (1000) robert    (1000)     4745 2023-05-19 09:20:54.000000 metaindex-2.1.1/CHANGELOG.md
--rw-r--r--   0 robert    (1000) robert    (1000)     1107 2022-02-23 18:45:10.000000 metaindex-2.1.1/LICENSE
--rw-r--r--   0 robert    (1000) robert    (1000)      220 2021-09-01 18:34:21.000000 metaindex-2.1.1/MANIFEST.in
--rw-r--r--   0 robert    (1000) robert    (1000)     4861 2023-05-19 10:57:14.327107 metaindex-2.1.1/PKG-INFO
--rw-r--r--   0 robert    (1000) robert    (1000)     4038 2023-05-19 09:18:53.000000 metaindex-2.1.1/README.md
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-19 10:57:14.307107 metaindex-2.1.1/doc/
--rw-r--r--   0 robert    (1000) robert    (1000)      638 2022-02-23 18:26:43.000000 metaindex-2.1.1/doc/Makefile
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-19 10:57:14.307107 metaindex-2.1.1/doc/build/
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-19 10:57:14.313773 metaindex-2.1.1/doc/build/doctrees/
--rw-r--r--   0 robert    (1000) robert    (1000)    14332 2022-03-20 10:53:27.000000 metaindex-2.1.1/doc/build/doctrees/addons.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    32378 2022-03-20 10:53:27.000000 metaindex-2.1.1/doc/build/doctrees/changelog.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    25916 2022-03-20 10:53:27.000000 metaindex-2.1.1/doc/build/doctrees/cmdoptions.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     6598 2022-03-20 10:53:27.000000 metaindex-2.1.1/doc/build/doctrees/cmdusage.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    38700 2022-03-20 10:53:27.000000 metaindex-2.1.1/doc/build/doctrees/configuration.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     5614 2022-03-20 10:53:27.000000 metaindex-2.1.1/doc/build/doctrees/description.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    69762 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/doctrees/environment.pickle
--rw-r--r--   0 robert    (1000) robert    (1000)    12145 2022-03-20 10:53:27.000000 metaindex-2.1.1/doc/build/doctrees/examples.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    24665 2022-03-20 10:53:27.000000 metaindex-2.1.1/doc/build/doctrees/extrametadata.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     8436 2022-03-20 10:53:27.000000 metaindex-2.1.1/doc/build/doctrees/index.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    27055 2022-03-20 10:53:27.000000 metaindex-2.1.1/doc/build/doctrees/indexers.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     9541 2022-03-20 10:53:27.000000 metaindex-2.1.1/doc/build/doctrees/install.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     6122 2022-03-20 10:53:27.000000 metaindex-2.1.1/doc/build/doctrees/license.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)   177806 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/doctrees/reference.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    12666 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/doctrees/searchsyntax.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     2656 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/doctrees/synopsis.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    26715 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/doctrees/usage.doctree
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-19 10:57:14.317107 metaindex-2.1.1/doc/build/html/
--rw-r--r--   0 robert    (1000) robert    (1000)      230 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/html/.buildinfo
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-19 10:57:14.317107 metaindex-2.1.1/doc/build/html/_sources/
--rw-r--r--   0 robert    (1000) robert    (1000)     2736 2022-03-13 15:27:55.000000 metaindex-2.1.1/doc/build/html/_sources/addons.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       80 2022-02-23 18:39:36.000000 metaindex-2.1.1/doc/build/html/_sources/changelog.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     4029 2022-02-25 19:33:14.000000 metaindex-2.1.1/doc/build/html/_sources/cmdoptions.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      773 2022-02-25 21:17:37.000000 metaindex-2.1.1/doc/build/html/_sources/cmdusage.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     6605 2022-03-13 16:28:39.000000 metaindex-2.1.1/doc/build/html/_sources/configuration.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      726 2022-03-10 18:16:36.000000 metaindex-2.1.1/doc/build/html/_sources/description.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     1052 2022-03-20 09:25:44.000000 metaindex-2.1.1/doc/build/html/_sources/examples.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     4869 2022-02-25 20:09:22.000000 metaindex-2.1.1/doc/build/html/_sources/extrametadata.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      332 2022-03-13 15:16:59.000000 metaindex-2.1.1/doc/build/html/_sources/index.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     5934 2022-03-15 19:41:05.000000 metaindex-2.1.1/doc/build/html/_sources/indexers.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     1151 2022-02-23 18:37:25.000000 metaindex-2.1.1/doc/build/html/_sources/install.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       58 2022-02-23 18:40:10.000000 metaindex-2.1.1/doc/build/html/_sources/license.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      664 2022-03-20 10:20:29.000000 metaindex-2.1.1/doc/build/html/_sources/reference.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     1964 2022-03-13 16:29:46.000000 metaindex-2.1.1/doc/build/html/_sources/searchsyntax.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      105 2022-02-25 19:48:09.000000 metaindex-2.1.1/doc/build/html/_sources/synopsis.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       55 2022-02-25 19:48:15.000000 metaindex-2.1.1/doc/build/html/_sources/usage.rst.txt
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-19 10:57:14.320440 metaindex-2.1.1/doc/build/html/_static/
--rw-r--r--   0 robert    (1000) robert    (1000)    14692 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/html/_static/basic.css
--rw-r--r--   0 robert    (1000) robert    (1000)     9758 2022-02-23 18:30:51.000000 metaindex-2.1.1/doc/build/html/_static/doctools.js
--rw-r--r--   0 robert    (1000) robert    (1000)      350 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/html/_static/documentation_options.js
--rw-r--r--   0 robert    (1000) robert    (1000)      286 2022-02-23 18:30:51.000000 metaindex-2.1.1/doc/build/html/_static/file.png
--rw-r--r--   0 robert    (1000) robert    (1000)   287630 2022-02-23 18:30:51.000000 metaindex-2.1.1/doc/build/html/_static/jquery-3.5.1.js
--rw-r--r--   0 robert    (1000) robert    (1000)    89476 2022-02-23 18:30:51.000000 metaindex-2.1.1/doc/build/html/_static/jquery.js
--rw-r--r--   0 robert    (1000) robert    (1000)    10854 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/html/_static/language_data.js
--rw-r--r--   0 robert    (1000) robert    (1000)       90 2022-02-23 18:30:51.000000 metaindex-2.1.1/doc/build/html/_static/minus.png
--rw-r--r--   0 robert    (1000) robert    (1000)     4181 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/html/_static/nature.css
--rw-r--r--   0 robert    (1000) robert    (1000)       90 2022-02-23 18:30:51.000000 metaindex-2.1.1/doc/build/html/_static/plus.png
--rw-r--r--   0 robert    (1000) robert    (1000)     5432 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/html/_static/pygments.css
--rw-r--r--   0 robert    (1000) robert    (1000)    16793 2022-02-23 18:30:51.000000 metaindex-2.1.1/doc/build/html/_static/searchtools.js
--rw-r--r--   0 robert    (1000) robert    (1000)    68420 2022-02-23 18:30:51.000000 metaindex-2.1.1/doc/build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 robert    (1000) robert    (1000)    19530 2022-02-23 18:30:51.000000 metaindex-2.1.1/doc/build/html/_static/underscore.js
--rw-r--r--   0 robert    (1000) robert    (1000)    11398 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/html/addons.html
--rw-r--r--   0 robert    (1000) robert    (1000)    16853 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/html/changelog.html
--rw-r--r--   0 robert    (1000) robert    (1000)    12806 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/html/cmdoptions.html
--rw-r--r--   0 robert    (1000) robert    (1000)     6745 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/html/cmdusage.html
--rw-r--r--   0 robert    (1000) robert    (1000)    20977 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/html/configuration.html
--rw-r--r--   0 robert    (1000) robert    (1000)     4029 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/html/description.html
--rw-r--r--   0 robert    (1000) robert    (1000)    13768 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/html/examples.html
--rw-r--r--   0 robert    (1000) robert    (1000)    16741 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/html/extrametadata.html
--rw-r--r--   0 robert    (1000) robert    (1000)    18918 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/html/genindex.html
--rw-r--r--   0 robert    (1000) robert    (1000)     6742 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/html/index.html
--rw-r--r--   0 robert    (1000) robert    (1000)    20498 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/html/indexers.html
--rw-r--r--   0 robert    (1000) robert    (1000)     7101 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/html/install.html
--rw-r--r--   0 robert    (1000) robert    (1000)     5360 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/html/license.html
--rw-r--r--   0 robert    (1000) robert    (1000)     1235 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/html/objects.inv
--rw-r--r--   0 robert    (1000) robert    (1000)    66164 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/html/reference.html
--rw-r--r--   0 robert    (1000) robert    (1000)     3093 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/html/search.html
--rw-r--r--   0 robert    (1000) robert    (1000)    17128 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/html/searchindex.js
--rw-r--r--   0 robert    (1000) robert    (1000)     9155 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/html/searchsyntax.html
--rw-r--r--   0 robert    (1000) robert    (1000)     3970 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/html/synopsis.html
--rw-r--r--   0 robert    (1000) robert    (1000)    14783 2022-03-20 10:53:28.000000 metaindex-2.1.1/doc/build/html/usage.html
--rw-r--r--   0 robert    (1000) robert    (1000)     3334 2022-02-25 14:43:32.000000 metaindex-2.1.1/doc/cmdoptions.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      804 2022-02-23 18:26:43.000000 metaindex-2.1.1/doc/make.bat
--rw-r--r--   0 robert    (1000) robert    (1000)      901 2022-02-25 21:18:16.000000 metaindex-2.1.1/doc/metaindex.rst
--rw-r--r--   0 robert    (1000) robert    (1000)       19 2022-02-23 18:30:21.000000 metaindex-2.1.1/doc/requirements.txt
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-19 10:57:14.323773 metaindex-2.1.1/doc/source/
--rw-r--r--   0 robert    (1000) robert    (1000)     2736 2022-03-13 15:27:55.000000 metaindex-2.1.1/doc/source/addons.rst
--rw-r--r--   0 robert    (1000) robert    (1000)       80 2022-02-23 18:39:36.000000 metaindex-2.1.1/doc/source/changelog.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     5130 2023-05-11 18:09:52.000000 metaindex-2.1.1/doc/source/cmdoptions.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      653 2023-05-11 18:09:52.000000 metaindex-2.1.1/doc/source/cmdusage.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     1871 2022-02-23 18:29:41.000000 metaindex-2.1.1/doc/source/conf.py
--rw-r--r--   0 robert    (1000) robert    (1000)     8069 2023-05-18 15:06:36.000000 metaindex-2.1.1/doc/source/configuration.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      726 2022-03-10 18:16:36.000000 metaindex-2.1.1/doc/source/description.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     1052 2022-03-20 09:25:44.000000 metaindex-2.1.1/doc/source/examples.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     4869 2022-02-25 20:09:22.000000 metaindex-2.1.1/doc/source/extrametadata.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      332 2022-03-13 15:16:59.000000 metaindex-2.1.1/doc/source/index.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     6931 2023-05-19 09:14:51.000000 metaindex-2.1.1/doc/source/indexers.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     1151 2022-02-23 18:37:25.000000 metaindex-2.1.1/doc/source/install.rst
--rw-r--r--   0 robert    (1000) robert    (1000)       58 2022-02-23 18:40:10.000000 metaindex-2.1.1/doc/source/license.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      664 2022-03-20 10:20:29.000000 metaindex-2.1.1/doc/source/reference.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     1964 2022-03-13 16:29:46.000000 metaindex-2.1.1/doc/source/searchsyntax.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      105 2022-02-25 19:48:09.000000 metaindex-2.1.1/doc/source/synopsis.rst
--rw-r--r--   0 robert    (1000) robert    (1000)       55 2022-02-25 19:48:15.000000 metaindex-2.1.1/doc/source/usage.rst
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-19 10:57:14.323773 metaindex-2.1.1/examples/
--rw-r--r--   0 robert    (1000) robert    (1000)     1223 2022-03-20 09:43:43.000000 metaindex-2.1.1/examples/indexing.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-19 10:57:14.323773 metaindex-2.1.1/man/
--rw-r--r--   0 robert    (1000) robert    (1000)    36476 2023-05-19 10:57:14.000000 metaindex-2.1.1/man/metaindex.1
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-19 10:57:14.323773 metaindex-2.1.1/metaindex/
--rw-r--r--   0 robert    (1000) robert    (1000)      274 2023-05-16 17:26:33.000000 metaindex-2.1.1/metaindex/__init__.py
--rw-r--r--   0 robert    (1000) robert    (1000)    15817 2023-05-11 18:09:52.000000 metaindex-2.1.1/metaindex/cache.py
--rw-r--r--   0 robert    (1000) robert    (1000)    12235 2023-05-18 17:20:46.000000 metaindex-2.1.1/metaindex/cacheentry.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1968 2023-05-11 18:09:52.000000 metaindex-2.1.1/metaindex/client.py
--rw-r--r--   0 robert    (1000) robert    (1000)    23595 2023-05-18 15:06:53.000000 metaindex-2.1.1/metaindex/configuration.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-19 10:57:14.323773 metaindex-2.1.1/metaindex/docs/
--rw-r--r--   0 robert    (1000) robert    (1000)    13555 2023-05-19 10:57:14.000000 metaindex-2.1.1/metaindex/docs/cmdoptions.html
--rw-r--r--   0 robert    (1000) robert    (1000)    54380 2023-05-19 10:57:14.000000 metaindex-2.1.1/metaindex/docs/metaindex.html
--rw-r--r--   0 robert    (1000) robert    (1000)     2859 2023-05-11 18:09:52.000000 metaindex-2.1.1/metaindex/find.py
--rw-r--r--   0 robert    (1000) robert    (1000)    18409 2021-10-16 07:30:31.000000 metaindex-2.1.1/metaindex/fuse.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4287 2022-06-18 22:14:53.000000 metaindex-2.1.1/metaindex/humanizer.py
--rw-r--r--   0 robert    (1000) robert    (1000)    15257 2023-05-11 18:09:52.000000 metaindex-2.1.1/metaindex/indexer.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-19 10:57:14.327107 metaindex-2.1.1/metaindex/indexers/
--rw-r--r--   0 robert    (1000) robert    (1000)      472 2022-06-28 21:59:17.000000 metaindex-2.1.1/metaindex/indexers/__init__.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1972 2022-08-21 19:12:49.000000 metaindex-2.1.1/metaindex/indexers/abc.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1157 2022-05-11 17:49:48.000000 metaindex-2.1.1/metaindex/indexers/audio.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4953 2023-05-11 18:09:52.000000 metaindex-2.1.1/metaindex/indexers/collections.py
--rw-r--r--   0 robert    (1000) robert    (1000)     6003 2022-06-27 12:23:21.000000 metaindex-2.1.1/metaindex/indexers/comicbook.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1498 2022-06-27 12:23:51.000000 metaindex-2.1.1/metaindex/indexers/epub.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3810 2022-04-30 12:58:34.000000 metaindex-2.1.1/metaindex/indexers/filetags.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4354 2022-06-27 12:21:13.000000 metaindex-2.1.1/metaindex/indexers/gpx.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1686 2022-05-04 19:09:52.000000 metaindex-2.1.1/metaindex/indexers/html.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3238 2022-05-29 12:11:11.000000 metaindex-2.1.1/metaindex/indexers/images.py
--rw-r--r--   0 robert    (1000) robert    (1000)     2711 2022-06-28 22:04:20.000000 metaindex-2.1.1/metaindex/indexers/ooxml.py
--rw-r--r--   0 robert    (1000) robert    (1000)     2799 2022-06-28 22:03:27.000000 metaindex-2.1.1/metaindex/indexers/opendocument.py
--rw-r--r--   0 robert    (1000) robert    (1000)     6824 2022-05-11 17:43:40.000000 metaindex-2.1.1/metaindex/indexers/pdf.py
--rw-r--r--   0 robert    (1000) robert    (1000)    10676 2023-05-19 08:45:31.000000 metaindex-2.1.1/metaindex/indexers/ruleindexer.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4560 2023-05-11 18:09:52.000000 metaindex-2.1.1/metaindex/json.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1566 2023-05-19 08:54:45.000000 metaindex-2.1.1/metaindex/logger.py
--rw-r--r--   0 robert    (1000) robert    (1000)     8767 2023-05-11 18:09:52.000000 metaindex-2.1.1/metaindex/main.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3407 2022-05-10 20:51:51.000000 metaindex-2.1.1/metaindex/ocr.py
--rw-r--r--   0 robert    (1000) robert    (1000)     2017 2023-05-11 18:09:52.000000 metaindex-2.1.1/metaindex/opf.py
--rw-r--r--   0 robert    (1000) robert    (1000)     8167 2023-05-11 18:09:52.000000 metaindex-2.1.1/metaindex/proto.py
--rw-r--r--   0 robert    (1000) robert    (1000)    27228 2023-05-18 17:19:00.000000 metaindex-2.1.1/metaindex/server.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4214 2023-05-11 18:09:52.000000 metaindex-2.1.1/metaindex/shared.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3198 2023-05-11 18:09:52.000000 metaindex-2.1.1/metaindex/stores.py
--rw-r--r--   0 robert    (1000) robert    (1000)       23 2023-05-19 10:56:54.000000 metaindex-2.1.1/metaindex/version.py
--rw-r--r--   0 robert    (1000) robert    (1000)      734 2022-06-27 12:20:41.000000 metaindex-2.1.1/metaindex/xmlproxy.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3920 2023-05-11 18:09:52.000000 metaindex-2.1.1/metaindex/yaml.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-19 10:57:14.323773 metaindex-2.1.1/metaindex.egg-info/
--rw-r--r--   0 robert    (1000) robert    (1000)     4861 2023-05-19 10:57:14.000000 metaindex-2.1.1/metaindex.egg-info/PKG-INFO
--rw-r--r--   0 robert    (1000) robert    (1000)     4390 2023-05-19 10:57:14.000000 metaindex-2.1.1/metaindex.egg-info/SOURCES.txt
--rw-r--r--   0 robert    (1000) robert    (1000)        1 2023-05-19 10:57:14.000000 metaindex-2.1.1/metaindex.egg-info/dependency_links.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       88 2023-05-19 10:57:14.000000 metaindex-2.1.1/metaindex.egg-info/entry_points.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      241 2023-05-19 10:57:14.000000 metaindex-2.1.1/metaindex.egg-info/requires.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       29 2023-05-19 10:57:14.000000 metaindex-2.1.1/metaindex.egg-info/top_level.txt
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-19 10:57:14.327107 metaindex-2.1.1/misc/
--rw-r--r--   0 robert    (1000) robert    (1000)     2161 2023-05-11 18:09:52.000000 metaindex-2.1.1/misc/metaindex.conf
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-19 10:57:14.327107 metaindex-2.1.1/misc/ranger_metaindex/
--rw-r--r--   0 robert    (1000) robert    (1000)       41 2021-09-01 18:34:21.000000 metaindex-2.1.1/misc/ranger_metaindex/__init__.py
--rw-r--r--   0 robert    (1000) robert    (1000)      737 2023-05-11 18:09:16.000000 metaindex-2.1.1/misc/ranger_metaindex/linemode.py
--rw-r--r--   0 robert    (1000) robert    (1000)       38 2023-05-19 10:57:14.327107 metaindex-2.1.1/setup.cfg
--rw-r--r--   0 robert    (1000) robert    (1000)     3667 2023-05-11 18:09:52.000000 metaindex-2.1.1/setup.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-19 10:57:14.327107 metaindex-2.1.1/tests/
--rw-r--r--   0 robert    (1000) robert    (1000)     1072 2022-08-21 19:09:08.000000 metaindex-2.1.1/tests/test_abc.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4343 2023-05-11 18:09:52.000000 metaindex-2.1.1/tests/test_cache.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3043 2022-06-24 07:16:59.000000 metaindex-2.1.1/tests/test_cacheentry.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3933 2022-06-27 09:57:52.000000 metaindex-2.1.1/tests/test_cleanup.py
--rw-r--r--   0 robert    (1000) robert    (1000)     2529 2022-02-26 17:13:44.000000 metaindex-2.1.1/tests/test_collect.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4866 2022-03-13 18:33:11.000000 metaindex-2.1.1/tests/test_humanizer.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1460 2022-03-15 17:55:22.000000 metaindex-2.1.1/tests/test_indexers.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3895 2022-02-26 16:28:16.000000 metaindex-2.1.1/tests/test_json.py
--rw-r--r--   0 robert    (1000) robert    (1000)     2549 2022-04-30 12:43:40.000000 metaindex-2.1.1/tests/test_ruleindexer.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-27 19:17:27.497623 metaindex-2.2.0/
+-rw-r--r--   0 robert    (1000) robert    (1000)     5703 2023-05-27 19:16:50.000000 metaindex-2.2.0/CHANGELOG.md
+-rw-r--r--   0 robert    (1000) robert    (1000)     1107 2022-02-23 18:45:10.000000 metaindex-2.2.0/LICENSE
+-rw-r--r--   0 robert    (1000) robert    (1000)      220 2021-09-01 18:34:21.000000 metaindex-2.2.0/MANIFEST.in
+-rw-r--r--   0 robert    (1000) robert    (1000)     4861 2023-05-27 19:17:27.497623 metaindex-2.2.0/PKG-INFO
+-rw-r--r--   0 robert    (1000) robert    (1000)     4038 2023-05-27 09:09:36.000000 metaindex-2.2.0/README.md
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-27 19:17:27.477623 metaindex-2.2.0/doc/
+-rw-r--r--   0 robert    (1000) robert    (1000)      638 2022-02-23 18:26:43.000000 metaindex-2.2.0/doc/Makefile
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-27 19:17:27.477623 metaindex-2.2.0/doc/build/
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-27 19:17:27.484290 metaindex-2.2.0/doc/build/doctrees/
+-rw-r--r--   0 robert    (1000) robert    (1000)    14332 2022-03-20 10:53:27.000000 metaindex-2.2.0/doc/build/doctrees/addons.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    32378 2022-03-20 10:53:27.000000 metaindex-2.2.0/doc/build/doctrees/changelog.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    25916 2022-03-20 10:53:27.000000 metaindex-2.2.0/doc/build/doctrees/cmdoptions.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     6598 2022-03-20 10:53:27.000000 metaindex-2.2.0/doc/build/doctrees/cmdusage.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    38700 2022-03-20 10:53:27.000000 metaindex-2.2.0/doc/build/doctrees/configuration.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     5614 2022-03-20 10:53:27.000000 metaindex-2.2.0/doc/build/doctrees/description.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    69762 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/doctrees/environment.pickle
+-rw-r--r--   0 robert    (1000) robert    (1000)    12145 2022-03-20 10:53:27.000000 metaindex-2.2.0/doc/build/doctrees/examples.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    24665 2022-03-20 10:53:27.000000 metaindex-2.2.0/doc/build/doctrees/extrametadata.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     8436 2022-03-20 10:53:27.000000 metaindex-2.2.0/doc/build/doctrees/index.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    27055 2022-03-20 10:53:27.000000 metaindex-2.2.0/doc/build/doctrees/indexers.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     9541 2022-03-20 10:53:27.000000 metaindex-2.2.0/doc/build/doctrees/install.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     6122 2022-03-20 10:53:27.000000 metaindex-2.2.0/doc/build/doctrees/license.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)   177806 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/doctrees/reference.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    12666 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/doctrees/searchsyntax.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     2656 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/doctrees/synopsis.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    26715 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/doctrees/usage.doctree
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-27 19:17:27.487623 metaindex-2.2.0/doc/build/html/
+-rw-r--r--   0 robert    (1000) robert    (1000)      230 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/html/.buildinfo
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-27 19:17:27.490957 metaindex-2.2.0/doc/build/html/_sources/
+-rw-r--r--   0 robert    (1000) robert    (1000)     2736 2022-03-13 15:27:55.000000 metaindex-2.2.0/doc/build/html/_sources/addons.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       80 2022-02-23 18:39:36.000000 metaindex-2.2.0/doc/build/html/_sources/changelog.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     4029 2022-02-25 19:33:14.000000 metaindex-2.2.0/doc/build/html/_sources/cmdoptions.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      773 2022-02-25 21:17:37.000000 metaindex-2.2.0/doc/build/html/_sources/cmdusage.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     6605 2022-03-13 16:28:39.000000 metaindex-2.2.0/doc/build/html/_sources/configuration.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      726 2022-03-10 18:16:36.000000 metaindex-2.2.0/doc/build/html/_sources/description.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     1052 2022-03-20 09:25:44.000000 metaindex-2.2.0/doc/build/html/_sources/examples.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     4869 2022-02-25 20:09:22.000000 metaindex-2.2.0/doc/build/html/_sources/extrametadata.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      332 2022-03-13 15:16:59.000000 metaindex-2.2.0/doc/build/html/_sources/index.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     5934 2022-03-15 19:41:05.000000 metaindex-2.2.0/doc/build/html/_sources/indexers.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     1151 2022-02-23 18:37:25.000000 metaindex-2.2.0/doc/build/html/_sources/install.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       58 2022-02-23 18:40:10.000000 metaindex-2.2.0/doc/build/html/_sources/license.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      664 2022-03-20 10:20:29.000000 metaindex-2.2.0/doc/build/html/_sources/reference.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     1964 2022-03-13 16:29:46.000000 metaindex-2.2.0/doc/build/html/_sources/searchsyntax.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      105 2022-02-25 19:48:09.000000 metaindex-2.2.0/doc/build/html/_sources/synopsis.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       55 2022-02-25 19:48:15.000000 metaindex-2.2.0/doc/build/html/_sources/usage.rst.txt
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-27 19:17:27.494290 metaindex-2.2.0/doc/build/html/_static/
+-rw-r--r--   0 robert    (1000) robert    (1000)    14692 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/html/_static/basic.css
+-rw-r--r--   0 robert    (1000) robert    (1000)     9758 2022-02-23 18:30:51.000000 metaindex-2.2.0/doc/build/html/_static/doctools.js
+-rw-r--r--   0 robert    (1000) robert    (1000)      350 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/html/_static/documentation_options.js
+-rw-r--r--   0 robert    (1000) robert    (1000)      286 2022-02-23 18:30:51.000000 metaindex-2.2.0/doc/build/html/_static/file.png
+-rw-r--r--   0 robert    (1000) robert    (1000)   287630 2022-02-23 18:30:51.000000 metaindex-2.2.0/doc/build/html/_static/jquery-3.5.1.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    89476 2022-02-23 18:30:51.000000 metaindex-2.2.0/doc/build/html/_static/jquery.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    10854 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/html/_static/language_data.js
+-rw-r--r--   0 robert    (1000) robert    (1000)       90 2022-02-23 18:30:51.000000 metaindex-2.2.0/doc/build/html/_static/minus.png
+-rw-r--r--   0 robert    (1000) robert    (1000)     4181 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/html/_static/nature.css
+-rw-r--r--   0 robert    (1000) robert    (1000)       90 2022-02-23 18:30:51.000000 metaindex-2.2.0/doc/build/html/_static/plus.png
+-rw-r--r--   0 robert    (1000) robert    (1000)     5432 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/html/_static/pygments.css
+-rw-r--r--   0 robert    (1000) robert    (1000)    16793 2022-02-23 18:30:51.000000 metaindex-2.2.0/doc/build/html/_static/searchtools.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    68420 2022-02-23 18:30:51.000000 metaindex-2.2.0/doc/build/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    19530 2022-02-23 18:30:51.000000 metaindex-2.2.0/doc/build/html/_static/underscore.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    11398 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/html/addons.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    16853 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/html/changelog.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    12806 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/html/cmdoptions.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     6745 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/html/cmdusage.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    20977 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/html/configuration.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     4029 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/html/description.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    13768 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/html/examples.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    16741 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/html/extrametadata.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    18918 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/html/genindex.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     6742 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/html/index.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    20498 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/html/indexers.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     7101 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/html/install.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     5360 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/html/license.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     1235 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/html/objects.inv
+-rw-r--r--   0 robert    (1000) robert    (1000)    66164 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/html/reference.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     3093 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/html/search.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    17128 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/html/searchindex.js
+-rw-r--r--   0 robert    (1000) robert    (1000)     9155 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/html/searchsyntax.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     3970 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/html/synopsis.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    14783 2022-03-20 10:53:28.000000 metaindex-2.2.0/doc/build/html/usage.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     3334 2022-02-25 14:43:32.000000 metaindex-2.2.0/doc/cmdoptions.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      804 2022-02-23 18:26:43.000000 metaindex-2.2.0/doc/make.bat
+-rw-r--r--   0 robert    (1000) robert    (1000)      901 2022-02-25 21:18:16.000000 metaindex-2.2.0/doc/metaindex.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)       19 2022-02-23 18:30:21.000000 metaindex-2.2.0/doc/requirements.txt
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-27 19:17:27.494290 metaindex-2.2.0/doc/source/
+-rw-r--r--   0 robert    (1000) robert    (1000)     2736 2022-03-13 15:27:55.000000 metaindex-2.2.0/doc/source/addons.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)       80 2022-02-23 18:39:36.000000 metaindex-2.2.0/doc/source/changelog.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     5229 2023-05-27 16:55:33.000000 metaindex-2.2.0/doc/source/cmdoptions.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      653 2023-05-11 18:09:52.000000 metaindex-2.2.0/doc/source/cmdusage.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     1871 2022-02-23 18:29:41.000000 metaindex-2.2.0/doc/source/conf.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     8069 2023-05-18 15:06:36.000000 metaindex-2.2.0/doc/source/configuration.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      726 2022-03-10 18:16:36.000000 metaindex-2.2.0/doc/source/description.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     1052 2022-03-20 09:25:44.000000 metaindex-2.2.0/doc/source/examples.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     4869 2022-02-25 20:09:22.000000 metaindex-2.2.0/doc/source/extrametadata.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      332 2022-03-13 15:16:59.000000 metaindex-2.2.0/doc/source/index.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     6931 2023-05-19 09:14:51.000000 metaindex-2.2.0/doc/source/indexers.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     1151 2022-02-23 18:37:25.000000 metaindex-2.2.0/doc/source/install.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)       58 2022-02-23 18:40:10.000000 metaindex-2.2.0/doc/source/license.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      664 2022-03-20 10:20:29.000000 metaindex-2.2.0/doc/source/reference.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     1964 2022-03-13 16:29:46.000000 metaindex-2.2.0/doc/source/searchsyntax.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      105 2022-02-25 19:48:09.000000 metaindex-2.2.0/doc/source/synopsis.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)       55 2022-02-25 19:48:15.000000 metaindex-2.2.0/doc/source/usage.rst
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-27 19:17:27.494290 metaindex-2.2.0/examples/
+-rw-r--r--   0 robert    (1000) robert    (1000)     1223 2022-03-20 09:43:43.000000 metaindex-2.2.0/examples/indexing.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-27 19:17:27.494290 metaindex-2.2.0/man/
+-rw-r--r--   0 robert    (1000) robert    (1000)    36585 2023-05-27 19:17:27.000000 metaindex-2.2.0/man/metaindex.1
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-27 19:17:27.497623 metaindex-2.2.0/metaindex/
+-rw-r--r--   0 robert    (1000) robert    (1000)      274 2023-05-16 17:26:33.000000 metaindex-2.2.0/metaindex/__init__.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    16060 2023-05-27 16:53:24.000000 metaindex-2.2.0/metaindex/cache.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    12458 2023-05-27 07:57:02.000000 metaindex-2.2.0/metaindex/cacheentry.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1968 2023-05-11 18:09:52.000000 metaindex-2.2.0/metaindex/client.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    24347 2023-05-27 19:11:56.000000 metaindex-2.2.0/metaindex/configuration.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-27 19:17:27.497623 metaindex-2.2.0/metaindex/docs/
+-rw-r--r--   0 robert    (1000) robert    (1000)    13555 2023-05-27 19:17:27.000000 metaindex-2.2.0/metaindex/docs/cmdoptions.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    54591 2023-05-27 19:17:27.000000 metaindex-2.2.0/metaindex/docs/metaindex.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     2859 2023-05-11 18:09:52.000000 metaindex-2.2.0/metaindex/find.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    18409 2021-10-16 07:30:31.000000 metaindex-2.2.0/metaindex/fuse.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4287 2022-06-18 22:14:53.000000 metaindex-2.2.0/metaindex/humanizer.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    15257 2023-05-27 08:40:30.000000 metaindex-2.2.0/metaindex/indexer.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-27 19:17:27.497623 metaindex-2.2.0/metaindex/indexers/
+-rw-r--r--   0 robert    (1000) robert    (1000)      512 2023-05-27 08:36:14.000000 metaindex-2.2.0/metaindex/indexers/__init__.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1972 2022-08-21 19:12:49.000000 metaindex-2.2.0/metaindex/indexers/abc.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1157 2022-05-11 17:49:48.000000 metaindex-2.2.0/metaindex/indexers/audio.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4956 2023-05-23 18:18:09.000000 metaindex-2.2.0/metaindex/indexers/collections.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     6714 2023-05-27 16:39:21.000000 metaindex-2.2.0/metaindex/indexers/comicbook.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1498 2022-06-27 12:23:51.000000 metaindex-2.2.0/metaindex/indexers/epub.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4742 2023-05-27 16:27:19.000000 metaindex-2.2.0/metaindex/indexers/filetags.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4435 2023-05-27 16:28:19.000000 metaindex-2.2.0/metaindex/indexers/gpx.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3061 2023-05-27 18:49:01.000000 metaindex-2.2.0/metaindex/indexers/html.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3801 2023-05-27 18:51:23.000000 metaindex-2.2.0/metaindex/indexers/images.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     2788 2023-05-27 18:54:57.000000 metaindex-2.2.0/metaindex/indexers/ooxml.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     2876 2023-05-27 18:56:00.000000 metaindex-2.2.0/metaindex/indexers/opendocument.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3353 2023-05-27 19:11:05.000000 metaindex-2.2.0/metaindex/indexers/pdf.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    10676 2023-05-19 08:45:31.000000 metaindex-2.2.0/metaindex/indexers/ruleindexer.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4503 2023-05-27 08:16:14.000000 metaindex-2.2.0/metaindex/json.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1566 2023-05-19 08:54:45.000000 metaindex-2.2.0/metaindex/logger.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     9165 2023-05-27 16:56:12.000000 metaindex-2.2.0/metaindex/main.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4853 2023-05-23 19:05:27.000000 metaindex-2.2.0/metaindex/ocr.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     2757 2023-05-27 16:14:29.000000 metaindex-2.2.0/metaindex/opf.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     8167 2023-05-27 09:09:18.000000 metaindex-2.2.0/metaindex/proto.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    27524 2023-05-27 08:10:45.000000 metaindex-2.2.0/metaindex/server.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4322 2023-05-27 16:15:51.000000 metaindex-2.2.0/metaindex/shared.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3198 2023-05-11 18:09:52.000000 metaindex-2.2.0/metaindex/stores.py
+-rw-r--r--   0 robert    (1000) robert    (1000)       23 2023-05-27 19:17:06.000000 metaindex-2.2.0/metaindex/version.py
+-rw-r--r--   0 robert    (1000) robert    (1000)      734 2022-06-27 12:20:41.000000 metaindex-2.2.0/metaindex/xmlproxy.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3898 2023-05-27 08:16:00.000000 metaindex-2.2.0/metaindex/yaml.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-27 19:17:27.497623 metaindex-2.2.0/metaindex.egg-info/
+-rw-r--r--   0 robert    (1000) robert    (1000)     4861 2023-05-27 19:17:27.000000 metaindex-2.2.0/metaindex.egg-info/PKG-INFO
+-rw-r--r--   0 robert    (1000) robert    (1000)     4390 2023-05-27 19:17:27.000000 metaindex-2.2.0/metaindex.egg-info/SOURCES.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)        1 2023-05-27 19:17:27.000000 metaindex-2.2.0/metaindex.egg-info/dependency_links.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       88 2023-05-27 19:17:27.000000 metaindex-2.2.0/metaindex.egg-info/entry_points.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      235 2023-05-27 19:17:27.000000 metaindex-2.2.0/metaindex.egg-info/requires.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       29 2023-05-27 19:17:27.000000 metaindex-2.2.0/metaindex.egg-info/top_level.txt
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-27 19:17:27.497623 metaindex-2.2.0/misc/
+-rw-r--r--   0 robert    (1000) robert    (1000)     2161 2023-05-11 18:09:52.000000 metaindex-2.2.0/misc/metaindex.conf
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-27 19:17:27.497623 metaindex-2.2.0/misc/ranger_metaindex/
+-rw-r--r--   0 robert    (1000) robert    (1000)       41 2021-09-01 18:34:21.000000 metaindex-2.2.0/misc/ranger_metaindex/__init__.py
+-rw-r--r--   0 robert    (1000) robert    (1000)      737 2023-05-11 18:09:16.000000 metaindex-2.2.0/misc/ranger_metaindex/linemode.py
+-rw-r--r--   0 robert    (1000) robert    (1000)       38 2023-05-27 19:17:27.497623 metaindex-2.2.0/setup.cfg
+-rw-r--r--   0 robert    (1000) robert    (1000)     3664 2023-05-21 10:28:55.000000 metaindex-2.2.0/setup.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-27 19:17:27.497623 metaindex-2.2.0/tests/
+-rw-r--r--   0 robert    (1000) robert    (1000)     1072 2022-08-21 19:09:08.000000 metaindex-2.2.0/tests/test_abc.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4343 2023-05-11 18:09:52.000000 metaindex-2.2.0/tests/test_cache.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3043 2022-06-24 07:16:59.000000 metaindex-2.2.0/tests/test_cacheentry.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3933 2022-06-27 09:57:52.000000 metaindex-2.2.0/tests/test_cleanup.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     2529 2022-02-26 17:13:44.000000 metaindex-2.2.0/tests/test_collect.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4866 2022-03-13 18:33:11.000000 metaindex-2.2.0/tests/test_humanizer.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1460 2022-03-15 17:55:22.000000 metaindex-2.2.0/tests/test_indexers.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3895 2022-02-26 16:28:16.000000 metaindex-2.2.0/tests/test_json.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     2549 2022-04-30 12:43:40.000000 metaindex-2.2.0/tests/test_ruleindexer.py
```

### Comparing `metaindex-2.1.1/CHANGELOG.md` & `metaindex-2.2.0/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,31 @@
 # Changelog
 
 This file contains the changes made between released versions.
 
 The format is based on [Keep a changelog](https://keepachangelog.com/) and the versioning tries to follow
 [Semantic Versioning](https://semver.org).
 
+## Not released yet
+### Changed
+- Use [PyPDF](https://pypi.org/project/pypdf/) instead of pdfminer for PDF indexing
+- `OCRFacility.run` can be given a language to work with to prevent guessing
+- Collection and side-car files are processed first now, instead of last to allow defining languages
+- The optional `callback`, that can be used to inspect the status of the indexer, sees the un-`reduce`d `CacheEntry`. Makes it more useful for testing rule indexers and such.
+- Timestamp-like occurrences (like `filetags.date`) have been split into `.date` and `.time`. You can search each respectively with `date:` or `time:`
+
+### Added
+- `OCRFacility` can be queried for supported languages
+- Another level of verbosity when indexing: `-vvvvv`, prints also all found metadata
+
+### Fixed
+- Server could crash when read-only connections were made and the cache directory doesn’t exist yet
+- Some code duplication removed for writing YAML and JSON sidecar files
+
+
 ## 2.1.1
 ### Changed
 - Server will return results even if the match score is very low
 
 ### Fixed
 - The rule based indexer will be more resilient against non-matching `find` directives
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `metaindex-2.1.1/LICENSE` & `metaindex-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/PKG-INFO` & `metaindex-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaindex
-Version: 2.1.1
+Version: 2.2.0
 Summary: Utilities to tag files
 Home-page: https://vonshednob.cc/metaindex
 Author: R
 Author-email: devel+metaindex@kakaomilchkuh.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `metaindex-2.1.1/README.md` & `metaindex-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/Makefile` & `metaindex-2.2.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/doctrees/addons.doctree` & `metaindex-2.2.0/doc/build/doctrees/addons.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/doctrees/changelog.doctree` & `metaindex-2.2.0/doc/build/doctrees/changelog.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/doctrees/cmdoptions.doctree` & `metaindex-2.2.0/doc/build/doctrees/cmdoptions.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/doctrees/cmdusage.doctree` & `metaindex-2.2.0/doc/build/doctrees/cmdusage.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/doctrees/configuration.doctree` & `metaindex-2.2.0/doc/build/doctrees/configuration.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/doctrees/description.doctree` & `metaindex-2.2.0/doc/build/doctrees/description.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/doctrees/environment.pickle` & `metaindex-2.2.0/doc/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/doctrees/examples.doctree` & `metaindex-2.2.0/doc/build/doctrees/examples.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/doctrees/extrametadata.doctree` & `metaindex-2.2.0/doc/build/doctrees/extrametadata.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/doctrees/index.doctree` & `metaindex-2.2.0/doc/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/doctrees/indexers.doctree` & `metaindex-2.2.0/doc/build/doctrees/indexers.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/doctrees/install.doctree` & `metaindex-2.2.0/doc/build/doctrees/install.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/doctrees/license.doctree` & `metaindex-2.2.0/doc/build/doctrees/license.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/doctrees/reference.doctree` & `metaindex-2.2.0/doc/build/doctrees/reference.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/doctrees/searchsyntax.doctree` & `metaindex-2.2.0/doc/build/doctrees/searchsyntax.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/doctrees/synopsis.doctree` & `metaindex-2.2.0/doc/build/doctrees/synopsis.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/doctrees/usage.doctree` & `metaindex-2.2.0/doc/build/doctrees/usage.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/_sources/addons.rst.txt` & `metaindex-2.2.0/doc/build/html/_sources/addons.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/_sources/cmdoptions.rst.txt` & `metaindex-2.2.0/doc/build/html/_sources/cmdoptions.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/_sources/cmdusage.rst.txt` & `metaindex-2.2.0/doc/build/html/_sources/cmdusage.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/_sources/configuration.rst.txt` & `metaindex-2.2.0/doc/build/html/_sources/configuration.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/_sources/description.rst.txt` & `metaindex-2.2.0/doc/build/html/_sources/description.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/_sources/examples.rst.txt` & `metaindex-2.2.0/doc/build/html/_sources/examples.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/_sources/extrametadata.rst.txt` & `metaindex-2.2.0/doc/build/html/_sources/extrametadata.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/_sources/indexers.rst.txt` & `metaindex-2.2.0/doc/build/html/_sources/indexers.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/_sources/install.rst.txt` & `metaindex-2.2.0/doc/build/html/_sources/install.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/_sources/reference.rst.txt` & `metaindex-2.2.0/doc/build/html/_sources/reference.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/_sources/searchsyntax.rst.txt` & `metaindex-2.2.0/doc/build/html/_sources/searchsyntax.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/_static/basic.css` & `metaindex-2.2.0/doc/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/_static/doctools.js` & `metaindex-2.2.0/doc/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/_static/jquery-3.5.1.js` & `metaindex-2.2.0/doc/build/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/_static/jquery.js` & `metaindex-2.2.0/doc/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/_static/language_data.js` & `metaindex-2.2.0/doc/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/_static/nature.css` & `metaindex-2.2.0/doc/build/html/_static/nature.css`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/_static/pygments.css` & `metaindex-2.2.0/doc/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/_static/searchtools.js` & `metaindex-2.2.0/doc/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/_static/underscore-1.13.1.js` & `metaindex-2.2.0/doc/build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/_static/underscore.js` & `metaindex-2.2.0/doc/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/addons.html` & `metaindex-2.2.0/doc/build/html/addons.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/changelog.html` & `metaindex-2.2.0/doc/build/html/changelog.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/cmdoptions.html` & `metaindex-2.2.0/doc/build/html/cmdoptions.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/cmdusage.html` & `metaindex-2.2.0/doc/build/html/cmdusage.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/configuration.html` & `metaindex-2.2.0/doc/build/html/configuration.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/description.html` & `metaindex-2.2.0/doc/build/html/description.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/examples.html` & `metaindex-2.2.0/doc/build/html/examples.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/extrametadata.html` & `metaindex-2.2.0/doc/build/html/extrametadata.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/genindex.html` & `metaindex-2.2.0/doc/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/index.html` & `metaindex-2.2.0/doc/build/html/index.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/indexers.html` & `metaindex-2.2.0/doc/build/html/indexers.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/install.html` & `metaindex-2.2.0/doc/build/html/install.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/license.html` & `metaindex-2.2.0/doc/build/html/license.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/objects.inv` & `metaindex-2.2.0/doc/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/reference.html` & `metaindex-2.2.0/doc/build/html/reference.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/search.html` & `metaindex-2.2.0/doc/build/html/search.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/searchindex.js` & `metaindex-2.2.0/doc/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/searchsyntax.html` & `metaindex-2.2.0/doc/build/html/searchsyntax.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/synopsis.html` & `metaindex-2.2.0/doc/build/html/synopsis.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/build/html/usage.html` & `metaindex-2.2.0/doc/build/html/usage.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/cmdoptions.rst` & `metaindex-2.2.0/doc/cmdoptions.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/make.bat` & `metaindex-2.2.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/metaindex.rst` & `metaindex-2.2.0/doc/metaindex.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/source/addons.rst` & `metaindex-2.2.0/doc/source/addons.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/source/cmdoptions.rst` & `metaindex-2.2.0/doc/source/cmdoptions.rst`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,15 @@
     times (``-vvvv``). The steps are:
 
      * No ``-v``: no output other than errors or information from certain indexers
      * ``-v``: print a ``.`` per file indexed
      * ``-vv``: same as ``-v`` and print how many files were indexed in the end
      * ``-vvv``: same as ``-vv`` but also show how long it took
      * ``-vvvv``: same as ``-vvv`` but print the path of each indexed file instead of just a ``.``
+     * ``-vvvvv``: same as ``-vvvv`` but also prints all found metadata tags (except for fulltext)
 
   ``paths``
     Run the indexer on these paths.
     If ``paths`` is ``-``, the list of files will be read from stdin, one
     file per line.
```

### Comparing `metaindex-2.1.1/doc/source/cmdusage.rst` & `metaindex-2.2.0/doc/source/cmdusage.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/source/conf.py` & `metaindex-2.2.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/source/configuration.rst` & `metaindex-2.2.0/doc/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/source/description.rst` & `metaindex-2.2.0/doc/source/description.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/source/examples.rst` & `metaindex-2.2.0/doc/source/examples.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/source/extrametadata.rst` & `metaindex-2.2.0/doc/source/extrametadata.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/source/indexers.rst` & `metaindex-2.2.0/doc/source/indexers.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/source/install.rst` & `metaindex-2.2.0/doc/source/install.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/source/reference.rst` & `metaindex-2.2.0/doc/source/reference.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/doc/source/searchsyntax.rst` & `metaindex-2.2.0/doc/source/searchsyntax.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/examples/indexing.py` & `metaindex-2.2.0/examples/indexing.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/man/metaindex.1` & `metaindex-2.2.0/man/metaindex.1`

 * *Files 1% similar despite different names*

```diff
@@ -250,14 +250,16 @@
 \fB\-v\fP: print a \fB\&.\fP per file indexed
 .IP \(bu 2
 \fB\-vv\fP: same as \fB\-v\fP and print how many files were indexed in the end
 .IP \(bu 2
 \fB\-vvv\fP: same as \fB\-vv\fP but also show how long it took
 .IP \(bu 2
 \fB\-vvvv\fP: same as \fB\-vvv\fP but print the path of each indexed file instead of just a \fB\&.\fP
+.IP \(bu 2
+\fB\-vvvvv\fP: same as \fB\-vvvv\fP but also prints all found metadata tags (except for fulltext)
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .TP
 .B \fBpaths\fP
 Run the indexer on these paths.
 If \fBpaths\fP is \fB\-\fP, the list of files will be read from stdin, one
```

### Comparing `metaindex-2.1.1/metaindex/cache.py` & `metaindex-2.2.0/metaindex/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,17 @@
         processes may be set to a number of processes that will be used in
         parallel to index the files. If left at None, there will be as many
         processes launched as CPUs are available.
 
         ``callback`` may be a function that accepts one parameter: the CacheEntry
         instance of a newly indexed document. When indexing many files, this
         callback will be called per file, if it's not ``None``.
+        Note that the CacheEntry will not have been reduced (see CacheBase.reduce)
+        for the callback. If you want to only use the metadata that will actually
+        end up in the index cache, call ``.reduce()`` on it first.
 
         ``storage`` is the human-readable (and human-provided) label for the storage
         that the files are residing on'
         """
         raise NotImplementedError()
 
     def cleanup(self, paths=None):
@@ -124,14 +127,30 @@
 
         for filename in data.keys():
             data[filename][shared.IS_RECURSIVE] = data[filename][shared.IS_RECURSIVE] and \
                                                   self.config.recursive_extra_metadata
 
         return data
 
+    def reduce(self, entry):
+        """Reduces the tags in ``CacheEntry`` ``entry`` in place
+
+        Modifications are done in place to ``entry``, but for convenience, ``entry`` is
+        also returned.
+
+        It removes all metadata fields that are not in the synonyms.
+        """
+        for key in set(entry.metadata.keys()):
+            if key in self.config.synonymized:
+                entry.metadata[key] = list(set(entry.metadata[key]))
+            else:
+                del entry.metadata[key]
+
+        return entry
+
 
 class XapianClientCache(CacheBase):
     """A Cache-interface that connects to the local xapian server backend"""
     def __init__(self, config=None):
         super().__init__(config)
         self.client = Client(self.config)
         try:
@@ -231,28 +250,28 @@
         results = []
         for result in generator:
             if not result.success and not self.config.index_unknown:
                 continue
 
             try:
                 result.info.last_modified = last_modified[result.filename]
-                indexed = self.reduce(result.info)
+                indexed = self.reduce(result.info.copy())
                 indexed.rel_path = shared.make_mount_relative(indexed.path)
                 indexed.storage_label = storage
                 results.append(indexed)
 
                 self.client.ensure_connection()
                 self.client.send(proto.Update(entries=[indexed]))
                 response = self.client.recv()
                 if not response:
                     logger.error("Failed to update database: %s", response.reason)
                     break
 
                 if callback is not None:
-                    callback(indexed)
+                    callback(result.info)
             except KeyboardInterrupt:
                 break
 
         return results
 
     def insert(self, item):
         self.client.ensure_connection()
@@ -296,30 +315,14 @@
                      for path in paths]
         entries = [CacheEntry(p) for p in paths]
 
         self.client.ensure_connection()
         self.client.send(proto.Update(entries=entries))
         self.client.recv()
 
-    def reduce(self, entry):
-        """Reduces the tags in ``CacheEntry`` ``entry`` in place
-
-        Modifications are done in place to ``entry``, but for convenience, ``entry`` is
-        also returned.
-
-        It removes all metadata fields that are not in the synonyms.
-        """
-        for key in set(entry.metadata.keys()):
-            if key in self.config.synonymized:
-                entry.metadata[key] = list(set(entry.metadata[key]))
-            else:
-                del entry.metadata[key]
-
-        return entry
-
 
 class ThreadedCache(CacheBase):
     """Special version of Cache to be used in multi-threaded applications
 
     To use this, create an instance and execute ``start``.
     """
     GET = "get"
```

### Comparing `metaindex-2.1.1/metaindex/cacheentry.py` & `metaindex-2.2.0/metaindex/cacheentry.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,14 +183,18 @@
         result = {'path': str(self.path),
                   'last_modified': strfdt(self.last_modified),
                   'slbl': self.storage_label,
                   'rpath': jsonify(self.rel_path),
                   'mime': self.mimetype,
                   'metadata': {key: [jsonify(v.raw_value) for v in values]
                                for key, values in self.metadata.items()}}
+        # reduce unnecessary lists to single entries
+        for key in set(result['metadata'].keys()):
+            if len(result['metadata'][key]) == 1:
+                result['metadata'][key] = result['metadata'][key][0]
         return result
 
     def copy(self):
         """Create a deep copy of this cache entry"""
         that = type(self)(str(self.path))
         that.metadata = {key: [v.copy() for v in values]
                          for key, values in self.metadata.items()}
```

### Comparing `metaindex-2.1.1/metaindex/client.py` & `metaindex-2.2.0/metaindex/client.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/metaindex/configuration.py` & `metaindex-2.2.0/metaindex/configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,31 @@
             'date': {
                 "extra.date",
                 "rules.date",
                 "comicbook.date",
                 "gpx.time",
                 "opendocument.date",
                 "officeopenxml.date",
+                "filetags.date",
+                "html.date",
+                "exif.date",
+                "pdf.date",
+                "pdf.creation_date",
+                "pdf.modification_date",
                 },
+            'time': {
+                "extra.time",
+                "rules.time",
+                "filetags.time",
+                "html.time",
+                "exif.time",
+                "opendocument.time",
+                "officeopenxml.time",
+                "pdf.time",
+            },
             'title': {
                 "extra.title",
                 "opf.title",
                 "id3.title",
                 "rules.title",
                 "pdf.title",
                 "filetags.title",
@@ -93,19 +109,23 @@
                 "comicbook.tags",
                 "opf.subject",
                 "gpx.keyword",
                 "opendocument.keyword",
                 "opendocument.subject",
                 "officeopenxml.keyword",
                 "officeopenxml.subject",
+                "filetags.tag",
                 },
             'rating': {
                 "extra.rating",
                 "xmp.rating",
                 },
+            'resolution': {
+                "image.resolution",
+            },
             'language': {
                 "opf.language",
                 "pdf.Language",
                 "xmp.dc.language",
                 "extra.language",
                 "rules.language",
                 "comicbook.languageiso"
@@ -134,14 +154,18 @@
 
 SOCKETPATH /= SOCKETPATH / (PROGRAMNAME + '.sock')
 
 ADDONSPATH = DATAPATH / "addons"
 LOGFILEPATH = CACHEPATH / "metaindex.log"
 LOGLEVEL = 'WARNING'
 
+EXTRA_MIMETYPES = [
+    ('application/gpx+xml', '.gpx'),
+]
+
 SECTION_GENERAL = 'General'
 SECTION_SYNONYMS = 'Synonyms'
 SECTION_INCLUDE = 'Include'
 SECTION_SERVER = 'Server'
 CONFIG_CACHE = 'cache'
 CONFIG_SOCKET = 'socket'
 CONFIG_RECURSIVE_EXTRA_METADATA = 'recursive-extra-metadata'
@@ -557,14 +581,17 @@
     def load_mimetypes(self):
         """Load the user-configured extra mimetypes"""
         extra_mimetypes = [str(pathlib.Path(fn.strip()).expanduser().resolve())
                            for fn in self.list(SECTION_GENERAL, CONFIG_MIMETYPES, "", "\n")]
         if len(extra_mimetypes) > 0:
             mimetypes.init(files=extra_mimetypes)
 
+        for type_, suffix in EXTRA_MIMETYPES:
+            mimetypes.add_type(type_, suffix)
+
     @staticmethod
     def load_addons():
         """Load the indexer addons"""
         # load indexer addons
         if ADDONSPATH.exists():
             prev_sys_path = sys.path.copy()
             sys.path = [str(ADDONSPATH)] + prev_sys_path
```

### Comparing `metaindex-2.1.1/metaindex/docs/cmdoptions.html` & `metaindex-2.2.0/metaindex/docs/cmdoptions.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/metaindex/docs/metaindex.html` & `metaindex-2.2.0/metaindex/docs/metaindex.html`

 * *Files 0% similar despite different names*

#### Comparing `metaindex-2.1.1/metaindex/docs/metaindex.html` & `metaindex-2.2.0/metaindex/docs/metaindex.html`

```diff
@@ -713,14 +713,24 @@
                       : same as
                       <tt class="docutils literal">
                         <span class="pre">-vvv</span>
                       </tt>
                       but print the path of each indexed file instead of just a
                       <tt class="docutils literal">.</tt>
                     </li>
+                    <li>
+                      <tt class="docutils literal">
+                        <span class="pre">-vvvvv</span>
+                      </tt>
+                      : same as
+                      <tt class="docutils literal">
+                        <span class="pre">-vvvv</span>
+                      </tt>
+                      but also prints all found metadata tags (except for fulltext)
+                    </li>
                   </ul>
                 </blockquote>
               </dd>
               <dt>
                 <tt class="docutils literal">paths</tt>
               </dt>
               <dd>
```

### Comparing `metaindex-2.1.1/metaindex/find.py` & `metaindex-2.2.0/metaindex/find.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/metaindex/fuse.py` & `metaindex-2.2.0/metaindex/fuse.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/metaindex/humanizer.py` & `metaindex-2.2.0/metaindex/humanizer.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/metaindex/indexer.py` & `metaindex-2.2.0/metaindex/indexer.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/metaindex/indexers/abc.py` & `metaindex-2.2.0/metaindex/indexers/abc.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/metaindex/indexers/audio.py` & `metaindex-2.2.0/metaindex/indexers/audio.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/metaindex/indexers/collections.py` & `metaindex-2.2.0/metaindex/indexers/collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,37 +105,37 @@
 
 
 class JsonSidecarIndexer(CollectionSidecarIndexer):
     """JSON collection sidecar indexer"""
     NAME = 'json-sidecar'
     ACCEPT = '*'
     PREFIX = ''
-    ORDER = Order.LAST
+    ORDER = Order.FIRST
 
     def run(self, path, metadata, last_cached):
         return self.run_with_store(json, path, metadata, last_cached)
 
 
 class OpfSidecarIndexer(CollectionSidecarIndexer):
     """OPF collection sidecar indexer"""
     NAME = 'opf-sidecar'
     ACCEPT = '*'
     PREFIX = ''
-    ORDER = Order.LAST
+    ORDER = Order.FIRST
 
     def run(self, path, metadata, _):
         self.cache_collection_sidecars(path, opf)
         for key, value in self.get_collection_metadata(path, opf.SUFFIX):
             if key != shared.IS_RECURSIVE:
                 metadata.add(key, value)
 
 
 if yaml is not None:
     class YamlSidecarIndexer(CollectionSidecarIndexer):
         """YAML collection sidecar indexer"""
         NAME = 'yaml-sidecar'
         ACCEPT = '*'
         PREFIX = ''
-        ORDER = Order.LAST
+        ORDER = Order.FIRST
 
         def run(self, path, metadata, last_cached):
             return self.run_with_store(yaml, path, metadata, last_cached)
```

### Comparing `metaindex-2.1.1/metaindex/indexers/comicbook.py` & `metaindex-2.2.0/metaindex/indexers/comicbook.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,23 +96,40 @@
         assert isinstance(self.PREFIX, (set, tuple, list))
 
         root = etree.fromstring(str(xmldata, 'utf-8'))
         if root.tag != ComicBookInfo.ROOT_TAG:
             logger.info("Invalid root tag %s for ComicInfo.xml", root.tag)
             return
 
+        year_month_day = [0, 0, 0]
         for node in root:
             if node.tag in ComicBookInfo.FIELDS and node.text is not None:
                 metadata.add(self.PREFIX[0] + "." + node.tag.lower(),
                              node.text)
             elif node.tag == 'Pages':
                 pass  # TODO - do anything useful with pages?
             else:
                 logger.info("Unexpected tag %s in comicinfo.xml", node.tag)
 
+            if node.text is not None and \
+               node.text.isnumeric() and \
+               node.tag.lower() in ['year', 'month', 'day']:
+                if node.tag.lower() == 'year':
+                    year_month_day[0] = int(node.text)
+                elif node.tag.lower() == 'month':
+                    year_month_day[1] = int(node.text)
+                elif node.tag.lower() == 'day':
+                    year_month_day[2] = int(node.text)
+
+        arranged = []
+        while year_month_day[0] != 0:
+            arranged.append(str(year_month_day.pop(0)))
+        if len(arranged) > 0:
+            metadata.add(self.PREFIX[0] + '.date', '-'.join(arranged))
+
 
 class CBZArchiveReader(ArchiveReader):
     """CBZ archive reader"""
     def do_open(self):
         return zipfile.ZipFile(self.path, 'r')
 
     def do_close(self):
```

### Comparing `metaindex-2.1.1/metaindex/indexers/epub.py` & `metaindex-2.2.0/metaindex/indexers/epub.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/metaindex/indexers/gpx.py` & `metaindex-2.2.0/metaindex/indexers/gpx.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,16 @@
 
             for node in meta.findall('{*}time'):
                 if node.text is None:
                     continue
                 try:
                     timestamp = datetime.datetime.strptime(node.text[:19],
                                                            '%Y-%m-%dT%H:%M:%S')
-                    metadata.add(self.PREFIX + '.time', timestamp)
+                    metadata.add(self.PREFIX + '.date', timestamp.date())
+                    metadata.add(self.PREFIX + '.time', timestamp.time())
                 except ValueError:
                     pass
 
             for node in meta.findall('{*}keywords'):
                 if node.text is None or len(node.text.strip()) == 0:
                     continue
                 for word in node.text.split():
```

### Comparing `metaindex-2.1.1/metaindex/indexers/images.py` & `metaindex-2.2.0/metaindex/indexers/images.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,14 +62,16 @@
                             charset = charset.split('=', 1)[1]
                             value = str(bytes(value, 'utf-8'), charset)
                         except ValueError as exc:
                             logger.error(exc)
                 if key in ['exif.photo.datetimeoriginal', 'exif.photo.datetimedigitized',
                            'exif.image.datetime']:
                     value = datetime.datetime.strptime(value, '%Y:%m:%d %H:%M:%S')
+                    metadata.add('exif.date', value.date())
+                    metadata.add('exif.time', value.time())
 
                 if isinstance(value, str) and len(value) == 0:
                     continue
                 if isinstance(value, list):
                     result += [(key, v) for v in value]
                     continue
                 if isinstance(value, dict):
@@ -90,17 +92,27 @@
             logger.debug(f"[image, pillow] processing {path.name}")
 
             try:
                 meta = PIL.Image.open(path)
             except:
                 return
 
+            language = None
+            for tag, value in metadata:
+                if not tag.endswith('.language'):
+                    continue
+                if self.ocr.language_supported(str(value)):
+                    language = str(value)
+                    logger.debug(f"... assuming language is '{language}'")
+                    break
+
             if meta is not None:
                 metadata.add('image.resolution', "{}x{}".format(*meta.size))
                 if self.should_ocr(path):
-                    ocr = self.ocr.run(meta)
-                    if ocr.success:
+                    ocr = None
+                    if language is None or self.should_fulltext(path):
+                        ocr = self.ocr.run(meta, language)
+                    if ocr is not None and ocr.success:
                         metadata.add('ocr.language', ocr.language)
-                        if self.should_fulltext(path) and \
-                           len(ocr.fulltext) > 0:
-                            metadata.add('ocr.fulltext', ocr.fulltext)
+                        if len(ocr.fulltext.strip()) > 0:
+                            metadata.add('ocr.fulltext', ocr.fulltext.strip())
                 meta.close()
```

### Comparing `metaindex-2.1.1/metaindex/indexers/ooxml.py` & `metaindex-2.2.0/metaindex/indexers/ooxml.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,15 +55,16 @@
                 if node.text is None or len(node.text) == 0:
                     continue
                 try:
                     timestamp = datetime.datetime.strptime(node.text[:19],
                                                            '%Y-%m-%dT%H:%M:%S')
                 except ValueError:
                     continue
-                metadata.add(self.PREFIX + '.date', timestamp)
+                metadata.add(self.PREFIX + '.date', timestamp.date())
+                metadata.add(self.PREFIX + '.time', timestamp.time())
 
             for kwtag in ['keyword', 'keywords']:
                 for node in meta.findall('{*}' + kwtag):
                     if node.text is None or len(node.text) == 0:
                         continue
                     keywords = node.text.split()
                     for keyword in keywords:
```

### Comparing `metaindex-2.1.1/metaindex/indexers/opendocument.py` & `metaindex-2.2.0/metaindex/indexers/opendocument.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,15 +58,16 @@
                 if node.text is None or len(node.text) == 0:
                     continue
                 try:
                     timestamp = datetime.datetime.strptime(node.text[:19],
                                                            '%Y-%m-%dT%H:%M:%S')
                 except ValueError:
                     continue
-                metadata.add(self.PREFIX + '.date', timestamp)
+                metadata.add(self.PREFIX + '.date', timestamp.date())
+                metadata.add(self.PREFIX + '.time', timestamp.time())
 
             for node in meta.findall('{*}keyword'):
                 if node.text is None or len(node.text) == 0:
                     continue
                 keywords = node.text.split()
                 for keyword in keywords:
                     if len(keyword.strip()) == 0:
```

### Comparing `metaindex-2.1.1/metaindex/indexers/ruleindexer.py` & `metaindex-2.2.0/metaindex/indexers/ruleindexer.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/metaindex/json.py` & `metaindex-2.2.0/metaindex/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,17 +108,16 @@
         raise TypeError()
 
     blob = json.dumps(data, indent=2, ensure_ascii=False, sort_keys=True)
     filename.write(blob)
 
 
 def _cacheentry_as_dict(entry):
-    return {key.split('.', 1)[1]: [_raw_value_for_json(v.raw_value)
-                                   for v in values]
-            for key, values in entry.metadata.items()
+    return {key.split('.', 1)[1]: _raw_value_for_json(values)
+            for key, values in entry.as_dict().items()
             if key.startswith(shared.EXTRA)}
 
 
 def _raw_value_for_json(value):
     if value is None:
         return value
```

### Comparing `metaindex-2.1.1/metaindex/logger.py` & `metaindex-2.2.0/metaindex/logger.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/metaindex/main.py` & `metaindex-2.2.0/metaindex/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -160,14 +160,24 @@
 def index_status(config, entry):
     global indexed_files_count
     indexed_files_count += 1
     if 0 < config.verbose <= 3:
         print(".", end="", flush=True)
     if config.verbose >= 4:
         print(entry.path)
+    if config.verbose >= 5:
+        for key, values in entry.as_dict()['metadata'].items():
+            if key.endswith('.fulltext'):
+                continue
+            if isinstance(values, list) and len(values) > 1:
+                print(f"  {key}:")
+                for value in values:
+                    print(f"    - {value}")
+            else:
+                print(f"  {key}: {values}")
 
 
 def run():
     args = parse_args()
     logger.setup(level=args.log_level.upper(), filename=args.log_file)
 
     config = configuration.load(args.config)
```

### Comparing `metaindex-2.1.1/metaindex/opf.py` & `metaindex-2.2.0/metaindex/opf.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pathlib
+import datetime
 
 from metaindex import shared
 from metaindex.cacheentry import CacheEntry
 from metaindex.xmlproxy import etree, check_defusedxml
 
 
 SUFFIX = '.opf'
@@ -28,29 +29,51 @@
     data = parse_opf(metadatafile.read(), prefix=shared.EXTRA)
     data.path = basepath
     data.add(shared.IS_RECURSIVE, True)
 
     return {basepath: data}
 
 
+DT_FORMATS = [('%Y-%m-%dT%H:%M:%S', 19, ''),
+              ('%Y-%m-%d', 10, 'date')]
+
+
 def parse_opf(content, prefix='opf.'):
     check_defusedxml()
     result = CacheEntry(None)
 
     try:
         root = etree.fromstring(content)
     except:
         return result
 
     for node in root.findall('.//{http://purl.org/dc/elements/1.1/}*'):
         # tag name will start with {namespace}, get rid of it
         _, tagname = node.tag.split('}', 1)
 
+        text = node.text
+        if tagname == 'date':
+            for fmt, length, type_ in DT_FORMATS:
+                try:
+                    text = datetime.datetime.strptime(text[:length], fmt)
+                    if type_ == 'date':
+                        text = text.date()
+                    break
+                except ValueError as exc:
+                    pass
+
         tagname = prefix + tagname
-        result.add(tagname, node.text)
+
+        if isinstance(text, datetime.datetime):
+            result.add(prefix + 'date', text.date())
+            result.add(prefix + 'time', text.time())
+        elif isinstance(text, datetime.date):
+            result.add(prefix + 'date', text)
+        else:
+            result.add(tagname, text)
 
     for node in root.findall('.//{http://www.idpf.org/2007/opf}meta'):
         _, tagname = node.tag.split('}', 1)
 
         if 'name' not in node.keys() or 'content' not in node.keys():
             continue
```

### Comparing `metaindex-2.1.1/metaindex/proto.py` & `metaindex-2.2.0/metaindex/proto.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/metaindex/server.py` & `metaindex-2.2.0/metaindex/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,25 +206,32 @@
         self.prefix_to_human = {value: key
                                 for key, value in self.human_to_prefix.items()}
         # reset the queryparser to enforce reloading of the translations
         self._qparser = None
 
     def save_prefix_translations(self):
         """Save the translations of tag->xapian prefix to disk"""
+        self.prefixpath.parent.mkdir(parents=True, exist_ok=True)
+
         with open(self.prefixpath, 'wt', newline='', encoding='utf-8') as prefixfile:
             writer = csv.writer(prefixfile)
             writer.writerows([[title, prefix]
                               for title, prefix in sorted(self.human_to_prefix.items())])
 
     def ensure_connection(self):
         """Ensure that the xapian database connection is established and "fresh".
 
         Returns 'False' if no database connection could be established.
         """
         if self.dbconn is None:
+            if not self.dbpath.exists() or len(list(self.dbpath.iterdir())) == 0:
+                self.dbpath.mkdir(parents=True)
+                dbconn = xapian.WritableDatabase(str(self.dbpath))
+                dbconn.close()
+
             try:
                 self.dbconn = xapian.Database(str(self.dbpath))
             except xapian.DatabaseNotFoundError as exc:
                 logger.debug("Read connection failed: %s", exc)
                 return False
 
         self.dbconn.reopen()
```

### Comparing `metaindex-2.1.1/metaindex/shared.py` & `metaindex-2.2.0/metaindex/shared.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import codecs
 import datetime
 from pathlib import Path
 
 EXTRA = 'extra.'
 IS_RECURSIVE = 'extra_metadata_is_recursive'
 LAST_MODIFIED = 'extra_metadata_last_modified'
-TIMESTAMP_FORMAT = "%Y%m%dT%H%M%S"
+TIMESTAMP_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 DUBLINCORE_TAGS = {
     'contributor',
     'coverage',
     'creator',
     'date',
     'description',
@@ -112,17 +112,21 @@
 
 def jsonify(that):
     """Return ``that`` in a form that can be exported as JSON"""
     if isinstance(that, datetime.datetime):
         return strfdt(that)
 
     if isinstance(that, datetime.date):
-        text = that.strftime("%Y%m%d")
+        text = that.strftime("%Y-%m-%d")
         return "0"*(max(0, 8-len(text)))+text
 
+    if isinstance(that, datetime.time):
+        text = that.strftime("%H:%M:%S")
+        return text
+
     if isinstance(that, (tuple, set)):
         return list(that)
 
     if isinstance(that, Path):
         return str(that)
 
     return that
```

### Comparing `metaindex-2.1.1/metaindex/stores.py` & `metaindex-2.2.0/metaindex/stores.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/metaindex/xmlproxy.py` & `metaindex-2.2.0/metaindex/xmlproxy.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/metaindex/yaml.py` & `metaindex-2.2.0/metaindex/yaml.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,16 +109,16 @@
         raise TypeError()
 
     blob = yaml.safe_dump(data, indent=4, allow_unicode=True)
     filename.write(blob)
 
 
 def _cacheentry_as_dict(entry):
-    return {key.split('.', 1)[1]: [v.raw_value for v in values]
-            for key, values in entry.metadata.items()
+    return {key.split('.', 1)[1]: values
+            for key, values in entry.as_dict().items()
             if key.startswith(shared.EXTRA)}
 
 
 def _read_yaml_file(filename):
     try:
         data = yaml.safe_load(filename.read())
     except Exception as exc:
```

### Comparing `metaindex-2.1.1/metaindex.egg-info/PKG-INFO` & `metaindex-2.2.0/metaindex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaindex
-Version: 2.1.1
+Version: 2.2.0
 Summary: Utilities to tag files
 Home-page: https://vonshednob.cc/metaindex
 Author: R
 Author-email: devel+metaindex@kakaomilchkuh.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `metaindex-2.1.1/metaindex.egg-info/SOURCES.txt` & `metaindex-2.2.0/metaindex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/misc/metaindex.conf` & `metaindex-2.2.0/misc/metaindex.conf`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/misc/ranger_metaindex/linemode.py` & `metaindex-2.2.0/misc/ranger_metaindex/linemode.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/setup.py` & `metaindex-2.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 def example_files():
     path = pathlib.Path('./examples')
     return list('examples/' + fn.name for fn in path.iterdir() if fn.suffix == '.py')
 
 
 xdg_reqs = ['pyxdg']
 image_reqs = ['pyexiv2', 'pillow']
-pdf_reqs = ['pdfminer']
+pdf_reqs = ['pypdf']
 audio_reqs = ['mutagen']
 video_reqs = ['mutagen']
 ebook_reqs = ['defusedxml']
 fuse_reqs = ['trio', 'pyfuse3']
 yaml_reqs = ['pyyaml']
 ocr_reqs = ['pillow>=6.2.0']
 all_reqs = set(sum([xdg_reqs, image_reqs, pdf_reqs, audio_reqs, video_reqs,
```

### Comparing `metaindex-2.1.1/tests/test_abc.py` & `metaindex-2.2.0/tests/test_abc.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/tests/test_cache.py` & `metaindex-2.2.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/tests/test_cacheentry.py` & `metaindex-2.2.0/tests/test_cacheentry.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/tests/test_cleanup.py` & `metaindex-2.2.0/tests/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/tests/test_collect.py` & `metaindex-2.2.0/tests/test_collect.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/tests/test_humanizer.py` & `metaindex-2.2.0/tests/test_humanizer.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/tests/test_indexers.py` & `metaindex-2.2.0/tests/test_indexers.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/tests/test_json.py` & `metaindex-2.2.0/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.1.1/tests/test_ruleindexer.py` & `metaindex-2.2.0/tests/test_ruleindexer.py`

 * *Files identical despite different names*

