# Comparing `tmp/charidotella-1.1.0.tar.gz` & `tmp/charidotella-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charidotella-1.1.0.tar", last modified: Sat May  6 01:21:36 2023, max compression
+gzip compressed data, was "charidotella-1.2.0.tar", last modified: Sun May 28 11:10:07 2023, max compression
```

## Comparing `charidotella-1.1.0.tar` & `charidotella-1.2.0.tar`

### file list

```diff
@@ -1,78 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:21:36.490579 charidotella-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-06 01:21:36.000000 charidotella-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-05-06 01:21:36.490579 charidotella-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-06 01:20:30.000000 charidotella-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:21:36.466579 charidotella-1.1.0/charidotella/
--rw-r--r--   0 runner    (1001) docker     (123)    44162 2023-05-06 01:20:30.000000 charidotella-1.1.0/charidotella/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-06 01:20:30.000000 charidotella-1.1.0/charidotella/animals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:21:36.474579 charidotella-1.1.0/charidotella/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    27056 2023-05-06 01:20:30.000000 charidotella-1.1.0/charidotella/assets/configuration-schema.json
--rwxr-xr-x   0 runner    (1001) docker     (123)  1035600 2023-05-06 01:21:04.000000 charidotella-1.1.0/charidotella/assets/es_to_frames
--rwxr-xr-x   0 runner    (1001) docker     (123)   286032 2023-05-06 01:21:12.000000 charidotella-1.1.0/charidotella/assets/event_rate
--rwxr-xr-x   0 runner    (1001) docker     (123)    63800 2023-05-06 01:21:15.000000 charidotella-1.1.0/charidotella/assets/size
--rwxr-xr-x   0 runner    (1001) docker     (123)  1011024 2023-05-06 01:21:24.000000 charidotella-1.1.0/charidotella/assets/spatiospectrogram
--rwxr-xr-x   0 runner    (1001) docker     (123)   396632 2023-05-06 01:21:36.000000 charidotella-1.1.0/charidotella/assets/spectrogram
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-06 01:20:30.000000 charidotella-1.1.0/charidotella/charidotella_extension_placeholder.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:21:36.474579 charidotella-1.1.0/charidotella/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-06 01:20:30.000000 charidotella-1.1.0/charidotella/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-06 01:20:30.000000 charidotella-1.1.0/charidotella/filters/arbiter_saturation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-06 01:20:30.000000 charidotella-1.1.0/charidotella/filters/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-06 01:20:30.000000 charidotella-1.1.0/charidotella/filters/hot_pixels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-06 01:20:30.000000 charidotella-1.1.0/charidotella/filters/transpose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:21:36.478579 charidotella-1.1.0/charidotella/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-06 01:20:30.000000 charidotella-1.1.0/charidotella/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-06 01:20:30.000000 charidotella-1.1.0/charidotella/tasks/colourtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-06 01:20:30.000000 charidotella-1.1.0/charidotella/tasks/event_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-06 01:20:30.000000 charidotella-1.1.0/charidotella/tasks/spatiospectrogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-06 01:20:30.000000 charidotella-1.1.0/charidotella/tasks/spectrogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-06 01:20:30.000000 charidotella-1.1.0/charidotella/tasks/video.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-05-06 01:20:30.000000 charidotella-1.1.0/charidotella/tasks/wiggle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-06 01:20:30.000000 charidotella-1.1.0/charidotella/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-06 01:20:30.000000 charidotella-1.1.0/charidotella/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:21:36.470579 charidotella-1.1.0/charidotella.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-05-06 01:21:36.000000 charidotella-1.1.0/charidotella.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-06 01:21:36.000000 charidotella-1.1.0/charidotella.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 01:21:36.000000 charidotella-1.1.0/charidotella.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-06 01:21:36.000000 charidotella-1.1.0/charidotella.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-06 01:21:36.000000 charidotella-1.1.0/charidotella.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-06 01:21:36.000000 charidotella-1.1.0/charidotella.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:21:36.478579 charidotella-1.1.0/command_line_tools/
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-05-06 01:20:31.000000 charidotella-1.1.0/command_line_tools/premake4.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:21:36.486579 charidotella-1.1.0/command_line_tools/source/
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-05-06 01:20:31.000000 charidotella-1.1.0/command_line_tools/source/crop.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-06 01:20:31.000000 charidotella-1.1.0/command_line_tools/source/cut.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-05-06 01:20:31.000000 charidotella-1.1.0/command_line_tools/source/dat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-06 01:20:31.000000 charidotella-1.1.0/command_line_tools/source/dat_to_es.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-06 01:20:31.000000 charidotella-1.1.0/command_line_tools/source/es_to_csv.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    49088 2023-05-06 01:20:31.000000 charidotella-1.1.0/command_line_tools/source/es_to_frames.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-05-06 01:20:31.000000 charidotella-1.1.0/command_line_tools/source/es_to_ply.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26684 2023-05-06 01:20:31.000000 charidotella-1.1.0/command_line_tools/source/event_rate.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-05-06 01:20:31.000000 charidotella-1.1.0/command_line_tools/source/evt3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-06 01:20:31.000000 charidotella-1.1.0/command_line_tools/source/evt3_to_es.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-06 01:20:31.000000 charidotella-1.1.0/command_line_tools/source/font.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    22250 2023-05-06 01:20:31.000000 charidotella-1.1.0/command_line_tools/source/html.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-05-06 01:20:31.000000 charidotella-1.1.0/command_line_tools/source/rainbow.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21823 2023-05-06 01:20:31.000000 charidotella-1.1.0/command_line_tools/source/rainmaker.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-06 01:20:31.000000 charidotella-1.1.0/command_line_tools/source/size.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    31302 2023-05-06 01:20:31.000000 charidotella-1.1.0/command_line_tools/source/spatiospectrogram.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26665 2023-05-06 01:20:31.000000 charidotella-1.1.0/command_line_tools/source/spectrogram.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-05-06 01:20:31.000000 charidotella-1.1.0/command_line_tools/source/statistics.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    18045 2023-05-06 01:20:31.000000 charidotella-1.1.0/command_line_tools/source/synth.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-06 01:20:31.000000 charidotella-1.1.0/command_line_tools/source/timecode.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:21:36.486579 charidotella-1.1.0/command_line_tools/third_party/
--rw-r--r--   0 runner    (1001) docker     (123)   730079 2023-05-06 01:20:31.000000 charidotella-1.1.0/command_line_tools/third_party/monaco.ttf.base64.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:21:36.462579 charidotella-1.1.0/command_line_tools/third_party/pontella/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:21:36.486579 charidotella-1.1.0/command_line_tools/third_party/pontella/source/
--rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-05-06 01:20:33.000000 charidotella-1.1.0/command_line_tools/third_party/pontella/source/pontella.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:21:36.462579 charidotella-1.1.0/command_line_tools/third_party/sepia/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:21:36.486579 charidotella-1.1.0/command_line_tools/third_party/sepia/source/
--rw-r--r--   0 runner    (1001) docker     (123)   104459 2023-05-06 01:20:34.000000 charidotella-1.1.0/command_line_tools/third_party/sepia/source/sepia.hpp
--rw-r--r--   0 runner    (1001) docker     (123)   213770 2023-05-06 01:20:31.000000 charidotella-1.1.0/command_line_tools/third_party/stb_truetype.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:21:36.462579 charidotella-1.1.0/command_line_tools/third_party/tarsier/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:21:36.490579 charidotella-1.1.0/command_line_tools/third_party/tarsier/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-06 01:20:37.000000 charidotella-1.1.0/command_line_tools/third_party/tarsier/source/replicate.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-06 01:20:37.000000 charidotella-1.1.0/command_line_tools/third_party/tarsier/source/stitch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    27056 2023-05-06 01:20:30.000000 charidotella-1.1.0/configuration-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-06 01:20:30.000000 charidotella-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 01:21:36.490579 charidotella-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-05-06 01:20:30.000000 charidotella-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.009798 charidotella-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-28 11:10:06.000000 charidotella-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-05-28 11:10:07.009798 charidotella-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-28 11:09:03.000000 charidotella-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.001798 charidotella-1.2.0/charidotella/
+-rw-r--r--   0 runner    (1001) docker     (123)    45110 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/animals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.005798 charidotella-1.2.0/charidotella/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    24928 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/assets/configuration-schema.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1035600 2023-05-28 11:09:36.000000 charidotella-1.2.0/charidotella/assets/es_to_frames
+-rwxr-xr-x   0 runner    (1001) docker     (123)   286032 2023-05-28 11:09:44.000000 charidotella-1.2.0/charidotella/assets/event_rate
+-rwxr-xr-x   0 runner    (1001) docker     (123)    63800 2023-05-28 11:09:46.000000 charidotella-1.2.0/charidotella/assets/size
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1011024 2023-05-28 11:09:55.000000 charidotella-1.2.0/charidotella/assets/spatiospectrogram
+-rwxr-xr-x   0 runner    (1001) docker     (123)   396632 2023-05-28 11:10:06.000000 charidotella-1.2.0/charidotella/assets/spectrogram
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/charidotella_extension_placeholder.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.005798 charidotella-1.2.0/charidotella/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/filters/arbiter_saturation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/filters/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/filters/hot_pixels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/filters/refractory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/filters/transpose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.005798 charidotella-1.2.0/charidotella/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/tasks/colourtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/tasks/event_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/tasks/spatiospectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/tasks/spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/tasks/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/tasks/wiggle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.001798 charidotella-1.2.0/charidotella.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-05-28 11:10:06.000000 charidotella-1.2.0/charidotella.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-28 11:10:06.000000 charidotella-1.2.0/charidotella.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 11:10:06.000000 charidotella-1.2.0/charidotella.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-28 11:10:06.000000 charidotella-1.2.0/charidotella.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-28 11:10:06.000000 charidotella-1.2.0/charidotella.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-28 11:10:06.000000 charidotella-1.2.0/charidotella.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.005798 charidotella-1.2.0/command_line_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/premake4.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.009798 charidotella-1.2.0/command_line_tools/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/crop.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/cut.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/dat.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/dat_to_es.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/es_to_csv.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    49088 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/es_to_frames.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/es_to_ply.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26684 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/event_rate.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/evt3.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/evt3_to_es.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/font.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22250 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/html.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/rainbow.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21823 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/rainmaker.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/size.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    31302 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/spatiospectrogram.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26665 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/spectrogram.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/statistics.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18045 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/synth.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/timecode.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.009798 charidotella-1.2.0/command_line_tools/third_party/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.009798 charidotella-1.2.0/command_line_tools/third_party/lodepng/
+-rw-r--r--   0 runner    (1001) docker     (123)   260001 2023-05-28 11:09:05.000000 charidotella-1.2.0/command_line_tools/third_party/lodepng/lodepng.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    93636 2023-05-28 11:09:05.000000 charidotella-1.2.0/command_line_tools/third_party/lodepng/lodepng.h
+-rw-r--r--   0 runner    (1001) docker     (123)   730079 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/third_party/monaco.ttf.base64.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:06.997798 charidotella-1.2.0/command_line_tools/third_party/pontella/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.009798 charidotella-1.2.0/command_line_tools/third_party/pontella/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-05-28 11:09:05.000000 charidotella-1.2.0/command_line_tools/third_party/pontella/source/pontella.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.001798 charidotella-1.2.0/command_line_tools/third_party/sepia/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.009798 charidotella-1.2.0/command_line_tools/third_party/sepia/source/
+-rw-r--r--   0 runner    (1001) docker     (123)   104459 2023-05-28 11:09:07.000000 charidotella-1.2.0/command_line_tools/third_party/sepia/source/sepia.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)   213770 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/third_party/stb_truetype.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.001798 charidotella-1.2.0/command_line_tools/third_party/tarsier/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.009798 charidotella-1.2.0/command_line_tools/third_party/tarsier/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-28 11:09:09.000000 charidotella-1.2.0/command_line_tools/third_party/tarsier/source/replicate.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-28 11:09:09.000000 charidotella-1.2.0/command_line_tools/third_party/tarsier/source/stitch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24928 2023-05-28 11:09:03.000000 charidotella-1.2.0/configuration-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-28 11:09:03.000000 charidotella-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 11:10:07.009798 charidotella-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-28 11:09:03.000000 charidotella-1.2.0/setup.py
```

### Comparing `charidotella-1.1.0/MANIFEST.in` & `charidotella-1.2.0/MANIFEST.in`

 * *Files 19% similar despite different names*

```diff
@@ -3,8 +3,10 @@
 include command_line_tools/premake4.lua
 include command_line_tools/third_party/pontella/source/pontella.hpp
 include command_line_tools/third_party/sepia/source/sepia.hpp
 include command_line_tools/third_party/tarsier/source/replicate.hpp
 include command_line_tools/third_party/tarsier/source/stitch.hpp
 include command_line_tools/third_party/stb_truetype.hpp
 include command_line_tools/third_party/monaco.ttf.base64.hpp
+include command_line_tools/third_party/lodepng/lodepng.h
+include command_line_tools/third_party/lodepng/lodepng.cpp
 include configuration-schema.json
```

### Comparing `charidotella-1.1.0/PKG-INFO` & `charidotella-1.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: charidotella
-Version: 1.1.0
-Summary: Charidotella is a toolbox to organise and visualise Event Stream (.es) recordings
-Home-page: https://github.com/neuromorphicsystems/charidotella
-Author: Alexandre Marcireau
-Author-email: alexandre.marcireau@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-
 ![banner](banner.png)
 
 Charidotella (https://en.wikipedia.org/wiki/Charidotella_sexpunctata) is a toolbox to organise and visualise Event Stream (.es) recordings.
 
 It supports Python 3.9, 3.10, and 3.11.
 
 - [Dependencies](#dependencies)
@@ -43,46 +31,72 @@
         winget install python3 --scope machine
         winget install ffmpeg --scope machine
         ```
     2. Reboot the machine
 
 ## Get started
 
-1. Install the Python package
-
-    -   **Debian / Ubuntu**
-        ```sh
-        sudo python3 -m pip install charidotella
-        ```
-
-    -   **macOS**
-        ```sh
-        python3 -m pip install charidotella
-        ```
-
-    -   **Windows**
+1.  Install the Python package (system-wide or in a virtual environment)
 
-        Run in an elevated Powershell (right-click > Run as Administrator)
-        ```powershell
-        & 'C:\Program Files\Python311\python.exe' -m pip install charidotella
-        ```
+    a. System-wide installation
 
+        -   **Debian / Ubuntu**
+            ```sh
+            sudo python3 -m pip install charidotella
+            ```
+
+        -   **macOS**
+            ```sh
+            python3 -m pip install charidotella
+            ```
+
+        -   **Windows**
+
+            Run in an elevated Powershell (right-click > Run as Administrator)
+            ```powershell
+            & 'C:\Program Files\Python311\python.exe' -m pip install charidotella
+            ```
+
+    b. Installation in a virtual environment
+
+        -   **Debian / Ubuntu**
+            ```sh
+            python3 -m venv charidotella_venv
+            source charidotella_venv/bin/activate
+            pip install charidotella
+            ```
+
+        -   **macOS**
+            ```sh
+            python3 -m venv charidotella_venv
+            source charidotella_venv/bin/activate
+            pip install charidotella
+            ```
+
+        -   **Windows**
+
+            Run in an elevated Powershell (right-click > Run as Administrator)
+            ```powershell
+            & 'C:\Program Files\Python311\python.exe' -m venv charidotella_venv
+            charidotella_venv\Scripts\Activate.ps1
+            pip install charidotella
+            ```
 
-2. Create a directory _my-wonderful-project_ with the following structure (the file names do not matter as long as their extension is _.es_)
+2.  Create a directory _my-wonderful-project_ with the following structure (the file names do not matter as long as their extension is _.es_)
 
     ```txt
     my-wonderful-project
     └── recordings
         ├── file_1.es
         ├── file_2.es
         ├── ...
         └── file_n.es
     ```
 
-3. Generate a configuration file
+3.  Generate a configuration file
 
     ```sh
     cd my-wonderful-project
     charidotella init 'recordings/*.es'
     ```
 
     The directory now has the following structure
@@ -93,17 +107,17 @@
     │   ├── file_1.es
     │   ├── file_2.es
     │   ├── ...
     │   └── file_n.es
     └── charidotella-configuration.toml
     ```
 
-4. (Optional) Edit `charidotella-configuration.toml` to change the jobs' parameters
+4.  (Optional) Edit `charidotella-configuration.toml` to change the jobs' parameters
 
-5. Run the jobs
+5.  Run the jobs
 
     ```
     charidotella run
     ```
 
     The directory now has the following structure
 
@@ -122,15 +136,15 @@
     │   │    └── rendered-file-m.es
     │   ├── adjective-animal-2
     │   ├── ...
     │   └── adjective-animal-n
     └── charidotella-configuration.toml
     ```
 
-6. (Optional) Edit `charidotella-configuration.toml` and run `charidotella run` again (job that have already been completed will be skipped unless `--force` is used)
+6.  (Optional) Edit `charidotella-configuration.toml` and run `charidotella run` again (job that have already been completed will be skipped unless `--force` is used)
 
 See `charidotella --help` for a list of other options.
 
 ## Contribute
 
 After code edits, run the formatters and linters.
```

### Comparing `charidotella-1.1.0/README.md` & `charidotella-1.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: charidotella
+Version: 1.2.0
+Summary: Charidotella is a toolbox to organise and visualise Event Stream (.es) recordings
+Home-page: https://github.com/neuromorphicsystems/charidotella
+Author: Alexandre Marcireau
+Author-email: alexandre.marcireau@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+
 ![banner](banner.png)
 
 Charidotella (https://en.wikipedia.org/wiki/Charidotella_sexpunctata) is a toolbox to organise and visualise Event Stream (.es) recordings.
 
 It supports Python 3.9, 3.10, and 3.11.
 
 - [Dependencies](#dependencies)
@@ -31,46 +43,72 @@
         winget install python3 --scope machine
         winget install ffmpeg --scope machine
         ```
     2. Reboot the machine
 
 ## Get started
 
-1. Install the Python package
-
-    -   **Debian / Ubuntu**
-        ```sh
-        sudo python3 -m pip install charidotella
-        ```
-
-    -   **macOS**
-        ```sh
-        python3 -m pip install charidotella
-        ```
-
-    -   **Windows**
+1.  Install the Python package (system-wide or in a virtual environment)
 
-        Run in an elevated Powershell (right-click > Run as Administrator)
-        ```powershell
-        & 'C:\Program Files\Python311\python.exe' -m pip install charidotella
-        ```
+    a. System-wide installation
 
+        -   **Debian / Ubuntu**
+            ```sh
+            sudo python3 -m pip install charidotella
+            ```
+
+        -   **macOS**
+            ```sh
+            python3 -m pip install charidotella
+            ```
+
+        -   **Windows**
+
+            Run in an elevated Powershell (right-click > Run as Administrator)
+            ```powershell
+            & 'C:\Program Files\Python311\python.exe' -m pip install charidotella
+            ```
+
+    b. Installation in a virtual environment
+
+        -   **Debian / Ubuntu**
+            ```sh
+            python3 -m venv charidotella_venv
+            source charidotella_venv/bin/activate
+            pip install charidotella
+            ```
+
+        -   **macOS**
+            ```sh
+            python3 -m venv charidotella_venv
+            source charidotella_venv/bin/activate
+            pip install charidotella
+            ```
+
+        -   **Windows**
+
+            Run in an elevated Powershell (right-click > Run as Administrator)
+            ```powershell
+            & 'C:\Program Files\Python311\python.exe' -m venv charidotella_venv
+            charidotella_venv\Scripts\Activate.ps1
+            pip install charidotella
+            ```
 
-2. Create a directory _my-wonderful-project_ with the following structure (the file names do not matter as long as their extension is _.es_)
+2.  Create a directory _my-wonderful-project_ with the following structure (the file names do not matter as long as their extension is _.es_)
 
     ```txt
     my-wonderful-project
     └── recordings
         ├── file_1.es
         ├── file_2.es
         ├── ...
         └── file_n.es
     ```
 
-3. Generate a configuration file
+3.  Generate a configuration file
 
     ```sh
     cd my-wonderful-project
     charidotella init 'recordings/*.es'
     ```
 
     The directory now has the following structure
@@ -81,17 +119,17 @@
     │   ├── file_1.es
     │   ├── file_2.es
     │   ├── ...
     │   └── file_n.es
     └── charidotella-configuration.toml
     ```
 
-4. (Optional) Edit `charidotella-configuration.toml` to change the jobs' parameters
+4.  (Optional) Edit `charidotella-configuration.toml` to change the jobs' parameters
 
-5. Run the jobs
+5.  Run the jobs
 
     ```
     charidotella run
     ```
 
     The directory now has the following structure
 
@@ -110,15 +148,15 @@
     │   │    └── rendered-file-m.es
     │   ├── adjective-animal-2
     │   ├── ...
     │   └── adjective-animal-n
     └── charidotella-configuration.toml
     ```
 
-6. (Optional) Edit `charidotella-configuration.toml` and run `charidotella run` again (job that have already been completed will be skipped unless `--force` is used)
+6.  (Optional) Edit `charidotella-configuration.toml` and run `charidotella run` again (job that have already been completed will be skipped unless `--force` is used)
 
 See `charidotella --help` for a list of other options.
 
 ## Contribute
 
 After code edits, run the formatters and linters.
```

### Comparing `charidotella-1.1.0/charidotella/__init__.py` & `charidotella-1.2.0/charidotella/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     None,
 ]
 
 FILTERS: dict[str, filter_apply] = {
     "default": filters.default.apply,
     "arbiter_saturation": filters.arbiter_saturation.apply,
     "hot_pixels": filters.hot_pixels.apply,
+    "refractory": filters.refractory.apply,
     "transpose": filters.transpose.apply,
 }
 
 task_run = typing.Callable[
     [
         pathlib.Path,
         pathlib.Path,
@@ -199,15 +200,16 @@
     @functools.lru_cache(maxsize=None)
     def configuration_schema():
         with open(
             str(
                 importlib.resources.files("charidotella").joinpath(
                     "assets/configuration-schema.json"
                 )
-            )
+            ),
+            "r",
         ) as configuration_schema_file:
             return json.load(configuration_schema_file)
 
     def load_parameters(path: pathlib.Path):
         if path.is_file():
             with open(path, "r", encoding="utf-8") as file:
                 return toml.load(file)
@@ -408,15 +410,15 @@
             toml.dump({"directory": "renders"}, configuration_file, encoder=Encoder())
             configuration_file.write(
                 "\n\n# filters configuration (filters are applied before tasks)\n\n"
             )
             toml.dump(
                 {
                     "filters": {
-                        "default": {"type": "default", "icon": "⏳", "suffix": ""},
+                        "default": {"type": "default", "icon": "🔆", "suffix": ""},
                     }
                 },
                 configuration_file,
                 encoder=Encoder(),
             )
             configuration_file.write(
                 "\n\n# filters generators (advanced filter generation with templates)\n"
@@ -447,14 +449,32 @@
                                 "suffix": "hp@ratio",
                                 "ratio": "@raw(ratio)",
                             },
                         },
                         {
                             "parameters": {
                                 "suffix": [
+                                    10**exponent for exponent in (0, 1, 2, 3, 4, 5, 6)
+                                ],
+                                "refractory": [
+                                    utilities.timestamp_to_timecode(10**exponent)
+                                    for exponent in (0, 1, 2, 3, 4, 5, 6)
+                                ],
+                            },
+                            "template": {
+                                "name": "refractory-@suffix",
+                                "type": "refractory",
+                                "icon": "⏳",
+                                "suffix": "rf@suffix",
+                                "refractory": "@refractory",
+                            },
+                        },
+                        {
+                            "parameters": {
+                                "suffix": [
                                     "flip-left-right",
                                     "flip-top-bottom",
                                     "rotate-90",
                                     "rotate-180",
                                     "rotate-270",
                                     "transpose",
                                     "transverse",
```

### Comparing `charidotella-1.1.0/charidotella/animals.py` & `charidotella-1.2.0/charidotella/animals.py`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/charidotella/assets/configuration-schema.json` & `charidotella-1.2.0/charidotella/assets/configuration-schema.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999826388888889%*

 * *Differences: {"'properties'": "{'filters': {'additionalProperties': {'anyOf': {insert: [(3, "*

 * *                 "OrderedDict([('additionalProperties', False), ('properties', "*

 * *                 "OrderedDict([('icon', OrderedDict([('type', 'string')])), ('refractory', "*

 * *                 "OrderedDict([('type', ['string', 'number'])])), ('suffix', OrderedDict([('type', "*

 * *                 "'string')])), ('type', OrderedDict([('enum', ['refractory']), ('type', "*

 * *                 "'string')]))])), ('required', ['type', 'icon',  […]*

```diff
@@ -100,14 +100,44 @@
                             "icon",
                             "suffix",
                             "ratio"
                         ],
                         "type": "object"
                     },
                     {
+                        "additionalProperties": false,
+                        "properties": {
+                            "icon": {
+                                "type": "string"
+                            },
+                            "refractory": {
+                                "type": [
+                                    "string",
+                                    "number"
+                                ]
+                            },
+                            "suffix": {
+                                "type": "string"
+                            },
+                            "type": {
+                                "enum": [
+                                    "refractory"
+                                ],
+                                "type": "string"
+                            }
+                        },
+                        "required": [
+                            "type",
+                            "icon",
+                            "suffix",
+                            "refractory"
+                        ],
+                        "type": "object"
+                    },
+                    {
                         "properties": {
                             "icon": {
                                 "type": "string"
                             },
                             "method": {
                                 "enum": [
                                     "flip_left_right",
```

### Comparing `charidotella-1.1.0/charidotella/assets/es_to_frames` & `charidotella-1.2.0/charidotella/assets/es_to_frames`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/charidotella/assets/event_rate` & `charidotella-1.2.0/charidotella/assets/event_rate`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/charidotella/assets/size` & `charidotella-1.2.0/charidotella/assets/size`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/charidotella/assets/spatiospectrogram` & `charidotella-1.2.0/charidotella/assets/spatiospectrogram`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/charidotella/assets/spectrogram` & `charidotella-1.2.0/charidotella/assets/spectrogram`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/charidotella/charidotella_extension_placeholder.c` & `charidotella-1.2.0/charidotella/charidotella_extension_placeholder.c`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/charidotella/filters/arbiter_saturation.py` & `charidotella-1.2.0/charidotella/filters/arbiter_saturation.py`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/charidotella/filters/default.py` & `charidotella-1.2.0/charidotella/filters/default.py`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/charidotella/filters/hot_pixels.py` & `charidotella-1.2.0/charidotella/filters/hot_pixels.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,46 +27,46 @@
             elif begin is not None and packet["t"][0] < begin:
                 events = packet[packet["t"] >= begin]
             elif end is not None and packet["t"][-1] >= end:
                 events = packet[packet["t"] < end]
             else:
                 events = packet
             numpy.add.at(count, (events["x"], events["y"]), 1)
-        shifted: list[numpy.ndarray] = []
-        for x, y in ((1, 0), (0, 1), (1, 2), (2, 1)):
-            kernel = numpy.zeros((3, 3))
-            kernel[x, y] = 1.0
-            shifted.append(
-                scipy.ndimage.convolve(
-                    input=count,
-                    weights=kernel,
-                    mode="constant",
-                    cval=0.0,
-                )
+    shifted: list[numpy.ndarray] = []
+    for x, y in ((1, 0), (0, 1), (1, 2), (2, 1)):
+        kernel = numpy.zeros((3, 3))
+        kernel[x, y] = 1.0
+        shifted.append(
+            scipy.ndimage.convolve(
+                input=count,
+                weights=kernel,
+                mode="constant",
+                cval=0.0,
             )
-        ratios = numpy.divide(count, numpy.maximum.reduce(shifted) + 1.0)
-        mask = ratios < parameters["ratio"]
-        with event_stream.Decoder(input) as decoder:
-            with event_stream.Encoder(
-                output,
-                "dvs",
-                decoder.width,
-                decoder.height,
-            ) as encoder:
-                for packet in decoder:
-                    if packet["t"][-1] < begin:
-                        continue
-                    if packet["t"][0] >= end:
-                        break
-                    if packet["t"][0] < begin and packet["t"][-1] >= end:
-                        events = packet[
-                            numpy.logical_and(packet["t"] >= begin, packet["t"] < end)
-                        ]
-                    elif begin is not None and packet["t"][0] < begin:
-                        events = packet[packet["t"] >= begin]
-                    elif end is not None and packet["t"][-1] >= end:
-                        events = packet[packet["t"] < end]
-                    else:
-                        events = packet
-                    events = events[mask[events["x"], events["y"]]]
-                    if len(events) > 0:
-                        encoder.write(events)
+        )
+    ratios = numpy.divide(count, numpy.maximum.reduce(shifted) + 1.0)
+    mask = ratios < parameters["ratio"]
+    with event_stream.Decoder(input) as decoder:
+        with event_stream.Encoder(
+            output,
+            "dvs",
+            decoder.width,
+            decoder.height,
+        ) as encoder:
+            for packet in decoder:
+                if packet["t"][-1] < begin:
+                    continue
+                if packet["t"][0] >= end:
+                    break
+                if packet["t"][0] < begin and packet["t"][-1] >= end:
+                    events = packet[
+                        numpy.logical_and(packet["t"] >= begin, packet["t"] < end)
+                    ]
+                elif begin is not None and packet["t"][0] < begin:
+                    events = packet[packet["t"] >= begin]
+                elif end is not None and packet["t"][-1] >= end:
+                    events = packet[packet["t"] < end]
+                else:
+                    events = packet
+                events = events[mask[events["x"], events["y"]]]
+                if len(events) > 0:
+                    encoder.write(events)
```

### Comparing `charidotella-1.1.0/charidotella/filters/transpose.py` & `charidotella-1.2.0/charidotella/filters/transpose.py`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/charidotella/tasks/colourtime.py` & `charidotella-1.2.0/charidotella/tasks/colourtime.py`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/charidotella/tasks/event_rate.py` & `charidotella-1.2.0/charidotella/tasks/event_rate.py`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/charidotella/tasks/spatiospectrogram.py` & `charidotella-1.2.0/charidotella/tasks/spatiospectrogram.py`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/charidotella/tasks/spectrogram.py` & `charidotella-1.2.0/charidotella/tasks/spectrogram.py`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/charidotella/tasks/video.py` & `charidotella-1.2.0/charidotella/tasks/video.py`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/charidotella/tasks/wiggle.py` & `charidotella-1.2.0/charidotella/tasks/wiggle.py`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/charidotella/utilities.py` & `charidotella-1.2.0/charidotella/utilities.py`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/charidotella.egg-info/PKG-INFO` & `charidotella-1.2.0/charidotella.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charidotella
-Version: 1.1.0
+Version: 1.2.0
 Summary: Charidotella is a toolbox to organise and visualise Event Stream (.es) recordings
 Home-page: https://github.com/neuromorphicsystems/charidotella
 Author: Alexandre Marcireau
 Author-email: alexandre.marcireau@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -43,46 +43,72 @@
         winget install python3 --scope machine
         winget install ffmpeg --scope machine
         ```
     2. Reboot the machine
 
 ## Get started
 
-1. Install the Python package
+1.  Install the Python package (system-wide or in a virtual environment)
 
-    -   **Debian / Ubuntu**
-        ```sh
-        sudo python3 -m pip install charidotella
-        ```
-
-    -   **macOS**
-        ```sh
-        python3 -m pip install charidotella
-        ```
-
-    -   **Windows**
-
-        Run in an elevated Powershell (right-click > Run as Administrator)
-        ```powershell
-        & 'C:\Program Files\Python311\python.exe' -m pip install charidotella
-        ```
+    a. System-wide installation
 
+        -   **Debian / Ubuntu**
+            ```sh
+            sudo python3 -m pip install charidotella
+            ```
+
+        -   **macOS**
+            ```sh
+            python3 -m pip install charidotella
+            ```
+
+        -   **Windows**
+
+            Run in an elevated Powershell (right-click > Run as Administrator)
+            ```powershell
+            & 'C:\Program Files\Python311\python.exe' -m pip install charidotella
+            ```
+
+    b. Installation in a virtual environment
+
+        -   **Debian / Ubuntu**
+            ```sh
+            python3 -m venv charidotella_venv
+            source charidotella_venv/bin/activate
+            pip install charidotella
+            ```
+
+        -   **macOS**
+            ```sh
+            python3 -m venv charidotella_venv
+            source charidotella_venv/bin/activate
+            pip install charidotella
+            ```
+
+        -   **Windows**
+
+            Run in an elevated Powershell (right-click > Run as Administrator)
+            ```powershell
+            & 'C:\Program Files\Python311\python.exe' -m venv charidotella_venv
+            charidotella_venv\Scripts\Activate.ps1
+            pip install charidotella
+            ```
 
-2. Create a directory _my-wonderful-project_ with the following structure (the file names do not matter as long as their extension is _.es_)
+2.  Create a directory _my-wonderful-project_ with the following structure (the file names do not matter as long as their extension is _.es_)
 
     ```txt
     my-wonderful-project
     └── recordings
         ├── file_1.es
         ├── file_2.es
         ├── ...
         └── file_n.es
     ```
 
-3. Generate a configuration file
+3.  Generate a configuration file
 
     ```sh
     cd my-wonderful-project
     charidotella init 'recordings/*.es'
     ```
 
     The directory now has the following structure
@@ -93,17 +119,17 @@
     │   ├── file_1.es
     │   ├── file_2.es
     │   ├── ...
     │   └── file_n.es
     └── charidotella-configuration.toml
     ```
 
-4. (Optional) Edit `charidotella-configuration.toml` to change the jobs' parameters
+4.  (Optional) Edit `charidotella-configuration.toml` to change the jobs' parameters
 
-5. Run the jobs
+5.  Run the jobs
 
     ```
     charidotella run
     ```
 
     The directory now has the following structure
 
@@ -122,15 +148,15 @@
     │   │    └── rendered-file-m.es
     │   ├── adjective-animal-2
     │   ├── ...
     │   └── adjective-animal-n
     └── charidotella-configuration.toml
     ```
 
-6. (Optional) Edit `charidotella-configuration.toml` and run `charidotella run` again (job that have already been completed will be skipped unless `--force` is used)
+6.  (Optional) Edit `charidotella-configuration.toml` and run `charidotella run` again (job that have already been completed will be skipped unless `--force` is used)
 
 See `charidotella --help` for a list of other options.
 
 ## Contribute
 
 After code edits, run the formatters and linters.
```

### Comparing `charidotella-1.1.0/charidotella.egg-info/SOURCES.txt` & `charidotella-1.2.0/charidotella.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 charidotella/assets/size
 charidotella/assets/spatiospectrogram
 charidotella/assets/spectrogram
 charidotella/filters/__init__.py
 charidotella/filters/arbiter_saturation.py
 charidotella/filters/default.py
 charidotella/filters/hot_pixels.py
+charidotella/filters/refractory.py
 charidotella/filters/transpose.py
 charidotella/tasks/__init__.py
 charidotella/tasks/colourtime.py
 charidotella/tasks/event_rate.py
 charidotella/tasks/spatiospectrogram.py
 charidotella/tasks/spectrogram.py
 charidotella/tasks/video.py
@@ -51,11 +52,13 @@
 command_line_tools/source/spatiospectrogram.cpp
 command_line_tools/source/spectrogram.cpp
 command_line_tools/source/statistics.cpp
 command_line_tools/source/synth.cpp
 command_line_tools/source/timecode.hpp
 command_line_tools/third_party/monaco.ttf.base64.hpp
 command_line_tools/third_party/stb_truetype.hpp
+command_line_tools/third_party/lodepng/lodepng.cpp
+command_line_tools/third_party/lodepng/lodepng.h
 command_line_tools/third_party/pontella/source/pontella.hpp
 command_line_tools/third_party/sepia/source/sepia.hpp
 command_line_tools/third_party/tarsier/source/replicate.hpp
 command_line_tools/third_party/tarsier/source/stitch.hpp
```

### Comparing `charidotella-1.1.0/command_line_tools/premake4.lua` & `charidotella-1.2.0/command_line_tools/premake4.lua`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/command_line_tools/source/crop.cpp` & `charidotella-1.2.0/command_line_tools/source/crop.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/command_line_tools/source/cut.cpp` & `charidotella-1.2.0/command_line_tools/source/cut.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/command_line_tools/source/dat.hpp` & `charidotella-1.2.0/command_line_tools/source/dat.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/command_line_tools/source/dat_to_es.cpp` & `charidotella-1.2.0/command_line_tools/source/dat_to_es.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/command_line_tools/source/es_to_csv.cpp` & `charidotella-1.2.0/command_line_tools/source/es_to_csv.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/command_line_tools/source/es_to_frames.cpp` & `charidotella-1.2.0/command_line_tools/source/es_to_frames.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/command_line_tools/source/es_to_ply.cpp` & `charidotella-1.2.0/command_line_tools/source/es_to_ply.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/command_line_tools/source/event_rate.cpp` & `charidotella-1.2.0/command_line_tools/source/event_rate.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/command_line_tools/source/evt3.hpp` & `charidotella-1.2.0/command_line_tools/source/evt3.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/command_line_tools/source/evt3_to_es.cpp` & `charidotella-1.2.0/command_line_tools/source/evt3_to_es.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/command_line_tools/source/font.hpp` & `charidotella-1.2.0/command_line_tools/source/font.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/command_line_tools/source/html.hpp` & `charidotella-1.2.0/command_line_tools/source/html.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/command_line_tools/source/rainbow.cpp` & `charidotella-1.2.0/command_line_tools/source/rainbow.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/command_line_tools/source/rainmaker.cpp` & `charidotella-1.2.0/command_line_tools/source/rainmaker.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/command_line_tools/source/size.cpp` & `charidotella-1.2.0/command_line_tools/source/size.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/command_line_tools/source/spatiospectrogram.cpp` & `charidotella-1.2.0/command_line_tools/source/spatiospectrogram.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/command_line_tools/source/spectrogram.cpp` & `charidotella-1.2.0/command_line_tools/source/spectrogram.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/command_line_tools/source/statistics.cpp` & `charidotella-1.2.0/command_line_tools/source/statistics.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/command_line_tools/source/synth.cpp` & `charidotella-1.2.0/command_line_tools/source/synth.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/command_line_tools/source/timecode.hpp` & `charidotella-1.2.0/command_line_tools/source/timecode.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/command_line_tools/third_party/monaco.ttf.base64.hpp` & `charidotella-1.2.0/command_line_tools/third_party/monaco.ttf.base64.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/command_line_tools/third_party/pontella/source/pontella.hpp` & `charidotella-1.2.0/command_line_tools/third_party/pontella/source/pontella.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/command_line_tools/third_party/sepia/source/sepia.hpp` & `charidotella-1.2.0/command_line_tools/third_party/sepia/source/sepia.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/command_line_tools/third_party/stb_truetype.hpp` & `charidotella-1.2.0/command_line_tools/third_party/stb_truetype.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/command_line_tools/third_party/tarsier/source/replicate.hpp` & `charidotella-1.2.0/command_line_tools/third_party/tarsier/source/replicate.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/command_line_tools/third_party/tarsier/source/stitch.hpp` & `charidotella-1.2.0/command_line_tools/third_party/tarsier/source/stitch.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.1.0/configuration-schema.json` & `charidotella-1.2.0/configuration-schema.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999826388888889%*

 * *Differences: {"'properties'": "{'filters': {'additionalProperties': {'anyOf': {insert: [(3, "*

 * *                 "OrderedDict([('additionalProperties', False), ('properties', "*

 * *                 "OrderedDict([('icon', OrderedDict([('type', 'string')])), ('refractory', "*

 * *                 "OrderedDict([('type', ['string', 'number'])])), ('suffix', OrderedDict([('type', "*

 * *                 "'string')])), ('type', OrderedDict([('enum', ['refractory']), ('type', "*

 * *                 "'string')]))])), ('required', ['type', 'icon',  […]*

```diff
@@ -100,14 +100,44 @@
                             "icon",
                             "suffix",
                             "ratio"
                         ],
                         "type": "object"
                     },
                     {
+                        "additionalProperties": false,
+                        "properties": {
+                            "icon": {
+                                "type": "string"
+                            },
+                            "refractory": {
+                                "type": [
+                                    "string",
+                                    "number"
+                                ]
+                            },
+                            "suffix": {
+                                "type": "string"
+                            },
+                            "type": {
+                                "enum": [
+                                    "refractory"
+                                ],
+                                "type": "string"
+                            }
+                        },
+                        "required": [
+                            "type",
+                            "icon",
+                            "suffix",
+                            "refractory"
+                        ],
+                        "type": "object"
+                    },
+                    {
                         "properties": {
                             "icon": {
                                 "type": "string"
                             },
                             "method": {
                                 "enum": [
                                     "flip_left_right",
```

### Comparing `charidotella-1.1.0/setup.py` & `charidotella-1.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,16 @@
         "include command_line_tools/premake4.lua",
         "include command_line_tools/third_party/pontella/source/pontella.hpp",
         "include command_line_tools/third_party/sepia/source/sepia.hpp",
         "include command_line_tools/third_party/tarsier/source/replicate.hpp",
         "include command_line_tools/third_party/tarsier/source/stitch.hpp",
         "include command_line_tools/third_party/stb_truetype.hpp",
         "include command_line_tools/third_party/monaco.ttf.base64.hpp",
+        "include command_line_tools/third_party/lodepng/lodepng.h",
+        "include command_line_tools/third_party/lodepng/lodepng.cpp",
     ]
     if "sdist" in sys.argv:
         manifest_lines.append(f"include configuration-schema.json")
     else:
         shutil.rmtree(dirname / "charidotella" / "assets", ignore_errors=True)
         (dirname / "charidotella" / "assets").mkdir()
         if sys.platform == "win32":
```

