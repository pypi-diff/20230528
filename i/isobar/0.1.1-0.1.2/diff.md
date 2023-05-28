# Comparing `tmp/isobar-0.1.1.tar.gz` & `tmp/isobar-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/isobar-0.1.1.tar", last modified: Wed Oct  7 15:41:01 2020, max compression
+gzip compressed data, was "isobar-0.1.2.tar", last modified: Sun May 28 19:32:23 2023, max compression
```

## Comparing `isobar-0.1.1.tar` & `isobar-0.1.2.tar`

### file list

```diff
@@ -1,87 +1,100 @@
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2020-10-07 15:41:01.000000 isobar-0.1.1/
--rw-r--r--   0 daniel     (501) staff       (20)    13641 2020-10-07 15:41:01.000000 isobar-0.1.1/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)    11547 2020-10-07 14:03:58.000000 isobar-0.1.1/README.md
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2020-10-07 15:41:01.000000 isobar-0.1.1/isobar/
--rw-r--r--   0 daniel     (501) staff       (20)      563 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)     1619 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/chord.py
--rw-r--r--   0 daniel     (501) staff       (20)     3957 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/constants.py
--rw-r--r--   0 daniel     (501) staff       (20)      982 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/exceptions.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2020-10-07 15:41:01.000000 isobar-0.1.1/isobar/io/
--rw-r--r--   0 daniel     (501) staff       (20)      891 2020-10-07 13:48:12.000000 isobar-0.1.1/isobar/io/__init__.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2020-10-07 15:41:01.000000 isobar-0.1.1/isobar/io/dummy/
--rw-r--r--   0 daniel     (501) staff       (20)       70 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/io/dummy/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)      895 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/io/dummy/output.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2020-10-07 15:41:01.000000 isobar-0.1.1/isobar/io/midi/
--rw-r--r--   0 daniel     (501) staff       (20)      641 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/io/midi/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)     4757 2020-10-07 13:48:54.000000 isobar-0.1.1/isobar/io/midi/input.py
--rw-r--r--   0 daniel     (501) staff       (20)     3650 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/io/midi/output.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2020-10-07 15:41:01.000000 isobar-0.1.1/isobar/io/midifile/
--rw-r--r--   0 daniel     (501) staff       (20)      178 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/io/midifile/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)     5760 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/io/midifile/input.py
--rw-r--r--   0 daniel     (501) staff       (20)     3332 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/io/midifile/output.py
--rw-r--r--   0 daniel     (501) staff       (20)      339 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/io/midinote.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2020-10-07 15:41:01.000000 isobar-0.1.1/isobar/io/osc/
--rw-r--r--   0 daniel     (501) staff       (20)       66 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/io/osc/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)     1179 2020-10-07 13:49:01.000000 isobar-0.1.1/isobar/io/osc/output.py
--rw-r--r--   0 daniel     (501) staff       (20)      703 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/io/output.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2020-10-07 15:41:01.000000 isobar-0.1.1/isobar/io/signalflow/
--rw-r--r--   0 daniel     (501) staff       (20)       81 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/io/signalflow/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)     1387 2020-10-07 13:49:54.000000 isobar-0.1.1/isobar/io/signalflow/output.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2020-10-07 15:41:01.000000 isobar-0.1.1/isobar/io/socketio/
--rw-r--r--   0 daniel     (501) staff       (20)       76 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/io/socketio/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)     1017 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/io/socketio/output.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2020-10-07 15:41:01.000000 isobar-0.1.1/isobar/io/supercollider/
--rw-r--r--   0 daniel     (501) staff       (20)       86 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/io/supercollider/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)     1381 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/io/supercollider/output.py
--rw-r--r--   0 daniel     (501) staff       (20)     4475 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/key.py
--rw-r--r--   0 daniel     (501) staff       (20)      514 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/note.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2020-10-07 15:41:01.000000 isobar-0.1.1/isobar/pattern/
--rw-r--r--   0 daniel     (501) staff       (20)      545 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/pattern/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)    12651 2020-10-07 13:50:37.000000 isobar-0.1.1/isobar/pattern/chance.py
--rw-r--r--   0 daniel     (501) staff       (20)    20233 2020-10-07 13:50:05.000000 isobar-0.1.1/isobar/pattern/core.py
--rw-r--r--   0 daniel     (501) staff       (20)     4972 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/pattern/fade.py
--rw-r--r--   0 daniel     (501) staff       (20)     1992 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/pattern/lsystem.py
--rw-r--r--   0 daniel     (501) staff       (20)     7186 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/pattern/markov.py
--rw-r--r--   0 daniel     (501) staff       (20)      783 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/pattern/oscillator.py
--rw-r--r--   0 daniel     (501) staff       (20)     8647 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/pattern/scalar.py
--rw-r--r--   0 daniel     (501) staff       (20)    30103 2020-10-07 13:50:20.000000 isobar-0.1.1/isobar/pattern/sequence.py
--rw-r--r--   0 daniel     (501) staff       (20)     2547 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/pattern/static.py
--rw-r--r--   0 daniel     (501) staff       (20)     2304 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/pattern/tonal.py
--rw-r--r--   0 daniel     (501) staff       (20)     3512 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/pattern/warp.py
--rw-r--r--   0 daniel     (501) staff       (20)     5696 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/scale.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2020-10-07 15:41:01.000000 isobar-0.1.1/isobar/timeline/
--rw-r--r--   0 daniel     (501) staff       (20)      149 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/timeline/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)     4517 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/timeline/clock.py
--rw-r--r--   0 daniel     (501) staff       (20)     6978 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/timeline/event.py
--rw-r--r--   0 daniel     (501) staff       (20)    15693 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/timeline/timeline.py
--rw-r--r--   0 daniel     (501) staff       (20)    16194 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/timeline/track.py
--rw-r--r--   0 daniel     (501) staff       (20)     3697 2020-10-07 13:23:04.000000 isobar-0.1.1/isobar/util.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2020-10-07 15:41:01.000000 isobar-0.1.1/isobar.egg-info/
--rw-r--r--   0 daniel     (501) staff       (20)    13641 2020-10-07 15:41:01.000000 isobar-0.1.1/isobar.egg-info/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)     1832 2020-10-07 15:41:01.000000 isobar-0.1.1/isobar.egg-info/SOURCES.txt
--rw-r--r--   0 daniel     (501) staff       (20)        1 2020-10-07 15:41:01.000000 isobar-0.1.1/isobar.egg-info/dependency_links.txt
--rw-r--r--   0 daniel     (501) staff       (20)       30 2020-10-07 15:41:01.000000 isobar-0.1.1/isobar.egg-info/requires.txt
--rw-r--r--   0 daniel     (501) staff       (20)       13 2020-10-07 15:41:01.000000 isobar-0.1.1/isobar.egg-info/top_level.txt
--rw-r--r--   0 daniel     (501) staff       (20)       98 2020-10-07 15:41:01.000000 isobar-0.1.1/setup.cfg
--rw-r--r--   0 daniel     (501) staff       (20)      836 2020-10-07 15:38:42.000000 isobar-0.1.1/setup.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2020-10-07 15:41:01.000000 isobar-0.1.1/tests/
--rw-r--r--   0 daniel     (501) staff       (20)      231 2020-10-07 13:23:04.000000 isobar-0.1.1/tests/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)     1571 2020-10-07 13:23:04.000000 isobar-0.1.1/tests/test_io_midi.py
--rw-r--r--   0 daniel     (501) staff       (20)     1450 2020-10-07 13:23:04.000000 isobar-0.1.1/tests/test_io_midifile.py
--rw-r--r--   0 daniel     (501) staff       (20)     2236 2020-10-07 13:23:04.000000 isobar-0.1.1/tests/test_key.py
--rw-r--r--   0 daniel     (501) staff       (20)     2380 2020-10-07 13:23:04.000000 isobar-0.1.1/tests/test_pattern.py
--rw-r--r--   0 daniel     (501) staff       (20)     4251 2020-10-07 13:23:04.000000 isobar-0.1.1/tests/test_pattern_chance.py
--rw-r--r--   0 daniel     (501) staff       (20)     2166 2020-10-07 13:23:04.000000 isobar-0.1.1/tests/test_pattern_core.py
--rw-r--r--   0 daniel     (501) staff       (20)      241 2020-10-07 13:23:04.000000 isobar-0.1.1/tests/test_pattern_lsystem.py
--rw-r--r--   0 daniel     (501) staff       (20)      325 2020-10-07 13:23:04.000000 isobar-0.1.1/tests/test_pattern_markov.py
--rw-r--r--   0 daniel     (501) staff       (20)     3126 2020-10-07 13:23:04.000000 isobar-0.1.1/tests/test_pattern_operators.py
--rw-r--r--   0 daniel     (501) staff       (20)     2465 2020-10-07 13:23:04.000000 isobar-0.1.1/tests/test_pattern_scalar.py
--rw-r--r--   0 daniel     (501) staff       (20)     5541 2020-10-07 13:23:04.000000 isobar-0.1.1/tests/test_pattern_sequence.py
--rw-r--r--   0 daniel     (501) staff       (20)      672 2020-10-07 13:23:04.000000 isobar-0.1.1/tests/test_pattern_static.py
--rw-r--r--   0 daniel     (501) staff       (20)      838 2020-10-07 13:23:04.000000 isobar-0.1.1/tests/test_pattern_tonal.py
--rw-r--r--   0 daniel     (501) staff       (20)    11237 2020-10-07 13:23:04.000000 isobar-0.1.1/tests/test_timeline.py
--rw-r--r--   0 daniel     (501) staff       (20)     2053 2020-10-07 13:23:04.000000 isobar-0.1.1/tests/test_timeline_clock.py
--rw-r--r--   0 daniel     (501) staff       (20)     7723 2020-10-07 13:23:04.000000 isobar-0.1.1/tests/test_timeline_event.py
--rw-r--r--   0 daniel     (501) staff       (20)     3092 2020-10-07 13:23:04.000000 isobar-0.1.1/tests/test_timeline_event_control.py
--rw-r--r--   0 daniel     (501) staff       (20)      891 2020-10-07 13:23:04.000000 isobar-0.1.1/tests/test_timeline_event_supercollider.py
--rw-r--r--   0 daniel     (501) staff       (20)      365 2020-10-07 13:23:04.000000 isobar-0.1.1/tests/test_timeline_track.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-28 19:32:23.892121 isobar-0.1.2/
+-rw-r--r--   0 daniel     (501) staff       (20)     1081 2020-10-07 13:32:20.000000 isobar-0.1.2/LICENSE.md
+-rw-r--r--   0 daniel     (501) staff       (20)    12846 2023-05-28 19:32:23.892193 isobar-0.1.2/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)    12314 2022-12-22 09:17:15.000000 isobar-0.1.2/README.md
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-28 19:32:23.877923 isobar-0.1.2/isobar/
+-rw-r--r--   0 daniel     (501) staff       (20)      563 2020-10-07 13:23:04.000000 isobar-0.1.2/isobar/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1619 2020-10-07 13:23:04.000000 isobar-0.1.2/isobar/chord.py
+-rw-r--r--   0 daniel     (501) staff       (20)     4792 2022-12-21 11:04:26.000000 isobar-0.1.2/isobar/constants.py
+-rw-r--r--   0 daniel     (501) staff       (20)      982 2020-10-07 13:23:04.000000 isobar-0.1.2/isobar/exceptions.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-28 19:32:23.879112 isobar-0.1.2/isobar/io/
+-rw-r--r--   0 daniel     (501) staff       (20)     1000 2021-02-19 11:54:20.000000 isobar-0.1.2/isobar/io/__init__.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-28 19:32:23.879694 isobar-0.1.2/isobar/io/cv/
+-rw-r--r--   0 daniel     (501) staff       (20)      113 2020-10-12 16:16:40.000000 isobar-0.1.2/isobar/io/cv/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2818 2020-10-12 16:43:57.000000 isobar-0.1.2/isobar/io/cv/output.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-28 19:32:23.880126 isobar-0.1.2/isobar/io/dummy/
+-rw-r--r--   0 daniel     (501) staff       (20)       70 2020-10-07 13:23:04.000000 isobar-0.1.2/isobar/io/dummy/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)      895 2020-10-07 13:23:04.000000 isobar-0.1.2/isobar/io/dummy/output.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-28 19:32:23.880679 isobar-0.1.2/isobar/io/midi/
+-rw-r--r--   0 daniel     (501) staff       (20)      738 2020-10-08 10:49:55.000000 isobar-0.1.2/isobar/io/midi/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     4757 2020-10-07 13:48:54.000000 isobar-0.1.2/isobar/io/midi/input.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3761 2022-03-27 15:42:50.000000 isobar-0.1.2/isobar/io/midi/output.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-28 19:32:23.881201 isobar-0.1.2/isobar/io/midifile/
+-rw-r--r--   0 daniel     (501) staff       (20)      261 2020-10-08 10:48:38.000000 isobar-0.1.2/isobar/io/midifile/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     5760 2020-10-07 13:23:04.000000 isobar-0.1.2/isobar/io/midifile/input.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3896 2022-01-27 23:02:46.000000 isobar-0.1.2/isobar/io/midifile/output.py
+-rw-r--r--   0 daniel     (501) staff       (20)      339 2020-10-07 13:23:04.000000 isobar-0.1.2/isobar/io/midinote.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-28 19:32:23.881889 isobar-0.1.2/isobar/io/netclock/
+-rw-r--r--   0 daniel     (501) staff       (20)       81 2022-05-20 17:33:26.000000 isobar-0.1.2/isobar/io/netclock/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1702 2022-05-22 14:35:17.000000 isobar-0.1.2/isobar/io/netclock/receiver.py
+-rw-r--r--   0 daniel     (501) staff       (20)      994 2022-05-22 14:35:04.000000 isobar-0.1.2/isobar/io/netclock/sender.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-28 19:32:23.882491 isobar-0.1.2/isobar/io/netglobals/
+-rw-r--r--   0 daniel     (501) staff       (20)       85 2022-05-31 07:49:24.000000 isobar-0.1.2/isobar/io/netglobals/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1358 2022-06-01 21:23:31.000000 isobar-0.1.2/isobar/io/netglobals/receiver.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1226 2022-06-01 21:24:41.000000 isobar-0.1.2/isobar/io/netglobals/sender.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-28 19:32:23.882873 isobar-0.1.2/isobar/io/osc/
+-rw-r--r--   0 daniel     (501) staff       (20)       66 2020-10-07 13:23:04.000000 isobar-0.1.2/isobar/io/osc/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1179 2020-10-07 13:49:01.000000 isobar-0.1.2/isobar/io/osc/output.py
+-rw-r--r--   0 daniel     (501) staff       (20)      703 2020-10-07 13:23:04.000000 isobar-0.1.2/isobar/io/output.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-28 19:32:23.883196 isobar-0.1.2/isobar/io/signalflow/
+-rw-r--r--   0 daniel     (501) staff       (20)       81 2020-10-07 16:56:31.000000 isobar-0.1.2/isobar/io/signalflow/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2116 2022-12-21 11:08:28.000000 isobar-0.1.2/isobar/io/signalflow/output.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-28 19:32:23.883731 isobar-0.1.2/isobar/io/socketio/
+-rw-r--r--   0 daniel     (501) staff       (20)       76 2020-10-07 13:23:04.000000 isobar-0.1.2/isobar/io/socketio/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1017 2020-10-07 13:23:04.000000 isobar-0.1.2/isobar/io/socketio/output.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-28 19:32:23.884141 isobar-0.1.2/isobar/io/supercollider/
+-rw-r--r--   0 daniel     (501) staff       (20)       86 2020-10-07 13:23:04.000000 isobar-0.1.2/isobar/io/supercollider/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1381 2020-10-07 13:23:04.000000 isobar-0.1.2/isobar/io/supercollider/output.py
+-rw-r--r--   0 daniel     (501) staff       (20)     4601 2022-03-28 21:18:58.000000 isobar-0.1.2/isobar/key.py
+-rw-r--r--   0 daniel     (501) staff       (20)      514 2020-10-07 13:23:04.000000 isobar-0.1.2/isobar/note.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-28 19:32:23.887039 isobar-0.1.2/isobar/pattern/
+-rw-r--r--   0 daniel     (501) staff       (20)      545 2020-10-07 13:23:04.000000 isobar-0.1.2/isobar/pattern/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)    17678 2022-03-27 14:25:17.000000 isobar-0.1.2/isobar/pattern/chance.py
+-rw-r--r--   0 daniel     (501) staff       (20)    20262 2022-05-31 23:29:53.000000 isobar-0.1.2/isobar/pattern/core.py
+-rw-r--r--   0 daniel     (501) staff       (20)     4972 2020-10-07 13:23:04.000000 isobar-0.1.2/isobar/pattern/fade.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1992 2020-10-07 13:23:04.000000 isobar-0.1.2/isobar/pattern/lsystem.py
+-rw-r--r--   0 daniel     (501) staff       (20)     7186 2020-10-07 13:23:04.000000 isobar-0.1.2/isobar/pattern/markov.py
+-rw-r--r--   0 daniel     (501) staff       (20)      959 2022-03-26 09:32:33.000000 isobar-0.1.2/isobar/pattern/oscillator.py
+-rw-r--r--   0 daniel     (501) staff       (20)     8497 2023-02-19 17:51:41.000000 isobar-0.1.2/isobar/pattern/scalar.py
+-rw-r--r--   0 daniel     (501) staff       (20)    31770 2022-03-26 09:48:41.000000 isobar-0.1.2/isobar/pattern/sequence.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3587 2023-03-10 19:51:51.000000 isobar-0.1.2/isobar/pattern/static.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2304 2020-10-07 13:23:04.000000 isobar-0.1.2/isobar/pattern/tonal.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3512 2020-10-07 13:23:04.000000 isobar-0.1.2/isobar/pattern/warp.py
+-rw-r--r--   0 daniel     (501) staff       (20)     5823 2022-04-01 11:33:33.000000 isobar-0.1.2/isobar/scale.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-28 19:32:23.888342 isobar-0.1.2/isobar/timeline/
+-rw-r--r--   0 daniel     (501) staff       (20)      149 2020-10-07 13:23:04.000000 isobar-0.1.2/isobar/timeline/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     4582 2022-03-28 21:35:24.000000 isobar-0.1.2/isobar/timeline/clock.py
+-rw-r--r--   0 daniel     (501) staff       (20)     4652 2022-03-21 21:32:29.000000 isobar-0.1.2/isobar/timeline/clock.warp.py
+-rw-r--r--   0 daniel     (501) staff       (20)     8893 2022-12-21 11:01:54.000000 isobar-0.1.2/isobar/timeline/event.py
+-rw-r--r--   0 daniel     (501) staff       (20)    18856 2022-05-20 10:40:02.000000 isobar-0.1.2/isobar/timeline/timeline.py
+-rw-r--r--   0 daniel     (501) staff       (20)    20387 2022-12-22 09:14:56.000000 isobar-0.1.2/isobar/timeline/track.py
+-rw-r--r--   0 daniel     (501) staff       (20)     4909 2022-05-20 18:20:09.000000 isobar-0.1.2/isobar/util.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-28 19:32:23.878594 isobar-0.1.2/isobar.egg-info/
+-rw-r--r--   0 daniel     (501) staff       (20)    12846 2023-05-28 19:32:23.000000 isobar-0.1.2/isobar.egg-info/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)     2109 2023-05-28 19:32:23.000000 isobar-0.1.2/isobar.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2023-05-28 19:32:23.000000 isobar-0.1.2/isobar.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       30 2023-05-28 19:32:23.000000 isobar-0.1.2/isobar.egg-info/requires.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       13 2023-05-28 19:32:23.000000 isobar-0.1.2/isobar.egg-info/top_level.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       98 2023-05-28 19:32:23.892470 isobar-0.1.2/setup.cfg
+-rw-r--r--   0 daniel     (501) staff       (20)      836 2023-05-28 19:26:06.000000 isobar-0.1.2/setup.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-28 19:32:23.891986 isobar-0.1.2/tests/
+-rw-r--r--   0 daniel     (501) staff       (20)      231 2020-10-07 13:23:04.000000 isobar-0.1.2/tests/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1571 2020-10-07 13:23:04.000000 isobar-0.1.2/tests/test_io_midi.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1450 2020-10-07 13:23:04.000000 isobar-0.1.2/tests/test_io_midifile.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2071 2021-02-19 22:05:49.000000 isobar-0.1.2/tests/test_key.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2380 2020-10-07 13:23:04.000000 isobar-0.1.2/tests/test_pattern.py
+-rw-r--r--   0 daniel     (501) staff       (20)     4472 2020-11-03 12:28:49.000000 isobar-0.1.2/tests/test_pattern_chance.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2166 2022-03-28 21:31:38.000000 isobar-0.1.2/tests/test_pattern_core.py
+-rw-r--r--   0 daniel     (501) staff       (20)      241 2020-10-07 13:23:04.000000 isobar-0.1.2/tests/test_pattern_lsystem.py
+-rw-r--r--   0 daniel     (501) staff       (20)      325 2020-10-07 13:23:04.000000 isobar-0.1.2/tests/test_pattern_markov.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3126 2020-10-07 13:23:04.000000 isobar-0.1.2/tests/test_pattern_operators.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2465 2020-10-07 13:23:04.000000 isobar-0.1.2/tests/test_pattern_scalar.py
+-rw-r--r--   0 daniel     (501) staff       (20)     5571 2022-03-26 09:47:58.000000 isobar-0.1.2/tests/test_pattern_sequence.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1516 2020-10-08 10:22:32.000000 isobar-0.1.2/tests/test_pattern_static.py
+-rw-r--r--   0 daniel     (501) staff       (20)      838 2020-10-07 13:23:04.000000 isobar-0.1.2/tests/test_pattern_tonal.py
+-rw-r--r--   0 daniel     (501) staff       (20)    12525 2022-03-20 16:25:08.000000 isobar-0.1.2/tests/test_timeline.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2053 2020-10-07 13:23:04.000000 isobar-0.1.2/tests/test_timeline_clock.py
+-rw-r--r--   0 daniel     (501) staff       (20)     7159 2021-02-19 21:15:32.000000 isobar-0.1.2/tests/test_timeline_event.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3092 2020-10-07 13:23:04.000000 isobar-0.1.2/tests/test_timeline_event_control.py
+-rw-r--r--   0 daniel     (501) staff       (20)      891 2020-10-07 13:23:04.000000 isobar-0.1.2/tests/test_timeline_event_supercollider.py
+-rw-r--r--   0 daniel     (501) staff       (20)      365 2020-10-07 13:23:04.000000 isobar-0.1.2/tests/test_timeline_track.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `isobar-0.1.1/PKG-INFO` & `isobar-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,213 +1,200 @@
-Metadata-Version: 2.1
-Name: isobar
-Version: 0.1.1
-Summary: A Python library to express and manipulate musical patterns
-Home-page: https://github.com/ideoforms/isobar
-Author: Daniel Jones
-Author-email: dan-isobar@erase.net
-License: UNKNOWN
-Description: # isobar
-        
-        ![ci](https://github.com/ideoforms/isobar/workflows/ci/badge.svg)
-        
-        isobar is a Python library for creating and manipulating musical patterns, designed for use in algorithmic composition, generative music and sonification. It makes it quick and easy to express complex musical ideas, and can send and receive events from various different sources including MIDI, MIDI files, and OSC.
-        
-        The core element is a Timeline, which can control its own tempo or sync to an external clock. Onto this, you can schedule Patterns, which can be note sequences, control events, program changes, or other arbitrary events via lambda functions. Pattern are used as templates to generate Events, which trigger notes or control changes on an OutputDevice (Check out a [diagrammatic overview](http://ideoforms.github.io/isobar/#flow-diagram).)
-        
-        isobar includes a large array of basic compositional building blocks (see [Pattern Classes](#pattern-classes)), plus some advanced pattern generators for more sophisticated operations (arpeggiators, Euclidean rhythms, L-systems, Markov chains).
-        
-        ## Usage
-        
-        ```python
-        import isobar as iso
-        
-        #------------------------------------------------------------------------
-        # Create a geometric series on a minor scale.
-        # PingPong plays the series forward then backward. PLoop loops forever.
-        #------------------------------------------------------------------------
-        arpeggio = iso.PSeries(0, 2, 6)
-        arpeggio = iso.PDegree(arpeggio, iso.Scale.minor) + 72
-        arpeggio = iso.PPingPong(arpeggio)
-        arpeggio = iso.PLoop(arpeggio)
-        
-        #------------------------------------------------------------------------
-        # Create a velocity sequence, with emphasis every 4th note,
-        # plus a random walk to create gradual dynamic changes.
-        # Amplitudes are in the MIDI velocity range (0..127).
-        #------------------------------------------------------------------------
-        amplitude = iso.PSequence([50, 35, 25, 35]) + iso.PBrown(0, 1, -20, 20)
-        
-        #------------------------------------------------------------------------
-        # A Timeline schedules events at a specified tempo. By default, events
-        # are send to the system's default MIDI output.
-        #------------------------------------------------------------------------
-        timeline = iso.Timeline(120)
-        
-        #------------------------------------------------------------------------
-        # Schedule events, with properties generated by the Pattern objects.
-        #------------------------------------------------------------------------
-        timeline.schedule({
-            "note": arpeggio,
-            "duration": 0.25,
-            "amplitude": amplitude
-        })
-        
-        #------------------------------------------------------------------------
-        # Run the timeline.
-        # Call timeline.background() to run in a separate thread.
-        #------------------------------------------------------------------------
-        timeline.run()
-        ```
-        
-        ## Installation
-        
-        The short answer: `pip3 install isobar`
-        
-        The long answer: [isobar Getting Started guide](http://ideoforms.github.io/isobar/getting-started/)
-        
-        ## Documentation
-        
-        For complete documentation, see [ideoforms.github.io/isobar](http://ideoforms.github.io/isobar/).
-        
-        ## Examples
-        
-        Examples are available in the [examples](examples) directory with this
-        distribution:
-        
-        * [00.ex-hello-world.py](examples/00.ex-hello-world.py)
-        * [01.ex-basics.py](examples/01.ex-basics.py)
-        * [02.ex-subsequence.py](examples/02.ex-subsequence.py)
-        * [03.ex-euclidean.py](examples/03.ex-euclidean.py)
-        * [04.ex-permutations.py](examples/04.ex-permutations.py)
-        * [05.ex-piano-phase.py](examples/05.ex-piano-phase.py)
-        * [06.ex-walk.py](examples/06.ex-walk.py)
-        * [07.ex-static-pattern.py](examples/07.ex-static-pattern.py)
-        * [10.ex-lsystem-stochastic.py](examples/10.ex-lsystem-stochastic.py)
-        * [11.ex-lsystem-rhythm.py](examples/11.ex-lsystem-rhythm.py)
-        * [12.ex-lsystem-grapher.py](examples/12.ex-lsystem-grapher.py)
-        * [20.ex-midi-input.py](examples/20.ex-midi-input.py)
-        * [21.ex-midi-clock-sync-in.py](examples/21.ex-midi-clock-sync-in.py)
-        * [22.ex-midi-markov-learner.py](examples/22.ex-midi-markov-learner.py)
-        * [23.ex-midi-monitor.py](examples/23.ex-midi-monitor.py)
-        * [30.ex-midifile-read.py](examples/30.ex-midifile-read.py)
-        * [31.ex-midifile-write.py](examples/31.ex-midifile-write.py)
-        * [32.ex-midifile-markov.py](examples/32.ex-midifile-markov.py)
-        * [40.ex-osc-send.py](examples/40.ex-osc-send.py)
-        
-        ### Pattern classes
-        
-            CORE (core.py)
-            Pattern              - Abstract superclass of all pattern generators.
-            PConstant            - Returns a fixed value.
-            PRef                 - Contains a reference to another pattern, which can be replaced dynamically.
-            PFunc                - Returns the value generated by a function.
-            PArrayIndex          - Request a specified index from an array.
-            PDict                - Construct a pattern from a dict of arrays, or an array of dicts.
-            PDictKey             - Request a specified key from a dictionary.
-            PConcatenate         - Concatenate the output of multiple sequences.
-            PAbs                 - Absolute value of `input`
-            PInt                 - Integer value of `input`
-            PAdd                 - Add elements of two patterns (shorthand: patternA + patternB)
-            PSub                 - Subtract elements of two patterns (shorthand: patternA - patternB)
-            PMul                 - Multiply elements of two patterns (shorthand: patternA * patternB)
-            PDiv                 - Divide elements of two patterns (shorthand: patternA / patternB)
-            PFloorDiv            - Integer division (shorthand: patternA // patternB)
-            PMod                 - Modulo elements of two patterns (shorthand: patternA % patternB)
-            PPow                 - One pattern to the power of another (shorthand: patternA ** patternB)
-            PLShift              - Binary left-shift (shorthand: patternA << patternB)
-            PRShift              - Binary right-shift (shorthand: patternA << patternB)
-            PEqual               - Return 1 if a == b, 0 otherwise (shorthand: patternA == patternB)
-            PGreaterThanOrEqual  - Return 1 if a != b, 0 otherwise (shorthand: patternA != patternB)
-            PGreaterThan         - Return 1 if a > b, 0 otherwise (shorthand: patternA > patternB)
-            PGreaterThanOrEqual  - Return 1 if a >= b, 0 otherwise (shorthand: patternA >= patternB)
-            PLessThan            - Return 1 if a < b, 0 otherwise (shorthand: patternA < patternB)
-            PLessThanOrEqual     - Return 1 if a <= b, 0 otherwise (shorthand: patternA <= patternB)
-        
-            SCALAR (scalar.py)
-            PChanged             - Outputs a 1 if the value of a pattern has changed.
-            PDiff                - Outputs the difference between the current and previous values of an input pattern
-            PSkipIf              - If `skip` is false, returns `input`; otherwise, returns None.
-            PNormalise           - Adaptively normalise `input` to [0..1] over a linear scale.
-            PMap                 - Apply an arbitrary function to an input pattern.
-            PMapEnumerated       - Apply arbitrary function to input, passing a counter.
-            PLinLin              - Map `input` from linear range [a,b] to linear range [c,d].
-            PLinExp              - Map `input` from linear range [a,b] to exponential range [c,d].
-            PRound               - Round `input` to N decimal places.
-            PScalar              - Reduce tuples and lists into single scalar values,
-            PWrap                - Wrap input note values within <min>, <max>.
-            PIndexOf             - Find index of items from `pattern` in <list>
-        
-            SEQUENCE (sequence.py)
-            PSeries              - Arithmetic series, beginning at `start`, increment by `step`
-            PRange               - Similar to PSeries, but specify a max/step value.
-            PGeom                - Geometric series, beginning at `start`, multiplied by `step`
-            PImpulse             - Outputs a 1 every <period> events, otherwise 0.
-            PLoop                - Repeats a finite `pattern` for `n` repeats.
-            PPingPong            - Ping-pong input pattern back and forth N times.
-            PCreep               - Loop `length`-note segment, progressing `creep` notes after `repeats` repeats.
-            PStutter             - Play each note of `pattern` `count` times.
-            PSubsequence         - Returns a finite subsequence of an input pattern.
-            PReverse             - Reverses a finite sequence.
-            PReset               - Resets `pattern` whenever `trigger` is true
-            PCounter             - Increments a counter by 1 for each zero-crossing in `trigger`.
-            PCollapse            - Skip over any rests in `input`
-            PNoRepeats           - Skip over repeated values in `input`
-            PPad                 - Pad `pattern` with rests until it reaches length `length`.
-            PPadToMultiple       - Pad `pattern` with rests until its length is divisible by `multiple`.
-            PArpeggiator         - Arpeggiator.
-            PEuclidean           - Generate Euclidean rhythms.
-            PPermut              - Generate every permutation of `count` input items.
-            PPatternGeneratorAction - Each time its pattern is exhausted, request a new pattern by calling <fn>.
-            PSequenceAction      - Iterate over an array, perform a function, and repeat.
-        
-            CHANCE (chance.py)
-            PWhite               - White noise between `min` and `max`.
-            PBrown               - Brownian noise.
-            PWalk                - Random walk around list.
-            PChoice              - Pick a random element from `values`, weighted by optional `weights`.
-            PSample              - Pick multiple random elements from `values`, weighted by optional `weights`,
-            PShuffle             - Shuffled list.
-            PShuffleInput        - Every `n` steps, take `n` values from `pattern` and reorder.
-            PSkip                - Skip events with some probability, 1 - <play>.
-            PFlipFlop            - flip a binary bit with some probability.
-            PSwitchOne           - Capture `length` input values; loop, repeatedly switching two adjacent values.
-        
-            TONAL (tonal.py)
-            PDegree              - Map scale index <degree> to MIDI notes in <scale>.
-            PFilterByKey         - Filter notes based on their presence in <key>.
-            PNearestNoteInKey    - Return the nearest note in <key>.
-            PMidiNoteToFrequency - Map MIDI note to frequency value.
-        
-            STATIC (static.py)
-            PGlobals             - Static global value identified by a string.
-            PCurrentTime         - Returns the position (in beats) of the current timeline.
-        
-            FADE (fade.py)
-            PFadeNotewise        - Fade a pattern in/out by introducing notes at a gradual rate.
-            PFadeNotewiseRandom  - Fade a pattern in/out by gradually introducing random notes.
-        
-            MARKOV (markov.py)
-            PMarkov              - First-order Markov chain generator.
-        
-            LSYSTEM (lsystem.py)
-            PLSystem             - integer sequence derived from Lindenmayer systems
-        
-            WARP (warp.py)
-            PWInterpolate        - Requests a new target warp value from `pattern` every `length` beats
-            PWSine               - Sinosoidal warp, period `length` beats, amplitude +/-<amp>.
-            PWRallantando        - Exponential deceleration to <amp> times the current tempo over `length` beats.
-        
-        ## Background
-        
-        isobar was first designed for the generative sound installation [Variable 4](http://www.variable4.org.uk), in which it was used to generate musical structures in response to changing weather conditions. It was more recently used in [The Listening Machine](http://www.thelisteningmachine.org/), taking live input from Twitter and generating musical output from language patterns, streamed live over the internet.
-        
-        Many of the concepts behind Pattern and its subclasses are inspired by the brilliant pattern library of the [SuperCollider](http://supercollider.sf.net) synthesis language.
-        
-        
-Keywords: sound,music,composition
-Platform: UNKNOWN
-Classifier: Topic :: Multimedia :: Sound/Audio
-Classifier: Topic :: Artistic Software
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Description-Content-Type: text/markdown
+# isobar
+
+![ci](https://github.com/ideoforms/isobar/workflows/ci/badge.svg) [![stability-mature](https://img.shields.io/badge/stability-mature-008000.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#mature)
+
+isobar is a Python library for creating and manipulating musical patterns, designed for use in algorithmic composition, generative music and sonification. It makes it quick and easy to express complex musical ideas, and can send and receive events from various different sources including MIDI, MIDI files, and OSC.
+
+The core element is a Timeline, which can control its own tempo or sync to an external clock. Onto this, you can schedule Patterns, which can be note sequences, control events, program changes, or other arbitrary events via lambda functions. Pattern are used as templates to generate Events, which trigger notes or control changes on an OutputDevice (Check out a [diagrammatic overview](http://ideoforms.github.io/isobar/#flow-diagram).)
+
+isobar includes a large array of basic compositional building blocks (see [Pattern Classes](#pattern-classes)), plus some advanced pattern generators for more sophisticated operations (arpeggiators, Euclidean rhythms, L-systems, Markov chains).
+
+## Usage
+
+```python
+import isobar as iso
+
+#------------------------------------------------------------------------
+# Create a geometric series on a minor scale.
+# PingPong plays the series forward then backward. PLoop loops forever.
+#------------------------------------------------------------------------
+arpeggio = iso.PSeries(0, 2, 6)
+arpeggio = iso.PDegree(arpeggio, iso.Scale.minor) + 72
+arpeggio = iso.PPingPong(arpeggio)
+arpeggio = iso.PLoop(arpeggio)
+
+#------------------------------------------------------------------------
+# Create a velocity sequence, with emphasis every 4th note,
+# plus a random walk to create gradual dynamic changes.
+# Amplitudes are in the MIDI velocity range (0..127).
+#------------------------------------------------------------------------
+amplitude = iso.PSequence([50, 35, 25, 35]) + iso.PBrown(0, 1, -20, 20)
+
+#------------------------------------------------------------------------
+# A Timeline schedules events at a specified tempo. By default, events
+# are send to the system's default MIDI output.
+#------------------------------------------------------------------------
+timeline = iso.Timeline(120)
+
+#------------------------------------------------------------------------
+# Schedule events, with properties generated by the Pattern objects.
+#------------------------------------------------------------------------
+timeline.schedule({
+    "note": arpeggio,
+    "duration": 0.25,
+    "amplitude": amplitude
+})
+
+#------------------------------------------------------------------------
+# Run the timeline.
+# Call timeline.background() to run in a separate thread.
+#------------------------------------------------------------------------
+timeline.run()
+```
+
+## Installation
+
+The short answer: `pip3 install isobar`
+
+The long answer: [isobar Getting Started guide](http://ideoforms.github.io/isobar/getting-started/)
+
+## Documentation
+
+For complete documentation, see [ideoforms.github.io/isobar](http://ideoforms.github.io/isobar/).
+
+## Examples
+
+Examples are available in the [examples](examples) directory with this
+distribution:
+
+* [00.ex-hello-world.py](examples/00.ex-hello-world.py)
+* [01.ex-basics.py](examples/01.ex-basics.py)
+* [02.ex-subsequence.py](examples/02.ex-subsequence.py)
+* [03.ex-euclidean.py](examples/03.ex-euclidean.py)
+* [04.ex-permutations.py](examples/04.ex-permutations.py)
+* [05.ex-piano-phase.py](examples/05.ex-piano-phase.py)
+* [06.ex-walk.py](examples/06.ex-walk.py)
+* [07.ex-static-pattern.py](examples/07.ex-static-pattern.py)
+* [10.ex-lsystem-stochastic.py](examples/10.ex-lsystem-stochastic.py)
+* [11.ex-lsystem-rhythm.py](examples/11.ex-lsystem-rhythm.py)
+* [12.ex-lsystem-grapher.py](examples/12.ex-lsystem-grapher.py)
+* [20.ex-midi-input.py](examples/20.ex-midi-input.py)
+* [21.ex-midi-clock-sync-in.py](examples/21.ex-midi-clock-sync-in.py)
+* [22.ex-midi-markov-learner.py](examples/22.ex-midi-markov-learner.py)
+* [23.ex-midi-monitor.py](examples/23.ex-midi-monitor.py)
+* [30.ex-midifile-read.py](examples/30.ex-midifile-read.py)
+* [31.ex-midifile-write.py](examples/31.ex-midifile-write.py)
+* [32.ex-midifile-markov.py](examples/32.ex-midifile-markov.py)
+* [40.ex-osc-send.py](examples/40.ex-osc-send.py)
+
+### Pattern classes
+
+    CORE (core.py)
+    Pattern                  - Abstract superclass of all pattern generators.
+    PConstant                - Returns a fixed value.
+    PRef                     - Contains a reference to another pattern, which can be replaced dynamically.
+    PFunc                    - Returns the value generated by a function.
+    PArrayIndex              - Request a specified index from an array.
+    PDict                    - Construct a pattern from a dict of arrays, or an array of dicts.
+    PDictKey                 - Request a specified key from a dictionary.
+    PConcatenate             - Concatenate the output of multiple sequences.
+    PAbs                     - Absolute value of `input`
+    PInt                     - Integer value of `input`
+    PAdd                     - Add elements of two patterns (shorthand: patternA + patternB)
+    PSub                     - Subtract elements of two patterns (shorthand: patternA - patternB)
+    PMul                     - Multiply elements of two patterns (shorthand: patternA * patternB)
+    PDiv                     - Divide elements of two patterns (shorthand: patternA / patternB)
+    PFloorDiv                - Integer division (shorthand: patternA // patternB)
+    PMod                     - Modulo elements of two patterns (shorthand: patternA % patternB)
+    PPow                     - One pattern to the power of another (shorthand: patternA ** patternB)
+    PLShift                  - Binary left-shift (shorthand: patternA << patternB)
+    PRShift                  - Binary right-shift (shorthand: patternA << patternB)
+    PEqual                   - Return 1 if a == b, 0 otherwise (shorthand: patternA == patternB)
+    PGreaterThanOrEqual      - Return 1 if a != b, 0 otherwise (shorthand: patternA != patternB)
+    PGreaterThan             - Return 1 if a > b, 0 otherwise (shorthand: patternA > patternB)
+    PGreaterThanOrEqual      - Return 1 if a >= b, 0 otherwise (shorthand: patternA >= patternB)
+    PLessThan                - Return 1 if a < b, 0 otherwise (shorthand: patternA < patternB)
+    PLessThanOrEqual         - Return 1 if a <= b, 0 otherwise (shorthand: patternA <= patternB)
+
+    SCALAR (scalar.py)
+    PChanged                 - Outputs a 1 if the value of the input pattern has changed,
+    PDiff                    - Outputs the difference between the current and previous values of an input pattern
+    PSkipIf                  - If `skip` is false, returns `input`; otherwise, returns None.
+    PNormalise               - Adaptively normalise `input` to [0..1] over a linear scale.
+    PMap                     - Apply an arbitrary function to an input pattern.
+    PMapEnumerated           - Apply arbitrary function to input, passing a counter.
+    PScaleLinLin             - Map `input` from linear range [a,b] to linear range [c,d].
+    PScaleLinExp             - Map `input` from linear range [a,b] to exponential range [c,d].
+    PRound                   - Round `input` to N decimal places.
+    PScalar                  - Reduce tuples and lists into single scalar values,
+    PWrap                    - Wrap input note values within <min>, <max>.
+    PIndexOf                 - Find index of items from `pattern` in <list>
+
+    SEQUENCE (sequence.py)
+    PSeries                  - Arithmetic series, beginning at `start`, increment by `step`
+    PRange                   - Similar to PSeries, but specify a max/step value.
+    PGeom                    - Geometric series, beginning at `start`, multiplied by `step`
+    PImpulse                 - Outputs a 1 every <period> events, otherwise 0.
+    PLoop                    - Repeats a finite `pattern` for `n` repeats.
+    PPingPong                - Ping-pong input pattern back and forth N times.
+    PCreep                   - Loop `length`-note segment, progressing `creep` notes after `repeats` repeats.
+    PStutter                 - Play each note of `pattern` `count` times.
+    PSubsequence             - Returns a finite subsequence of an input pattern.
+    PReverse                 - Reverses a finite sequence.
+    PReset                   - Resets `pattern` whenever `trigger` is true
+    PCounter                 - Increments a counter by 1 for each zero-crossing in `trigger`.
+    PCollapse                - Skip over any rests in `input`
+    PNoRepeats               - Skip over repeated values in `input`
+    PPad                     - Pad `pattern` with rests until it reaches length `length`.
+    PPadToMultiple           - Pad `pattern` with rests until its length is divisible by `multiple`.
+    PArpeggiator             - Arpeggiator.
+    PEuclidean               - Generate Euclidean rhythms.
+    PPermut                  - Generate every permutation of `count` input items.
+    PPatternGeneratorAction  - Each time its pattern is exhausted, request a new pattern by calling <fn>.
+    PSequenceAction          - Iterate over an array, perform a function, and repeat.
+
+    CHANCE (chance.py)
+    PWhite                   - White noise between `min` and `max`.
+    PBrown                   - Brownian noise.
+    PCoin                    - Coin toss, returning either 0 or 1 given some `probability`.
+    PWalk                    - Random walk around list.
+    PChoice                  - Pick a random element from `values`, weighted by optional `weights`.
+    PSample                  - Pick multiple random elements from `values`, weighted by optional `weights`,
+    PShuffle                 - Shuffled list.
+    PShuffleInput            - Every `n` steps, take `n` values from `pattern` and reorder.
+    PSkip                    - Skip events with some probability, 1 - `play`.
+    PFlipFlop                - flip a binary bit with some probability.
+    PSwitchOne               - Capture `length` input values; loop, repeatedly switching two adjacent values.
+    PRandomExponential       - Random uniform on exponential curve between `min` and `max`,
+    PRandomImpulseSequence   - Random sequence of impulses with probability `probability`.
+
+    TONAL (tonal.py)
+    PDegree                  - Map scale index <degree> to MIDI notes in <scale>.
+    PFilterByKey             - Filter notes based on their presence in <key>.
+    PNearestNoteInKey        - Return the nearest note in <key>.
+    PMidiNoteToFrequency     - Map MIDI note to frequency value.
+
+    STATIC (static.py)
+    PGlobals                 - Static global value identified by a string.
+    PCurrentTime             - Returns the position (in beats) of the current timeline.
+
+    FADE (fade.py)
+    PFadeNotewise            - Fade a pattern in/out by introducing notes at a gradual rate.
+    PFadeNotewiseRandom      - Fade a pattern in/out by gradually introducing random notes.
+
+    MARKOV (markov.py)
+    PMarkov                  - First-order Markov chain generator.
+
+    LSYSTEM (lsystem.py)
+    PLSystem                 - integer sequence derived from Lindenmayer systems
+
+    WARP (warp.py)
+    PWInterpolate            - Requests a new target warp value from `pattern` every `length` beats
+    PWSine                   - Sinosoidal warp, period `length` beats, amplitude +/-<amp>.
+    PWRallantando            - Exponential deceleration to <amp> times the current tempo over `length` beats.
+
+## Background
+
+isobar was first designed for the generative sound installation [Variable 4](http://www.variable4.org.uk), in which it was used to generate musical structures in response to changing weather conditions. It was more recently used in [The Listening Machine](http://www.thelisteningmachine.org/), taking live input from Twitter and generating musical output from language patterns, streamed live over the internet.
+
+Many of the concepts behind Pattern and its subclasses are inspired by the brilliant pattern library of the [SuperCollider](http://supercollider.sf.net) synthesis language.
+
```

### Comparing `isobar-0.1.1/README.md` & `isobar-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,27 @@
+Metadata-Version: 2.1
+Name: isobar
+Version: 0.1.2
+Summary: A Python library to express and manipulate musical patterns
+Home-page: https://github.com/ideoforms/isobar
+Author: Daniel Jones
+Author-email: dan-isobar@erase.net
+License: UNKNOWN
+Keywords: sound,music,composition
+Platform: UNKNOWN
+Classifier: Topic :: Multimedia :: Sound/Audio
+Classifier: Topic :: Artistic Software
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 # isobar
 
-![ci](https://github.com/ideoforms/isobar/workflows/ci/badge.svg)
+![ci](https://github.com/ideoforms/isobar/workflows/ci/badge.svg) [![stability-mature](https://img.shields.io/badge/stability-mature-008000.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#mature)
 
 isobar is a Python library for creating and manipulating musical patterns, designed for use in algorithmic composition, generative music and sonification. It makes it quick and easy to express complex musical ideas, and can send and receive events from various different sources including MIDI, MIDI files, and OSC.
 
 The core element is a Timeline, which can control its own tempo or sync to an external clock. Onto this, you can schedule Patterns, which can be note sequences, control events, program changes, or other arbitrary events via lambda functions. Pattern are used as templates to generate Events, which trigger notes or control changes on an OutputDevice (Check out a [diagrammatic overview](http://ideoforms.github.io/isobar/#flow-diagram).)
 
 isobar includes a large array of basic compositional building blocks (see [Pattern Classes](#pattern-classes)), plus some advanced pattern generators for more sophisticated operations (arpeggiators, Euclidean rhythms, L-systems, Markov chains).
 
@@ -85,113 +102,118 @@
 * [31.ex-midifile-write.py](examples/31.ex-midifile-write.py)
 * [32.ex-midifile-markov.py](examples/32.ex-midifile-markov.py)
 * [40.ex-osc-send.py](examples/40.ex-osc-send.py)
 
 ### Pattern classes
 
     CORE (core.py)
-    Pattern              - Abstract superclass of all pattern generators.
-    PConstant            - Returns a fixed value.
-    PRef                 - Contains a reference to another pattern, which can be replaced dynamically.
-    PFunc                - Returns the value generated by a function.
-    PArrayIndex          - Request a specified index from an array.
-    PDict                - Construct a pattern from a dict of arrays, or an array of dicts.
-    PDictKey             - Request a specified key from a dictionary.
-    PConcatenate         - Concatenate the output of multiple sequences.
-    PAbs                 - Absolute value of `input`
-    PInt                 - Integer value of `input`
-    PAdd                 - Add elements of two patterns (shorthand: patternA + patternB)
-    PSub                 - Subtract elements of two patterns (shorthand: patternA - patternB)
-    PMul                 - Multiply elements of two patterns (shorthand: patternA * patternB)
-    PDiv                 - Divide elements of two patterns (shorthand: patternA / patternB)
-    PFloorDiv            - Integer division (shorthand: patternA // patternB)
-    PMod                 - Modulo elements of two patterns (shorthand: patternA % patternB)
-    PPow                 - One pattern to the power of another (shorthand: patternA ** patternB)
-    PLShift              - Binary left-shift (shorthand: patternA << patternB)
-    PRShift              - Binary right-shift (shorthand: patternA << patternB)
-    PEqual               - Return 1 if a == b, 0 otherwise (shorthand: patternA == patternB)
-    PGreaterThanOrEqual  - Return 1 if a != b, 0 otherwise (shorthand: patternA != patternB)
-    PGreaterThan         - Return 1 if a > b, 0 otherwise (shorthand: patternA > patternB)
-    PGreaterThanOrEqual  - Return 1 if a >= b, 0 otherwise (shorthand: patternA >= patternB)
-    PLessThan            - Return 1 if a < b, 0 otherwise (shorthand: patternA < patternB)
-    PLessThanOrEqual     - Return 1 if a <= b, 0 otherwise (shorthand: patternA <= patternB)
+    Pattern                  - Abstract superclass of all pattern generators.
+    PConstant                - Returns a fixed value.
+    PRef                     - Contains a reference to another pattern, which can be replaced dynamically.
+    PFunc                    - Returns the value generated by a function.
+    PArrayIndex              - Request a specified index from an array.
+    PDict                    - Construct a pattern from a dict of arrays, or an array of dicts.
+    PDictKey                 - Request a specified key from a dictionary.
+    PConcatenate             - Concatenate the output of multiple sequences.
+    PAbs                     - Absolute value of `input`
+    PInt                     - Integer value of `input`
+    PAdd                     - Add elements of two patterns (shorthand: patternA + patternB)
+    PSub                     - Subtract elements of two patterns (shorthand: patternA - patternB)
+    PMul                     - Multiply elements of two patterns (shorthand: patternA * patternB)
+    PDiv                     - Divide elements of two patterns (shorthand: patternA / patternB)
+    PFloorDiv                - Integer division (shorthand: patternA // patternB)
+    PMod                     - Modulo elements of two patterns (shorthand: patternA % patternB)
+    PPow                     - One pattern to the power of another (shorthand: patternA ** patternB)
+    PLShift                  - Binary left-shift (shorthand: patternA << patternB)
+    PRShift                  - Binary right-shift (shorthand: patternA << patternB)
+    PEqual                   - Return 1 if a == b, 0 otherwise (shorthand: patternA == patternB)
+    PGreaterThanOrEqual      - Return 1 if a != b, 0 otherwise (shorthand: patternA != patternB)
+    PGreaterThan             - Return 1 if a > b, 0 otherwise (shorthand: patternA > patternB)
+    PGreaterThanOrEqual      - Return 1 if a >= b, 0 otherwise (shorthand: patternA >= patternB)
+    PLessThan                - Return 1 if a < b, 0 otherwise (shorthand: patternA < patternB)
+    PLessThanOrEqual         - Return 1 if a <= b, 0 otherwise (shorthand: patternA <= patternB)
 
     SCALAR (scalar.py)
-    PChanged             - Outputs a 1 if the value of a pattern has changed.
-    PDiff                - Outputs the difference between the current and previous values of an input pattern
-    PSkipIf              - If `skip` is false, returns `input`; otherwise, returns None.
-    PNormalise           - Adaptively normalise `input` to [0..1] over a linear scale.
-    PMap                 - Apply an arbitrary function to an input pattern.
-    PMapEnumerated       - Apply arbitrary function to input, passing a counter.
-    PLinLin              - Map `input` from linear range [a,b] to linear range [c,d].
-    PLinExp              - Map `input` from linear range [a,b] to exponential range [c,d].
-    PRound               - Round `input` to N decimal places.
-    PScalar              - Reduce tuples and lists into single scalar values,
-    PWrap                - Wrap input note values within <min>, <max>.
-    PIndexOf             - Find index of items from `pattern` in <list>
+    PChanged                 - Outputs a 1 if the value of the input pattern has changed,
+    PDiff                    - Outputs the difference between the current and previous values of an input pattern
+    PSkipIf                  - If `skip` is false, returns `input`; otherwise, returns None.
+    PNormalise               - Adaptively normalise `input` to [0..1] over a linear scale.
+    PMap                     - Apply an arbitrary function to an input pattern.
+    PMapEnumerated           - Apply arbitrary function to input, passing a counter.
+    PScaleLinLin             - Map `input` from linear range [a,b] to linear range [c,d].
+    PScaleLinExp             - Map `input` from linear range [a,b] to exponential range [c,d].
+    PRound                   - Round `input` to N decimal places.
+    PScalar                  - Reduce tuples and lists into single scalar values,
+    PWrap                    - Wrap input note values within <min>, <max>.
+    PIndexOf                 - Find index of items from `pattern` in <list>
 
     SEQUENCE (sequence.py)
-    PSeries              - Arithmetic series, beginning at `start`, increment by `step`
-    PRange               - Similar to PSeries, but specify a max/step value.
-    PGeom                - Geometric series, beginning at `start`, multiplied by `step`
-    PImpulse             - Outputs a 1 every <period> events, otherwise 0.
-    PLoop                - Repeats a finite `pattern` for `n` repeats.
-    PPingPong            - Ping-pong input pattern back and forth N times.
-    PCreep               - Loop `length`-note segment, progressing `creep` notes after `repeats` repeats.
-    PStutter             - Play each note of `pattern` `count` times.
-    PSubsequence         - Returns a finite subsequence of an input pattern.
-    PReverse             - Reverses a finite sequence.
-    PReset               - Resets `pattern` whenever `trigger` is true
-    PCounter             - Increments a counter by 1 for each zero-crossing in `trigger`.
-    PCollapse            - Skip over any rests in `input`
-    PNoRepeats           - Skip over repeated values in `input`
-    PPad                 - Pad `pattern` with rests until it reaches length `length`.
-    PPadToMultiple       - Pad `pattern` with rests until its length is divisible by `multiple`.
-    PArpeggiator         - Arpeggiator.
-    PEuclidean           - Generate Euclidean rhythms.
-    PPermut              - Generate every permutation of `count` input items.
-    PPatternGeneratorAction - Each time its pattern is exhausted, request a new pattern by calling <fn>.
-    PSequenceAction      - Iterate over an array, perform a function, and repeat.
+    PSeries                  - Arithmetic series, beginning at `start`, increment by `step`
+    PRange                   - Similar to PSeries, but specify a max/step value.
+    PGeom                    - Geometric series, beginning at `start`, multiplied by `step`
+    PImpulse                 - Outputs a 1 every <period> events, otherwise 0.
+    PLoop                    - Repeats a finite `pattern` for `n` repeats.
+    PPingPong                - Ping-pong input pattern back and forth N times.
+    PCreep                   - Loop `length`-note segment, progressing `creep` notes after `repeats` repeats.
+    PStutter                 - Play each note of `pattern` `count` times.
+    PSubsequence             - Returns a finite subsequence of an input pattern.
+    PReverse                 - Reverses a finite sequence.
+    PReset                   - Resets `pattern` whenever `trigger` is true
+    PCounter                 - Increments a counter by 1 for each zero-crossing in `trigger`.
+    PCollapse                - Skip over any rests in `input`
+    PNoRepeats               - Skip over repeated values in `input`
+    PPad                     - Pad `pattern` with rests until it reaches length `length`.
+    PPadToMultiple           - Pad `pattern` with rests until its length is divisible by `multiple`.
+    PArpeggiator             - Arpeggiator.
+    PEuclidean               - Generate Euclidean rhythms.
+    PPermut                  - Generate every permutation of `count` input items.
+    PPatternGeneratorAction  - Each time its pattern is exhausted, request a new pattern by calling <fn>.
+    PSequenceAction          - Iterate over an array, perform a function, and repeat.
 
     CHANCE (chance.py)
-    PWhite               - White noise between `min` and `max`.
-    PBrown               - Brownian noise.
-    PWalk                - Random walk around list.
-    PChoice              - Pick a random element from `values`, weighted by optional `weights`.
-    PSample              - Pick multiple random elements from `values`, weighted by optional `weights`,
-    PShuffle             - Shuffled list.
-    PShuffleInput        - Every `n` steps, take `n` values from `pattern` and reorder.
-    PSkip                - Skip events with some probability, 1 - <play>.
-    PFlipFlop            - flip a binary bit with some probability.
-    PSwitchOne           - Capture `length` input values; loop, repeatedly switching two adjacent values.
+    PWhite                   - White noise between `min` and `max`.
+    PBrown                   - Brownian noise.
+    PCoin                    - Coin toss, returning either 0 or 1 given some `probability`.
+    PWalk                    - Random walk around list.
+    PChoice                  - Pick a random element from `values`, weighted by optional `weights`.
+    PSample                  - Pick multiple random elements from `values`, weighted by optional `weights`,
+    PShuffle                 - Shuffled list.
+    PShuffleInput            - Every `n` steps, take `n` values from `pattern` and reorder.
+    PSkip                    - Skip events with some probability, 1 - `play`.
+    PFlipFlop                - flip a binary bit with some probability.
+    PSwitchOne               - Capture `length` input values; loop, repeatedly switching two adjacent values.
+    PRandomExponential       - Random uniform on exponential curve between `min` and `max`,
+    PRandomImpulseSequence   - Random sequence of impulses with probability `probability`.
 
     TONAL (tonal.py)
-    PDegree              - Map scale index <degree> to MIDI notes in <scale>.
-    PFilterByKey         - Filter notes based on their presence in <key>.
-    PNearestNoteInKey    - Return the nearest note in <key>.
-    PMidiNoteToFrequency - Map MIDI note to frequency value.
+    PDegree                  - Map scale index <degree> to MIDI notes in <scale>.
+    PFilterByKey             - Filter notes based on their presence in <key>.
+    PNearestNoteInKey        - Return the nearest note in <key>.
+    PMidiNoteToFrequency     - Map MIDI note to frequency value.
 
     STATIC (static.py)
-    PGlobals             - Static global value identified by a string.
-    PCurrentTime         - Returns the position (in beats) of the current timeline.
+    PGlobals                 - Static global value identified by a string.
+    PCurrentTime             - Returns the position (in beats) of the current timeline.
 
     FADE (fade.py)
-    PFadeNotewise        - Fade a pattern in/out by introducing notes at a gradual rate.
-    PFadeNotewiseRandom  - Fade a pattern in/out by gradually introducing random notes.
+    PFadeNotewise            - Fade a pattern in/out by introducing notes at a gradual rate.
+    PFadeNotewiseRandom      - Fade a pattern in/out by gradually introducing random notes.
 
     MARKOV (markov.py)
-    PMarkov              - First-order Markov chain generator.
+    PMarkov                  - First-order Markov chain generator.
 
     LSYSTEM (lsystem.py)
-    PLSystem             - integer sequence derived from Lindenmayer systems
+    PLSystem                 - integer sequence derived from Lindenmayer systems
 
     WARP (warp.py)
-    PWInterpolate        - Requests a new target warp value from `pattern` every `length` beats
-    PWSine               - Sinosoidal warp, period `length` beats, amplitude +/-<amp>.
-    PWRallantando        - Exponential deceleration to <amp> times the current tempo over `length` beats.
+    PWInterpolate            - Requests a new target warp value from `pattern` every `length` beats
+    PWSine                   - Sinosoidal warp, period `length` beats, amplitude +/-<amp>.
+    PWRallantando            - Exponential deceleration to <amp> times the current tempo over `length` beats.
 
 ## Background
 
 isobar was first designed for the generative sound installation [Variable 4](http://www.variable4.org.uk), in which it was used to generate musical structures in response to changing weather conditions. It was more recently used in [The Listening Machine](http://www.thelisteningmachine.org/), taking live input from Twitter and generating musical output from language patterns, streamed live over the internet.
 
 Many of the concepts behind Pattern and its subclasses are inspired by the brilliant pattern library of the [SuperCollider](http://supercollider.sf.net) synthesis language.
 
+
+
```

### Comparing `isobar-0.1.1/isobar/__init__.py` & `isobar-0.1.2/isobar/__init__.py`

 * *Files identical despite different names*

### Comparing `isobar-0.1.1/isobar/chord.py` & `isobar-0.1.2/isobar/chord.py`

 * *Files identical despite different names*

### Comparing `isobar-0.1.1/isobar/constants.py` & `isobar-0.1.2/isobar/constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -55,48 +55,68 @@
 EVENT_CONTROL = "control"
 EVENT_OSC_ADDRESS = "osc_address"
 EVENT_OSC_PARAMS = "osc_params"
 EVENT_VALUE = "value"
 EVENT_TIME = "time"
 EVENT_PATCH = "patch"
 EVENT_PATCH_PARAMS = "params"
+EVENT_PATCH_OUTPUT = "output"
+EVENT_TRIGGER_NAME = "trigger_name"
+EVENT_TRIGGER_VALUE = "trigger_value"
 EVENT_PROGRAM_CHANGE = "program_change"
 EVENT_SUPERCOLLIDER_SYNTH = "synth"
 EVENT_SUPERCOLLIDER_SYNTH_PARAMS = "params"
 
+#------------------------------------------------------------------------
+# Quantize is used to beat-align events, so should not be included
+# directly in the dictionary.
+#------------------------------------------------------------------------
+EVENT_QUANTIZE = "quantize"
+
+#------------------------------------------------------------------------
+# Legacy keys.
+#------------------------------------------------------------------------
+EVENT_DURATION_LEGACY = "dur"
+EVENT_AMPLITUDE_LEGACY = "amp"
+
 ALL_EVENT_PARAMETERS = [
     EVENT_TYPE, EVENT_ACTIVE, EVENT_CHANNEL, EVENT_AMPLITUDE, EVENT_DURATION,
     EVENT_GATE, EVENT_NOTE, EVENT_DEGREE, EVENT_KEY, EVENT_SCALE, EVENT_OCTAVE,
     EVENT_TRANSPOSE, EVENT_EVENT, EVENT_ACTION, EVENT_ACTION_ARGS, EVENT_CONTROL,
     EVENT_OSC_ADDRESS, EVENT_OSC_PARAMS, EVENT_VALUE, EVENT_TIME, EVENT_PATCH,
-    EVENT_PATCH_PARAMS, EVENT_PROGRAM_CHANGE, EVENT_SUPERCOLLIDER_SYNTH,
-    EVENT_SUPERCOLLIDER_SYNTH_PARAMS
+    EVENT_PATCH_PARAMS, EVENT_PATCH_OUTPUT, EVENT_PROGRAM_CHANGE, EVENT_SUPERCOLLIDER_SYNTH,
+    EVENT_SUPERCOLLIDER_SYNTH_PARAMS, EVENT_QUANTIZE,
+    EVENT_DURATION_LEGACY, EVENT_AMPLITUDE_LEGACY,
+    EVENT_TRIGGER_NAME, EVENT_TRIGGER_VALUE
 ]
 
 #------------------------------------------------------------------------
 # Event types
 #------------------------------------------------------------------------
 EVENT_TYPE_UNKNOWN = "unknown"
 EVENT_TYPE_NOTE = "note"
 EVENT_TYPE_CONTROL = "control"
 EVENT_TYPE_PROGRAM_CHANGE = "program_change"
 EVENT_TYPE_OSC = "osc"
 EVENT_TYPE_ACTION = "action"
-EVENT_TYPE_PATCH = "patch"
+EVENT_TYPE_PATCH_CREATE = "patch"
+EVENT_TYPE_PATCH_TRIGGER = "trigger"
+EVENT_TYPE_PATCH_SET = "set"
 EVENT_TYPE_SUPERCOLLIDER = "supercollider"
 
 #------------------------------------------------------------------------
 # Default parameter values
 #------------------------------------------------------------------------
 DEFAULT_EVENT_CHANNEL = 0
 DEFAULT_EVENT_DURATION = 1
 DEFAULT_EVENT_GATE = 1.0
 DEFAULT_EVENT_AMPLITUDE = 64
 DEFAULT_EVENT_OCTAVE = 0
 DEFAULT_EVENT_TRANSPOSE = 0
+DEFAULT_EVENT_QUANTIZE = 0
 
 #------------------------------------------------------------------------
 # Interpolation modes for continuous signals.
 #------------------------------------------------------------------------
 INTERPOLATION_NONE = "none"
 INTERPOLATION_LINEAR = "linear"
 INTERPOLATION_COSINE = "cosine"
```

### Comparing `isobar-0.1.1/isobar/exceptions.py` & `isobar-0.1.2/isobar/exceptions.py`

 * *Files identical despite different names*

### Comparing `isobar-0.1.1/isobar/io/__init__.py` & `isobar-0.1.2/isobar/io/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 __author__ = "Daniel Jones <http://www.erase.net/>"
 
 from .output import OutputDevice
 from .dummy import DummyOutputDevice
 from .midi import MidiInputDevice, MidiOutputDevice, get_midi_output_names, get_midi_input_names
 from .midifile import MidiFileInputDevice, MidiFileOutputDevice, PatternWriterMIDI
 from .osc import OSCOutputDevice
+from .cv import CVOutputDevice, get_cv_output_devices
 from .socketio import SocketIOOutputDevice
-from .signalflow import SignalflowOutputDevice
+from .signalflow import SignalFlowOutputDevice
 from .midinote import MidiNote
 from .supercollider import SuperColliderOutputDevice
 
 __all__ = ["OutputDevice", "DummyOutputDevice", "MidiInputDevice", "MidiOutputDevice"]
 __all__ += ["get_midi_output_names", "get_midi_input_names"]
 __all__ += ["MidiFileInputDevice", "MidiFileOutputDevice", "PatternWriterMIDI"]
-__all__ += ["OSCOutputDevice", "SocketIOOutputDevice", "SignalflowOutputDevice",
-            "MidiNote", "SuperColliderOutputDevice"]
+__all__ += ["OSCOutputDevice", "SocketIOOutputDevice", "SignalFlowOutputDevice",
+            "MidiNote", "SuperColliderOutputDevice", "CVOutputDevice"]
+__all__ += ["get_cv_output_devices"]
```

### Comparing `isobar-0.1.1/isobar/io/dummy/output.py` & `isobar-0.1.2/isobar/io/dummy/output.py`

 * *Files identical despite different names*

### Comparing `isobar-0.1.1/isobar/io/midi/__init__.py` & `isobar-0.1.2/isobar/io/midi/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,7 +20,11 @@
     Returns:
         List[str]: A list of all possible MIDI input device names.
     """
     input_names = mido.get_input_names()
     return input_names
 
 __all__ = ["MidiInputDevice", "MidiOutputDevice", "get_midi_input_names", "get_midi_output_names"]
+
+# Class aliases for backwards-compatibility
+MidiOut = MidiOutputDevice
+MidiIn = MidiInputDevice
```

### Comparing `isobar-0.1.1/isobar/io/midi/input.py` & `isobar-0.1.2/isobar/io/midi/input.py`

 * *Files identical despite different names*

### Comparing `isobar-0.1.1/isobar/io/midi/output.py` & `isobar-0.1.2/isobar/io/midi/output.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,9 +86,13 @@
         self.midi.send(msg)
 
     def pitch_bend(self, pitch=0, channel=0):
         log.debug("[midi] Pitch bend (channel %d, pitch %d)" % (channel, pitch))
         msg = mido.Message('pitchwheel', pitch=int(pitch), channel=int(channel))
         self.midi.send(msg)
 
+    def set_song_pos(self, pos=0):
+        msg = mido.Message('songpos', pos=pos)
+        self.midi.send(msg)
+
     def __del__(self):
         del self.midi
```

### Comparing `isobar-0.1.1/isobar/io/midifile/input.py` & `isobar-0.1.2/isobar/io/midifile/input.py`

 * *Files identical despite different names*

### Comparing `isobar-0.1.1/isobar/io/midifile/output.py` & `isobar-0.1.2/isobar/io/midifile/output.py`

 * *Files 16% similar despite different names*

```diff
@@ -37,14 +37,22 @@
     def note_off(self, note=60, channel=0):
         dt = self.time - self.last_event_time
         dt_ticks = int(round(dt * self.midifile.ticks_per_beat))
         self.miditrack.append(Message('note_off', note=note, channel=channel, time=dt_ticks))
         self.last_event_time = self.time
 
     def write(self):
+        #------------------------------------------------------------------------
+        # When closing the MIDI file, append a dummy `note_off` event to ensure
+        # any rests at the end of the file remain intact
+        # (cf. https://forum.noteworthycomposer.com/?topic=4708.0)
+        #------------------------------------------------------------------------
+        dt = self.time - self.last_event_time
+        dt_ticks = int(round(dt * self.midifile.ticks_per_beat))
+        self.miditrack.append(Message('note_off', note=0, channel=0, time=dt_ticks))
         self.midifile.save(self.filename)
 
 class PatternWriterMIDI:
     """ Writes a pattern to a MIDI file.
         Requires the MIDIUtil package:
         https://code.google.com/p/midiutil/ """
```

### Comparing `isobar-0.1.1/isobar/io/osc/output.py` & `isobar-0.1.2/isobar/io/osc/output.py`

 * *Files identical despite different names*

### Comparing `isobar-0.1.1/isobar/io/output.py` & `isobar-0.1.2/isobar/io/output.py`

 * *Files identical despite different names*

### Comparing `isobar-0.1.1/isobar/io/socketio/output.py` & `isobar-0.1.2/isobar/io/socketio/output.py`

 * *Files identical despite different names*

### Comparing `isobar-0.1.1/isobar/io/supercollider/output.py` & `isobar-0.1.2/isobar/io/supercollider/output.py`

 * *Files identical despite different names*

### Comparing `isobar-0.1.1/isobar/key.py` & `isobar-0.1.2/isobar/key.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 from .scale import Scale
 from .note import Note
 from .util import midi_note_to_note_name, note_name_to_midi_note
-from .exceptions import InvalidKeyException
 
 import random
 
 class Key:
     """ Represents a harmonic structure, containing a tonic and scale.
     """
 
     def __init__(self, tonic=0, scale=Scale.major):
         if type(tonic) == str:
-            tonic = note_name_to_midi_note(tonic)
+            # TODO unit test for this
+            if " " in tonic:
+                tonic_str, scale_str = tuple(tonic.split(" "))
+                tonic = note_name_to_midi_note(tonic_str)
+                scale = Scale.byname(scale_str)
+            else:
+                tonic = note_name_to_midi_note(tonic)
         if type(scale) == str:
             scale = Scale.byname(scale)
-        if tonic < 0:
-            raise InvalidKeyException("Tonic must be >= 0")
-        if tonic >= scale.octave_size:
-            raise InvalidKeyException("Tonic cannot be beyond octave size")
 
         self.tonic = tonic
         self.scale = scale
 
     def __eq__(self, other):
         return self.tonic == other.tonic and self.scale == other.scale
 
     def __str__(self):
         return "Key: %s %s" % (midi_note_to_note_name(self.tonic)[:], self.scale.name)
 
     def __repr__(self):
         return 'Key(%s, "%s")' % (self.tonic, self.scale.name)
 
+    def __hash__(self):
+        return hash((self.tonic, hash(self.scale)))
+
     def get(self, degree):
         """ Returns the <degree>th semitone within this key. """
         if degree is None:
             return None
 
         semitone = self.scale[degree]
         return semitone + self.tonic
@@ -124,7 +128,9 @@
         t = random.randint(0, 11)
         s = Scale.random()
         return Key(t, s)
 
     @staticmethod
     def all():
         return [Key(note, scale) for note in Note.all() for scale in Scale.all()]
+
+Key.default = Key("C", "major")
```

### Comparing `isobar-0.1.1/isobar/note.py` & `isobar-0.1.2/isobar/note.py`

 * *Files identical despite different names*

### Comparing `isobar-0.1.1/isobar/pattern/__init__.py` & `isobar-0.1.2/isobar/pattern/__init__.py`

 * *Files identical despite different names*

### Comparing `isobar-0.1.1/isobar/pattern/chance.py` & `isobar-0.1.2/isobar/pattern/chance.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import copy
 import random
 
 from .core import Pattern
-from ..util import wnchoice
+from ..util import wnchoice, scale_lin_exp
 
 class PStochasticPattern(Pattern):
     """
     PStochasticPattern is the superclass of all chance-based patterns.
     It contains its own random number generator and state, so that it can be
     seeded independently of other RNG processes in the application.
 
@@ -35,23 +35,23 @@
         if seed is None:
             seed = random.randint(0, sys.maxsize)
         self._seed = seed
         self.rng.seed(self._seed)
 
 class PWhite(PStochasticPattern):
     """ PWhite: White noise between `min` and `max`.
-       If values are given as floats, output values are also floats < max.
-       If values are ints, output values are ints <= max (as random.randint)
+        If values are given as floats, output values are also floats < max.
+        If values are ints, output values are ints <= max (as random.randint)
 
         >>> PWhite(0, 10).nextn(16)
         [8, 10, 8, 1, 7, 3, 1, 9, 9, 3, 2, 10, 7, 5, 10, 4]
 
         >>> PWhite(0.0, 10.0).nextn(16)
         [3.6747936220022082, 0.61313530428271923, 9.1515368696591555, ... 6.2963694390145974 ]
-       """
+        """
 
     def __init__(self, min=0.0, max=1.0):
         super().__init__()
 
         self.min = min
         self.max = max
 
@@ -113,14 +113,38 @@
             steps = list(range(-vstep, vstep + 1))
             self.value += self.rng.choice(steps)
         self.value = min(max(self.value, vmin), vmax)
 
         return rv
 
 
+class PCoin(PStochasticPattern):
+    """ PCoin: Coin toss, returning either 0 or 1 given some `probability`.
+               `probability` is the chance of returning 1, and must be between [0, 1].
+
+               This is a convenience pattern which could also be written
+                as `PWhite(0, 1) < probability`
+
+        >>> PCoin(0.75).nextn(16)
+        [1, 1, 1, 1, 1, 1, 1, 0, 0, 1, 0, 1, 1, 0, 0, 1]
+       """
+
+    def __init__(self, probability=0.5):
+        super().__init__()
+        self.probability = probability
+
+    def __next__(self):
+        probability = Pattern.value(self.probability)
+
+        if self.rng.uniform(0, 1) < probability:
+            return 1
+        else:
+            return 0
+
+
 class PRandomWalk(PStochasticPattern):
     """ PWalk: Random walk around list.
                Jumps between `min` and `max` steps inclusive.
 
         >>> PRandomWalk([ 0, 2, 5, 8, 11 ], min=1, max=2).nextn(16)
         [8, 11, 0, 8, 0, 11, 2, 11, 2, 0, 5, 8, 11, 8, 5, 8]
         """
@@ -309,30 +333,30 @@
             self.rng.shuffle(self.values)
 
         rv = self.values[self.pos]
         self.pos += 1
         return rv
 
 class PSkip(PStochasticPattern):
-    """ PSkip: Skip events with some probability, 1 - <play>.
-               Set <regularise> to True to skip events regularly.
+    """ PSkip: Skip events with some probability, 1 - `play`.
+               Set <regular> to True to skip events regularly.
         """
 
-    def __init__(self, pattern, play, regularise=False):
+    def __init__(self, pattern, play, regular=False):
         super().__init__()
         self.pattern = pattern
         self.play = play
-        self.regularise = regularise
+        self.regular = regular
         self.pos = 0.0
 
     def __next__(self):
         value = Pattern.value(self.pattern)
         play = Pattern.value(self.play)
 
-        if self.regularise:
+        if self.regular:
             self.pos += play
             if self.pos >= 1:
                 self.pos -= 1
                 return value
         else:
             if self.rng.uniform(0, 1) < play:
                 return value
@@ -405,7 +429,122 @@
             indexP = (index + 1) % len(self.values)
             self.values[index], self.values[indexP] = self.values[indexP], self.values[index]
             self.pos = 0
 
         rv = self.values[self.pos]
         self.pos += 1
         return rv
+
+class PRandomExponential(PStochasticPattern):
+    """ PRandomExponential: Random uniform on exponential curve between `min` and `max`,
+                            both of which must be strictly positive.
+        If values are given as floats, output values are also floats < max.
+        If values are ints, output values are ints <= max (as random.randint)
+
+        >>> PRandomExponential(1, 100).nextn(16)
+        [3, 2, 12, 1, 6, 13, 14, 25, 78, 78, 4, 49, 5, 97, 69, 12]
+
+        >>> PRandomExponential(1.0, 100.0).nextn(16)
+        [54.84880471711992, 89.53150541306805, 2.4077905492103318, ... ]
+        """
+
+    def __init__(self, min=1.0, max=10.0):
+        super().__init__()
+
+        self.min = min
+        self.max = max
+
+    def __next__(self):
+        min = Pattern.value(self.min)
+        max = Pattern.value(self.max)
+
+        norm = self.rng.uniform(0, 1)
+        rv = scale_lin_exp(norm, 0, 1, min, max)
+        if type(min) == float:
+            return rv
+        else:
+            return int(rv)
+
+class PRandomImpulseSequence(PStochasticPattern):
+    """ PRandomImpulseSequence: Random sequence of impulses with probability `probability`.
+
+        >>> PRandomImpulseSequence(0.3, 16).nextn(16)
+        [...]
+
+        """
+
+    def __init__(self, probability=0.0, length=8):
+        super().__init__()
+
+        self.probability = probability
+        self.length = length
+        self.current_length = 0
+        self.values = []
+        self.pos = 0
+        self.every(0)
+
+    def generate(self):
+        probability = Pattern.value(self.probability)
+        self.current_length = Pattern.value(self.length)
+        self.values = [int(self.rng.uniform(0, 1) < probability) for _ in range(self.current_length)]
+        self.pos = 0
+
+    def every(self, n, action=None):
+        if action == "explore":
+            self.every_action = lambda: self.explore()
+        elif action == "reset":
+            self.every_action = lambda: self.reset()
+        elif action == "generate":
+            self.every_action = lambda: self.generate()
+        else:
+            self.every_action = action
+        self.every_count = n
+        self.every_index = 0
+
+        # return self so this can be used in scheduling:
+        # "active": PRandomImpulseSequence(0.3, 8).every(8, "explore"),
+        return self
+
+    def explore(self):
+        # TODO: Merge function with PExplorer
+        P_SWITCH = 0
+        P_MUTATE = 1
+        P_ROTATE = 2
+        op = self.rng.choice([P_SWITCH, P_MUTATE, P_ROTATE])
+        if op == P_SWITCH:
+            indices = list(range(len(self.values)))
+            self.rng.shuffle(indices)
+            self.values[indices[0]], self.values[indices[1]] = self.values[indices[1]], self.values[indices[0]]
+        elif op == P_MUTATE:
+            index = random.randrange(len(self.values))
+            self.values[index] = 1 - self.values[index]
+        elif op == P_ROTATE:
+            direction_right = self.rng.uniform(0, 1) < 0.5
+            if direction_right:
+                self.values = [self.values[-1]] + self.values[:-1]
+            else:
+                self.values = self.values[1:] + [self.values[0]]
+
+    def __next__(self):
+        if self.every_action:
+            if self.every_index == self.every_count:
+                self.every_action()
+                self.every_index = 0
+            self.every_index += 1
+
+        if self.pos >= len(self.values):
+            self.pos = 0
+            self.current_length = Pattern.value(self.length)
+            #--------------------------------------------------------------------------------
+            # Each time through the cycle, check if the length input has changed.
+            # If yes, change the loop length by appending or trimming.
+            #--------------------------------------------------------------------------------
+            if self.current_length > len(self.values):
+                probability = Pattern.value(self.probability)
+                range_diff = self.current_length - len(self.values)
+                self.values += [int(self.rng.uniform(0, 1) < probability) for _ in range(range_diff)]
+            if self.current_length < len(self.values):
+                self.values = self.values[:self.current_length]
+
+        rv = self.values[self.pos]
+        self.pos += 1
+        return rv
```

### Comparing `isobar-0.1.1/isobar/pattern/core.py` & `isobar-0.1.2/isobar/pattern/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,123 +35,113 @@
 
     def __abs__(self):
         """ Absolute value. """
         return PAbs(self)
 
     def __add__(self, operand):
         """Binary op: add two patterns"""
-        operand = Pattern.pattern(operand)
         return PAdd(self, operand)
 
     def __radd__(self, operand):
         """Binary op: add two patterns"""
         return self.__add__(operand)
 
     def __sub__(self, operand):
         """Binary op: subtract two patterns"""
-        operand = Pattern.pattern(operand)
         return PSub(self, operand)
 
     def __rsub__(self, operand):
         """Binary op: subtract two patterns"""
-        operand = Pattern.pattern(operand)
         return PSub(operand, self)
 
     def __mul__(self, operand):
         """Binary op: multiply two patterns"""
-        operand = Pattern.pattern(operand)
         return PMul(self, operand)
 
     def __rmul__(self, operand):
         """Binary op: multiply two patterns"""
         return self.__mul__(operand)
 
     def __truediv__(self, operand):
         """Binary op: divide two patterns"""
-        operand = Pattern.pattern(operand)
         return PDiv(self, operand)
 
     def __rtruediv__(self, operand):
         """Binary op: divide two patterns"""
-        operand = Pattern.pattern(operand)
         return PDiv(operand, self)
 
     def __floordiv__(self, operand):
         """Binary op: integer divide two patterns"""
-        operand = Pattern.pattern(operand)
         return PFloorDiv(self, operand)
 
     def __rfloordiv__(self, operand):
         """Binary op: integer divide two patterns"""
-        operand = Pattern.pattern(operand)
         return PFloorDiv(operand, self)
 
     def __mod__(self, operand):
         """Modulo"""
-        operand = Pattern.pattern(operand)
         return PMod(self, operand)
 
     def __rmod__(self, operand):
         """Modulo (as operand)"""
         operand = Pattern.pattern(operand)
         return operand.__mod__(self)
 
     def __pow__(self, operand):
         """Power"""
-        operand = Pattern.pattern(operand)
         return PPow(self, operand)
 
     def __rpow__(self, operand):
         """Power (as operand)"""
         operand = Pattern.pattern(operand)
         return operand.__pow__(self)
 
     def __lshift__(self, operand):
         """Left bitshift"""
-        operand = Pattern.pattern(operand)
         return PLShift(self, operand)
 
     def __rlshift__(self, operand):
         """Left bitshift"""
-        operand = Pattern.pattern(operand)
         return PLShift(operand, self)
 
     def __rshift__(self, operand):
         """Right bitshift"""
-        operand = Pattern.pattern(operand)
         return PRShift(self, operand)
 
     def __rrshift__(self, operand):
         """Right bitshift"""
-        operand = Pattern.pattern(operand)
         return PRShift(operand, self)
 
     def __eq__(self, operand):
         """ Equal """
-        return PEqual(self, Pattern.pattern(operand))
+        return PEqual(self, operand)
 
     def __ne__(self, operand):
         """ Not equal """
-        return PNotEqual(self, Pattern.pattern(operand))
+        return PNotEqual(self, operand)
 
     def __gt__(self, operand):
         """ Greater than """
-        return PGreaterThan(self, Pattern.pattern(operand))
+        return PGreaterThan(self, operand)
 
     def __ge__(self, operand):
         """ Greater than or equal """
-        return PGreaterThanOrEqual(self, Pattern.pattern(operand))
+        return PGreaterThanOrEqual(self, operand)
 
     def __lt__(self, operand):
         """ Less than """
-        return PLessThan(self, Pattern.pattern(operand))
+        return PLessThan(self, operand)
 
     def __le__(self, operand):
         """ Less than or equal """
-        return PLessThanOrEqual(self, Pattern.pattern(operand))
+        return PLessThanOrEqual(self, operand)
+
+    def __and__(self, operand):
+        """ And """
+        return PAnd(self, operand)
 
     def __iter__(self):
         return self
 
     def nextn(self, count):
         """
         Returns the next `count` output values.
@@ -370,14 +360,17 @@
 
     def __getitem__(self, key):
         return self.dict[key]
 
     def __setitem__(self, key, value):
         self.dict[key] = value
 
+    def __delitem__(self, key):
+        del self.dict[key]
+
     def __contains__(self, key):
         return key in self.dict
 
     def load(self, filename, quantize=None):
         """
         Load pattern data from a MIDI file.
 
@@ -436,21 +429,21 @@
 
         return rv
 
 class PDictKey(Pattern):
     """ PDictKey: Request a specified key from a dictionary.
         """
 
-    def __init__(self, key, dict):
-        self.key = key
+    def __init__(self, dict, key):
         self.dict = dict
+        self.key = key
 
     def __next__(self):
-        vkey = Pattern.value(self.key)
         vdict = Pattern.value(self.dict)
+        vkey = Pattern.value(self.key)
         return vdict[vkey]
 
 class PConcatenate(Pattern):
     """ PConcatenate: Concatenate the output of multiple sequences.
 
         >>> PConcatenate([ PSequence([ 1, 2, 3 ], 2), PSequence([ 9, 8, 7 ], 2) ]).nextn(16)
         [1, 2, 3, 1, 2, 3, 9, 8, 7, 9, 8, 7]
@@ -511,164 +504,175 @@
 class PAdd(PBinOp):
     """ PAdd: Add elements of two patterns (shorthand: patternA + patternB) """
 
     def __str__(self):
         return "%s + %s" % (self.a, self.b)
 
     def __next__(self):
-        a = next(self.a)
-        b = next(self.b)
+        a = Pattern.value(self.a)
+        b = Pattern.value(self.b)
         return None if a is None or b is None else a + b
 
 class PSub(PBinOp):
     """ PSub: Subtract elements of two patterns (shorthand: patternA - patternB) """
 
     def __str__(self):
         return "%s - %s" % (self.a, self.b)
 
     def __next__(self):
-        a = next(self.a)
-        b = next(self.b)
+        a = Pattern.value(self.a)
+        b = Pattern.value(self.b)
         return None if a is None or b is None else a - b
 
 class PMul(PBinOp):
     """ PMul: Multiply elements of two patterns (shorthand: patternA * patternB) """
 
     def __str__(self):
         return "(%s) * (%s)" % (self.a, self.b)
 
     def __next__(self):
-        a = next(self.a)
-        b = next(self.b)
+        a = Pattern.value(self.a)
+        b = Pattern.value(self.b)
         return None if a is None or b is None else a * b
 
 class PDiv(PBinOp):
     """ PDiv: Divide elements of two patterns (shorthand: patternA / patternB) """
 
     def __str__(self):
         return "(%s) / (%s)" % (self.a, self.b)
 
     def __next__(self):
-        a = next(self.a)
-        b = next(self.b)
+        a = Pattern.value(self.a)
+        b = Pattern.value(self.b)
         return None if a is None or b is None else a / b
 
 class PFloorDiv(PBinOp):
     """ PFloorDiv: Integer division (shorthand: patternA // patternB) """
 
     def __str__(self):
         return "(%s) // (%s)" % (self.a, self.b)
 
     def __next__(self):
-        a = next(self.a)
-        b = next(self.b)
+        a = Pattern.value(self.a)
+        b = Pattern.value(self.b)
         return None if a is None or b is None else a // b
 
 class PMod(PBinOp):
     """ PMod: Modulo elements of two patterns (shorthand: patternA % patternB) """
 
     def __str__(self):
         return "(%s) %% (%s)" % (self.a, self.b)
 
     def __next__(self):
-        a = next(self.a)
-        b = next(self.b)
+        a = Pattern.value(self.a)
+        b = Pattern.value(self.b)
         return None if a is None or b is None else a % b
 
 class PPow(PBinOp):
     """ PPow: One pattern to the power of another (shorthand: patternA ** patternB) """
 
     def __str__(self):
         return "pow(%s, %s)" % (self.a, self.b)
 
     def __next__(self):
-        a = next(self.a)
-        b = next(self.b)
+        a = Pattern.value(self.a)
+        b = Pattern.value(self.b)
         return None if a is None or b is None else pow(a, b)
 
 class PLShift(PBinOp):
     """ PLShift: Binary left-shift (shorthand: patternA << patternB) """
 
     def __str__(self):
         return "(%s << %s)" % (self.a, self.b)
 
     def __next__(self):
-        a = next(self.a)
-        b = next(self.b)
+        a = Pattern.value(self.a)
+        b = Pattern.value(self.b)
         return None if a is None or b is None else a << b
 
 class PRShift(PBinOp):
     """ PRShift: Binary right-shift (shorthand: patternA << patternB) """
 
     def __str__(self):
         return "(%s >> %s)" % (self.a, self.b)
 
     def __next__(self):
-        a = next(self.a)
-        b = next(self.b)
+        a = Pattern.value(self.a)
+        b = Pattern.value(self.b)
         return None if a is None or b is None else a >> b
 
 class PEqual(PBinOp):
     """ PEqual: Return 1 if a == b, 0 otherwise (shorthand: patternA == patternB) """
 
     def __str__(self):
         return "%s == %s" % (self.a, self.b)
 
     def __next__(self):
-        a = next(self.a)
-        b = next(self.b)
+        a = Pattern.value(self.a)
+        b = Pattern.value(self.b)
         return None if a is None or b is None else a == b
 
 class PNotEqual(PBinOp):
     """ PGreaterThanOrEqual: Return 1 if a != b, 0 otherwise (shorthand: patternA != patternB) """
 
     def __str__(self):
         return "%s != %s" % (self.a, self.b)
 
     def __next__(self):
-        a = next(self.a)
-        b = next(self.b)
+        a = Pattern.value(self.a)
+        b = Pattern.value(self.b)
         return None if a is None or b is None else a != b
 
 class PGreaterThan(PBinOp):
     """ PGreaterThan: Return 1 if a > b, 0 otherwise (shorthand: patternA > patternB) """
 
     def __str__(self):
         return "%s > %s" % (self.a, self.b)
 
     def __next__(self):
-        a = next(self.a)
-        b = next(self.b)
+        a = Pattern.value(self.a)
+        b = Pattern.value(self.b)
         return None if a is None or b is None else a > b
 
 class PGreaterThanOrEqual(PBinOp):
     """ PGreaterThanOrEqual: Return 1 if a >= b, 0 otherwise (shorthand: patternA >= patternB) """
 
     def __str__(self):
         return "%s >= %s" % (self.a, self.b)
 
     def __next__(self):
-        a = next(self.a)
-        b = next(self.b)
+        a = Pattern.value(self.a)
+        b = Pattern.value(self.b)
         return None if a is None or b is None else a >= b
 
 class PLessThan(PBinOp):
     """ PLessThan: Return 1 if a < b, 0 otherwise (shorthand: patternA < patternB) """
 
     def __str__(self):
         return "%s < %s" % (self.a, self.b)
 
     def __next__(self):
-        a = next(self.a)
-        b = next(self.b)
+        a = Pattern.value(self.a)
+        b = Pattern.value(self.b)
         return None if a is None or b is None else a < b
 
 class PLessThanOrEqual(PBinOp):
     """ PLessThanOrEqual: Return 1 if a <= b, 0 otherwise (shorthand: patternA <= patternB) """
 
     def __str__(self):
         return "%s <= %s" % (self.a, self.b)
 
     def __next__(self):
-        a = next(self.a)
-        b = next(self.b)
+        a = Pattern.value(self.a)
+        b = Pattern.value(self.b)
         return None if a is None or b is None else a <= b
+
+class PAnd(PBinOp):
+    """ PAnd: Return True if a and b, False otherwise (shorthand: patternA & patternB) """
+
+    def __str__(self):
+        return "%s & %s" % (self.a, self.b)
+
+    def __next__(self):
+        a = Pattern.value(self.a)
+        b = Pattern.value(self.b)
+        return True if a and b else False
```

### Comparing `isobar-0.1.1/isobar/pattern/fade.py` & `isobar-0.1.2/isobar/pattern/fade.py`

 * *Files identical despite different names*

### Comparing `isobar-0.1.1/isobar/pattern/lsystem.py` & `isobar-0.1.2/isobar/pattern/lsystem.py`

 * *Files identical despite different names*

### Comparing `isobar-0.1.1/isobar/pattern/markov.py` & `isobar-0.1.2/isobar/pattern/markov.py`

 * *Files identical despite different names*

### Comparing `isobar-0.1.1/isobar/pattern/oscillator.py` & `isobar-0.1.2/isobar/pattern/oscillator.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,28 +6,33 @@
     """ PTri: Generates a triangle waveform of period `length`.
 
         >>> p = PTri(10)
         >>> p.nextn(10)
         [0.0, 0.2, 0.4, 0.6, 0.8, 1.0, 0.8, 0.6, 0.4, 0.2]
         """
 
-    def __init__(self, length=10):
+    def __init__(self, length=10, min=0.0, max=1.0):
         self.length = length
+        self.min = min
+        self.max = max
         self.reset()
 
     def reset(self):
         self.phase = 0.0
 
     def __next__(self):
         length = Pattern.value(self.length)
+        min = Pattern.value(self.min)
+        max = Pattern.value(self.max)
 
         norm_phase = float(self.phase) / length
         if norm_phase < 0.5:
             rv = norm_phase * 2.0
         else:
             rv = 1.0 - (norm_phase - 0.5) * 2.0
+        rv = min + (max - min) * rv
 
         self.phase += 1
         if self.phase > length:
             self.phase -= length
 
         return rv
```

### Comparing `isobar-0.1.1/isobar/pattern/scalar.py` & `isobar-0.1.2/isobar/pattern/scalar.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 from .core import Pattern
 from .sequence import PSeries
+from ..util import scale_lin_exp, scale_lin_lin
 
 class PChanged(Pattern):
-    """ PChanged: Outputs a 1 if the value of a pattern has changed.
-        The length of the output patter is always 1 less than the length of the input.
+    """ PChanged: Outputs a 1 if the value of the input pattern has changed,
+        or 0 otherwise.
+
+        >>> a = PSequence([1, 0, 1, 2, 2, 2, 1, 0, 0, 1], repeats=1)
+        >>> b = PChanged(a)
+        >>> b.all()
+        [1, 1, 1, 0, 0, 1, 1, 0, 1]
         """
 
     def __init__(self, source):
         self.source = source
         self.current = Pattern.value(self.source)
 
     def reset(self):
@@ -19,15 +25,21 @@
         rv = 0 if next == self.current else 1
         self.current = next
         return rv
 
 class PDiff(Pattern):
     """ PDiff: Outputs the difference between the current and previous values of an input pattern
         If the current or next value are None, a value of None will be output.
+
         The length of the output pattern is always 1 less than the length of the input.
+
+        >>> a = PSequence([1, 0, 1, 2, 2, 2, 1, 0, 0, 1], repeats=1)
+        >>> b = PDiff(a)
+        >>> b.all()
+        [-1, 1, 1, 0, 0, -1, -1, 0, 1]
         """
 
     def __init__(self, source):
         self.source = source
         self.current = Pattern.value(self.source)
 
     def reset(self):
@@ -141,45 +153,34 @@
         args = [Pattern.value(value) for value in self.args]
         kwargs = dict((key, Pattern.value(value)) for key, value in list(self.kwargs.items()))
         value = next(self.input)
         rv = self.operator(next(self.counter), value, *args, **kwargs)
         return rv
 
 class PScaleLinLin(PMap):
-    """ PLinLin: Map `input` from linear range [a,b] to linear range [c,d].
+    """ PScaleLinLin: Map `input` from linear range [a,b] to linear range [c,d].
 
         >>> p = PScaleLinLin(PWhite(), 0, 1, -50, 50)
         >>> p.nextn(16)
         [-34.434991496625955, -33.38823791706497, 42.153457333940267, 16.692545937573783, ... -48.850511242044604 ]
         """
 
-    def linlin(self, value, from_min=0, from_max=1, to_min=0, to_max=1):
-        norm = float(value - from_min) / (from_max - from_min)
-        return norm * float(to_max - to_min) + to_min
-
     def __init__(self, input, *args):
-        PMap.__init__(self, input, self.linlin, *args)
+        super().__init__(input, scale_lin_lin, *args)
 
 class PScaleLinExp(PMap):
-    """ PLinExp: Map `input` from linear range [a,b] to exponential range [c,d].
+    """ PScaleLinExp: Map `input` from linear range [a,b] to exponential range [c,d].
 
         >>> p = PScaleLinExp(PWhite(0.0, 1.0), 0, 1, 40, 20000)
         >>> p.nextn(16)
         [946.888, 282.944, 2343.145, 634.637, 218.844, 19687.330, 4457.627, 172.419, 934.666, ... 46.697 ]
         """
 
-    def linexp(self, value, from_min=0, from_max=1, to_min=1, to_max=10):
-        if value < from_min:
-            return to_min
-        if value > from_max:
-            return to_max
-        return ((to_max / to_min) ** ((value - from_min) / (from_max - from_min))) * to_min
-
     def __init__(self, input, *args):
-        super(self, input, self.linexp, *args)
+        super().__init__(input, scale_lin_exp, *args)
 
 class PRound(PMap):
     """ PRound: Round `input` to N decimal places.
 
         >>> p = PRound(PWhite(0.0, 10.0))
         >>> p.nextn(16)
         [6, 8, 6, 0, 7, 6, 6, 4, 7, 7, 8, 7, 6, 8, 8, 4]
```

### Comparing `isobar-0.1.1/isobar/pattern/sequence.py` & `isobar-0.1.2/isobar/pattern/sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -339,16 +339,16 @@
         >>> p.nextn(16)
         [0, 0, 1, 1, 2, 2, 3, 3, 4, 4, 5, 5, 6, 6, 7, 7]
         """
 
     def __init__(self, pattern, count=2):
         self.pattern = pattern
         self.count = count
-        self.count_current = Pattern.value(count)
-        self.pos = self.count_current
+        self.count_current = 0
+        self.pos = 0
         self.value = 0
 
     def __next__(self):
         if self.pos >= self.count_current:
             self.count_current = Pattern.value(self.count)
             self.value = next(self.pattern)
             self.pos = 0
@@ -686,26 +686,36 @@
         if self.pos >= len(sequence):
             self.pos = 0
         rv = sequence[self.pos]
         self.pos += 1
         return rv
 
     def _split_remainder(self, seq):
+        """
+        Assuming an input array of the form [a, a, a, a, b, b, b],
+        partitions the input into two halves and returns
+        ([a, a, a, a], [b, b, b])
+        """
         last = None
         a = []
         b = []
         for value in seq:
             if last is None or value == last:
                 a.append(value)
                 last = value
             else:
                 b.append(value)
         return (a, b)
 
     def _interleave(self, a, b):
+        """
+        Assuming two input arrays of the form ([a, a, a, a], [b, b, b]),
+        interleaves the two with concatenation and returns
+        ([ab, ab, ab, a])
+        """
         if len(a) < len(b):
             return [a[n] + b[n] for n in range(len(a))] + b[len(a) - len(b):]
         elif len(b) < len(a):
             return [a[n] + b[n] for n in range(len(b))] + a[len(b) - len(a):]
         else:
             return [a[n] + b[n] for n in range(len(b))]
 
@@ -721,26 +731,28 @@
                 break
             seqs = self._interleave(seqs, remainder)
             seqs, remainder = self._split_remainder(seqs)
 
         return reduce(lambda a, b: a + b, seqs + remainder)
 
 class PExplorer(Pattern):
-    def __init__(self, density=0.5, length=4, length_min=2, length_max=6, value_max=12, jump_max=4):
+    def __init__(self, density=0.5, length=4, length_min=2, length_max=6, value_max=12, jump_max=4, loop=None):
         self.density = density
         self.length = length
         self.length_min = length_min
         self.length_max = length_max
         self.value_max = value_max
         self.jump_max = jump_max
+        self.loop = loop
         self.reset()
 
     def reset(self):
         super().reset()
         self.counter = 0
+        self.loop_pos = 0
         self.values = []
         self._generate_values()
 
     def _generate_values(self):
         self.values = []
         value_last = None
         for n in range(self.length):
@@ -783,16 +795,17 @@
         log.debug("PExplorer: Selected operation: %s" % OPERATION_NAMES[operation])
 
         #------------------------------------------------------------------------
         # MUTATE: Replace a note with another note found within the sequence.
         #------------------------------------------------------------------------
         if operation == OP_MUTATE:
             filled_indices = [n[0] for n in filter(lambda n: n[1] is not None, list(enumerate(values)))]
-            index = random.choice(filled_indices)
-            values[index] = random.randint(0, self.value_max)
+            if len(filled_indices) > 0:
+                index = random.choice(filled_indices)
+                values[index] = random.randint(0, self.value_max)
 
         #------------------------------------------------------------------------
         # ROTATE: Rotate the sequence forwards or backwards one slot.
         #------------------------------------------------------------------------
         elif operation == OP_ROTATE:
             if random.uniform(0, 1) < 0.1:
                 values = values[-1:] + values[:-1]
@@ -846,15 +859,22 @@
 
         self.values = values
         self.counter = 0
         return self
 
     def __next__(self):
         if self.counter >= len(self.values):
-            raise StopIteration
+            if self.loop is None:
+                raise StopIteration
+            else:
+                self.loop_pos += 1
+                if self.loop_pos >= self.loop:
+                    self.explore()
+                    self.loop_pos = 0
+                self.counter = 0
 
         rv = self.values[self.counter]
         self.counter += 1
         return rv
 
 class PPermut(Pattern):
     """ PPermut: Generate every permutation of `count` input items.
@@ -959,7 +979,39 @@
             repeats = Pattern.value(self.repeats)
             self.repeat_counter += 1
             if self.repeat_counter >= repeats:
                 raise StopIteration
             self.list = self.fn(self.list)
             self.sequence = PSequence(self.list, 1)
             return next(self)
+
+class PMetropolis(Pattern):
+    def __init__(self, notes, repeats, rests):
+        self.notes = notes
+        self.repeats = repeats
+        self.rests = rests
+        self.note_index = 0
+        self.note_offset = 0
+
+    def __next__(self):
+        repeats = self.repeats
+        if len(repeats) < len(self.notes):
+            repeats = repeats * int(math.ceil(len(self.notes) / len(repeats)))
+        rests = self.rests
+        if len(rests) < len(self.notes):
+            rests = rests * int(math.ceil(len(self.notes) / len(rests)))
+
+        if self.note_offset > repeats[self.note_index] + rests[self.note_index]:
+            self.note_index += 1
+            self.note_offset = 0
+        if self.note_index >= len(self.notes):
+            self.note_index = 0
+            self.note_offset = 0
+
+        if self.note_offset < repeats[self.note_index]:
+            rv = self.notes[self.note_index]
+        else:
+            rv = None
+
+        self.note_offset += 1
+        return rv
+
```

### Comparing `isobar-0.1.1/isobar/pattern/tonal.py` & `isobar-0.1.2/isobar/pattern/tonal.py`

 * *Files identical despite different names*

### Comparing `isobar-0.1.1/isobar/pattern/warp.py` & `isobar-0.1.2/isobar/pattern/warp.py`

 * *Files identical despite different names*

### Comparing `isobar-0.1.1/isobar/scale.py` & `isobar-0.1.2/isobar/scale.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 
     def __eq__(self, other):
         return self.semitones == other.semitones and self.octave_size == other.octave_size
 
     def __contains__(self, semitone):
         return (semitone % self.scale.octave_size) in self.semitones
 
+    def __hash__(self):
+        return hash(tuple((tuple(self.semitones), tuple(self.weights), self.name, self.octave_size)))
+
     def get(self, n):
         """ Retrieve the n'th degree of this scale. """
         if n is None:
             return None
 
         octave = n // len(self.semitones)
         degree = n % len(self.semitones)
```

### Comparing `isobar-0.1.1/isobar/timeline/clock.py` & `isobar-0.1.2/isobar/timeline/clock.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,17 @@
 
     def warp(self, warper):
         self.warpers.append(warper)
 
     def unwarp(self, warper):
         self.warpers.remove(warper)
 
+    def rewind(self):
+        self.clock_target.set_song_pos(0)
+
 class DummyClock (Clock):
     """
     Clock subclass used in testing, which ticks at the highest rate possible.
     """
     def run(self):
         while True:
             self.clock_target.tick()
```

### Comparing `isobar-0.1.1/isobar/timeline/event.py` & `isobar-0.1.2/isobar/timeline/event.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,62 @@
 from ..pattern import Pattern
-from ..key import Key
 from ..scale import Scale
+from ..key import Key
 from ..constants import *
 from ..exceptions import InvalidEventException
 import logging
 from typing import Iterable
 
 log = logging.getLogger(__name__)
 
+class EventDefaults:
+    def __init__(self):
+        default_values = {
+            EVENT_ACTIVE: True,
+            EVENT_CHANNEL: DEFAULT_EVENT_CHANNEL,
+            EVENT_DURATION: DEFAULT_EVENT_DURATION,
+            EVENT_GATE: DEFAULT_EVENT_GATE,
+            EVENT_AMPLITUDE: DEFAULT_EVENT_AMPLITUDE,
+            EVENT_OCTAVE: DEFAULT_EVENT_OCTAVE,
+            EVENT_TRANSPOSE: DEFAULT_EVENT_TRANSPOSE,
+            EVENT_KEY: Key("C", Scale.default),
+            EVENT_QUANTIZE: DEFAULT_EVENT_QUANTIZE
+        }
+        for key, value in default_values.items():
+            setattr(self, key, value)
+
 class Event:
-    def __init__(self, event_values):
+    def __init__(self, event_values, defaults=EventDefaults()):
         for key in event_values.keys():
             if key not in ALL_EVENT_PARAMETERS:
                 raise ValueError("Invalid key for event: %s" % (key))
 
-        event_values.setdefault(EVENT_ACTIVE, True)
-        event_values.setdefault(EVENT_CHANNEL, DEFAULT_EVENT_CHANNEL)
-        event_values.setdefault(EVENT_DURATION, DEFAULT_EVENT_DURATION)
-        event_values.setdefault(EVENT_GATE, DEFAULT_EVENT_GATE)
-        event_values.setdefault(EVENT_AMPLITUDE, DEFAULT_EVENT_AMPLITUDE)
-        event_values.setdefault(EVENT_OCTAVE, DEFAULT_EVENT_OCTAVE)
-        event_values.setdefault(EVENT_TRANSPOSE, DEFAULT_EVENT_TRANSPOSE)
-        event_values.setdefault(EVENT_SCALE, Scale.default)
+        if EVENT_DURATION_LEGACY in event_values:
+            event_values[EVENT_DURATION] = event_values[EVENT_DURATION_LEGACY]
+        if EVENT_AMPLITUDE_LEGACY in event_values:
+            event_values[EVENT_AMPLITUDE] = event_values[EVENT_AMPLITUDE_LEGACY]
+
+        for key, value in defaults.__dict__.items():
+            # Defaults can be patterns too
+            event_values.setdefault(key, Pattern.value(value))
 
         if EVENT_NOTE in event_values and EVENT_DEGREE in event_values:
             raise InvalidEventException("Cannot specify both note and degree")
 
         #------------------------------------------------------------------------
         # Note/degree/etc: Send a MIDI note
         #------------------------------------------------------------------------
         if EVENT_DEGREE in event_values:
             degree = event_values[EVENT_DEGREE]
             if degree is None:
                 event_values[EVENT_NOTE] = None
             else:
-                if EVENT_KEY in event_values:
-                    key = event_values[EVENT_KEY]
-                else:
-                    key = Key(0, event_values[EVENT_SCALE])
+                key = event_values[EVENT_KEY]
+                if isinstance(key, str):
+                    key = Key(key)
 
                 #----------------------------------------------------------------------
                 # handle lists of notes (eg chords).
                 # TODO: create a class which allows for scalars and arrays to handle
                 # addition transparently
                 #----------------------------------------------------------------------
                 try:
@@ -86,29 +101,59 @@
             self.type = EVENT_TYPE_ACTION
             self.action = event_values[EVENT_ACTION]
             self.args = {}
             if EVENT_ACTION_ARGS in event_values:
                 self.args = dict((key, Pattern.value(value)) for key, value in event_values[EVENT_ACTION_ARGS].items())
 
         elif EVENT_PATCH in event_values:
-            self.type = EVENT_TYPE_PATCH
+            #----------------------------------------------------------------------
+            # Patches support different event types:
+            #  - create from PatchSpec (EVENT_TYPE_PATCH_CREATE)
+            #  - trigger Patch (EVENT_TYPE_PATCH_TRIGGER)
+            #  - set Patch params (EVENT_TYPE_PATCH_SET)
+            #----------------------------------------------------------------------
             self.patch = event_values[EVENT_PATCH]
+            self.output = None
+
+            if EVENT_TYPE in event_values:
+                self.type = event_values[EVENT_TYPE]
+            else:
+                if type(self.patch).__name__ == "PatchSpec" or isinstance(self.patch, type):
+                    self.type = EVENT_TYPE_PATCH_CREATE
+                else:
+                    self.type = EVENT_TYPE_PATCH_SET
+
+            if EVENT_PATCH_OUTPUT in event_values:
+                self.output = event_values[EVENT_PATCH_OUTPUT]
+
             self.params = {}
             if EVENT_PATCH_PARAMS in event_values:
                 self.params = event_values[EVENT_PATCH_PARAMS]
 
+            if EVENT_NOTE in event_values:
+                self.note = event_values[EVENT_NOTE]
+
+            # TODO: Different kinds of event should really be different classes
+            self.trigger_name = None
+            self.trigger_value = None
+            if EVENT_TRIGGER_NAME in event_values:
+                self.trigger_name = event_values[EVENT_TRIGGER_NAME]
+            if EVENT_TRIGGER_VALUE in event_values:
+                self.trigger_value = event_values[EVENT_TRIGGER_VALUE]
+
         elif EVENT_CONTROL in event_values:
             self.type = EVENT_TYPE_CONTROL
             self.control = event_values[EVENT_CONTROL]
             self.value = event_values[EVENT_VALUE]
             self.channel = event_values[EVENT_CHANNEL]
 
         elif EVENT_PROGRAM_CHANGE in event_values:
-            # TODO: Implement program changes
             self.type = EVENT_TYPE_PROGRAM_CHANGE
+            self.program_change = event_values[EVENT_PROGRAM_CHANGE]
+            self.channel = event_values[EVENT_CHANNEL]
 
         elif EVENT_OSC_ADDRESS in event_values:
             self.type = EVENT_TYPE_OSC
             self.osc_address = event_values[EVENT_OSC_ADDRESS]
             self.osc_params = {}
             if EVENT_OSC_PARAMS in event_values:
                 if not isinstance(event_values[EVENT_OSC_PARAMS], Iterable):
@@ -120,22 +165,25 @@
             self.synth_name = event_values[EVENT_SUPERCOLLIDER_SYNTH]
             self.synth_params = {}
             if EVENT_SUPERCOLLIDER_SYNTH_PARAMS in event_values:
                 if not isinstance(event_values[EVENT_SUPERCOLLIDER_SYNTH_PARAMS], dict):
                     raise ValueError("SuperCollider params must be a dict")
                 self.synth_params = event_values[EVENT_SUPERCOLLIDER_SYNTH_PARAMS]
 
-        elif EVENT_NOTE in event_values or EVENT_DEGREE in event_values:
+        elif EVENT_NOTE in event_values:
             self.type = EVENT_TYPE_NOTE
             self.note = event_values[EVENT_NOTE]
             self.amplitude = event_values[EVENT_AMPLITUDE]
             self.gate = event_values[EVENT_GATE]
             self.channel = event_values[EVENT_CHANNEL]
 
         else:
             possible_event_types = [EVENT_NOTE, EVENT_DEGREE, EVENT_ACTION, EVENT_PATCH, EVENT_CONTROL,
                                     EVENT_PROGRAM_CHANGE, EVENT_OSC_ADDRESS]
             raise InvalidEventException("No event type specified (must provide one of %s)" % possible_event_types)
 
         self.duration = event_values[EVENT_DURATION]
         self.active = event_values[EVENT_ACTIVE]
         self.fields = event_values
+
+    def __str__(self):
+        return "Event (%s)" % self.fields
```

### Comparing `isobar-0.1.1/isobar/timeline/timeline.py` & `isobar-0.1.2/isobar/timeline/timeline.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import math
 import copy
 import threading
 
 from .track import Track
 from .clock import Clock
+from .event import EventDefaults
+from ..key import Key
 from ..io import MidiOutputDevice
 from ..constants import DEFAULT_TICKS_PER_BEAT, DEFAULT_TEMPO
 from ..constants import EVENT_TIME, EVENT_ACTION, INTERPOLATION_NONE
 from ..exceptions import TrackLimitReachedException, TrackNotFoundException
 from ..util import make_clock_multiplier
 import logging
 
@@ -46,14 +48,22 @@
         self.max_tracks = 0
         self.tracks = []
 
         self.thread = None
         self.stop_when_done = False
         self.events = []
         self.running = False
+        self.ignore_exceptions = False
+
+        self.defaults = EventDefaults()
+
+        #--------------------------------------------------------------------------------
+        # Optional callback to trigger each time an event is performed.
+        #--------------------------------------------------------------------------------
+        self.on_event_callback = None
 
     def get_clock_source(self):
         return self._clock_source
 
     def set_clock_source(self, clock_source):
         clock_source.clock_target = self
         self._clock_source = clock_source
@@ -99,19 +109,14 @@
 
     def seconds_to_beats(self, seconds):
         return seconds * self.tempo / 60.0
 
     def beats_to_seconds(self, beats):
         return beats * 60.0 / self.tempo
 
-    def unschedule(self, track):
-        if track not in self.tracks:
-            raise TrackNotFoundException("Track is not currently scheduled")
-        self.tracks.remove(track)
-
     def tick(self):
         """
         Called once every tick to trigger new events.
 
         Raises:
             StopIteration: If `stop_when_done` is true and no more events are scheduled.
         """
@@ -142,15 +147,21 @@
                 event[EVENT_ACTION]()
                 self.events.remove(event)
 
         #--------------------------------------------------------------------------------
         # Copy self.tracks because removing from it whilst using it = bad idea
         #--------------------------------------------------------------------------------
         for track in self.tracks[:]:
-            track.tick()
+            try:
+                track.tick()
+            except Exception as e:
+                if self.ignore_exceptions:
+                    print("*** Exception in track: %s" % e)
+                else:
+                    raise
             if track.is_finished and track.remove_when_done:
                 self.tracks.remove(track)
                 log.info("Timeline: Track finished, removing from scheduler (total tracks: %d)" % len(self.tracks))
 
         #--------------------------------------------------------------------------------
         # If we've run out of notes, raise a StopIteration.
         #--------------------------------------------------------------------------------
@@ -205,23 +216,20 @@
 
     def background(self):
         """ Run this Timeline in a background thread. """
         self.thread = threading.Thread(target=self.run)
         self.thread.setDaemon(True)
         self.thread.start()
 
-    def run(self, stop_when_done=None, background=False):
+    def run(self, stop_when_done=None):
         """ Run this Timeline in the foreground.
 
         If stop_when_done is set, returns when no tracks are currently
         scheduled; otherwise, keeps running indefinitely. """
 
-        if stop_when_done and background:
-            raise Exception("Can't select both stop_when_done and background")
-
         self.start()
 
         if stop_when_done is not None:
             self.stop_when_done = stop_when_done
 
         try:
             #--------------------------------------------------------------------------------
@@ -238,15 +246,16 @@
             # This will be hit if every Pattern in a timeline is exhausted.
             #--------------------------------------------------------------------------------
             log.info("Timeline: Finished")
             self.running = False
 
         except Exception as e:
             print((" *** Exception in Timeline thread: %s" % e))
-            raise e
+            if not self.ignore_exceptions:
+                raise e
 
     def start(self):
         log.info("Timeline: Starting")
 
     def stop(self):
         log.info("Timeline: Stopping")
         for device in self.output_devices:
@@ -277,72 +286,101 @@
     def add_output_device(self, output_device):
         """ Append a new output device to our output list. """
         self.output_devices.append(output_device)
         self.clock_multipliers[output_device] = make_clock_multiplier(output_device.ticks_per_beat, self.ticks_per_beat)
 
     def schedule(self,
                  params=None,
-                 quantize=0,
+                 quantize=None,
                  delay=0,
                  count=None,
                  interpolate=INTERPOLATION_NONE,
                  output_device=None,
-                 remove_when_done=True):
+                 remove_when_done=True,
+                 name=None,
+                 replace=False):
         """
         Schedule a new track within this Timeline.
 
         Args:
             params (dict):           Event dictionary. Keys are generally EVENT_* values, defined in constants.py.
                                      If params is None, a new empty Track will be scheduled and returned.
-                                     This can be updated with Track.update() to begin generating events.
+                                     This can be updated with Track.update().
+                                     params can alternatively be a Pattern that generates a dict output.
+            name (str):              Optional name for the track.
             quantize (float):        Quantize level, in beats. For example, 1.0 will begin executing the
                                      events on the next whole beats.
             delay (float):           Delay time, in beats, before events should be executed.
                                      If `quantize` and `delay` are both specified, quantization is applied,
                                      and the event is scheduled `delay` beats after the quantization time.
             count (int):             Number of events to process, or unlimited if not specified.
             interpolate (int):       Interpolation mode for control segments.
             output_device:           Output device to send events to. Uses the Timeline default if not specified.
             remove_when_done (bool): If True, removes the Track from the Timeline when it is finished.
                                      Otherwise, retains the Track, so update() can later be called to schedule
                                      additional events on it.
+            name (str):              Optional name to identify the Track. If given, can be used to update the track's
+                                     parameters in future calls to schedule() by specifying replace=True.
+            replace (bool):          Must be used in conjunction with the `name` parameter. Instead of scheduling a
+                                     new Track, this updates the parameters of an existing track with the same name.
 
         Returns:
             The new `Track` object.
 
         Raises:
             TrackLimitReachedException: If `max_tracks` has been reached.
         """
 
-        #--------------------------------------------------------------------------------
-        # Take a copy of params to avoid modifying the original
-        #--------------------------------------------------------------------------------
-        params = copy.copy(params)
-
         if not output_device:
             #--------------------------------------------------------------------------------
             # If no output device exists, send to the system default MIDI output.
             #--------------------------------------------------------------------------------
             if not self.output_devices:
                 self.add_output_device(MidiOutputDevice())
             output_device = self.output_devices[0]
 
+        #--------------------------------------------------------------------------------
+        # If replace=True is specified, updated the params of any existing track
+        # with the same name. If none exists, proceed to create it as usual.
+        #--------------------------------------------------------------------------------
+        if replace:
+            if name is None:
+                raise ValueError("Must specify a track name if `replace` is specified")
+            for existing_track in self.tracks:
+                if existing_track.name == name:
+                    existing_track.update(params, quantize=quantize)
+                    return
+
         if self.max_tracks and len(self.tracks) >= self.max_tracks:
             raise TrackLimitReachedException("Timeline: Refusing to schedule track (hit limit of %d)" % self.max_tracks)
 
         def start_track(track):
             #--------------------------------------------------------------------------------
             # Add a new track.
             #--------------------------------------------------------------------------------
             self.tracks.append(track)
             log.info("Timeline: Scheduled new track (total tracks: %d)" % len(self.tracks))
 
-        track = Track(self, params, max_event_count=count, interpolate=interpolate,
-                      output_device=output_device, remove_when_done=remove_when_done)
+        if isinstance(params, Track):
+            track = params
+            track.reset()
+        else:
+            #--------------------------------------------------------------------------------
+            # Take a copy of params to avoid modifying the original
+            #--------------------------------------------------------------------------------
+            track = Track(self,
+                          copy.copy(params),
+                          max_event_count=count,
+                          interpolate=interpolate,
+                          output_device=output_device,
+                          remove_when_done=remove_when_done,
+                          name=name)
 
+        if quantize is None:
+            quantize = self.defaults.quantize
         if quantize or delay:
             #--------------------------------------------------------------------------------
             # We don't want to begin events right away -- either wait till
             # the next beat boundary (quantize), or delay a number of beats.
             #--------------------------------------------------------------------------------
             scheduled_time = self.current_time
             if quantize:
@@ -361,7 +399,46 @@
 
         return track
 
     #--------------------------------------------------------------------------------
     # Backwards-compatibility
     #--------------------------------------------------------------------------------
     sched = schedule
+
+    def unschedule(self, track):
+        """
+        Remove a track from playback.
+
+        Args:
+            track: The Track object.
+            
+        Raises:
+            TrackNotFoundException: If the track is not playing.
+        """
+        if track not in self.tracks:
+            raise TrackNotFoundException("Track is not currently scheduled")
+        self.tracks.remove(track)
+
+    def get_track(self, track_id):
+        """
+        Get the Track corresponding to the given track_id.
+        track_id can be a numeric index, or the name corresponding to a track.
+
+        Args:
+            track_id: An index or name
+
+        Returns:
+            The Track object, or None if not found.
+        """
+        if isinstance(track_id, int):
+            return self.tracks[track_id]
+        elif isinstance(track_id, str):
+            for track in self.tracks:
+                if track.name == track_id:
+                    return track
+            return None
+        else:
+            raise TypeError("Invalid type for track_id (must be an int or str)")
+
+    def clear(self):
+        for track in self.tracks[:]:
+            self.unschedule(track)
```

### Comparing `isobar-0.1.1/isobar/timeline/track.py` & `isobar-0.1.2/isobar/timeline/track.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,61 +2,95 @@
 import math
 import inspect
 
 from .event import Event
 from ..pattern import Pattern, PSequence, PDict, PInterpolate
 from ..constants import *
 from ..exceptions import InvalidEventException
+from ..util import midi_note_to_frequency
 import logging
 
 log = logging.getLogger(__name__)
 
 class Track:
     def __init__(self, timeline, events, max_event_count=None, interpolate=INTERPOLATION_NONE,
-                 output_device=None, remove_when_done=True):
+                 output_device=None, remove_when_done=True, name=None):
         #--------------------------------------------------------------------------------
         # Ensure that events is a pattern that generates a dict when it is iterated.
         #--------------------------------------------------------------------------------
+        self.event_stream = {}
+        self.timeline = timeline
         self.current_time = 0
         self.next_event_time = 0
         self.max_event_count = max_event_count
         self.current_event_count = 0
+        self.name = name
 
         self.update(events)
         self.current_event = None
         self.next_event = None
         self.interpolating_event = PSequence([], 0)
 
-        self.timeline = timeline
         self.output_device = output_device
         self.interpolate = interpolate
 
         self.note_offs = []
         self.is_finished = False
         self.remove_when_done = remove_when_done
 
+    def __getattr__(self, item):
+        return self.event_stream[item]
+
+    def __setattr__(self, item, value):
+        #--------------------------------------------------------------------------------
+        # Benign magic so that you can do things like
+        #
+        #    track.note = 64
+        #
+        # Note that this will only work when the track has been created with a dict
+        # of key-value pairs (rather than a pattern that will itself generate dicts.)
+        #--------------------------------------------------------------------------------
+        if item != "event_stream" and isinstance(self.event_stream, PDict) and item in ALL_EVENT_PARAMETERS:
+            self.event_stream[item] = value
+        else:
+            super().__setattr__(item, value)
+
+    def __delattr__(self, item):
+        if item != "event_stream" and isinstance(self.event_stream, PDict) and item in ALL_EVENT_PARAMETERS:
+            del self.event_stream[item]
+        else:
+            super().__delattr__(item)
+
     def update(self, events, quantize=None):
         """
         Update the events that this Track produces.
 
         Args:
             events: A dict, a PDict, or a Pattern that generates dicts.
         """
+        if events is None:
+            events = {}
         if isinstance(events, dict):
             events = PDict(events)
 
+        if quantize is None:
+            quantize = self.timeline.defaults.quantize
+
         if quantize:
             self.next_event_time = quantize * math.ceil(float(self.current_time) / quantize)
         else:
             self.next_event_time = self.current_time
 
         self.event_stream = events
 
     def __str__(self):
-        return "Track (pos = %d)" % self.current_time
+        if self.name:
+            return "Track: %s (pos = %d)" % (self.name, self.current_time)
+        else:
+            return "Track (pos = %d)" % self.current_time
 
     @property
     def tick_duration(self):
         return self.timeline.tick_duration
 
     def tick(self):
         """
@@ -98,15 +132,15 @@
                 # Track has interpolation enabled.
                 # Interpolation is done by wrapping the evolving event in an
                 # interpolating_event, which generates a new value each tick until it is
                 # exhausted.
                 #--------------------------------------------------------------------------------
                 try:
                     interpolated_values = next(self.interpolating_event)
-                    interpolated_event = Event(interpolated_values)
+                    interpolated_event = Event(interpolated_values, self.timeline.defaults)
                     self.perform_event(interpolated_event)
                 except StopIteration:
                     is_first_event = False
                     if self.next_event is None:
                         #--------------------------------------------------------------------------------
                         # The current and next events are needed to perform interpolation.
                         # No events have yet been obtained, so query the current and next events off
@@ -145,15 +179,15 @@
                                                                                   self.next_event.fields[key]], 1),
                                                                        duration_ticks,
                                                                        self.interpolate)
 
                     self.interpolating_event = PDict(interpolating_event_fields)
                     if not is_first_event:
                         next(self.interpolating_event)
-                    event = Event(next(self.interpolating_event))
+                    event = Event(next(self.interpolating_event), self.timeline.defaults)
                     self.perform_event(event)
 
         except StopIteration:
             if len(self.note_offs) == 0:
                 self.is_finished = True
 
         self.current_time += self.tick_duration
@@ -163,15 +197,19 @@
 
     def reset(self):
         self.current_time = 0
         self.next_event_duration = 0
         self.next_event_time = 0
 
         for pattern in self.event_stream.values():
-            pattern.reset()
+            try:
+                pattern.reset()
+            except AttributeError:
+                # Event stream may contain constant values, in which case no reset is needed.
+                pass
 
     def get_next_event(self):
         """
         Retrieve the next event from the event stream dict.
 
         Returns:
             The next Event object
@@ -193,33 +231,41 @@
         #  - If self.events is a pattern which returns a dict, the next value
         #    is iterated.
         # Take a copy to avoid modifying the original.
         #------------------------------------------------------------------------
         event_values = next(self.event_stream)
         event_values = copy.copy(event_values)
 
-        event = Event(event_values)
+        event = Event(event_values, self.timeline.defaults)
         self.current_event_count += 1
 
         return event
 
     def perform_event(self, event):
         if not event.active:
             return
 
         #------------------------------------------------------------------------
         # Action: Carry out an action each time this event is triggered
         #------------------------------------------------------------------------
         if event.type == EVENT_TYPE_ACTION:
             try:
                 fn = event.action
-                fn_params = inspect.signature(fn).parameters
-                for key in event.args.keys():
-                    if key not in fn_params:
-                        raise Exception("Named argument not found in callback args: %s" % key)
+                try:
+                    fn_params = inspect.signature(fn).parameters
+                    for key in event.args.keys():
+                        if key not in fn_params:
+                            raise Exception("Named argument not found in callback args: %s" % key)
+                except ValueError:
+                    #------------------------------------------------------------------------
+                    # inspect.signature does not work on cython/pybind11 bindings, and
+                    # raises a ValueError. In these cases, simply pass the arguments
+                    # without validation.
+                    #------------------------------------------------------------------------
+                    pass
                 event.action(**event.args)
             except StopIteration:
                 raise StopIteration()
             except Exception as e:
                 print(("Exception when handling scheduled action: %s" % e))
                 import traceback
                 traceback.print_exc()
@@ -250,22 +296,53 @@
         #------------------------------------------------------------------------
         # SuperCollider synth
         #------------------------------------------------------------------------
         elif event.type == EVENT_TYPE_SUPERCOLLIDER:
             self.output_device.create(event.synth_name, event.synth_params)
 
         #------------------------------------------------------------------------
-        # Signalflow patch
+        # SignalFlow patch
         #------------------------------------------------------------------------
-        elif event.type == EVENT_TYPE_PATCH:
+        elif event.type == EVENT_TYPE_PATCH_CREATE:
+            #------------------------------------------------------------------------
+            # Action: Create patch
+            #------------------------------------------------------------------------
             if not hasattr(self.output_device, "create"):
                 raise InvalidEventException("Device %s does not support this kind of event" % self.output_device)
-            params = event.params
-            params = dict((key, Pattern.value(value)) for key, value in params.items())
-            self.output_device.create(event.patch, params)
+            params = dict((key, Pattern.value(value)) for key, value in event.params.items())
+            if hasattr(event, "note"):
+                notes = event.note if hasattr(event.note, '__iter__') else [event.note]
+
+                for note in notes:
+                    if note > 0:
+                        # TODO: Should use None to denote rests
+                        params["frequency"] = midi_note_to_frequency(note)
+                        self.output_device.create(event.patch, params, output=event.output)
+            else:
+                self.output_device.create(event.patch, params, output=event.output)
+
+        elif event.type == EVENT_TYPE_PATCH_SET or event.type == EVENT_TYPE_PATCH_TRIGGER:
+            #------------------------------------------------------------------------
+            # Action: Set patch's input(s) and/or trigger an event
+            #------------------------------------------------------------------------
+            for key, value in event.params.items():
+                value = Pattern.value(value)
+                event.patch.set_input(key, value)
+
+            if hasattr(event, "note"):
+                event.patch.set_input("frequency", midi_note_to_frequency(event.note))
+
+            if event.type == EVENT_TYPE_PATCH_TRIGGER:
+                #------------------------------------------------------------------------
+                # Action: Trigger a patch
+                #------------------------------------------------------------------------
+                if not hasattr(self.output_device, "trigger"):
+                    raise InvalidEventException("Device %s does not support this kind of event" % self.output_device)
+                params = dict((key, Pattern.value(value)) for key, value in event.params.items())
+                self.output_device.trigger(event.patch, event.trigger_name, event.trigger_value)
 
         #------------------------------------------------------------------------
         # Note: Classic MIDI note
         #------------------------------------------------------------------------
         elif event.type == EVENT_TYPE_NOTE:
             #----------------------------------------------------------------------
             # event: Certain devices (eg Socket IO) handle generic events,
@@ -317,9 +394,15 @@
                         self.output_device.note_on(note, amp, channel)
 
                         note_dur = event.duration * gate
                         self.schedule_note_off(self.current_time + note_dur, note, channel)
         else:
             raise InvalidEventException("Invalid event type: %s" % event.type)
 
+        if self.timeline.on_event_callback:
+            self.timeline.on_event_callback(self, event)
+
     def schedule_note_off(self, time, note, channel):
         self.note_offs.append([time, note, channel])
+
+    def stop(self):
+        self.timeline.unschedule(self)
```

### Comparing `isobar-0.1.1/isobar/util.py` & `isobar-0.1.2/isobar/util.py`

 * *Files 22% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     if name[-1].isdigit():
         octave = int(name[-1])
         name = name[:-1]
     else:
         octave = 0
 
     try:
+        # TODO: Fix such that note names can be lowercase (must also work with e.g. Bb)
         index = note_names.index([nameset for nameset in note_names if name in nameset][0])
     except IndexError:
         raise UnknownNoteName("Unknown note name: %s" % name)
 
     return octave * 12 + index
 
 def midi_note_to_note_name(note):
@@ -84,14 +85,42 @@
 
 def midi_note_to_frequency(note):
     """ Maps a MIDI note index to a frequency. """
     if note is None:
         return None
     return 440.0 * pow(2, (note - 69.0) / 12)
 
+def midi_note_to_frequency_just_intonation(note):
+    note_ratios = [1/1, 256/243, 9/8, 32/27, 81/64, 4/3, 729/512, 3/2, 128/81, 27/16, 16/9, 243/128]
+    octave = note // 12
+    octave_note = note % 12
+    octave_base_frequency = midi_note_to_frequency(octave * 12)
+    octave_note_frequency = octave_base_frequency * note_ratios[octave_note]
+    return octave_note_frequency
+
+def midi_semitones_to_frequency_ratio(semitones):
+    return pow(2, semitones / 12.0)
+
+def note_name_to_frequency(note_name):
+    return midi_note_to_frequency(note_name_to_midi_note(note_name))
+
+def frequency_ratio_to_midi_semitones(frequency_ratio):
+    return int(round(math.log2(frequency_ratio) * 12))
+
+def scale_lin_exp(value, from_min=0, from_max=1, to_min=1, to_max=10):
+    if value < from_min:
+        return to_min
+    if value > from_max:
+        return to_max
+    return ((to_max / to_min) ** ((value - from_min) / (from_max - from_min))) * to_min
+
+def scale_lin_lin(value, from_min=0, from_max=1, to_min=0, to_max=1):
+    norm = float(value - from_min) / (from_max - from_min)
+    return norm * float(to_max - to_min) + to_min
+
 def bipolar_diverge(maximum):
     """ Returns [0, 1, -1, ...., maximum, -maximum ] """
     sequence = list(sum(list(zip(list(range(maximum + 1)), list(range(0, -maximum - 1, -1)))), ()))
     sequence.pop(0)
     return sequence
 
 def filter_tone_row(source, target, bend_limit=7):
@@ -106,15 +135,15 @@
 def random_seed(seed):
     random.seed(seed)
 
 def make_clock_multiplier(output_clock_rate, input_clock_rate):
     multiple = 1.0
     if output_clock_rate and input_clock_rate:
         multiple = output_clock_rate / input_clock_rate
-    if (multiple > 1 and int(multiple) != multiple) or (multiple < 1 and 1/multiple != int(1/multiple)):
+    if (multiple > 1 and int(multiple) != multiple) or (multiple < 1 and 1 / multiple != int(1 / multiple)):
         raise ClockException("Cannot sync output device (clock rates must integer multiples of each other)")
 
     pos = 1
     while True:
         rv = 0
         pos += multiple
         while round(pos, 8) > 1:
```

### Comparing `isobar-0.1.1/isobar.egg-info/PKG-INFO` & `isobar-0.1.2/isobar.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,213 +1,219 @@
 Metadata-Version: 2.1
 Name: isobar
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library to express and manipulate musical patterns
 Home-page: https://github.com/ideoforms/isobar
 Author: Daniel Jones
 Author-email: dan-isobar@erase.net
 License: UNKNOWN
-Description: # isobar
-        
-        ![ci](https://github.com/ideoforms/isobar/workflows/ci/badge.svg)
-        
-        isobar is a Python library for creating and manipulating musical patterns, designed for use in algorithmic composition, generative music and sonification. It makes it quick and easy to express complex musical ideas, and can send and receive events from various different sources including MIDI, MIDI files, and OSC.
-        
-        The core element is a Timeline, which can control its own tempo or sync to an external clock. Onto this, you can schedule Patterns, which can be note sequences, control events, program changes, or other arbitrary events via lambda functions. Pattern are used as templates to generate Events, which trigger notes or control changes on an OutputDevice (Check out a [diagrammatic overview](http://ideoforms.github.io/isobar/#flow-diagram).)
-        
-        isobar includes a large array of basic compositional building blocks (see [Pattern Classes](#pattern-classes)), plus some advanced pattern generators for more sophisticated operations (arpeggiators, Euclidean rhythms, L-systems, Markov chains).
-        
-        ## Usage
-        
-        ```python
-        import isobar as iso
-        
-        #------------------------------------------------------------------------
-        # Create a geometric series on a minor scale.
-        # PingPong plays the series forward then backward. PLoop loops forever.
-        #------------------------------------------------------------------------
-        arpeggio = iso.PSeries(0, 2, 6)
-        arpeggio = iso.PDegree(arpeggio, iso.Scale.minor) + 72
-        arpeggio = iso.PPingPong(arpeggio)
-        arpeggio = iso.PLoop(arpeggio)
-        
-        #------------------------------------------------------------------------
-        # Create a velocity sequence, with emphasis every 4th note,
-        # plus a random walk to create gradual dynamic changes.
-        # Amplitudes are in the MIDI velocity range (0..127).
-        #------------------------------------------------------------------------
-        amplitude = iso.PSequence([50, 35, 25, 35]) + iso.PBrown(0, 1, -20, 20)
-        
-        #------------------------------------------------------------------------
-        # A Timeline schedules events at a specified tempo. By default, events
-        # are send to the system's default MIDI output.
-        #------------------------------------------------------------------------
-        timeline = iso.Timeline(120)
-        
-        #------------------------------------------------------------------------
-        # Schedule events, with properties generated by the Pattern objects.
-        #------------------------------------------------------------------------
-        timeline.schedule({
-            "note": arpeggio,
-            "duration": 0.25,
-            "amplitude": amplitude
-        })
-        
-        #------------------------------------------------------------------------
-        # Run the timeline.
-        # Call timeline.background() to run in a separate thread.
-        #------------------------------------------------------------------------
-        timeline.run()
-        ```
-        
-        ## Installation
-        
-        The short answer: `pip3 install isobar`
-        
-        The long answer: [isobar Getting Started guide](http://ideoforms.github.io/isobar/getting-started/)
-        
-        ## Documentation
-        
-        For complete documentation, see [ideoforms.github.io/isobar](http://ideoforms.github.io/isobar/).
-        
-        ## Examples
-        
-        Examples are available in the [examples](examples) directory with this
-        distribution:
-        
-        * [00.ex-hello-world.py](examples/00.ex-hello-world.py)
-        * [01.ex-basics.py](examples/01.ex-basics.py)
-        * [02.ex-subsequence.py](examples/02.ex-subsequence.py)
-        * [03.ex-euclidean.py](examples/03.ex-euclidean.py)
-        * [04.ex-permutations.py](examples/04.ex-permutations.py)
-        * [05.ex-piano-phase.py](examples/05.ex-piano-phase.py)
-        * [06.ex-walk.py](examples/06.ex-walk.py)
-        * [07.ex-static-pattern.py](examples/07.ex-static-pattern.py)
-        * [10.ex-lsystem-stochastic.py](examples/10.ex-lsystem-stochastic.py)
-        * [11.ex-lsystem-rhythm.py](examples/11.ex-lsystem-rhythm.py)
-        * [12.ex-lsystem-grapher.py](examples/12.ex-lsystem-grapher.py)
-        * [20.ex-midi-input.py](examples/20.ex-midi-input.py)
-        * [21.ex-midi-clock-sync-in.py](examples/21.ex-midi-clock-sync-in.py)
-        * [22.ex-midi-markov-learner.py](examples/22.ex-midi-markov-learner.py)
-        * [23.ex-midi-monitor.py](examples/23.ex-midi-monitor.py)
-        * [30.ex-midifile-read.py](examples/30.ex-midifile-read.py)
-        * [31.ex-midifile-write.py](examples/31.ex-midifile-write.py)
-        * [32.ex-midifile-markov.py](examples/32.ex-midifile-markov.py)
-        * [40.ex-osc-send.py](examples/40.ex-osc-send.py)
-        
-        ### Pattern classes
-        
-            CORE (core.py)
-            Pattern              - Abstract superclass of all pattern generators.
-            PConstant            - Returns a fixed value.
-            PRef                 - Contains a reference to another pattern, which can be replaced dynamically.
-            PFunc                - Returns the value generated by a function.
-            PArrayIndex          - Request a specified index from an array.
-            PDict                - Construct a pattern from a dict of arrays, or an array of dicts.
-            PDictKey             - Request a specified key from a dictionary.
-            PConcatenate         - Concatenate the output of multiple sequences.
-            PAbs                 - Absolute value of `input`
-            PInt                 - Integer value of `input`
-            PAdd                 - Add elements of two patterns (shorthand: patternA + patternB)
-            PSub                 - Subtract elements of two patterns (shorthand: patternA - patternB)
-            PMul                 - Multiply elements of two patterns (shorthand: patternA * patternB)
-            PDiv                 - Divide elements of two patterns (shorthand: patternA / patternB)
-            PFloorDiv            - Integer division (shorthand: patternA // patternB)
-            PMod                 - Modulo elements of two patterns (shorthand: patternA % patternB)
-            PPow                 - One pattern to the power of another (shorthand: patternA ** patternB)
-            PLShift              - Binary left-shift (shorthand: patternA << patternB)
-            PRShift              - Binary right-shift (shorthand: patternA << patternB)
-            PEqual               - Return 1 if a == b, 0 otherwise (shorthand: patternA == patternB)
-            PGreaterThanOrEqual  - Return 1 if a != b, 0 otherwise (shorthand: patternA != patternB)
-            PGreaterThan         - Return 1 if a > b, 0 otherwise (shorthand: patternA > patternB)
-            PGreaterThanOrEqual  - Return 1 if a >= b, 0 otherwise (shorthand: patternA >= patternB)
-            PLessThan            - Return 1 if a < b, 0 otherwise (shorthand: patternA < patternB)
-            PLessThanOrEqual     - Return 1 if a <= b, 0 otherwise (shorthand: patternA <= patternB)
-        
-            SCALAR (scalar.py)
-            PChanged             - Outputs a 1 if the value of a pattern has changed.
-            PDiff                - Outputs the difference between the current and previous values of an input pattern
-            PSkipIf              - If `skip` is false, returns `input`; otherwise, returns None.
-            PNormalise           - Adaptively normalise `input` to [0..1] over a linear scale.
-            PMap                 - Apply an arbitrary function to an input pattern.
-            PMapEnumerated       - Apply arbitrary function to input, passing a counter.
-            PLinLin              - Map `input` from linear range [a,b] to linear range [c,d].
-            PLinExp              - Map `input` from linear range [a,b] to exponential range [c,d].
-            PRound               - Round `input` to N decimal places.
-            PScalar              - Reduce tuples and lists into single scalar values,
-            PWrap                - Wrap input note values within <min>, <max>.
-            PIndexOf             - Find index of items from `pattern` in <list>
-        
-            SEQUENCE (sequence.py)
-            PSeries              - Arithmetic series, beginning at `start`, increment by `step`
-            PRange               - Similar to PSeries, but specify a max/step value.
-            PGeom                - Geometric series, beginning at `start`, multiplied by `step`
-            PImpulse             - Outputs a 1 every <period> events, otherwise 0.
-            PLoop                - Repeats a finite `pattern` for `n` repeats.
-            PPingPong            - Ping-pong input pattern back and forth N times.
-            PCreep               - Loop `length`-note segment, progressing `creep` notes after `repeats` repeats.
-            PStutter             - Play each note of `pattern` `count` times.
-            PSubsequence         - Returns a finite subsequence of an input pattern.
-            PReverse             - Reverses a finite sequence.
-            PReset               - Resets `pattern` whenever `trigger` is true
-            PCounter             - Increments a counter by 1 for each zero-crossing in `trigger`.
-            PCollapse            - Skip over any rests in `input`
-            PNoRepeats           - Skip over repeated values in `input`
-            PPad                 - Pad `pattern` with rests until it reaches length `length`.
-            PPadToMultiple       - Pad `pattern` with rests until its length is divisible by `multiple`.
-            PArpeggiator         - Arpeggiator.
-            PEuclidean           - Generate Euclidean rhythms.
-            PPermut              - Generate every permutation of `count` input items.
-            PPatternGeneratorAction - Each time its pattern is exhausted, request a new pattern by calling <fn>.
-            PSequenceAction      - Iterate over an array, perform a function, and repeat.
-        
-            CHANCE (chance.py)
-            PWhite               - White noise between `min` and `max`.
-            PBrown               - Brownian noise.
-            PWalk                - Random walk around list.
-            PChoice              - Pick a random element from `values`, weighted by optional `weights`.
-            PSample              - Pick multiple random elements from `values`, weighted by optional `weights`,
-            PShuffle             - Shuffled list.
-            PShuffleInput        - Every `n` steps, take `n` values from `pattern` and reorder.
-            PSkip                - Skip events with some probability, 1 - <play>.
-            PFlipFlop            - flip a binary bit with some probability.
-            PSwitchOne           - Capture `length` input values; loop, repeatedly switching two adjacent values.
-        
-            TONAL (tonal.py)
-            PDegree              - Map scale index <degree> to MIDI notes in <scale>.
-            PFilterByKey         - Filter notes based on their presence in <key>.
-            PNearestNoteInKey    - Return the nearest note in <key>.
-            PMidiNoteToFrequency - Map MIDI note to frequency value.
-        
-            STATIC (static.py)
-            PGlobals             - Static global value identified by a string.
-            PCurrentTime         - Returns the position (in beats) of the current timeline.
-        
-            FADE (fade.py)
-            PFadeNotewise        - Fade a pattern in/out by introducing notes at a gradual rate.
-            PFadeNotewiseRandom  - Fade a pattern in/out by gradually introducing random notes.
-        
-            MARKOV (markov.py)
-            PMarkov              - First-order Markov chain generator.
-        
-            LSYSTEM (lsystem.py)
-            PLSystem             - integer sequence derived from Lindenmayer systems
-        
-            WARP (warp.py)
-            PWInterpolate        - Requests a new target warp value from `pattern` every `length` beats
-            PWSine               - Sinosoidal warp, period `length` beats, amplitude +/-<amp>.
-            PWRallantando        - Exponential deceleration to <amp> times the current tempo over `length` beats.
-        
-        ## Background
-        
-        isobar was first designed for the generative sound installation [Variable 4](http://www.variable4.org.uk), in which it was used to generate musical structures in response to changing weather conditions. It was more recently used in [The Listening Machine](http://www.thelisteningmachine.org/), taking live input from Twitter and generating musical output from language patterns, streamed live over the internet.
-        
-        Many of the concepts behind Pattern and its subclasses are inspired by the brilliant pattern library of the [SuperCollider](http://supercollider.sf.net) synthesis language.
-        
-        
 Keywords: sound,music,composition
 Platform: UNKNOWN
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Artistic Software
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# isobar
+
+![ci](https://github.com/ideoforms/isobar/workflows/ci/badge.svg) [![stability-mature](https://img.shields.io/badge/stability-mature-008000.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#mature)
+
+isobar is a Python library for creating and manipulating musical patterns, designed for use in algorithmic composition, generative music and sonification. It makes it quick and easy to express complex musical ideas, and can send and receive events from various different sources including MIDI, MIDI files, and OSC.
+
+The core element is a Timeline, which can control its own tempo or sync to an external clock. Onto this, you can schedule Patterns, which can be note sequences, control events, program changes, or other arbitrary events via lambda functions. Pattern are used as templates to generate Events, which trigger notes or control changes on an OutputDevice (Check out a [diagrammatic overview](http://ideoforms.github.io/isobar/#flow-diagram).)
+
+isobar includes a large array of basic compositional building blocks (see [Pattern Classes](#pattern-classes)), plus some advanced pattern generators for more sophisticated operations (arpeggiators, Euclidean rhythms, L-systems, Markov chains).
+
+## Usage
+
+```python
+import isobar as iso
+
+#------------------------------------------------------------------------
+# Create a geometric series on a minor scale.
+# PingPong plays the series forward then backward. PLoop loops forever.
+#------------------------------------------------------------------------
+arpeggio = iso.PSeries(0, 2, 6)
+arpeggio = iso.PDegree(arpeggio, iso.Scale.minor) + 72
+arpeggio = iso.PPingPong(arpeggio)
+arpeggio = iso.PLoop(arpeggio)
+
+#------------------------------------------------------------------------
+# Create a velocity sequence, with emphasis every 4th note,
+# plus a random walk to create gradual dynamic changes.
+# Amplitudes are in the MIDI velocity range (0..127).
+#------------------------------------------------------------------------
+amplitude = iso.PSequence([50, 35, 25, 35]) + iso.PBrown(0, 1, -20, 20)
+
+#------------------------------------------------------------------------
+# A Timeline schedules events at a specified tempo. By default, events
+# are send to the system's default MIDI output.
+#------------------------------------------------------------------------
+timeline = iso.Timeline(120)
+
+#------------------------------------------------------------------------
+# Schedule events, with properties generated by the Pattern objects.
+#------------------------------------------------------------------------
+timeline.schedule({
+    "note": arpeggio,
+    "duration": 0.25,
+    "amplitude": amplitude
+})
+
+#------------------------------------------------------------------------
+# Run the timeline.
+# Call timeline.background() to run in a separate thread.
+#------------------------------------------------------------------------
+timeline.run()
+```
+
+## Installation
+
+The short answer: `pip3 install isobar`
+
+The long answer: [isobar Getting Started guide](http://ideoforms.github.io/isobar/getting-started/)
+
+## Documentation
+
+For complete documentation, see [ideoforms.github.io/isobar](http://ideoforms.github.io/isobar/).
+
+## Examples
+
+Examples are available in the [examples](examples) directory with this
+distribution:
+
+* [00.ex-hello-world.py](examples/00.ex-hello-world.py)
+* [01.ex-basics.py](examples/01.ex-basics.py)
+* [02.ex-subsequence.py](examples/02.ex-subsequence.py)
+* [03.ex-euclidean.py](examples/03.ex-euclidean.py)
+* [04.ex-permutations.py](examples/04.ex-permutations.py)
+* [05.ex-piano-phase.py](examples/05.ex-piano-phase.py)
+* [06.ex-walk.py](examples/06.ex-walk.py)
+* [07.ex-static-pattern.py](examples/07.ex-static-pattern.py)
+* [10.ex-lsystem-stochastic.py](examples/10.ex-lsystem-stochastic.py)
+* [11.ex-lsystem-rhythm.py](examples/11.ex-lsystem-rhythm.py)
+* [12.ex-lsystem-grapher.py](examples/12.ex-lsystem-grapher.py)
+* [20.ex-midi-input.py](examples/20.ex-midi-input.py)
+* [21.ex-midi-clock-sync-in.py](examples/21.ex-midi-clock-sync-in.py)
+* [22.ex-midi-markov-learner.py](examples/22.ex-midi-markov-learner.py)
+* [23.ex-midi-monitor.py](examples/23.ex-midi-monitor.py)
+* [30.ex-midifile-read.py](examples/30.ex-midifile-read.py)
+* [31.ex-midifile-write.py](examples/31.ex-midifile-write.py)
+* [32.ex-midifile-markov.py](examples/32.ex-midifile-markov.py)
+* [40.ex-osc-send.py](examples/40.ex-osc-send.py)
+
+### Pattern classes
+
+    CORE (core.py)
+    Pattern                  - Abstract superclass of all pattern generators.
+    PConstant                - Returns a fixed value.
+    PRef                     - Contains a reference to another pattern, which can be replaced dynamically.
+    PFunc                    - Returns the value generated by a function.
+    PArrayIndex              - Request a specified index from an array.
+    PDict                    - Construct a pattern from a dict of arrays, or an array of dicts.
+    PDictKey                 - Request a specified key from a dictionary.
+    PConcatenate             - Concatenate the output of multiple sequences.
+    PAbs                     - Absolute value of `input`
+    PInt                     - Integer value of `input`
+    PAdd                     - Add elements of two patterns (shorthand: patternA + patternB)
+    PSub                     - Subtract elements of two patterns (shorthand: patternA - patternB)
+    PMul                     - Multiply elements of two patterns (shorthand: patternA * patternB)
+    PDiv                     - Divide elements of two patterns (shorthand: patternA / patternB)
+    PFloorDiv                - Integer division (shorthand: patternA // patternB)
+    PMod                     - Modulo elements of two patterns (shorthand: patternA % patternB)
+    PPow                     - One pattern to the power of another (shorthand: patternA ** patternB)
+    PLShift                  - Binary left-shift (shorthand: patternA << patternB)
+    PRShift                  - Binary right-shift (shorthand: patternA << patternB)
+    PEqual                   - Return 1 if a == b, 0 otherwise (shorthand: patternA == patternB)
+    PGreaterThanOrEqual      - Return 1 if a != b, 0 otherwise (shorthand: patternA != patternB)
+    PGreaterThan             - Return 1 if a > b, 0 otherwise (shorthand: patternA > patternB)
+    PGreaterThanOrEqual      - Return 1 if a >= b, 0 otherwise (shorthand: patternA >= patternB)
+    PLessThan                - Return 1 if a < b, 0 otherwise (shorthand: patternA < patternB)
+    PLessThanOrEqual         - Return 1 if a <= b, 0 otherwise (shorthand: patternA <= patternB)
+
+    SCALAR (scalar.py)
+    PChanged                 - Outputs a 1 if the value of the input pattern has changed,
+    PDiff                    - Outputs the difference between the current and previous values of an input pattern
+    PSkipIf                  - If `skip` is false, returns `input`; otherwise, returns None.
+    PNormalise               - Adaptively normalise `input` to [0..1] over a linear scale.
+    PMap                     - Apply an arbitrary function to an input pattern.
+    PMapEnumerated           - Apply arbitrary function to input, passing a counter.
+    PScaleLinLin             - Map `input` from linear range [a,b] to linear range [c,d].
+    PScaleLinExp             - Map `input` from linear range [a,b] to exponential range [c,d].
+    PRound                   - Round `input` to N decimal places.
+    PScalar                  - Reduce tuples and lists into single scalar values,
+    PWrap                    - Wrap input note values within <min>, <max>.
+    PIndexOf                 - Find index of items from `pattern` in <list>
+
+    SEQUENCE (sequence.py)
+    PSeries                  - Arithmetic series, beginning at `start`, increment by `step`
+    PRange                   - Similar to PSeries, but specify a max/step value.
+    PGeom                    - Geometric series, beginning at `start`, multiplied by `step`
+    PImpulse                 - Outputs a 1 every <period> events, otherwise 0.
+    PLoop                    - Repeats a finite `pattern` for `n` repeats.
+    PPingPong                - Ping-pong input pattern back and forth N times.
+    PCreep                   - Loop `length`-note segment, progressing `creep` notes after `repeats` repeats.
+    PStutter                 - Play each note of `pattern` `count` times.
+    PSubsequence             - Returns a finite subsequence of an input pattern.
+    PReverse                 - Reverses a finite sequence.
+    PReset                   - Resets `pattern` whenever `trigger` is true
+    PCounter                 - Increments a counter by 1 for each zero-crossing in `trigger`.
+    PCollapse                - Skip over any rests in `input`
+    PNoRepeats               - Skip over repeated values in `input`
+    PPad                     - Pad `pattern` with rests until it reaches length `length`.
+    PPadToMultiple           - Pad `pattern` with rests until its length is divisible by `multiple`.
+    PArpeggiator             - Arpeggiator.
+    PEuclidean               - Generate Euclidean rhythms.
+    PPermut                  - Generate every permutation of `count` input items.
+    PPatternGeneratorAction  - Each time its pattern is exhausted, request a new pattern by calling <fn>.
+    PSequenceAction          - Iterate over an array, perform a function, and repeat.
+
+    CHANCE (chance.py)
+    PWhite                   - White noise between `min` and `max`.
+    PBrown                   - Brownian noise.
+    PCoin                    - Coin toss, returning either 0 or 1 given some `probability`.
+    PWalk                    - Random walk around list.
+    PChoice                  - Pick a random element from `values`, weighted by optional `weights`.
+    PSample                  - Pick multiple random elements from `values`, weighted by optional `weights`,
+    PShuffle                 - Shuffled list.
+    PShuffleInput            - Every `n` steps, take `n` values from `pattern` and reorder.
+    PSkip                    - Skip events with some probability, 1 - `play`.
+    PFlipFlop                - flip a binary bit with some probability.
+    PSwitchOne               - Capture `length` input values; loop, repeatedly switching two adjacent values.
+    PRandomExponential       - Random uniform on exponential curve between `min` and `max`,
+    PRandomImpulseSequence   - Random sequence of impulses with probability `probability`.
+
+    TONAL (tonal.py)
+    PDegree                  - Map scale index <degree> to MIDI notes in <scale>.
+    PFilterByKey             - Filter notes based on their presence in <key>.
+    PNearestNoteInKey        - Return the nearest note in <key>.
+    PMidiNoteToFrequency     - Map MIDI note to frequency value.
+
+    STATIC (static.py)
+    PGlobals                 - Static global value identified by a string.
+    PCurrentTime             - Returns the position (in beats) of the current timeline.
+
+    FADE (fade.py)
+    PFadeNotewise            - Fade a pattern in/out by introducing notes at a gradual rate.
+    PFadeNotewiseRandom      - Fade a pattern in/out by gradually introducing random notes.
+
+    MARKOV (markov.py)
+    PMarkov                  - First-order Markov chain generator.
+
+    LSYSTEM (lsystem.py)
+    PLSystem                 - integer sequence derived from Lindenmayer systems
+
+    WARP (warp.py)
+    PWInterpolate            - Requests a new target warp value from `pattern` every `length` beats
+    PWSine                   - Sinosoidal warp, period `length` beats, amplitude +/-<amp>.
+    PWRallantando            - Exponential deceleration to <amp> times the current tempo over `length` beats.
+
+## Background
+
+isobar was first designed for the generative sound installation [Variable 4](http://www.variable4.org.uk), in which it was used to generate musical structures in response to changing weather conditions. It was more recently used in [The Listening Machine](http://www.thelisteningmachine.org/), taking live input from Twitter and generating musical output from language patterns, streamed live over the internet.
+
+Many of the concepts behind Pattern and its subclasses are inspired by the brilliant pattern library of the [SuperCollider](http://supercollider.sf.net) synthesis language.
+
+
+
```

### Comparing `isobar-0.1.1/isobar.egg-info/SOURCES.txt` & `isobar-0.1.2/isobar.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 README.md
 setup.cfg
 setup.py
 isobar/__init__.py
 isobar/chord.py
 isobar/constants.py
 isobar/exceptions.py
@@ -13,22 +14,30 @@
 isobar.egg-info/SOURCES.txt
 isobar.egg-info/dependency_links.txt
 isobar.egg-info/requires.txt
 isobar.egg-info/top_level.txt
 isobar/io/__init__.py
 isobar/io/midinote.py
 isobar/io/output.py
+isobar/io/cv/__init__.py
+isobar/io/cv/output.py
 isobar/io/dummy/__init__.py
 isobar/io/dummy/output.py
 isobar/io/midi/__init__.py
 isobar/io/midi/input.py
 isobar/io/midi/output.py
 isobar/io/midifile/__init__.py
 isobar/io/midifile/input.py
 isobar/io/midifile/output.py
+isobar/io/netclock/__init__.py
+isobar/io/netclock/receiver.py
+isobar/io/netclock/sender.py
+isobar/io/netglobals/__init__.py
+isobar/io/netglobals/receiver.py
+isobar/io/netglobals/sender.py
 isobar/io/osc/__init__.py
 isobar/io/osc/output.py
 isobar/io/signalflow/__init__.py
 isobar/io/signalflow/output.py
 isobar/io/socketio/__init__.py
 isobar/io/socketio/output.py
 isobar/io/supercollider/__init__.py
@@ -43,14 +52,15 @@
 isobar/pattern/scalar.py
 isobar/pattern/sequence.py
 isobar/pattern/static.py
 isobar/pattern/tonal.py
 isobar/pattern/warp.py
 isobar/timeline/__init__.py
 isobar/timeline/clock.py
+isobar/timeline/clock.warp.py
 isobar/timeline/event.py
 isobar/timeline/timeline.py
 isobar/timeline/track.py
 tests/__init__.py
 tests/test_io_midi.py
 tests/test_io_midifile.py
 tests/test_key.py
```

### Comparing `isobar-0.1.1/setup.py` & `isobar-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
     name='isobar',
-    version='0.1.1',
+    version='0.1.2',
     description='A Python library to express and manipulate musical patterns',
     long_description = open("README.md", "r").read(),
     long_description_content_type = "text/markdown",
     author='Daniel Jones',
     author_email='dan-isobar@erase.net',
     url='https://github.com/ideoforms/isobar',
     packages=find_packages(),
```

### Comparing `isobar-0.1.1/tests/test_io_midi.py` & `isobar-0.1.2/tests/test_io_midi.py`

 * *Files identical despite different names*

### Comparing `isobar-0.1.1/tests/test_io_midifile.py` & `isobar-0.1.2/tests/test_io_midifile.py`

 * *Files identical despite different names*

### Comparing `isobar-0.1.1/tests/test_key.py` & `isobar-0.1.2/tests/test_key.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,19 +21,14 @@
     with pytest.raises(iso.UnknownNoteName):
         a = iso.Key("X", "major")
     with pytest.raises(iso.UnknownNoteName):
         a = iso.Key("H", "minor")
     with pytest.raises(iso.UnknownScaleName):
         a = iso.Key("C", "mundo")
 
-    with pytest.raises(iso.InvalidKeyException):
-        a = iso.Key(-1, "major")
-    with pytest.raises(iso.InvalidKeyException):
-        a = iso.Key(12, "minor")
-
 def test_key_get():
     a = iso.Key("C", "major")
     assert a.get(0) == a[0] == 0
     assert a.get(1) == a[1] == 2
     assert a.get(2) == a[2] == 4
     assert a.get(7) == a[7] == 12
     assert a.get(-1) == a[-1] == -1
```

### Comparing `isobar-0.1.1/tests/test_pattern.py` & `isobar-0.1.2/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `isobar-0.1.1/tests/test_pattern_chance.py` & `isobar-0.1.2/tests/test_pattern_chance.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,21 @@
     a = iso.PBrown(0.0, 1.0, -1.0, 1.0)
     a.seed(0)
     expected = [0.0, 0.6888437030500962, 1.0, 0.84114316166169, 0.3589766622476167, 0.38152610498483375, 0.19139437988566232, 0.7589915579552076, 0.36561701011306247, 0.3188109184177741]
     assert a.nextn(10) == expected
     a.reset()
     assert a.nextn(10) == expected
 
+def test_pcoin():
+    a = iso.PCoin(0.75)
+    a.seed(0)
+    assert a.nextn(16) == [0, 0, 1, 1, 1, 1, 0, 1, 1, 1, 0, 1, 1, 0, 1, 1]
+    a.seed(0)
+    assert a.nextn(16) == [0, 0, 1, 1, 1, 1, 0, 1, 1, 1, 0, 1, 1, 0, 1, 1]
+
 def test_pwalk():
     a = iso.PRandomWalk([0, 2, 4, 5, 12], min=iso.PConstant(1), max=iso.PConstant(2))
     expected = [4, 0, 5, 0, 4, 5, 2, 4, 12, 5, 12, 4, 2, 5, 12, 4, 0, 12, 2, 4]
     a.seed(0)
     assert a.nextn(20) == expected
     a.reset()
     assert a.nextn(20) == expected
```

### Comparing `isobar-0.1.1/tests/test_pattern_core.py` & `isobar-0.1.2/tests/test_pattern_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     assert list(b) == [1, 2, 3]
     assert list(a) == [{"a": 1}, {"a": 2}, {"a": 3}]
 
 def test_pdictkey():
     d1 = {"foo": "bar", "baz": "buzz"}
     d2 = {"foo": "boo", "baz": "bez"}
     a = iso.PSequence(["foo", "baz"], 1)
-    b = iso.PDictKey(a, iso.PSequence([d1, d2]))
+    b = iso.PDictKey(iso.PSequence([d1, d2]), a)
     assert list(b) == ["bar", "bez"]
 
 def test_pconcatenate():
     a = iso.PSequence([1, 2], 1)
     b = iso.PSequence([3, 4], 1)
     c = iso.PSequence([5], 1)
     d = iso.PConcatenate([a, b, c])
```

### Comparing `isobar-0.1.1/tests/test_pattern_operators.py` & `isobar-0.1.2/tests/test_pattern_operators.py`

 * *Files identical despite different names*

### Comparing `isobar-0.1.1/tests/test_pattern_scalar.py` & `isobar-0.1.2/tests/test_pattern_scalar.py`

 * *Files identical despite different names*

### Comparing `isobar-0.1.1/tests/test_pattern_sequence.py` & `isobar-0.1.2/tests/test_pattern_sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,17 +45,17 @@
 
 def test_pcreep():
     a = iso.PSequence([1, 2, 3, 4, 5], 1)
     b = iso.PCreep(a, 3, 1, 2)
     assert list(b) == [1, 2, 3, 1, 2, 3, 2, 3, 4, 2, 3, 4, 3, 4, 5, 3, 4, 5]
 
 def test_pstutter():
-    a = iso.PSequence([1, 2, 3], 1)
-    b = iso.PStutter(a, 3)
-    assert list(b) == [1, 1, 1, 2, 2, 2, 3, 3, 3]
+    a = iso.PSequence([1, 2, 3, 4], 1)
+    b = iso.PStutter(a, iso.PSequence([2, 3]))
+    assert b.nextn(16) == [1, 1, 2, 2, 2, 3, 3, 4, 4, 4]
 
 def test_psubsequence():
     a = iso.PSeries()
     b = iso.PSubsequence(a, 4, 4)
     assert list(b) == [4, 5, 6, 7]
 
 def test_pinterpolate():
```

### Comparing `isobar-0.1.1/tests/test_pattern_tonal.py` & `isobar-0.1.2/tests/test_pattern_tonal.py`

 * *Files identical despite different names*

### Comparing `isobar-0.1.1/tests/test_timeline.py` & `isobar-0.1.2/tests/test_timeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,14 +160,41 @@
         iso.EVENT_NOTE: iso.PSequence([1], 1)
     }, quantize=quantize)
     dummy_timeline.run()
     assert len(dummy_timeline.output_device.events) == 2
     assert dummy_timeline.output_device.events[0] == [0, "note_on", 1, 64, 0]
     assert dummy_timeline.output_device.events[1] == [pytest.approx(1.0, abs=dummy_timeline.tick_duration), "note_off", 1, 0]
 
+def test_timeline_schedule_default_quantize(dummy_timeline):
+    dummy_timeline.defaults.quantize = 1
+    dummy_timeline.stop_when_done = False
+    dummy_timeline.tick()
+    dummy_timeline.stop_when_done = True
+
+    dummy_timeline.schedule({
+        iso.EVENT_NOTE: iso.PSequence([1], 1)
+    })
+    dummy_timeline.run()
+    assert len(dummy_timeline.output_device.events) == 2
+    assert dummy_timeline.output_device.events[0] == [1, "note_on", 1, 64, 0]
+    assert dummy_timeline.output_device.events[1] == [pytest.approx(2, abs=dummy_timeline.tick_duration), "note_off", 1, 0]
+
+def test_timeline_schedule_default_quantize_override(dummy_timeline):
+    dummy_timeline.defaults.quantize = 1
+    dummy_timeline.stop_when_done = False
+    dummy_timeline.tick()
+    dummy_timeline.stop_when_done = True
+    dummy_timeline.schedule({
+        iso.EVENT_NOTE: iso.PSequence([1], 1)
+    }, quantize=0)
+    dummy_timeline.run()
+    assert len(dummy_timeline.output_device.events) == 2
+    assert dummy_timeline.output_device.events[0] == [pytest.approx(dummy_timeline.tick_duration, abs=dummy_timeline.tick_duration), "note_on", 1, 64, 0]
+    assert dummy_timeline.output_device.events[1] == [pytest.approx(1 + dummy_timeline.tick_duration, abs=dummy_timeline.tick_duration), "note_off", 1, 0]
+
 @pytest.mark.skip
 def test_timeline_schedule_time(dummy_timeline):
     dummy_timeline.schedule({
         iso.EVENT_NOTE: iso.PSequence([1], 1),
         iso.EVENT_DURATION: 1
     }, time=1.25)
     dummy_timeline.run()
@@ -225,15 +252,15 @@
     def set_executed():
         nonlocal executed
         executed += 1
     timeline.background()
     timeline.schedule({
         "action": set_executed,
         "duration": 0.05
-    }, delay=0.01)
+    }, delay=0.025)
     time.sleep(0.2)
     timeline.stop()
     assert executed == 4
 
 def test_timeline_running(dummy_timeline):
     # TODO
     pass
```

### Comparing `isobar-0.1.1/tests/test_timeline_clock.py` & `isobar-0.1.2/tests/test_timeline_clock.py`

 * *Files identical despite different names*

### Comparing `isobar-0.1.1/tests/test_timeline_event.py` & `isobar-0.1.2/tests/test_timeline_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,28 +58,14 @@
     assert dummy_timeline.output_device.events == [
         [0, 'note_on', 12, 64, 0], [1, 'note_off', 12, 0],
         [1, 'note_on', 19, 64, 0], [2, 'note_off', 19, 0],
         [2, 'note_on', 16, 64, 0], [3, 'note_off', 16, 0],
         [3, 'note_on', 22, 64, 0], [4, 'note_off', 22, 0]
     ]
 
-def test_event_scale(dummy_timeline):
-    dummy_timeline.schedule({
-        iso.EVENT_DEGREE: iso.PSequence([0, 1, 2, 3], 1),
-        iso.EVENT_SCALE: iso.PSequence([iso.Scale.major, iso.Scale.chromatic]),
-        iso.EVENT_TRANSPOSE: 36
-    })
-    dummy_timeline.run()
-    assert dummy_timeline.output_device.events == [
-        [0, 'note_on', 36, 64, 0], [1, 'note_off', 36, 0],
-        [1, 'note_on', 37, 64, 0], [2, 'note_off', 37, 0],
-        [2, 'note_on', 40, 64, 0], [3, 'note_off', 40, 0],
-        [3, 'note_on', 39, 64, 0], [4, 'note_off', 39, 0]
-    ]
-
 def test_event_dur(dummy_timeline):
     dummy_timeline.schedule({
         iso.EVENT_NOTE: iso.PSequence([1, 2, 3]),
         iso.EVENT_DURATION: iso.PSequence([1, 1.5, 2, 1.5], 1)
     })
     dummy_timeline.run()
     assert dummy_timeline.output_device.events == [
```

### Comparing `isobar-0.1.1/tests/test_timeline_event_control.py` & `isobar-0.1.2/tests/test_timeline_event_control.py`

 * *Files identical despite different names*

### Comparing `isobar-0.1.1/tests/test_timeline_event_supercollider.py` & `isobar-0.1.2/tests/test_timeline_event_supercollider.py`

 * *Files identical despite different names*

