# Comparing `tmp/python-seispy-1.3.3.tar.gz` & `tmp/python-seispy-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-seispy-1.3.3.tar", last modified: Wed Feb 22 08:15:42 2023, max compression
+gzip compressed data, was "python-seispy-1.3.4.tar", last modified: Sun May 28 15:34:54 2023, max compression
```

## Comparing `python-seispy-1.3.3.tar` & `python-seispy-1.3.4.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 08:15:42.660187 python-seispy-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-02-22 08:15:33.000000 python-seispy-1.3.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-02-22 08:15:42.660187 python-seispy-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-02-22 08:15:33.000000 python-seispy-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 08:15:42.644187 python-seispy-1.3.3/python_seispy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-02-22 08:15:42.000000 python-seispy-1.3.3/python_seispy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-02-22 08:15:42.000000 python-seispy-1.3.3/python_seispy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 08:15:42.000000 python-seispy-1.3.3/python_seispy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-02-22 08:15:42.000000 python-seispy-1.3.3/python_seispy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 08:15:42.000000 python-seispy-1.3.3/python_seispy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-02-22 08:15:42.000000 python-seispy-1.3.3/python_seispy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 08:15:42.000000 python-seispy-1.3.3/python_seispy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 08:15:42.652187 python-seispy-1.3.3/seispy/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/ccp3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/ccppara.py
--rw-r--r--   0 runner    (1001) docker     (123)    13927 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/ccpprofile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 08:15:42.656187 python-seispy-1.3.3/seispy/data/
--rwxr-xr-x   0 runner    (1001) docker     (123)  2645806 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/data/EventCMT.dat
--rwxr-xr-x   0 runner    (1001) docker     (123)      458 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/data/ak135.vel
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/data/cmpVsVp.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      978 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/data/cyan.mat
--rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/data/iasp91.vel
--rwxr-xr-x   0 runner    (1001) docker     (123)      875 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/data/mtna.vel
--rwxr-xr-x   0 runner    (1001) docker     (123)     3696 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/data/prem.vel
--rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/data/saveicon.png
--rw-r--r--   0 runner    (1001) docker     (123)    58484 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/data/seispy.png
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/decon.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/distaz.py
--rw-r--r--   0 runner    (1001) docker     (123)    19609 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/eq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/geo.py
--rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/get_cpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/harmonics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/hk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/hkpara.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/mccc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/modcreator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9269 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/para.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 08:15:42.656187 python-seispy-1.3.3/seispy/pickdepth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/pickdepth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/pickdepth/get_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)    12224 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/pickdepth/pickdepthui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 08:15:42.660187 python-seispy-1.3.3/seispy/pickrf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/pickrf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12794 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/pickrf/pickfigure.py
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/pickrf/pickui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/pickrf/rpickfigure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 08:15:42.660187 python-seispy-1.3.3/seispy/pickseis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/pickseis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/pickseis/sviewerui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/plotR.py
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/plotRT.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/psrayp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/recalrf.py
--rw-r--r--   0 runner    (1001) docker     (123)    23446 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/rf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/rf2depth_makedata.py
--rw-r--r--   0 runner    (1001) docker     (123)    15366 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/rfani.py
--rw-r--r--   0 runner    (1001) docker     (123)    39932 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/rfcorrect.py
--rw-r--r--   0 runner    (1001) docker     (123)    12166 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/seisfwd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/setuplog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/slantstack.py
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-02-22 08:15:33.000000 python-seispy-1.3.3/seispy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 08:15:42.660187 python-seispy-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-02-22 08:15:33.000000 python-seispy-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 08:15:42.660187 python-seispy-1.3.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-02-22 08:15:33.000000 python-seispy-1.3.3/test/test_case01.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-02-22 08:15:33.000000 python-seispy-1.3.3/test/test_case02.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-02-22 08:15:33.000000 python-seispy-1.3.3/test/test_case03.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-22 08:15:33.000000 python-seispy-1.3.3/test/test_case04.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-02-22 08:15:33.000000 python-seispy-1.3.3/test/test_case05.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:34:54.833228 python-seispy-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-28 15:34:45.000000 python-seispy-1.3.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-05-28 15:34:54.833228 python-seispy-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-05-28 15:34:45.000000 python-seispy-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:34:54.817228 python-seispy-1.3.4/python_seispy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-05-28 15:34:54.000000 python-seispy-1.3.4/python_seispy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-28 15:34:54.000000 python-seispy-1.3.4/python_seispy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 15:34:54.000000 python-seispy-1.3.4/python_seispy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-28 15:34:54.000000 python-seispy-1.3.4/python_seispy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 15:34:54.000000 python-seispy-1.3.4/python_seispy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-28 15:34:54.000000 python-seispy-1.3.4/python_seispy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-28 15:34:54.000000 python-seispy-1.3.4/python_seispy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:34:54.829228 python-seispy-1.3.4/seispy/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13469 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/ccp3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/ccppara.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14849 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/ccpprofile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:34:54.833228 python-seispy-1.3.4/seispy/data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)  2645806 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/data/EventCMT.dat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      458 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/data/ak135.vel
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/data/cmpVsVp.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      978 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/data/cyan.mat
+-rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/data/iasp91.vel
+-rwxr-xr-x   0 runner    (1001) docker     (123)      875 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/data/mtna.vel
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3696 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/data/prem.vel
+-rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/data/saveicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    58484 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/data/seispy.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/decon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/distaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19641 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/eq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/get_cpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/harmonics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/hkpara.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/mccc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/modcreator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/para.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:34:54.833228 python-seispy-1.3.4/seispy/pickdepth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/pickdepth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/pickdepth/get_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12208 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/pickdepth/pickdepthui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:34:54.833228 python-seispy-1.3.4/seispy/pickrf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/pickrf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/pickrf/pickfigure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/pickrf/pickui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/pickrf/rpickfigure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:34:54.833228 python-seispy-1.3.4/seispy/pickseis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/pickseis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/pickseis/sviewerui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/plotR.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/plotRT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/psrayp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/recalrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24236 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/rf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/rf2depth_makedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15314 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/rfani.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39953 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/rfcorrect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12166 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6725 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/seisfwd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/setuplog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/slantstack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-05-28 15:34:45.000000 python-seispy-1.3.4/seispy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 15:34:54.833228 python-seispy-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-28 15:34:45.000000 python-seispy-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:34:54.833228 python-seispy-1.3.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-05-28 15:34:45.000000 python-seispy-1.3.4/test/test_case01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-28 15:34:45.000000 python-seispy-1.3.4/test/test_case02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-28 15:34:45.000000 python-seispy-1.3.4/test/test_case03.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-28 15:34:45.000000 python-seispy-1.3.4/test/test_case04.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-28 15:34:45.000000 python-seispy-1.3.4/test/test_case05.py
```

### Comparing `python-seispy-1.3.3/LICENSE.txt` & `python-seispy-1.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.3/PKG-INFO` & `python-seispy-1.3.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-seispy
-Version: 1.3.3
+Version: 1.3.4
 Author: Mijian Xu
 Author-email: gomijianxu@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -37,24 +37,28 @@
 
 [![GitHub stars](https://img.shields.io/github/stars/xumi1993/seispy?style=social)]()
 [![](https://img.shields.io/github/forks/xumi1993/seispy?style=social)]()
 
 
 Seispy is a Python module for processing seismological data and calculating Receiver Functions. The advanced functions are available to improve the Obspy.
 
+## Acknowledgements
+
+For the use of the Seispy package, please cite as:
+
+- Xu, M. & He, J. (2023). Seispy: Python Module for Batch Calculation and Postprocessing of Receiver Functions. Seismological Research Letters, 94 (2A): 935–943. doi: https://doi.org/10.1785/0220220288
+
+For 3D time-difference correction, please also consider citing:
+
+- Xu, M., Huang, H., Huang, Z., Wang, P., Wang, L., Xu, M., ... & Yuan, X. (2018). Insight into the subducted Indian slab and origin of the Tengchong volcano in SE Tibet from receiver function analysis. Earth and Planetary Science Letters, 482, 567-579. doi: https://doi.org/10.1016/j.epsl.2017.11.048
+
+For 2D and 3D CCP stacking, please also consider citing:
+
+- Xu, M., Huang, Z., Wang, L., Xu, M., Zhang, Y., Mi, N., ... & Yuan, X. (2020). Sharp lateral Moho variations across the SE Tibetan margin and their implications for plateau growth. Journal of Geophysical Research: Solid Earth, 125(5), e2019JB018117. doi: https://doi.org/10.1029/2019JB018117
 
-## Dependencies
-  * [Python]() >= 3.8
-  * [ObsPy](http://docs.obspy.org) >= 1.2.0
-  * [NumPy](http://www.numpy.org/) >= 1.16
-  * [SciPy](http://www.scipy.org/) >= 1.2.0
-  * [matplotlib](https://matplotlib.org/) >= 3.6.0
-  * [PySide6](https://www.riverbankcomputing.com/software/pyqt/) >= 6.3.0
-  * [scikits.bootstrap](https://github.com/cgevans/scikits-bootstrap) >= 1.0.0
-  
 ## Installation
 
 See [Seispy documentation](https://seispy.xumijian.me/installation.html) in detail.
  
 ## Libraries
 - `seispy.distaz`: Calculate distance and azimuth credited by the [lithospheric seismology program at USC](http://www.seis.sc.edu/software/distaz/), but `numpy.ndarray` operations are supported.
 - `seispy.geo`: Tiny codes of geophysics.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-seispy Version: 1.3.3 Author: Mijian Xu
+Metadata-Version: 2.1 Name: python-seispy Version: 1.3.4 Author: Mijian Xu
 Author-email: gomijianxu@gmail.com License: GPLv3 Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Description-Content-Type: text/markdown License-
 File: LICENSE.txt # [https://user-images.githubusercontent.com/7437523/
 128596331-dc5c5e40-93e1-4d9e-b92d-9c53fe51145a.png] [![License](https://
 img.shields.io/github/license/xumi1993/seispy)]() [![](https://img.shields.io/
@@ -28,37 +28,46 @@
 (https://img.shields.io/pypi/v/python-seispy)](https://pypi.org/project/python-
 seispy/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
 python-seispy)](https://pypi.org/project/python-seispy/) [![GitHub stars]
 (https://img.shields.io/github/stars/xumi1993/seispy?style=social)]() [![]
 (https://img.shields.io/github/forks/xumi1993/seispy?style=social)]() Seispy is
 a Python module for processing seismological data and calculating Receiver
 Functions. The advanced functions are available to improve the Obspy. ##
-Dependencies * [Python]() >= 3.8 * [ObsPy](http://docs.obspy.org) >= 1.2.0 *
-[NumPy](http://www.numpy.org/) >= 1.16 * [SciPy](http://www.scipy.org/) >=
-1.2.0 * [matplotlib](https://matplotlib.org/) >= 3.6.0 * [PySide6](https://
-www.riverbankcomputing.com/software/pyqt/) >= 6.3.0 * [scikits.bootstrap]
-(https://github.com/cgevans/scikits-bootstrap) >= 1.0.0 ## Installation See
-[Seispy documentation](https://seispy.xumijian.me/installation.html) in detail.
-## Libraries - `seispy.distaz`: Calculate distance and azimuth credited by the
-[lithospheric seismology program at USC](http://www.seis.sc.edu/software/
-distaz/), but `numpy.ndarray` operations are supported. - `seispy.geo`: Tiny
-codes of geophysics. - `seispy.decon`: Functions of deconvolution transferred
-from [iwbailey/processRFmatlab](https://github.com/iwbailey/processRFmatlab)
-including - Iterative time domain deconvolution method (LigorrÃ­a and Ammon
-1999 BSSA). - Water level frequency domain deconvolution method (CJ. Ammon 1991
-BSSA) - `seispy.rf`: Procedure for RF calculation. The functions of `match_eq`,
-`search_eq` invoked `obspy.core.UTCDateTime` and `obspy.clients` from the
-[Obspy](https://docs.obspy.org/). - `seispy.eq`: RF processing for each event,
-which invoked `obspy.io.sac`, `obspy.signal`, `obspy.taup` and
-`obspy.core.Stream` from the [Obspy](https://docs.obspy.org/). - `seispy.hk`:
-H-k stacking for single station (Zhu and Kanamori 2000 JGR). - `seispy.rfani`:
-A joint method for crustal anisotropic calculation (Liu and Niu 2011 GJI). -
-`seispy.slantstack`: Slant stacking for single station (Tauzin et al., 2008) -
-`seispy.rfcorrect`: Subsequent process of RFs including moveout correction and
-time to depth conversion (1D and 3D) (see [Xu et al., 2018 EPSL](https://
+Acknowledgements For the use of the Seispy package, please cite as: - Xu, M. &
+He, J. (2023). Seispy: Python Module for Batch Calculation and Postprocessing
+of Receiver Functions. Seismological Research Letters, 94 (2A): 935â943. doi:
+https://doi.org/10.1785/0220220288 For 3D time-difference correction, please
+also consider citing: - Xu, M., Huang, H., Huang, Z., Wang, P., Wang, L., Xu,
+M., ... & Yuan, X. (2018). Insight into the subducted Indian slab and origin of
+the Tengchong volcano in SE Tibet from receiver function analysis. Earth and
+Planetary Science Letters, 482, 567-579. doi: https://doi.org/10.1016/
+j.epsl.2017.11.048 For 2D and 3D CCP stacking, please also consider citing: -
+Xu, M., Huang, Z., Wang, L., Xu, M., Zhang, Y., Mi, N., ... & Yuan, X. (2020).
+Sharp lateral Moho variations across the SE Tibetan margin and their
+implications for plateau growth. Journal of Geophysical Research: Solid Earth,
+125(5), e2019JB018117. doi: https://doi.org/10.1029/2019JB018117 ##
+Installation See [Seispy documentation](https://seispy.xumijian.me/
+installation.html) in detail. ## Libraries - `seispy.distaz`: Calculate
+distance and azimuth credited by the [lithospheric seismology program at USC]
+(http://www.seis.sc.edu/software/distaz/), but `numpy.ndarray` operations are
+supported. - `seispy.geo`: Tiny codes of geophysics. - `seispy.decon`:
+Functions of deconvolution transferred from [iwbailey/processRFmatlab](https://
+github.com/iwbailey/processRFmatlab) including - Iterative time domain
+deconvolution method (LigorrÃ­a and Ammon 1999 BSSA). - Water level frequency
+domain deconvolution method (CJ. Ammon 1991 BSSA) - `seispy.rf`: Procedure for
+RF calculation. The functions of `match_eq`, `search_eq` invoked
+`obspy.core.UTCDateTime` and `obspy.clients` from the [Obspy](https://
+docs.obspy.org/). - `seispy.eq`: RF processing for each event, which invoked
+`obspy.io.sac`, `obspy.signal`, `obspy.taup` and `obspy.core.Stream` from the
+[Obspy](https://docs.obspy.org/). - `seispy.hk`: H-k stacking for single
+station (Zhu and Kanamori 2000 JGR). - `seispy.rfani`: A joint method for
+crustal anisotropic calculation (Liu and Niu 2011 GJI). - `seispy.slantstack`:
+Slant stacking for single station (Tauzin et al., 2008) - `seispy.rfcorrect`:
+Subsequent process of RFs including moveout correction and time to depth
+conversion (1D and 3D) (see [Xu et al., 2018 EPSL](https://
 www.sciencedirect.com/science/article/pii/S0012821X17306921?via%3Dihub)) -
 `seispy.ccpprofile`: CCP stacking along a profile. - `seispy.ccp3d`: 3-D CCP
 stacking with extracting depth D410 and D660. [lithospheric seismology program
 at USC]: http://www.seis.sc.edu/software/distaz/ [scikits-bootstrap]: https://
 github.com/cgevans/scikits-bootstrap [iwbailey/processRFmatlab]: https://
 github.com/iwbailey/processRFmatlab [Obspy]: https://docs.obspy.org/ [Xu et
 al., 2018 EPSL]: https://www.sciencedirect.com/science/article/pii/
```

### Comparing `python-seispy-1.3.3/README.md` & `python-seispy-1.3.4/python_seispy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: python-seispy
+Version: 1.3.4
+Author: Mijian Xu
+Author-email: gomijianxu@gmail.com
+License: GPLv3
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # <img src="https://user-images.githubusercontent.com/7437523/128596331-dc5c5e40-93e1-4d9e-b92d-9c53fe51145a.png" width="500"/> 
 
 
 [![License](https://img.shields.io/github/license/xumi1993/seispy)]()
 [![](https://img.shields.io/github/last-commit/xumi1993/seispy)]()
 [![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/xumi1993/seispy)]()
 [![GitHub repo size](https://img.shields.io/github/repo-size/xumi1993/seispy)]()
@@ -24,24 +37,28 @@
 
 [![GitHub stars](https://img.shields.io/github/stars/xumi1993/seispy?style=social)]()
 [![](https://img.shields.io/github/forks/xumi1993/seispy?style=social)]()
 
 
 Seispy is a Python module for processing seismological data and calculating Receiver Functions. The advanced functions are available to improve the Obspy.
 
+## Acknowledgements
+
+For the use of the Seispy package, please cite as:
+
+- Xu, M. & He, J. (2023). Seispy: Python Module for Batch Calculation and Postprocessing of Receiver Functions. Seismological Research Letters, 94 (2A): 935–943. doi: https://doi.org/10.1785/0220220288
+
+For 3D time-difference correction, please also consider citing:
+
+- Xu, M., Huang, H., Huang, Z., Wang, P., Wang, L., Xu, M., ... & Yuan, X. (2018). Insight into the subducted Indian slab and origin of the Tengchong volcano in SE Tibet from receiver function analysis. Earth and Planetary Science Letters, 482, 567-579. doi: https://doi.org/10.1016/j.epsl.2017.11.048
+
+For 2D and 3D CCP stacking, please also consider citing:
+
+- Xu, M., Huang, Z., Wang, L., Xu, M., Zhang, Y., Mi, N., ... & Yuan, X. (2020). Sharp lateral Moho variations across the SE Tibetan margin and their implications for plateau growth. Journal of Geophysical Research: Solid Earth, 125(5), e2019JB018117. doi: https://doi.org/10.1029/2019JB018117
 
-## Dependencies
-  * [Python]() >= 3.8
-  * [ObsPy](http://docs.obspy.org) >= 1.2.0
-  * [NumPy](http://www.numpy.org/) >= 1.16
-  * [SciPy](http://www.scipy.org/) >= 1.2.0
-  * [matplotlib](https://matplotlib.org/) >= 3.6.0
-  * [PySide6](https://www.riverbankcomputing.com/software/pyqt/) >= 6.3.0
-  * [scikits.bootstrap](https://github.com/cgevans/scikits-bootstrap) >= 1.0.0
-  
 ## Installation
 
 See [Seispy documentation](https://seispy.xumijian.me/installation.html) in detail.
  
 ## Libraries
 - `seispy.distaz`: Calculate distance and azimuth credited by the [lithospheric seismology program at USC](http://www.seis.sc.edu/software/distaz/), but `numpy.ndarray` operations are supported.
 - `seispy.geo`: Tiny codes of geophysics.
```

#### html2text {}

```diff
@@ -1,59 +1,73 @@
-# [https://user-images.githubusercontent.com/7437523/128596331-dc5c5e40-93e1-
-4d9e-b92d-9c53fe51145a.png] [![License](https://img.shields.io/github/license/
-xumi1993/seispy)]() [![](https://img.shields.io/github/last-commit/xumi1993/
-seispy)]() [![GitHub code size in bytes](https://img.shields.io/github/
-languages/code-size/xumi1993/seispy)]() [![GitHub repo size](https://
-img.shields.io/github/repo-size/xumi1993/seispy)]() [![DOI](https://zenodo.org/
-badge/41006349.svg)](https://zenodo.org/badge/latestdoi/41006349) [![CRV test]
-(https://github.com/xumi1993/seispy/actions/workflows/test.yml/
-badge.svg?branch=dev)](https://github.com/xumi1993/seispy/actions/workflows/
-test.yml) [![codecov](https://codecov.io/gh/xumi1993/seispy/branch/dev/graph/
-badge.svg?token=XN3E3N6S3V)](https://codecov.io/gh/xumi1993/seispy) [![Upload
-Python Package](https://github.com/xumi1993/seispy/actions/workflows/python-
-publish.yml/badge.svg)](https://github.com/xumi1993/seispy/actions/workflows/
-python-publish.yml) [![Seispy docs](https://github.com/xumi1993/seispy/actions/
-workflows/doc_build.yml/badge.svg)](https://github.com/xumi1993/seispy/actions/
-workflows/doc_build.yml) [https://dev.azure.com/conda-forge/feedstock-builds/
-_apis/build/status/seispy-feedstock?branchName=master] [![Anaconda-Server
-Badge](https://anaconda.org/conda-forge/seispy/badges/version.svg)](https://
-anaconda.org/conda-forge/seispy) [![Conda Version](https://img.shields.io/
-conda/vn/conda-forge/seispy.svg)](https://anaconda.org/conda-forge/seispy) [!
+Metadata-Version: 2.1 Name: python-seispy Version: 1.3.4 Author: Mijian Xu
+Author-email: gomijianxu@gmail.com License: GPLv3 Classifier: Programming
+Language :: Python Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Description-Content-Type: text/markdown License-
+File: LICENSE.txt # [https://user-images.githubusercontent.com/7437523/
+128596331-dc5c5e40-93e1-4d9e-b92d-9c53fe51145a.png] [![License](https://
+img.shields.io/github/license/xumi1993/seispy)]() [![](https://img.shields.io/
+github/last-commit/xumi1993/seispy)]() [![GitHub code size in bytes](https://
+img.shields.io/github/languages/code-size/xumi1993/seispy)]() [![GitHub repo
+size](https://img.shields.io/github/repo-size/xumi1993/seispy)]() [![DOI]
+(https://zenodo.org/badge/41006349.svg)](https://zenodo.org/badge/latestdoi/
+41006349) [![CRV test](https://github.com/xumi1993/seispy/actions/workflows/
+test.yml/badge.svg?branch=dev)](https://github.com/xumi1993/seispy/actions/
+workflows/test.yml) [![codecov](https://codecov.io/gh/xumi1993/seispy/branch/
+dev/graph/badge.svg?token=XN3E3N6S3V)](https://codecov.io/gh/xumi1993/seispy)
+[![Upload Python Package](https://github.com/xumi1993/seispy/actions/workflows/
+python-publish.yml/badge.svg)](https://github.com/xumi1993/seispy/actions/
+workflows/python-publish.yml) [![Seispy docs](https://github.com/xumi1993/
+seispy/actions/workflows/doc_build.yml/badge.svg)](https://github.com/xumi1993/
+seispy/actions/workflows/doc_build.yml) [https://dev.azure.com/conda-forge/
+feedstock-builds/_apis/build/status/seispy-feedstock?branchName=master] [!
 [Anaconda-Server Badge](https://anaconda.org/conda-forge/seispy/badges/
-downloads.svg)](https://anaconda.org/conda-forge/seispy) [![PyPI](https://
-img.shields.io/pypi/v/python-seispy)](https://pypi.org/project/python-seispy/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/python-
-seispy)](https://pypi.org/project/python-seispy/) [![GitHub stars](https://
-img.shields.io/github/stars/xumi1993/seispy?style=social)]() [![](https://
-img.shields.io/github/forks/xumi1993/seispy?style=social)]() Seispy is a Python
-module for processing seismological data and calculating Receiver Functions.
-The advanced functions are available to improve the Obspy. ## Dependencies *
-[Python]() >= 3.8 * [ObsPy](http://docs.obspy.org) >= 1.2.0 * [NumPy](http://
-www.numpy.org/) >= 1.16 * [SciPy](http://www.scipy.org/) >= 1.2.0 *
-[matplotlib](https://matplotlib.org/) >= 3.6.0 * [PySide6](https://
-www.riverbankcomputing.com/software/pyqt/) >= 6.3.0 * [scikits.bootstrap]
-(https://github.com/cgevans/scikits-bootstrap) >= 1.0.0 ## Installation See
-[Seispy documentation](https://seispy.xumijian.me/installation.html) in detail.
-## Libraries - `seispy.distaz`: Calculate distance and azimuth credited by the
-[lithospheric seismology program at USC](http://www.seis.sc.edu/software/
-distaz/), but `numpy.ndarray` operations are supported. - `seispy.geo`: Tiny
-codes of geophysics. - `seispy.decon`: Functions of deconvolution transferred
-from [iwbailey/processRFmatlab](https://github.com/iwbailey/processRFmatlab)
-including - Iterative time domain deconvolution method (LigorrÃ­a and Ammon
-1999 BSSA). - Water level frequency domain deconvolution method (CJ. Ammon 1991
-BSSA) - `seispy.rf`: Procedure for RF calculation. The functions of `match_eq`,
-`search_eq` invoked `obspy.core.UTCDateTime` and `obspy.clients` from the
-[Obspy](https://docs.obspy.org/). - `seispy.eq`: RF processing for each event,
-which invoked `obspy.io.sac`, `obspy.signal`, `obspy.taup` and
-`obspy.core.Stream` from the [Obspy](https://docs.obspy.org/). - `seispy.hk`:
-H-k stacking for single station (Zhu and Kanamori 2000 JGR). - `seispy.rfani`:
-A joint method for crustal anisotropic calculation (Liu and Niu 2011 GJI). -
-`seispy.slantstack`: Slant stacking for single station (Tauzin et al., 2008) -
-`seispy.rfcorrect`: Subsequent process of RFs including moveout correction and
-time to depth conversion (1D and 3D) (see [Xu et al., 2018 EPSL](https://
+version.svg)](https://anaconda.org/conda-forge/seispy) [![Conda Version](https:
+//img.shields.io/conda/vn/conda-forge/seispy.svg)](https://anaconda.org/conda-
+forge/seispy) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/
+seispy/badges/downloads.svg)](https://anaconda.org/conda-forge/seispy) [![PyPI]
+(https://img.shields.io/pypi/v/python-seispy)](https://pypi.org/project/python-
+seispy/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
+python-seispy)](https://pypi.org/project/python-seispy/) [![GitHub stars]
+(https://img.shields.io/github/stars/xumi1993/seispy?style=social)]() [![]
+(https://img.shields.io/github/forks/xumi1993/seispy?style=social)]() Seispy is
+a Python module for processing seismological data and calculating Receiver
+Functions. The advanced functions are available to improve the Obspy. ##
+Acknowledgements For the use of the Seispy package, please cite as: - Xu, M. &
+He, J. (2023). Seispy: Python Module for Batch Calculation and Postprocessing
+of Receiver Functions. Seismological Research Letters, 94 (2A): 935â943. doi:
+https://doi.org/10.1785/0220220288 For 3D time-difference correction, please
+also consider citing: - Xu, M., Huang, H., Huang, Z., Wang, P., Wang, L., Xu,
+M., ... & Yuan, X. (2018). Insight into the subducted Indian slab and origin of
+the Tengchong volcano in SE Tibet from receiver function analysis. Earth and
+Planetary Science Letters, 482, 567-579. doi: https://doi.org/10.1016/
+j.epsl.2017.11.048 For 2D and 3D CCP stacking, please also consider citing: -
+Xu, M., Huang, Z., Wang, L., Xu, M., Zhang, Y., Mi, N., ... & Yuan, X. (2020).
+Sharp lateral Moho variations across the SE Tibetan margin and their
+implications for plateau growth. Journal of Geophysical Research: Solid Earth,
+125(5), e2019JB018117. doi: https://doi.org/10.1029/2019JB018117 ##
+Installation See [Seispy documentation](https://seispy.xumijian.me/
+installation.html) in detail. ## Libraries - `seispy.distaz`: Calculate
+distance and azimuth credited by the [lithospheric seismology program at USC]
+(http://www.seis.sc.edu/software/distaz/), but `numpy.ndarray` operations are
+supported. - `seispy.geo`: Tiny codes of geophysics. - `seispy.decon`:
+Functions of deconvolution transferred from [iwbailey/processRFmatlab](https://
+github.com/iwbailey/processRFmatlab) including - Iterative time domain
+deconvolution method (LigorrÃ­a and Ammon 1999 BSSA). - Water level frequency
+domain deconvolution method (CJ. Ammon 1991 BSSA) - `seispy.rf`: Procedure for
+RF calculation. The functions of `match_eq`, `search_eq` invoked
+`obspy.core.UTCDateTime` and `obspy.clients` from the [Obspy](https://
+docs.obspy.org/). - `seispy.eq`: RF processing for each event, which invoked
+`obspy.io.sac`, `obspy.signal`, `obspy.taup` and `obspy.core.Stream` from the
+[Obspy](https://docs.obspy.org/). - `seispy.hk`: H-k stacking for single
+station (Zhu and Kanamori 2000 JGR). - `seispy.rfani`: A joint method for
+crustal anisotropic calculation (Liu and Niu 2011 GJI). - `seispy.slantstack`:
+Slant stacking for single station (Tauzin et al., 2008) - `seispy.rfcorrect`:
+Subsequent process of RFs including moveout correction and time to depth
+conversion (1D and 3D) (see [Xu et al., 2018 EPSL](https://
 www.sciencedirect.com/science/article/pii/S0012821X17306921?via%3Dihub)) -
 `seispy.ccpprofile`: CCP stacking along a profile. - `seispy.ccp3d`: 3-D CCP
 stacking with extracting depth D410 and D660. [lithospheric seismology program
 at USC]: http://www.seis.sc.edu/software/distaz/ [scikits-bootstrap]: https://
 github.com/cgevans/scikits-bootstrap [iwbailey/processRFmatlab]: https://
 github.com/iwbailey/processRFmatlab [Obspy]: https://docs.obspy.org/ [Xu et
 al., 2018 EPSL]: https://www.sciencedirect.com/science/article/pii/
```

### Comparing `python-seispy-1.3.3/python_seispy.egg-info/PKG-INFO` & `python-seispy-1.3.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: python-seispy
-Version: 1.3.3
-Author: Mijian Xu
-Author-email: gomijianxu@gmail.com
-License: GPLv3
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # <img src="https://user-images.githubusercontent.com/7437523/128596331-dc5c5e40-93e1-4d9e-b92d-9c53fe51145a.png" width="500"/> 
 
 
 [![License](https://img.shields.io/github/license/xumi1993/seispy)]()
 [![](https://img.shields.io/github/last-commit/xumi1993/seispy)]()
 [![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/xumi1993/seispy)]()
 [![GitHub repo size](https://img.shields.io/github/repo-size/xumi1993/seispy)]()
@@ -37,24 +24,28 @@
 
 [![GitHub stars](https://img.shields.io/github/stars/xumi1993/seispy?style=social)]()
 [![](https://img.shields.io/github/forks/xumi1993/seispy?style=social)]()
 
 
 Seispy is a Python module for processing seismological data and calculating Receiver Functions. The advanced functions are available to improve the Obspy.
 
+## Acknowledgements
+
+For the use of the Seispy package, please cite as:
+
+- Xu, M. & He, J. (2023). Seispy: Python Module for Batch Calculation and Postprocessing of Receiver Functions. Seismological Research Letters, 94 (2A): 935–943. doi: https://doi.org/10.1785/0220220288
+
+For 3D time-difference correction, please also consider citing:
+
+- Xu, M., Huang, H., Huang, Z., Wang, P., Wang, L., Xu, M., ... & Yuan, X. (2018). Insight into the subducted Indian slab and origin of the Tengchong volcano in SE Tibet from receiver function analysis. Earth and Planetary Science Letters, 482, 567-579. doi: https://doi.org/10.1016/j.epsl.2017.11.048
+
+For 2D and 3D CCP stacking, please also consider citing:
+
+- Xu, M., Huang, Z., Wang, L., Xu, M., Zhang, Y., Mi, N., ... & Yuan, X. (2020). Sharp lateral Moho variations across the SE Tibetan margin and their implications for plateau growth. Journal of Geophysical Research: Solid Earth, 125(5), e2019JB018117. doi: https://doi.org/10.1029/2019JB018117
 
-## Dependencies
-  * [Python]() >= 3.8
-  * [ObsPy](http://docs.obspy.org) >= 1.2.0
-  * [NumPy](http://www.numpy.org/) >= 1.16
-  * [SciPy](http://www.scipy.org/) >= 1.2.0
-  * [matplotlib](https://matplotlib.org/) >= 3.6.0
-  * [PySide6](https://www.riverbankcomputing.com/software/pyqt/) >= 6.3.0
-  * [scikits.bootstrap](https://github.com/cgevans/scikits-bootstrap) >= 1.0.0
-  
 ## Installation
 
 See [Seispy documentation](https://seispy.xumijian.me/installation.html) in detail.
  
 ## Libraries
 - `seispy.distaz`: Calculate distance and azimuth credited by the [lithospheric seismology program at USC](http://www.seis.sc.edu/software/distaz/), but `numpy.ndarray` operations are supported.
 - `seispy.geo`: Tiny codes of geophysics.
```

#### html2text {}

```diff
@@ -1,64 +1,68 @@
-Metadata-Version: 2.1 Name: python-seispy Version: 1.3.3 Author: Mijian Xu
-Author-email: gomijianxu@gmail.com License: GPLv3 Classifier: Programming
-Language :: Python Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Description-Content-Type: text/markdown License-
-File: LICENSE.txt # [https://user-images.githubusercontent.com/7437523/
-128596331-dc5c5e40-93e1-4d9e-b92d-9c53fe51145a.png] [![License](https://
-img.shields.io/github/license/xumi1993/seispy)]() [![](https://img.shields.io/
-github/last-commit/xumi1993/seispy)]() [![GitHub code size in bytes](https://
-img.shields.io/github/languages/code-size/xumi1993/seispy)]() [![GitHub repo
-size](https://img.shields.io/github/repo-size/xumi1993/seispy)]() [![DOI]
-(https://zenodo.org/badge/41006349.svg)](https://zenodo.org/badge/latestdoi/
-41006349) [![CRV test](https://github.com/xumi1993/seispy/actions/workflows/
-test.yml/badge.svg?branch=dev)](https://github.com/xumi1993/seispy/actions/
-workflows/test.yml) [![codecov](https://codecov.io/gh/xumi1993/seispy/branch/
-dev/graph/badge.svg?token=XN3E3N6S3V)](https://codecov.io/gh/xumi1993/seispy)
-[![Upload Python Package](https://github.com/xumi1993/seispy/actions/workflows/
-python-publish.yml/badge.svg)](https://github.com/xumi1993/seispy/actions/
-workflows/python-publish.yml) [![Seispy docs](https://github.com/xumi1993/
-seispy/actions/workflows/doc_build.yml/badge.svg)](https://github.com/xumi1993/
-seispy/actions/workflows/doc_build.yml) [https://dev.azure.com/conda-forge/
-feedstock-builds/_apis/build/status/seispy-feedstock?branchName=master] [!
+# [https://user-images.githubusercontent.com/7437523/128596331-dc5c5e40-93e1-
+4d9e-b92d-9c53fe51145a.png] [![License](https://img.shields.io/github/license/
+xumi1993/seispy)]() [![](https://img.shields.io/github/last-commit/xumi1993/
+seispy)]() [![GitHub code size in bytes](https://img.shields.io/github/
+languages/code-size/xumi1993/seispy)]() [![GitHub repo size](https://
+img.shields.io/github/repo-size/xumi1993/seispy)]() [![DOI](https://zenodo.org/
+badge/41006349.svg)](https://zenodo.org/badge/latestdoi/41006349) [![CRV test]
+(https://github.com/xumi1993/seispy/actions/workflows/test.yml/
+badge.svg?branch=dev)](https://github.com/xumi1993/seispy/actions/workflows/
+test.yml) [![codecov](https://codecov.io/gh/xumi1993/seispy/branch/dev/graph/
+badge.svg?token=XN3E3N6S3V)](https://codecov.io/gh/xumi1993/seispy) [![Upload
+Python Package](https://github.com/xumi1993/seispy/actions/workflows/python-
+publish.yml/badge.svg)](https://github.com/xumi1993/seispy/actions/workflows/
+python-publish.yml) [![Seispy docs](https://github.com/xumi1993/seispy/actions/
+workflows/doc_build.yml/badge.svg)](https://github.com/xumi1993/seispy/actions/
+workflows/doc_build.yml) [https://dev.azure.com/conda-forge/feedstock-builds/
+_apis/build/status/seispy-feedstock?branchName=master] [![Anaconda-Server
+Badge](https://anaconda.org/conda-forge/seispy/badges/version.svg)](https://
+anaconda.org/conda-forge/seispy) [![Conda Version](https://img.shields.io/
+conda/vn/conda-forge/seispy.svg)](https://anaconda.org/conda-forge/seispy) [!
 [Anaconda-Server Badge](https://anaconda.org/conda-forge/seispy/badges/
-version.svg)](https://anaconda.org/conda-forge/seispy) [![Conda Version](https:
-//img.shields.io/conda/vn/conda-forge/seispy.svg)](https://anaconda.org/conda-
-forge/seispy) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/
-seispy/badges/downloads.svg)](https://anaconda.org/conda-forge/seispy) [![PyPI]
-(https://img.shields.io/pypi/v/python-seispy)](https://pypi.org/project/python-
-seispy/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
-python-seispy)](https://pypi.org/project/python-seispy/) [![GitHub stars]
-(https://img.shields.io/github/stars/xumi1993/seispy?style=social)]() [![]
-(https://img.shields.io/github/forks/xumi1993/seispy?style=social)]() Seispy is
-a Python module for processing seismological data and calculating Receiver
-Functions. The advanced functions are available to improve the Obspy. ##
-Dependencies * [Python]() >= 3.8 * [ObsPy](http://docs.obspy.org) >= 1.2.0 *
-[NumPy](http://www.numpy.org/) >= 1.16 * [SciPy](http://www.scipy.org/) >=
-1.2.0 * [matplotlib](https://matplotlib.org/) >= 3.6.0 * [PySide6](https://
-www.riverbankcomputing.com/software/pyqt/) >= 6.3.0 * [scikits.bootstrap]
-(https://github.com/cgevans/scikits-bootstrap) >= 1.0.0 ## Installation See
-[Seispy documentation](https://seispy.xumijian.me/installation.html) in detail.
-## Libraries - `seispy.distaz`: Calculate distance and azimuth credited by the
-[lithospheric seismology program at USC](http://www.seis.sc.edu/software/
-distaz/), but `numpy.ndarray` operations are supported. - `seispy.geo`: Tiny
-codes of geophysics. - `seispy.decon`: Functions of deconvolution transferred
-from [iwbailey/processRFmatlab](https://github.com/iwbailey/processRFmatlab)
-including - Iterative time domain deconvolution method (LigorrÃ­a and Ammon
-1999 BSSA). - Water level frequency domain deconvolution method (CJ. Ammon 1991
-BSSA) - `seispy.rf`: Procedure for RF calculation. The functions of `match_eq`,
-`search_eq` invoked `obspy.core.UTCDateTime` and `obspy.clients` from the
-[Obspy](https://docs.obspy.org/). - `seispy.eq`: RF processing for each event,
-which invoked `obspy.io.sac`, `obspy.signal`, `obspy.taup` and
-`obspy.core.Stream` from the [Obspy](https://docs.obspy.org/). - `seispy.hk`:
-H-k stacking for single station (Zhu and Kanamori 2000 JGR). - `seispy.rfani`:
-A joint method for crustal anisotropic calculation (Liu and Niu 2011 GJI). -
-`seispy.slantstack`: Slant stacking for single station (Tauzin et al., 2008) -
-`seispy.rfcorrect`: Subsequent process of RFs including moveout correction and
-time to depth conversion (1D and 3D) (see [Xu et al., 2018 EPSL](https://
+downloads.svg)](https://anaconda.org/conda-forge/seispy) [![PyPI](https://
+img.shields.io/pypi/v/python-seispy)](https://pypi.org/project/python-seispy/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/python-
+seispy)](https://pypi.org/project/python-seispy/) [![GitHub stars](https://
+img.shields.io/github/stars/xumi1993/seispy?style=social)]() [![](https://
+img.shields.io/github/forks/xumi1993/seispy?style=social)]() Seispy is a Python
+module for processing seismological data and calculating Receiver Functions.
+The advanced functions are available to improve the Obspy. ## Acknowledgements
+For the use of the Seispy package, please cite as: - Xu, M. & He, J. (2023).
+Seispy: Python Module for Batch Calculation and Postprocessing of Receiver
+Functions. Seismological Research Letters, 94 (2A): 935â943. doi: https://
+doi.org/10.1785/0220220288 For 3D time-difference correction, please also
+consider citing: - Xu, M., Huang, H., Huang, Z., Wang, P., Wang, L., Xu, M.,
+... & Yuan, X. (2018). Insight into the subducted Indian slab and origin of the
+Tengchong volcano in SE Tibet from receiver function analysis. Earth and
+Planetary Science Letters, 482, 567-579. doi: https://doi.org/10.1016/
+j.epsl.2017.11.048 For 2D and 3D CCP stacking, please also consider citing: -
+Xu, M., Huang, Z., Wang, L., Xu, M., Zhang, Y., Mi, N., ... & Yuan, X. (2020).
+Sharp lateral Moho variations across the SE Tibetan margin and their
+implications for plateau growth. Journal of Geophysical Research: Solid Earth,
+125(5), e2019JB018117. doi: https://doi.org/10.1029/2019JB018117 ##
+Installation See [Seispy documentation](https://seispy.xumijian.me/
+installation.html) in detail. ## Libraries - `seispy.distaz`: Calculate
+distance and azimuth credited by the [lithospheric seismology program at USC]
+(http://www.seis.sc.edu/software/distaz/), but `numpy.ndarray` operations are
+supported. - `seispy.geo`: Tiny codes of geophysics. - `seispy.decon`:
+Functions of deconvolution transferred from [iwbailey/processRFmatlab](https://
+github.com/iwbailey/processRFmatlab) including - Iterative time domain
+deconvolution method (LigorrÃ­a and Ammon 1999 BSSA). - Water level frequency
+domain deconvolution method (CJ. Ammon 1991 BSSA) - `seispy.rf`: Procedure for
+RF calculation. The functions of `match_eq`, `search_eq` invoked
+`obspy.core.UTCDateTime` and `obspy.clients` from the [Obspy](https://
+docs.obspy.org/). - `seispy.eq`: RF processing for each event, which invoked
+`obspy.io.sac`, `obspy.signal`, `obspy.taup` and `obspy.core.Stream` from the
+[Obspy](https://docs.obspy.org/). - `seispy.hk`: H-k stacking for single
+station (Zhu and Kanamori 2000 JGR). - `seispy.rfani`: A joint method for
+crustal anisotropic calculation (Liu and Niu 2011 GJI). - `seispy.slantstack`:
+Slant stacking for single station (Tauzin et al., 2008) - `seispy.rfcorrect`:
+Subsequent process of RFs including moveout correction and time to depth
+conversion (1D and 3D) (see [Xu et al., 2018 EPSL](https://
 www.sciencedirect.com/science/article/pii/S0012821X17306921?via%3Dihub)) -
 `seispy.ccpprofile`: CCP stacking along a profile. - `seispy.ccp3d`: 3-D CCP
 stacking with extracting depth D410 and D660. [lithospheric seismology program
 at USC]: http://www.seis.sc.edu/software/distaz/ [scikits-bootstrap]: https://
 github.com/cgevans/scikits-bootstrap [iwbailey/processRFmatlab]: https://
 github.com/iwbailey/processRFmatlab [Obspy]: https://docs.obspy.org/ [Xu et
 al., 2018 EPSL]: https://www.sciencedirect.com/science/article/pii/
```

### Comparing `python-seispy-1.3.3/python_seispy.egg-info/SOURCES.txt` & `python-seispy-1.3.4/python_seispy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.3/python_seispy.egg-info/entry_points.txt` & `python-seispy-1.3.4/python_seispy.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.3/seispy/catalog.py` & `python-seispy-1.3.4/seispy/catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,18 +21,18 @@
     else:
         query.events_raw.write(fname, format=format)
 
 
 def read_catalog_file(fname):
     col = ['date', 'evla', 'evlo', 'evdp', 'mag']
     colcata = ['year', 'month', 'day', 'hour', 'minute', 'second']
-    data_cata = pd.read_table(fname, header=None, sep=' |\t', engine='python')
+    data_cata = pd.read_table(fname, header=None, sep='\s+')
     date_cols = data_cata.loc[:, [0,1,2,4,5,6]]
     date_cols.columns = colcata
-    dates = pd.to_datetime(date_cols)
+    dates = pd.DataFrame(pd.to_datetime(date_cols))[0].apply(UTCDateTime)
     eq_lst = pd.concat([dates, data_cata.loc[:, 7:]], axis=1)
     eq_lst.columns = col
     return eq_lst
 
 
 def main():
     parser = argparse.ArgumentParser(description="Download Catalog to local file")
```

### Comparing `python-seispy-1.3.3/seispy/ccp3d.py` & `python-seispy-1.3.4/seispy/ccp3d.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,61 +1,59 @@
 import numpy as np
-from seispy.geo import km2deg, latlon_from, cosd, extrema, skm2srad, rad2deg
+from seispy.geo import km2deg, extrema, skm2srad, rad2deg
 from seispy import distaz
 from seispy.rfcorrect import DepModel
 from seispy.setuplog import setuplog
 from scikits.bootstrap import ci
 from seispy.ccppara import ccppara, CCPPara
 from seispy.signal import smooth
 from seispy.utils import check_stack_val, read_rfdep
 from scipy.interpolate import interp1d
+import pyproj
 import warnings
 import sys
 
 
 def gen_center_bin(center_lat, center_lon, len_lat, len_lon, val):
     """
-Create spaced grid point with coordinates of the center point in the area in spherical coordinates.
+    Create spaced grid point with coordinates of the center point in the area in spherical coordinates.
 
-:param center_lat: Latitude of the center point.
-:type center_lat: float
-:param center_lon: Longitude of the center point.
-:type center_lon: float
-:param len_lat: Half length in degree along latitude axis.
-:type len_lat: float
-:param len_lon: Half length in degree along longitude axis.
-:type len_lon: float
-:param val: Interval in degree between adjacent grid point.
-:type val: float
-:return: Coordinates of Grid points.
-:rtype: 2-D ndarray of floats with shape (n, 2), where n is the number of grid points.
+    :param center_lat: Latitude of the center point.
+    :type center_lat: float
+    :param center_lon: Longitude of the center point.
+    :type center_lon: float
+    :param len_lat: Half length in degree along latitude axis.
+    :type len_lat: float
+    :param len_lon: Half length in degree along longitude axis.
+    :type len_lon: float
+    :param val: Interval in degree between adjacent grid point.
+    :type val: float
+    :return: Coordinates of Grid points.
+    :rtype: 2-D ndarray of floats with shape (n, 2), where n is the number of grid points.
     """
-    lats = np.arange(0, 2*len_lat, val)
-    lons = np.arange(0, 2*len_lon, val)
-    plat, plon = latlon_from(center_lat, center_lon, 0, 90)
-    da = distaz(plat, plon, center_lat, center_lon)
-    begx = -len_lon 
-    begy = -len_lat
-    bin_loca = []
-    bin_mat = np.zeros([lats.size, lons.size, 2])
-    bin_map = np.zeros([lats.size, lons.size]).astype(int)
+    ellps="WGS84"
+    deg2km = 111.19
+    val_m = val*deg2km*1000
+    len_lat_m = len_lat*deg2km*1000
+    len_lon_m = len_lon*deg2km*1000
+    proj = pyproj.Proj(proj='aeqd', ellps=ellps, datum=ellps, lat_0=center_lat, lon_0=center_lon)
+    dx = np.arange(-len_lon_m, len_lon_m + val_m, val_m)
+    dy = np.arange(-len_lat_m, len_lat_m + val_m, val_m)
+    bin_mat = np.zeros([dy.size, dx.size, 2])
+    bin_map = np.zeros([dy.size, dx.size]).astype(int)
     n = 0
-    for j in range(lats.size):
-        delyinc = j * val + begy
-        delt = da.delta + delyinc
-        for i in range(lons.size):
-            azim = da.az + (begx + i * val) / cosd(delyinc)
-            glat, glon = latlon_from(plat, plon, azim, delt)
-            if glon > 180:
-                glon -= 360
+    bin_loca = []
+    for j, dyy in enumerate(dy):
+        for i, dxx in enumerate(dx):
+            glon, glat = proj(dxx, dyy, inverse=True)
             bin_loca.append([glat, glon])
             bin_mat[j, i, 0] = glat
             bin_mat[j, i, 1] = glon
             bin_map[j, i] = n
-            n += 1
+            n += 1 
     return np.array(bin_loca), bin_mat, bin_map
 
 
 def bin_shape(cpara):
     if cpara.shape == 'rect':
         raise ValueError('The shape of bins must be set to \'circle\' in ccp3d mode.')
     if cpara.bin_radius is None:
```

### Comparing `python-seispy-1.3.3/seispy/ccppara.py` & `python-seispy-1.3.4/seispy/ccppara.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 from os.path import expanduser, join, dirname, exists
 import configparser
 from seispy.geo import km2deg
+from seispy.utils import scalar_instance
 import warnings
 
 
 class CCPPara(object):
     def __init__(self):
         self.rfpath = expanduser('~')
         self.rayp_lib = None
@@ -36,15 +37,15 @@
 
     @property
     def bin_radius(self):
         return self._bin_radius
 
     @bin_radius.setter
     def bin_radius(self, value):
-        if not (isinstance(value, (int, float)) or value is None):
+        if not (scalar_instance(value) or value is None):
             raise TypeError('Error type of bin_radius')
         else:
             self._bin_radius = value
 
     @property
     def shape(self):
         return self._shape
@@ -114,24 +115,28 @@
         # para for line section
         lat1 = cf.getfloat('line', 'profile_lat1')
         lon1 = cf.getfloat('line', 'profile_lon1')
         lat2 = cf.getfloat('line', 'profile_lat2')
         lon2 = cf.getfloat('line', 'profile_lon2')
         cpara.line = np.array([lat1, lon1, lat2, lon2])
     except:
-        warnings.warn('line section not found. Setup it for ccp_profile')
+        # warnings.warn('line section not found. Setup it for ccp_profile')
+        pass
     try:
         # para for center bins
         cla = cf.getfloat('spacedbins', 'center_lat')
         clo = cf.getfloat('spacedbins', 'center_lon')
         hlla = cf.getfloat('spacedbins', 'half_len_lat')
         hllo = cf.getfloat('spacedbins', 'half_len_lon')
         cpara.center_bin = [cla, clo, hlla, hllo, km2deg(cpara.slide_val)]
     except:
-        warnings.warn('No such section of spacedbins and line. Setup them for CCP stacking')
+        # warnings.warn('No such section of spaced bins. Setup them for ccp3d')
+        pass
+    if cpara.line.size == 0 and len(cpara.center_bin) == 0:
+        raise ValueError('Please setup line or spacedbins section')
     # para for depth section
     dep_end = cf.getfloat('depth', 'dep_end')
     cpara.dep_val = cf.getfloat('depth', 'dep_val')
     try:
         cpara.phase = cf.getint('depth', 'phase')
     except:
         cpara.phase = 1
```

### Comparing `python-seispy-1.3.3/seispy/ccpprofile.py` & `python-seispy-1.3.4/seispy/ccpprofile.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,44 @@
 import numpy as np
-import seispy
-from seispy.geo import km2deg, deg2km, latlon_from, geoproject, sind, rad2deg, skm2srad
+from seispy.geo import km2deg, deg2km, latlon_from, \
+                       geoproject, sind, rad2deg, skm2srad, \
+                       geo2sph, sph2geo
 from seispy.setuplog import setuplog
 from seispy.distaz import distaz
 from seispy.rfcorrect import DepModel
 from seispy.rf2depth_makedata import Station
 from seispy.ccppara import ccppara, CCPPara
 from scikits.bootstrap import ci
 from seispy.ccp3d import boot_bin_stack
-from seispy.utils import check_stack_val, read_rfdep, create_center_bin_profile
+from seispy.utils import check_stack_val, read_rfdep
+from scipy.interpolate import interp1d
 from os.path import exists, dirname, basename, join
+import sys
+
+
+def prof_range(lat, lon):
+    dis = [0]
+    for i in range(lat.size-1):
+        dis.append(distaz(lat[i], lon[i], lat[i+1], lon[i+1]).degreesToKilometers())
+    return np.cumsum(dis)
+
+
+def create_center_bin_profile(stations, val=5, method='linear'):
+    if not isinstance(stations, Station):
+        raise TypeError('Stations should be seispy.rf2depth_makedata.Station')
+    dis_sta = prof_range(stations.stla, stations.stlo)
+    dis_inter = np.append(np.arange(0, dis_sta[-1], val), dis_sta[-1])
+    r, theta, phi = geo2sph(np.zeros(stations.stla.size), stations.stla, stations.stlo)
+    # t_po = np.arange(stations.stla.size)
+    # ip_t_po = np.linspace(0, stations.stla.size, bin_num)
+    theta_i = interp1d(dis_sta, theta, kind=method, bounds_error=False, fill_value='extrapolate')(dis_inter)
+    phi_i = interp1d(dis_sta, phi, kind=method, bounds_error=False, fill_value='extrapolate')(dis_inter)
+    _, lat, lon = sph2geo(r, theta_i, phi_i)
+    # dis = prof_range(lat, lon)
+    return lat, lon, dis_inter
 
 
 def line_proj(lat1, lon1, lat2, lon2):
     daz = distaz(lat1, lon1, lat2, lon2)
     az1_begin = (daz.baz - 90) % 360
     az2_begin = (daz.baz + 90) % 360
     az1_end = (daz.az - 90) % 360
@@ -142,40 +167,40 @@
                 try:
                     idx = self.staname.index(sta)
                     self.idxs.append(idx)
                 except ValueError:
                     self.logger.CCPlog.warning('{} does not in RFdepth structure'.format(sta))
                 if self.cpara.shape == 'rect' and self.cpara.adaptive == False:
                     self._pierce_project(self.rfdep[idx])
-        elif self.cpara.width is None and self.cpara.shape == 'circle':
+        elif self.cpara.shape == 'circle':
+            if self.cpara.width is not None:
+                self.logger.CCPlog.warning('The \'width\' will be ignored, when circle bin was set')
             dep_mod = DepModel(self.cpara.stack_range)
             x_s = np.cumsum((dep_mod.dz / dep_mod.R) / np.sqrt((1. / (skm2srad(0.085) ** 2. * (dep_mod.R / dep_mod.vs) ** -2)) - 1))
             dis = self.fzone[-1] + rad2deg(x_s[-1]) + 0.3
             # self.idxs = self._proj_sta(dis)
             self.idxs = []
             for i, bin_info in enumerate(self.bin_loca):
                 self.idxs.append(np.where(distaz(bin_info[0], bin_info[1], self.stalst[:, 0], self.stalst[:, 1]).delta <= dis)[0])
         elif self.cpara.width is not None and self.cpara.shape == 'rect':
             self.logger.CCPlog.info('Select stations within {} km perpendicular to the profile'.format(self.cpara.width))
             self.idxs = self._proj_sta(self.cpara.width)
-            self._write_sta()  
+            for idx in self.idxs:
+                self._pierce_project(self.rfdep[idx])      
+            if self.cpara.stack_sta_list != '':
+                self._write_sta()  
         else:
-            if self.cpara.width is not None:
-                self.logger.CCPlog.error('Width of profile was set, the bin shape of {} is invalid'.format(self.cpara.shape))
-                raise ValueError('Width of profile was set, the bin shape of {} is invalid'.format(self.cpara.shape))
-            else:
-                self.logger.CCPlog.error('Width of profile was not set, the bin shape of {} is invalid'.format(self.cpara.shape))
-                raise ValueError('Width of profile was not set, the bin shape of {} is invalid'.format(self.cpara.shape))
+            self.logger.CCPlog.error('Width of profile was not set, the bin shape of {} is invalid'.format(self.cpara.shape))
+            sys.exit(1)
 
     def _write_sta(self):
         with open(self.cpara.stack_sta_list, 'w') as f:
             for idx in self.idxs:
                 f.write('{}\t{:.3f}\t{:.3f}\n'.format(self.staname[idx],
                 self.stalst[idx,0], self.stalst[idx, 1]))
-                self._pierce_project(self.rfdep[idx])      
 
     def _proj_sta(self, width):
         az1_begin, az2_begin, az1_end, az2_end, daz = line_proj(*self.cpara.line)
         az_sta_begin = distaz(self.stalst[:, 0], self.stalst[:, 1], self.cpara.line[0], self.cpara.line[1]).az
         az_sta_end = distaz(self.stalst[:, 0], self.stalst[:, 1], self.cpara.line[2], self.cpara.line[3]).az
         if 0 <= daz.baz < 90 or 270 <= daz.baz < 360:
             tmp_idx_begin = np.where(((az1_begin < az_sta_begin)&(az_sta_begin < 360)) | ((0 < az_sta_begin)&(az_sta_begin < az2_begin)))[0]
@@ -188,15 +213,15 @@
         sta_daz = distaz(self.stalst[:, 0], self.stalst[:, 1], self.cpara.line[0], self.cpara.line[1])
         sta_dis = sind(daz.baz-sta_daz.az) * sta_daz.degreesToKilometers()
         proj_idx = np.where(np.abs(sta_dis) < width)[0]
         tmp_idx = np.intersect1d(tmp_idx_begin, tmp_idx_end)
         final_idx = np.intersect1d(tmp_idx, proj_idx).astype(int)
         if not final_idx.any():
             self.logger.CCPlog.error('No stations within the profile belt with width of {}'.format(width))
-            raise ValueError('Satisfied stations not found')
+            sys.exit(1)
         return final_idx
 
     def _pierce_project(self, rfsta):
         rfsta['projlat'] = np.zeros_like(rfsta['piercelat'])
         rfsta['projlon'] = np.zeros_like(rfsta['piercelon'])
         for i, dep in enumerate(self.cpara.depth_axis):
             rfsta['projlat'][:, i], rfsta['projlon'][:, i] = geoproject(rfsta['piercelat'][:, i], rfsta['piercelon'][:, i], *self.cpara.line)
@@ -214,15 +239,15 @@
             pass
         for i, bin_info in enumerate(self.bin_loca):
             boot_stack = {}
             bin_mu = np.zeros(self.cpara.stack_range.size)
             bin_ci = np.zeros([self.cpara.stack_range.size, 2])
             bin_count = np.zeros(self.cpara.stack_range.size)
             self.logger.CCPlog.info('{}/{} bin from {:.2f} km at lat: {:.3f} lon: {:.3f}'.format(i + 1, self.bin_loca.shape[0], self.profile_range[i], bin_info[0], bin_info[1]))
-            if self.cpara.width is None and self.cpara.shape == 'circle':
+            if self.cpara.shape == 'circle' and not exists(self.cpara.stack_sta_list):
                 idxs = self.idxs[i]
             else:
                 idxs = self.idxs
             for j, dep in enumerate(self.cpara.stack_range):
                 idx = int(j * self.stack_mul + self.cpara.stack_range[0]/self.cpara.dep_val)
                 bin_dep_amp = np.array([])
                 for k in idxs:
@@ -258,19 +283,27 @@
         if format == 'npz':
             np.savez(self.cpara.stackfile, cpara=self.cpara, stack_data=self.stack_data)
         elif format == 'dat':
             with open(self.cpara.stackfile, 'w') as f:
                 for i, bin in enumerate(self.stack_data):
                     for j, dep in enumerate(self.cpara.stack_range):
                         if dep == self.cpara.stack_range[-1]:
-                            f.write('{:.4f}\t{:.4f}\t{:.4f}\t{:.2f} nan nan nan nan\n'.format(bin['bin_lat'], bin['bin_lon'],
-                                                                                              self.profile_range[i], dep))
+                            f.write(
+                                '{:.4f}\t{:.4f}\t{:.4f}\t{:.2f} nan nan nan nan\n'.format(
+                                    bin['bin_lat'], bin['bin_lon'],
+                                    self.profile_range[i], dep
+                                )
+                            )
                         else:
-                            f.write('{:.4f}\t{:.4f}\t{:.4f}\t{:.2f}\t{:.4f}\t{:.4f}\t{:.4f}\t{:d}\n'.format(bin['bin_lat'], bin['bin_lon'],
-                                                                                    self.profile_range[i],
-                                                                                    dep, bin['mu'][j], bin['ci'][j, 0],
-                                                                                    bin['ci'][j, 1], int(bin['count'][j])))
+                            f.write(
+                                '{:.4f}\t{:.4f}\t{:.4f}\t{:.2f}\t{:.4f}\t{:.4f}\t{:.4f}\t{:d}\n'.format(
+                                    bin['bin_lat'], bin['bin_lon'],
+                                    self.profile_range[i],
+                                    dep, bin['mu'][j], bin['ci'][j, 0],
+                                    bin['ci'][j, 1], int(bin['count'][j])
+                                )
+                            )
 
 
 if __name__ == '__main__':
     bin_loca, _ = init_profile(27.5, 94, 36.5, 92, 5)
     print(bin_loca.shape)
```

### Comparing `python-seispy-1.3.3/seispy/data/EventCMT.dat` & `python-seispy-1.3.4/seispy/data/EventCMT.dat`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.3/seispy/data/cmpVsVp.txt` & `python-seispy-1.3.4/seispy/data/cmpVsVp.txt`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.3/seispy/data/cyan.mat` & `python-seispy-1.3.4/seispy/data/cyan.mat`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.3/seispy/data/iasp91.vel` & `python-seispy-1.3.4/seispy/data/iasp91.vel`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.3/seispy/data/mtna.vel` & `python-seispy-1.3.4/seispy/data/mtna.vel`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.3/seispy/data/prem.vel` & `python-seispy-1.3.4/seispy/data/prem.vel`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.3/seispy/data/saveicon.png` & `python-seispy-1.3.4/seispy/data/saveicon.png`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.3/seispy/data/seispy.png` & `python-seispy-1.3.4/seispy/data/seispy.png`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.3/seispy/decon.py` & `python-seispy-1.3.4/seispy/decon.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 # -*- coding: utf-8 -*-
 import numpy as np
 import obspy
-from obspy.io.sac import SACTrace
 from obspy.signal.util import next_pow_2
-from math import pi
-from numpy.fft import fft, ifft, ifftshift
+from numpy.fft import fft, ifft
 # from scipy.linalg import solve_toeplitz
-import matplotlib.pyplot as plt
 
 
 def gaussFilter(dt, nft, f0):
     df = 1.0 / (nft * dt)
     nft21 = 0.5 * nft + 1
     f = df * np.arange(0, nft21)
-    w = 2 * pi * f
+    w = 2 * np.pi * f
 
     gauss = np.zeros([nft, 1])
     gauss1 = np.exp(-0.25 * (w / f0) ** 2) / dt
     gauss1.shape = (len(gauss1), 1)
     gauss[0:int(nft21)] = gauss1
     gauss[int(nft21):] = np.flipud(gauss[1:int(nft21) - 1])
     gauss = gauss[:, 0]
@@ -37,17 +34,17 @@
     x = x.real
     return x
 
 
 def phaseshift(x, nfft, dt, tshift):
     Xf = fft(x, nfft)
     shift_i = int(tshift / dt)
-    p = 2 * pi * np.arange(1, nfft + 1) * shift_i / nfft
+    p = 2 * np.pi * np.arange(1, nfft + 1) * shift_i / nfft
     Xf = Xf * np.vectorize(complex)(np.cos(p), -np.sin(p))
-    x = ifft(Xf, nfft) / np.cos(2 * pi * shift_i / nfft)
+    x = ifft(Xf, nfft) / np.cos(2 * np.pi * shift_i / nfft)
     x = x.real
     return x
 
 
 def deconit(uin, win, dt, nt=None, tshift=10, f0=2.0, itmax=400, minderr=0.001, phase='P'):
     """
     Created on Wed Sep 10 14:21:38 2014
@@ -160,15 +157,15 @@
         raise ValueError('The length of the \'uin\' must be same as the \'win\'')
     nt = uin.size
     nft = next_pow_2(nt)
     nfpts = nft / 2 + 1     # number of freq samples
     fny = 1. / (2.* dt);     # nyquist
     delf = fny / (0.5 * nft)
     freq = delf * np.arange(nfpts)
-    w = 2 * pi * freq
+    w = 2 * np.pi * freq
 
     # containers
     # rff = np.zeros(nft); # Rfn in freq domain
     upf = np.zeros(nft); # predicted numer in freq domain
 
     # Convert seismograms to freq domain
     uf = fft(uin, nft)
```

### Comparing `python-seispy-1.3.3/seispy/distaz.py` & `python-seispy-1.3.4/seispy/distaz.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         """
         rhs1 = (aa - d) * (aa - d) + (bb - e) * (bb - e) + cc * cc - 2.
         rhs2 = (aa - g) * (aa - g) + (bb - h) * (bb - h) + (cc - k) * (cc - k) - 2.
         dbaz = np.arctan2(rhs1, rhs2)
 
         dbaz_idx = np.where(dbaz < 0.0)[0]
         if len(dbaz_idx) != 0:
-            if isinstance(dbaz, (int, float)):
+            if isinstance(dbaz, (int, float, np.integer, np.floating)):
                 dbaz += 2 * math.pi
             else:
                 dbaz[dbaz_idx] += 2 * math.pi
 
         self.baz = dbaz / rad
         """
 	c
```

### Comparing `python-seispy-1.3.3/seispy/eq.py` & `python-seispy-1.3.4/seispy/eq.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from obspy.io.sac import SACTrace
 from obspy.signal.rotate import rotate2zne, rotate_zne_lqt
 from scipy.signal import resample
 from os.path import join
 from seispy.decon import RFTrace
 from seispy.geo import snr, srad2skm, rotateSeisENtoTR, \
                        rssq, extrema
+from seispy.utils import scalar_instance
 from obspy.signal.trigger import recursive_sta_lta
 import glob
 
 
 class NotEnoughComponent(Exception):
     def __init__(self, matchkey):
         self.matchkey = matchkey
@@ -319,15 +320,15 @@
             Minium residual error, valid for method of ``iter``, by default 0.001
         wlevel : float, optional
             Water level, valid for method of ``water``, by default 0.05
         target_dt : None or float, optional
             Time delta for resampling, by default None
         """
         self.method = method
-        if isinstance(f0, (int, float)):
+        if scalar_instance(f0):
             f0 = [f0]
         for ff in f0:
             if method == 'iter':
                 kwargs = {'method': method,
                         'f0': ff,
                         'tshift': shift,
                         'itmax': itmax,
```

### Comparing `python-seispy-1.3.3/seispy/geo.py` & `python-seispy-1.3.4/seispy/geo.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
-from numpy import pi, mod
 from seispy import distaz
+from pyproj import Geod
+from seispy.utils import scalar_instance, array_instance
 
 def sind(deg):
     rad = np.radians(deg)
     return np.sin(rad)
 
 
 def cosd(deg):
@@ -35,45 +36,45 @@
 def atand(x):
     rad = np.arctan(x)
     return np.degrees(rad)
 
 
 def km2deg(km):
     radius = 6371
-    circum = 2*pi*radius
+    circum = 2*np.pi*radius
     conv = circum / 360
     deg = km / conv
     return deg
 
 
 def deg2km(deg):
     radius = 6371
-    circum = 2*pi*radius
+    circum = 2*np.pi*radius
     conv = circum / 360
     km = deg * conv
     return km
 
 
 def rad2deg(rad):
-    deg = rad*(360/(2*pi))
+    deg = rad*(360/(2*np.pi))
     return deg
 
 
 def skm2sdeg(skm):
     sdeg = skm * deg2km(1)
     return sdeg
 
 
 def sdeg2skm(sdeg):
     skm = sdeg / deg2km(1)
     return skm
 
 
 def srad2skm(srad):
-    sdeg = srad * ((2*pi)/360)
+    sdeg = srad * ((2*np.pi)/360)
     return sdeg / deg2km(1)
 
 
 def skm2srad(skm):
     sdeg = skm * deg2km(1)
     return rad2deg(sdeg)
 
@@ -87,23 +88,23 @@
     
     :param bazi: back-azimuth of station-event pair
     :param inc: Incidence angle
     :return: Coefficient matrix M
     
     """
 
-    if isinstance(inc, float) or isinstance(inc, int):
+    if scalar_instance(inc):
         value31 = 0
-    elif isinstance(inc, np.ndarray):
+    elif array_instance(inc):
         value31 = np.repeat(0, len(inc))
     else:
         raise TypeError('Input args sould be in \'float\', \'int\', or \'numpy.ndarray\'')
 
-    inc = inc / 180 * pi
-    bazi = bazi / 180 * pi
+    inc = inc / 180 * np.pi
+    bazi = bazi / 180 * np.pi
 
     M = np.array([[np.cos(inc), -np.sin(inc)*np.sin(bazi), -np.sin(inc)*np.cos(bazi)],
                   [np.sin(inc), np.cos(inc)*np.sin(bazi), np.cos(inc)*np.cos(bazi)],
                   [value31, -np.cos(bazi), np.sin(bazi)]])
     return M
 
 
@@ -120,15 +121,15 @@
     x = r * sind(cola) * cosd(lon)
     y = r * sind(cola) * sind(lon)
     z = r * cosd(cola)
     return x, y, z
 
 
 def rotateSeisENtoTR(E, N, BAZ):
-    angle = mod(BAZ+180, 360)
+    angle = np.mod(BAZ+180, 360)
     R = N*cosd(angle) + E*sind(angle)
     T = E*cosd(angle) - N*sind(angle)
     return T, R
 
 
 def rssq(x):
     return np.sqrt(np.sum(x**2)/len(x))
@@ -138,44 +139,99 @@
     spow = rssq(x)**2
     npow = rssq(y)**2
     if npow == 0:
         npow = 0.001
     return 10 * np.log10(spow / npow)
 
 
-def latlon_from(lat1, lon1, azimuth, gcarc_dist):
-    lat2 = asind((sind(lat1) * cosd(gcarc_dist)) + (cosd(lat1) * sind(gcarc_dist) * cosd(azimuth)))
-    if isinstance(gcarc_dist, np.ndarray):
-        lon2 = np.zeros_like(lat2)
-        for n in range(len(gcarc_dist)):
-            if cosd(gcarc_dist[n]) >= (cosd(90 - lat1) * cosd(90 - lat2[n])):
-                lon2[n] = lon1 + asind(sind(gcarc_dist[n]) * sind(azimuth) / cosd(lat2[n]))
-            else:
-                lon2[n] = lon1 + asind(sind(gcarc_dist[n]) * sind(azimuth) / cosd(lat2[n])) + 180
-    elif isinstance(azimuth, np.ndarray):
-        lon2 = np.zeros_like(lat2)
-        for n in range(len(azimuth)):
-            if cosd(gcarc_dist) >= (cosd(90 - lat1) * cosd(90 - lat2[n])):
-                lon2[n] = lon1 + asind(sind(gcarc_dist) * sind(azimuth[n]) / cosd(lat2[n]))
+def latlon_from(lat0, lon0, azimuth, gcarc_dist, ellps="WGS84"):
+    """
+    Determine position with given position of initial point, azimuth and distance
+
+    Accepted numeric scalar or array:
+    - :class:`int`
+    - :class:`float`
+    - :class:`numpy.floating`
+    - :class:`numpy.integer`
+    - :class:`list`
+    - :class:`tuple`
+    - :class:`array.array`
+    - :class:`numpy.ndarray`
+    - :class:`xarray.DataArray`
+    - :class:`pandas.Series`
+
+    :param lat0: Latitude of original point
+    :type lat0: float or array
+    :param lon0: Longitude of original point
+    :type lon0: float or array
+    :param azimuth: Azimuth(s) in degree
+    :type azimuth: float or array
+    :param gcarc_dist: Distance(s) between initial and terminus point(s) in degree
+    :type gcarc_dist: float or array
+    :param ellps: Ellipsoids supported by ``pyproj``, defaults to "WGS84"
+    :type ellps: :class:`str`, optional
+
+    Returns
+    -------
+    scalar or array:
+        Latitude(s) of terminus point(s)  
+    scalar or array:
+        Longitude(s) of terminus point(s)
+    """
+
+    def init_lalo(lat0, lon0, npts):
+        if hasattr(lat0, "__iter__") and hasattr(lon0, "__iter__"):
+            if len(lat0) != len(lon0):
+                raise ValueError('lat0 and lon0 must be in the same length')
+            elif len(lat0) != npts:
+                raise ValueError('initial points must be in the same length as azimuths')
+        elif scalar_instance(lat0) and scalar_instance(lon0):
+            lat1 = np.ones(npts) * lat0
+            lon1 = np.ones(npts) * lon0
+        else:
+            raise ValueError('lat0 and lon0 must be in the same length')
+        return lat1, lon1
+
+    if hasattr(azimuth, "__iter__") and hasattr(gcarc_dist, "__iter__"):
+        if len(azimuth) == len(gcarc_dist):
+            npts = len(azimuth)
+            init_lalo(lat0, lon0, npts)
+        else:
+            raise ValueError('azimuth and gcarc_dist must be in the same length')
+    elif scalar_instance(azimuth) and scalar_instance(gcarc_dist):
+        if hasattr(lat0, "__iter__") and hasattr(lon0, "__iter__"):
+            if len(lat0) != len(lon0):
+                raise ValueError('lat0 and lon0 must be in the same length')
             else:
-                lon2[n] = lon1 + asind(sind(gcarc_dist) * sind(azimuth[n]) / cosd(lat2[n])) + 180
-    else:
-        if (cosd(gcarc_dist) >= (cosd(90 - lat1) * cosd(90 - lat2))):
-            lon2 = lon1 + asind(sind(gcarc_dist) * sind(azimuth) / cosd(lat2))
+                azimuth = np.ones(lat0)*azimuth
+                gcarc_dist = np.ones(lat0)*gcarc_dist
+        elif scalar_instance(lat0) and scalar_instance(lon0):
+            pass
         else:
-            lon2 = lon1 + asind(sind(gcarc_dist) * sind(azimuth) / cosd(lat2)) + 180
-    return lat2, lon2
+            raise ValueError('lat0 and lon0 must be in the same length')            
+    elif scalar_instance(azimuth) and hasattr(gcarc_dist, "__iter__"):
+        npts = len(gcarc_dist)
+        azimuth = np.ones(npts)*azimuth
+        lat0, lon0 = init_lalo(lat0, lon0, npts)
+    elif scalar_instance(gcarc_dist) and hasattr(azimuth, "__iter__"):
+        npts = len(azimuth)
+        gcarc_dist = np.ones(lat0, lon0, npts)*gcarc_dist
+        lat0, lon0 = init_lalo(lat0, lon0, npts)
+
+    g = Geod(ellps=ellps)
+    lon, lat, _ = g.fwd(lon0, lat0, azimuth, deg2km(gcarc_dist)*1000)
+    return lat, lon
 
 
 def geoproject(lat_p, lon_p, lat1, lon1, lat2, lon2):
     azi = distaz(lat1, lon1, lat2, lon2).baz
     dis_center = distaz(lat1, lon1, lat_p, lon_p).delta
     azi_center = distaz(lat1, lon1, lat_p, lon_p).baz
     dis_along = atand(tand(dis_center))*cosd(azi-azi_center)
-    (lat, lon) = latlon_from(lat1, lon1, azi, dis_along)
+    lat, lon = latlon_from(lat1, lon1, azi, dis_along)
     return lat, lon
 
 
 def extrema(x, opt='max'):
     if opt == 'max':
         idx = np.intersect1d(np.where(np.diff(x) > 0)[0]+1, np.where(np.diff(x) < 0)[0])
     elif opt == 'min':
```

### Comparing `python-seispy-1.3.3/seispy/get_cpt.py` & `python-seispy-1.3.4/seispy/get_cpt.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.3/seispy/harmonics.py` & `python-seispy-1.3.4/seispy/harmonics.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from scipy.sparse.linalg import lsqr
 from seispy.geo import cosd, sind
 import matplotlib.pyplot as plt
 from obspy.io.sac import SACTrace
 from os.path import join
 
 
-
 class Harmonics():
     def __init__(self, rfsta, tmin=-5, tmax=10) -> None:
         """ Harmonic decomposition for extracting anisotropic and isotropic features from the radial and transverse RFs
 
         :param rfsta: data class of RFStation
         :type rfsta: :class:`seispy.rfcorrect.RFStation`
         :param tmin: Start time relative to P
```

### Comparing `python-seispy-1.3.3/seispy/hk.py` & `python-seispy-1.3.4/seispy/hk.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import numpy as np
 import re
 from obspy.io.sac.sactrace import SACTrace
 import matplotlib.pyplot as plt
-from os.path import dirname, join
+from os.path import join
 from seispy.rfcorrect import RFStation
 from seispy.hkpara import hkpara
 from seispy.geo import srad2skm
 import argparse
-from seispy.utils import load_cyan_map
+from seispy.utils import load_cyan_map, array_instance
 
 
 def transarray(array, axis=0):
-    if not isinstance(array, np.ndarray):
+    if not array_instance(array):
         raise ValueError('array should be `numpy.ndarray`')
     if len(array.shape) != 1:
         raise ValueError('array should be 1-d array')
     if axis == 0:
         return array.reshape(-1, array.shape[0])
     elif axis == 1:
         return array.reshape(array.shape[0], -1)
```

### Comparing `python-seispy-1.3.3/seispy/hkpara.py` & `python-seispy-1.3.4/seispy/hkpara.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from os.path import expanduser
 import configparser
 import numpy as np
-from seispy.utils import check_path
+from seispy.utils import check_path, array_instance
 
 
 class HKPara(object):
     def __init__(self):
         self.rfpath = expanduser('~')
         self.hkpath = expanduser('~')
         self.hklist = 'hk.dat'
@@ -20,26 +20,26 @@
 
     @property
     def hrange(self):
         return self._hrange
 
     @hrange.setter
     def hrange(self, value):
-        if not (isinstance(value, np.ndarray) or value is None):
+        if not (array_instance(value) or value is None):
             raise TypeError('Error type of hrange')
         else:
             self._hrange = value
 
     @property
     def krange(self):
         return self._krange
 
     @krange.setter
     def krange(self, value):
-        if not (isinstance(value, np.ndarray) or value is None):
+        if not (array_instance(value) or value is None):
             raise TypeError('Error type of krange')
         else:
             self._krange = value
 
 
 def hkpara(cfg_file):
     hpara = HKPara()
```

### Comparing `python-seispy-1.3.3/seispy/io.py` & `python-seispy-1.3.4/seispy/io.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,17 +23,25 @@
         if endtime-starttime < 365 * 86400:
             events += self.client.get_events(starttime=starttime,
                                             endtime=endtime,
                                             orderby='time-asc', **kwargs)
         else:
             chunk_length = 365 * 86400
             while starttime <= endtime:
-                events += self.client.get_events(starttime=starttime,
-                                                endtime=starttime + chunk_length,
+                if endtime-starttime < chunk_length:
+                    nowtime = endtime
+                else:
+                    nowtime=starttime + chunk_length
+                try:
+                    events += self.client.get_events(starttime=starttime,
+                                                endtime=nowtime,
                                                 orderby='time-asc', **kwargs)
+                except:
+                    starttime += chunk_length
+                    continue
                 if starttime + chunk_length > endtime:
                     chunk = endtime - starttime
                     if chunk <= 1:
                         break
                 starttime += chunk_length
 
         self.events = _cat2df(events)
```

### Comparing `python-seispy-1.3.3/seispy/mccc.py` & `python-seispy-1.3.4/seispy/mccc.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.3/seispy/modcreator.py` & `python-seispy-1.3.4/seispy/modcreator.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.3/seispy/para.py` & `python-seispy-1.3.4/seispy/para.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,16 @@
         self.offset = None
         self.tolerance = 210
         self.dateformat = '%Y.%j.%H.%M.%S'
         self.date_begin = obspy.UTCDateTime('19760101')
         self.date_end = obspy.UTCDateTime.now()
         self.magmin = 5.5
         self.magmax = 10
+        self.depthmin = 0.
+        self.depthmax = 800.
         self.dismin = 30
         self.dismax = 90
         self.ref_comp = 'BHZ'
         self.suffix = 'SAC'
         self.noisegate = 5
         self.noiselen = 50
         self.phase = 'P'
```

### Comparing `python-seispy-1.3.3/seispy/pickdepth/get_depth.py` & `python-seispy-1.3.4/seispy/pickdepth/get_depth.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.3/seispy/pickdepth/pickdepthui.py` & `python-seispy-1.3.4/seispy/pickdepth/pickdepthui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# import folium
 from .get_depth import GoodDepth
 from seispy.setuplog import setuplog
 from PySide6.QtCore import Qt
 from PySide6.QtWidgets import QApplication, QWidget, QHBoxLayout,\
                               QVBoxLayout, QSizePolicy, QGroupBox,\
                               QPushButton, QTableWidget, QLineEdit,\
                               QLabel, QAbstractItemView, QTableWidgetItem,\
```

### Comparing `python-seispy-1.3.3/seispy/pickrf/pickfigure.py` & `python-seispy-1.3.4/seispy/pickrf/pickfigure.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from curses import window
 import glob
 import os
 import sys
 import obspy
 import numpy as np
 import matplotlib.pyplot as plt
+import pandas as pd
 from matplotlib.figure import Figure
 from os.path import join, basename
 from seispy.setuplog import setuplog
 from seispy.plotRT import init_figure, set_fig, plot_waves
 
 
 def indexpags(evt_num, maxidx=20):
@@ -125,16 +125,16 @@
         self.axt.set_title("T component")
         self.axb.set_xlabel("Backazimuth (\N{DEGREE SIGN})")
         self.axg.set_xlabel('Distance (\N{DEGREE SIGN})')
 
     def read_sac(self, dt=0.1, order='baz'):
         if not isinstance(order, str):
             raise TypeError('The order must be str type')
-        elif not order in ['baz', 'dis']:
-            raise ValueError('The order must be \'baz\' or \'dis\'')
+        elif not order in ['baz', 'dis', 'date']:
+            raise ValueError('The order must be \'baz\', \'dis\' or \'date\'')
         else:
             pass
         if len(glob.glob(join(self.rfpath, '*P_R.sac'))) != 0:
             tmp_files = glob.glob(join(self.rfpath, '*P_R.sac'))  
             self.comp = 'R'
         elif len(glob.glob(join(self.rfpath, '*P_Q.sac'))) != 0:
             tmp_files = glob.glob(join(self.rfpath, '*P_Q.sac'))
@@ -166,22 +166,24 @@
                           self.staname, self.rrf[0].stats.sac.stla, self.rrf[0].stats.sac.stlo), fontsize=20)
 
     def _sort(self, order):
         if order == 'baz':
             idx = np.argsort(self.baz)
         elif order == 'dis':
             idx = np.argsort(self.gcarc)
+        elif order == 'date':
+            idx = pd.to_datetime(self.filenames, format='%Y.%j.%H.%M.%S').argsort()
         else:
             pass
         self.baz = self.baz[idx]
         self.gcarc = self.gcarc[idx]
         self.phases = [self.phases[i] for i in idx]
         self.rrf = obspy.Stream([self.rrf[i] for i in idx])
-        self.trf = obspy.Stream([self.trf[i] for i in idx])
-        # self.gcarc = [self.rrf[i].stats.sac.gcarc for i in range(self.evt_num)]
+        if hasattr(self, 'trf'):
+            self.trf = obspy.Stream([self.trf[i] for i in idx])
         self.filenames = [self.filenames[i] for i in idx]
 
     def plotwave(self):
         bound = np.zeros(self.time_axis.shape[0])
         for i in range(self.evt_num):
             r_amp_axis = self.rrf[i].data*self.enf+i+1
             t_amp_axis = self.trf[i].data*self.enf+i+1
```

### Comparing `python-seispy-1.3.3/seispy/pickrf/pickui.py` & `python-seispy-1.3.4/seispy/pickrf/pickui.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
         self.layout.addLayout(ctrl_layout)
 
 
 def main():
     parser = argparse.ArgumentParser(description="User interface for picking PRFs")
     parser.add_argument('rf_path', type=str, help='Path to PRFs')
     parser.add_argument('-a', help='Arrangement of RFs, defaults to \'baz\'', dest='order',
-                        default='baz', type=str, metavar='baz|dis')
+                        default='baz', type=str, metavar='baz|dis|date')
     parser.add_argument('-x', help="Set x limits of the current axes, defaults to 30s for RT, 85s for R.",
                         dest='xlim', default=None, type=float, metavar='xmax')
     arg = parser.parse_args()
     rfpath = arg.rf_path
     if not exists(rfpath):
         raise FileNotFoundError('No such directory of {}'.format(rfpath))
     if len(glob.glob(join(rfpath, '*_T.sac'))) == 0:
```

### Comparing `python-seispy-1.3.3/seispy/pickrf/rpickfigure.py` & `python-seispy-1.3.4/seispy/pickrf/rpickfigure.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
         self.axr = self.fig.add_axes([0.15, 0.05, 0.55, 0.84])
         self.axb = self.fig.add_axes([0.755, 0.05, 0.22, 0.84])
         self.axg = self.axb.twiny()
     
     def read_sac(self, dt=0.1, order='baz'):
         if not isinstance(order, str):
             raise TypeError('The order must be str type')
-        elif not order in ['baz', 'dis']:
-            raise ValueError('The order must be \'baz\' or \'dis\'')
+        elif not order in ['baz', 'dis', 'date']:
+            raise ValueError('The order must be \'baz\', \'dis\' or \'date\'')
         else:
             pass
         if len(glob.glob(join(self.rfpath, '*P_R.sac'))) != 0:
             tmp_files = glob.glob(join(self.rfpath, '*_R.sac'))  
             self.comp = 'R'
         elif len(glob.glob(join(self.rfpath, '*P_Q.sac'))) != 0:
             tmp_files = glob.glob(join(self.rfpath, '*P_Q.sac'))
@@ -59,27 +59,26 @@
         self.gcarc = np.array([tr.stats.sac.gcarc for tr in self.rrf])
         self.rayp = np.array([tr.stats.sac.user0 for tr in self.rrf])
         self._sort(order)
         self.axpages, self.rfidx = indexpags(self.evt_num, self.maxidx)
         self.staname = (self.rrf[0].stats.network+'.'+self.rrf[0].stats.station).strip('.')
         self.fig.suptitle("%s (Latitude: %5.2f\N{DEGREE SIGN}, Longitude: %5.2f\N{DEGREE SIGN})" % (self.staname, self.rrf[0].stats.sac.stla, self.rrf[0].stats.sac.stlo), fontsize=20)
 
-    def _sort(self, order):
-        if order == 'baz':
-            idx = np.argsort(self.baz)
-        elif order == 'dis':
-            idx = np.argsort(self.gcarc)
-        else:
-            pass
-        self.baz = self.baz[idx]
-        self.gcarc = self.gcarc[idx]
-        self.phases = [self.phases[i] for i in idx]
-        self.rrf = obspy.Stream([self.rrf[i] for i in idx])
-        # self.gcarc = [self.rrf[i].stats.sac.gcarc for i in range(self.evt_num)]
-        self.filenames = [self.filenames[i] for i in idx]
+    # def _sort(self, order):
+    #     if order == 'baz':
+    #         idx = np.argsort(self.baz)
+    #     elif order == 'dis':
+    #         idx = np.argsort(self.gcarc)
+    #     else:
+    #         pass
+    #     self.baz = self.baz[idx]
+    #     self.gcarc = self.gcarc[idx]
+    #     self.phases = [self.phases[i] for i in idx]
+    #     self.rrf = obspy.Stream([self.rrf[i] for i in idx])
+    #     self.filenames = [self.filenames[i] for i in idx]
 
     def set_figure(self):
         self.axr.grid(visible=True, which='major', axis='x')
         self.axb.grid(visible=True, which='major')
         self.axr.set_ylabel("Event")
         self.axr.set_xlabel("Time after P (s)")
         self.axr.set_title("{} component".format(self.comp))
```

### Comparing `python-seispy-1.3.3/seispy/pickseis/sviewerui.py` & `python-seispy-1.3.4/seispy/pickseis/sviewerui.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.3/seispy/plotR.py` & `python-seispy-1.3.4/seispy/plotR.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.3/seispy/plotRT.py` & `python-seispy-1.3.4/seispy/plotRT.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.3/seispy/psrayp.py` & `python-seispy-1.3.4/seispy/psrayp.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.3/seispy/recalrf.py` & `python-seispy-1.3.4/seispy/recalrf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from seispy.rf import RF, datestr2regex, SACFileNotFoundError
 from seispy.eq import EQ
+from seispy.utils import scalar_instance
 import numpy as np
 from obspy import UTCDateTime
 from datetime import timedelta
 import pandas as pd
 import glob
 from os.path import join
 import re
@@ -19,15 +20,15 @@
         raise SACFileNotFoundError(join(pathname, '*{0}*{1}'.format(ref_comp, suffix)))
     sac_files = []
     for ref_sac in ref_eqs:
         try:
             datestr = re.findall(pattern, ref_sac)[0]
         except IndexError:
             raise IndexError('Error data format of {} in {}'.format(dateformat, ref_sac))
-        if isinstance(offset, (int, float)):
+        if scalar_instance(offset):
             sac_files.append([datestr, UTCDateTime.strptime(datestr, dateformat), -offset])
         elif offset is None:
             try:
                 tr = obspy.read(ref_sac)[0]
             except TypeError:
                 continue
             sac_files.append([datestr, tr.stats.starttime-tr.stats.sac.b, tr.stats.sac.o])
```

### Comparing `python-seispy-1.3.3/seispy/rf.py` & `python-seispy-1.3.4/seispy/rf.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from os import makedirs
 from seispy.io import Query, _cat2df
 from seispy.para import RFPara
 from seispy import distaz
 from seispy.eq import EQ
 from seispy.setuplog import setuplog
 from seispy.catalog import read_catalog_file
+from seispy.utils import scalar_instance
 import glob
 import numpy as np
 from datetime import timedelta
 import pandas as pd
 import configparser
 import argparse
 import sys
@@ -66,15 +67,16 @@
     pattern = pattern.replace('%H', r'\d{2}')
     pattern = pattern.replace('%M', r'\d{2}')
     pattern = pattern.replace('%S', r'\d{2}')
     return pattern
 
 
 def read_catalog(logpath:str, b_time, e_time, stla:float, stlo:float,
-                 magmin=5.5, magmax=10., dismin=30., dismax=90.):
+                 magmin=5.5, magmax=10., dismin=30., dismax=90.,
+                 depthmin=0, depthmax=800):
     """Read local catalog with seispy or QUAKEML format
 
     :param logpath: Path to catalogs
     :type logpath: str
     :param b_time: Start time 
     :type b_time: obspy.UTCDateTime
     :param e_time: End time
@@ -98,14 +100,15 @@
         eq_lst = read_catalog_file(logpath)
     except:
         events = read_events(logpath, 'QUAKEML')
         eq_lst = _cat2df(events)
     dis = distaz(stla, stlo, eq_lst['evla'], eq_lst['evlo']).delta
     eq_lst = eq_lst[(eq_lst['date']>=b_time) & (eq_lst['date']<=e_time) & \
                     (eq_lst['mag']>=magmin) & (eq_lst['mag']<=magmax) & \
+                    (eq_lst['evdp']>=depthmin) & (eq_lst['evdp']<=depthmax) & \
                     (dis>=dismin) & (dis<=dismax)]
     return eq_lst
 
 
 def fetch_waveform(eq_lst, para, model, logger):
     tb = np.max([2*para.noiselen, 2*para.time_before])
     te = np.max([2*para.noiselen, 2*para.time_after])
@@ -238,29 +241,36 @@
     def date_end(self):
         return self.para.date_end
 
     @date_end.setter
     def date_end(self, value):
         self.para.date_end = value
 
-    def load_stainfo(self):
+    def load_stainfo(self, use_date_range=True):
         try:
             if self.para.use_remote_data:
                 self.logger.RFlog.info('Load station info of {}.{} from {} web-service'.format(
                     self.para.stainfo.network, self.para.stainfo.station, self.para.data_server))
-                self.para.stainfo.get_station_from_ws(self.para.data_server)
+                if use_date_range:
+                    self.para.stainfo.get_station_from_ws(
+                        self.para.data_server,
+                        starttime=self.para.date_begin,
+                        endtime=self.para.date_end
+                    )
+                else:
+                    self.para.stainfo.get_station_from_ws(self.para.data_server)
                 try:
                     self.para._check_date_range()
                 except Exception as e:
                     self.logger.RFlog.error('{}'.format(e))
                     sys.exit(1)
             else:
                 self.logger.RFlog.info('Load station info from {0}'.format(self.para.datapath))
                 self.para.stainfo.load_stainfo(self.para.datapath, self.para.ref_comp, self.para.suffix)
-            self.logger.RFlog.info('{}/{}, latitude: {:.3f}, longiture: {:.3f}'.format(
+            self.logger.RFlog.info('{}.{}, latitude: {:.3f}, longitude: {:.3f}'.format(
                 self.para.stainfo.network, self.para.stainfo.station, self.stainfo.stla, self.stainfo.stlo))
         except Exception as e:
             self.logger.RFlog.error('Error in loading station info: {0}'.format(e))
             sys.exit(1)
 
     def search_eq(self, local=False, catalog=None):
         if not local:
@@ -268,27 +278,30 @@
                 self.logger.RFlog.info('Searching earthquakes from {}'.format(self.para.cata_server))
                 if self.para.date_end > UTCDateTime():
                     self.para.date_end = UTCDateTime()
                 query = Query(self.para.cata_server)
                 query.get_events(starttime=self.para.date_begin, endtime=self.para.date_end,
                                  latitude=self.para.stainfo.stla, longitude=self.para.stainfo.stlo,
                                  minmagnitude=self.para.magmin, maxmagnitude=self.para.magmax,
-                                 minradius=self.para.dismin, maxradius=self.para.dismax, catalog=catalog)
+                                 minradius=self.para.dismin, maxradius=self.para.dismax, 
+                                 mindepth=self.para.depthmin, maxdepth=self.para.depthmax,
+                                 catalog=catalog)
                 self.eq_lst = query.events
             except Exception as e:
                 raise ConnectionError(e)
         else:
             try:
                 self.logger.RFlog.info(
                     'Searching earthquakes from {0} to {1}'.format(self.date_begin.strftime('%Y.%m.%dT%H:%M:%S'),
                                                                    self.date_end.strftime('%Y.%m.%dT%H:%M:%S')))
                 self.eq_lst = read_catalog(self.para.catalogpath, self.para.date_begin, self.para.date_end,
                                            self.para.stainfo.stla, self.para.stainfo.stlo,
                                            magmin=self.para.magmin, magmax=self.para.magmax,
-                                           dismin=self.para.dismin, dismax=self.para.dismax)
+                                           dismin=self.para.dismin, dismax=self.para.dismax,
+                                           depthmin=self.para.depthmin, depthmax=self.para.depthmax)
             except Exception as e:
                 self.logger.RFlog.error('{0}'.format(e))
                 raise e
         self.logger.RFlog.info('{} earthquakes are found'.format(self.eq_lst.shape[0]))
 
     def match_eq(self):
         try:
@@ -418,22 +431,25 @@
                 drop_idx.append(i)
                 continue
             if search_inc:
                 self.logger.RFlog.info('The incidence angle of {} was corrected by {:.1f} deg'.format(
                                        row['data'].datestr, row['data'].inc_correction))
         self.eqs.drop(drop_idx, inplace=True)
 
-    def drop_eq_snr(self, length=None):
+    def drop_eq_snr(self, length=None, z_only=False):
         if length is None:
             length = self.para.noiselen
         self.logger.RFlog.info('Reject data record with SNR less than {0}'.format(self.para.noisegate))
         drop_lst = []
         for i, row in self.eqs.iterrows():
             snr_E, snr_N, snr_Z = row['data'].snr(length=length)
-            mean_snr = np.mean([snr_E, snr_N, snr_Z])
+            if z_only:
+                mean_snr = snr_Z
+            else:
+                mean_snr = np.mean([snr_E, snr_N, snr_Z])
             if mean_snr < self.para.noisegate:
                 drop_lst.append(i)
         self.eqs.drop(drop_lst, inplace=True)
         self.logger.RFlog.info('{0} events left after SNR calculation'.format(self.eqs.shape[0]))
 
     def trim(self):
         self.logger.RFlog.info('Trim waveforms from {0:.2f} before {2} to {1:.2f} after {2}'.format(
@@ -443,16 +459,17 @@
     
     def pick(self, prepick=True, stl=5, ltl=10):
         if prepick:
             self.logger.RFlog.info('Pre-pick {} arrival using STA/LTA method'.format(self.para.phase))
             for _, row in self.eqs.iterrows():
                 row['data'].phase_trigger(self.para.time_before, self.para.time_after,
                                           stl=stl, ltl=ltl)
-        self.logger.RFlog.info('{0} events left after virtual checking'.format(self.eqs.shape[0]))
         pickphase(self.eqs, self.para, self.logger)
+        self.logger.RFlog.info('{0} events left after visual checking'.format(self.eqs.shape[0]))
+
 
     def deconv(self):
         shift = self.para.time_before
         time_after = self.para.time_after
         drop_lst = []
 
         count = 0
@@ -479,15 +496,15 @@
         if self.para.phase[-1] == 'P':
             shift = self.para.time_before
         elif self.para.phase[-1] == 'S':
             shift = self.para.time_after
         else:
             pass
         good_lst = []
-        if isinstance(self.para.gauss, (int, float)):
+        if scalar_instance(self.para.gauss):
             gauss = self.para.gauss
         elif gauss is None:
             gauss = self.para.gauss[0]
         else:
             if gauss in self.para.gauss:
                 pass
             else:
```

### Comparing `python-seispy-1.3.3/seispy/rf2depth_makedata.py` & `python-seispy-1.3.4/seispy/rf2depth_makedata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from seispy.rfcorrect import RFStation, psrf2depth, Mod3DPerturbation, psrf_1D_raytracing,\
     psrf_3D_migration, time2depth, psrf_3D_raytracing
 import numpy as np
 from seispy.ccppara import ccppara
 from seispy.setuplog import setuplog
-from seispy.geo import latlon_from, deg2km, rad2deg
-from os.path import join, dirname, exists
+from seispy.geo import latlon_from, rad2deg
+from os.path import join, exists
 import argparse
 import sys
 import glob
 
 
 class Station(object):
     def __init__(self, sta_lst):
```

### Comparing `python-seispy-1.3.3/seispy/rfani.py` & `python-seispy-1.3.4/seispy/rfani.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import numpy as np
-from obspy.io.sac import SACTrace
 from matplotlib.ticker import MultipleLocator
 import matplotlib.pyplot as plt
-from os.path import join, abspath, dirname
+from os.path import join
 from seispy.geo import cosd, sind, extrema
 from scipy.interpolate import griddata
 from seispy.utils import load_cyan_map
 
 
 def joint_stack(energy_r, energy_cc, energy_tc, weight=[0.4, 0.3, 0.3]):
     energy_r = energy_r / np.max(energy_r)
```

### Comparing `python-seispy-1.3.3/seispy/rfcorrect.py` & `python-seispy-1.3.4/seispy/rfcorrect.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-from multiprocessing.sharedctypes import Value
 from obspy.io.sac.sactrace import SACTrace
 import numpy as np
 from scipy.interpolate import interp1d, interpn
 from scipy.signal import resample
 from os.path import dirname, join, exists, isfile, abspath
 from seispy.geo import skm2srad, sdeg2skm, rad2deg, latlon_from, \
                        asind, tand, srad2skm, km2deg
 from seispy.psrayp import get_psrayp
 from seispy.rfani import RFAni
 from seispy.slantstack import SlantStack
 from seispy.harmonics import Harmonics
 from seispy.plotRT import plotrt as _plotrt
 from seispy.plotR import plotr as _plotr
-from seispy.utils import DepModel, Mod3DPerturbation
+from seispy.utils import DepModel, Mod3DPerturbation, scalar_instance
 import warnings
 import glob
 
 
 class RFStation(object):
     def __init__(self, data_path, only_r=False, prime_comp='R'):
         """
@@ -128,17 +127,17 @@
         prime_comp : str, optional
              Prime component of RF, by default 'R'
         """
         if len(stream) == 0:
             raise ValueError('No such RFTrace read')
         rfsta = cls('', only_r=True, prime_comp=prime_comp)
         ev_num = len(stream)
-        if isinstance(rayp, float):
+        if scalar_instance(rayp):
             rayp = np.ones(ev_num)*rayp
-        if isinstance(baz, (float, int)):
+        if scalar_instance(baz):
             baz = np.ones(ev_num)*baz
         if ev_num != rayp.size or ev_num != baz.size:
             raise ValueError('Array length of rayp and baz must be the same as stream')
         rfsta.init_property(ev_num)
         try:
             rfsta.staname = '{}.{}'.format(stream[0].stats.sac.knetwk, stream[0].stats.sac.kstnm)
             rfsta.stla = stream[0].stats.sac.stla
@@ -631,14 +630,15 @@
     pplat_p = np.zeros([stadatar.ev_num, YAxisRange.shape[0]])
     pplon_p = np.zeros([stadatar.ev_num, YAxisRange.shape[0]])
     tps = np.zeros([stadatar.ev_num, YAxisRange.shape[0]])
     if srayp is None:
         for i in range(stadatar.ev_num):
             tps[i], x_s, x_p, raylength_s[i], raylength_p[i] = xps_tps_map(
                 dep_mod, stadatar.rayp[i], stadatar.rayp[i], is_raylen=True, sphere=sphere, phase=phase)
+            print(type(stadatar.bazi[i]), type(rad2deg(x_s)))
             pplat_s[i], pplon_s[i] = latlon_from(stadatar.stla, stadatar.stlo, stadatar.bazi[i], rad2deg(x_s))
             pplat_p[i], pplon_p[i] = latlon_from(stadatar.stla, stadatar.stlo, stadatar.bazi[i], rad2deg(x_p))
     elif isinstance(srayp, str) or isinstance(srayp, np.lib.npyio.NpzFile):
         if isinstance(srayp, str):
             if not exists(srayp):
                 raise FileNotFoundError('Ps rayp lib file not found')
             else:
```

### Comparing `python-seispy-1.3.3/seispy/scripts.py` & `python-seispy-1.3.4/seispy/scripts.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.3/seispy/seisfwd.py` & `python-seispy-1.3.4/seispy/seisfwd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 from scipy.fftpack import ifft
 from obspy.signal.util import next_pow_2
+from seispy.utils import scalar_instance, array_instance
 from obspy import Trace, Stream
 from seispy.decon import RFTrace
 
 ei = 0+1j
 
 def e_inverse(omega, rho, alpha, beta, p):
     """ E_inverse (Aki & Richards, pp. 161, Eq. (5.71))
@@ -153,17 +154,17 @@
             samples of synthetic waveform
         ipha : _type_
             Specify incident wave 1 for P and -1 for S
         """
         self.depmod = depmod
         self.dt = dt
         self.npts = npts
-        if not isinstance(rayp, (float, list, np.ndarray)):
+        if not (array_instance(rayp) or scalar_instance(rayp)):
             raise TypeError('The rayp should be in float, list and np.ndarray')
-        if isinstance(rayp, float):
+        if scalar_instance(rayp):
             self.rayp = [rayp]
         else:
             self.rayp = rayp
         self.ipha = ipha
 
     def run_fwd(self):
         """Forward modelling synthetic seismograms.
```

### Comparing `python-seispy-1.3.3/seispy/setuplog.py` & `python-seispy-1.3.4/seispy/setuplog.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.3/seispy/signal.py` & `python-seispy-1.3.4/seispy/signal.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.3/seispy/slantstack.py` & `python-seispy-1.3.4/seispy/slantstack.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 import numpy as np
 from scipy.interpolate import interp1d
 import matplotlib.pyplot as plt
 from obspy.taup import TauPyModel
 from seispy.geo import srad2skm, skm2sdeg
+from seispy.utils import scalar_instance, array_instance
 
 class SlantStack():
     def __init__(self, seis, timeaxis, dis) -> None:
         """Slant stack in tau domain. Refer to Tauzin et al., 2008 JGR in detail.
 
         :param seis: 2D array for RFs with shape of (ev_num, npts)
         :type seis: numpy.ndarray
         :param timeaxis: 1D array for time axis
         :type timeaxis: numpy.ndarray
-        :param dis: 1D array for all event distance in km
+        :param dis: 1D array for all event distance in deg
         :type dis: numpy.ndarray
         """
         self.datar = seis
         self.time_axis = timeaxis
         self.dis = dis
         self.ref_dis = 65
         self.rayp_range = np.arange(-0.35, 0.35, 0.01)
         self.tau_range = np.arange(0, 100, 0.1)
         self.syn_tau = np.array([])
         self.syn_drayp = np.array([])
 
     def stack(self, ref_dis=None, rayp_range=None, tau_range=None):
-        if ref_dis is not None and isinstance(ref_dis, (int, float)):
+        if ref_dis is not None and scalar_instance(ref_dis):
             self.ref_dis = ref_dis
         elif ref_dis is None:
             pass
         else:
             raise TypeError('{} should be in int or float type.'.format(ref_dis))
-        if rayp_range is not None and isinstance(rayp_range, np.ndarray):
+        if rayp_range is not None and array_instance(rayp_range):
             self.rayp_range = rayp_range
         elif rayp_range is None:
             pass
         else:
             raise TypeError('{} should be in numpy.ndarray type.'.format(rayp_range))
-        if tau_range is not None and isinstance(tau_range, np.ndarray):
+        if tau_range is not None and array_instance(tau_range):
             self.tau_range = tau_range
         elif tau_range is None:
             pass
         else:
             raise TypeError('{} should be in numpy.ndarray type.'.format(tau_range))
         ev_num = self.datar.shape[0]
         taus, rayps = np.meshgrid(self.tau_range, self.rayp_range)
@@ -80,30 +81,30 @@
         """
         plt.style.use("bmh")
         self.fig = plt.figure(figsize=(8,5))
         self.ax = self.fig.add_subplot()
         if vmin is None and vmax is None:
             vmax = np.max(np.abs(self.stack_amp))*0.1
             vmin = -vmax
-        elif vmin is None and isinstance(vmax, (int, float)):
+        elif vmin is None and scalar_instance(vmax):
             vmin = np.min(self.stack_amp)
-        elif vmax is None and isinstance(vmin, (int, float)):
+        elif vmax is None and scalar_instance(vmin):
             vmax = np.max(self.stack_amp)
-        elif isinstance(vmax, (int, float)) and isinstance(vmin, (int, float)):
+        elif scalar_instance(vmax) and scalar_instance(vmin):
             pass
         else:
             raise TypeError('vmin and vmax must be in int or in float type')
         im = self.ax.pcolor(self.tau_range, self.rayp_range, self.stack_amp,
                             vmax=vmax, vmin=vmin, cmap=cmap)
         if colorbar:
             cax = self.fig.colorbar(im, ax=self.ax)
             cax.set_label('Stack Amplitude')
         self.ax.grid(visible=True)
         self.ax.scatter(self.syn_tau, self.syn_drayp, color='k', marker='x')
-        if xlim is not None and isinstance(xlim, (list, np.ndarray)):
+        if xlim is not None and array_instance(xlim):
             self.ax.set_xlim(xlim)
         self.ax.set_xlabel('Time (s)')
         self.ax.set_ylabel('Slowness (s/$^\circ$)')
         if figpath is not None and isinstance(figpath, str):
             self.fig.savefig(figpath, format='png', dpi=400, bbox_inches='tight')
         else:
             plt.show()
```

### Comparing `python-seispy-1.3.3/seispy/utils.py` & `python-seispy-1.3.4/seispy/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from os.path import join, dirname, exists
 from scipy.io import loadmat
 from matplotlib.colors import ListedColormap
 import matplotlib.pyplot as plt
-from seispy import geo
-from seispy.geo import geo2sph, sph2geo
-from seispy import distaz
 import numpy as np
 from scipy.interpolate import interp1d, interpn
-import seispy
+import pandas as pd
+import array
 
 
 def vs2vprho(vs):
     vp = 0.9409 + 2.0947*vs - 0.8206*vs**2 + 0.2683*vs**3 - 0.0251*vs**4
     rho = 1.6612*vp - 0.4721*vp**2 + 0.0671*vp**3 - 0.0043*vp**4 + 0.000106*vp**5
     # vs = 0.7858 - 1.2344*vp + 0.7949*vp**2 - 0.1238*vp**3 + 0.0064*vp**4
     return vp, rho
@@ -261,27 +259,34 @@
 
     def interpdvs(self, points):
         dvs = interpn((self.model['dep'], self.model['lat'], self.model['lon']), self.dvs, points,
                       bounds_error=False, fill_value=None)
         return dvs
 
 
-def create_center_bin_profile(stations, val=5, method='linear'):
-    if not isinstance(stations, seispy.rf2depth_makedata.Station):
-        raise TypeError('Stations should be seispy.rf2depth_makedata.Station')
-    dis_sta = prof_range(stations.stla, stations.stlo)
-    dis_inter = np.append(np.arange(0, dis_sta[-1], val), dis_sta[-1])
-    r, theta, phi = geo2sph(np.zeros(stations.stla.size), stations.stla, stations.stlo)
-    # t_po = np.arange(stations.stla.size)
-    # ip_t_po = np.linspace(0, stations.stla.size, bin_num)
-    theta_i = interp1d(dis_sta, theta, kind=method, bounds_error=False, fill_value='extrapolate')(dis_inter)
-    phi_i = interp1d(dis_sta, phi, kind=method, bounds_error=False, fill_value='extrapolate')(dis_inter)
-    _, lat, lon = sph2geo(r, theta_i, phi_i)
-    # dis = prof_range(lat, lon)
-    return lat, lon, dis_inter
-
-
-def prof_range(lat, lon):
-    dis = [0]
-    for i in range(lat.size-1):
-        dis.append(distaz(lat[i], lon[i], lat[i+1], lon[i+1]).degreesToKilometers())
-    return np.cumsum(dis)
+def scalar_instance(v):
+    if isinstance(
+        v,
+        (int,
+         float,
+         np.floating,
+         np.integer
+        )
+    ):
+        return True
+    else:
+        return False
+
+
+def array_instance(v):
+    if isinstance(
+        v,
+        (list,
+         tuple,
+         np.ndarray,
+         pd.Series,
+         array.array,
+        )
+    ):
+        return True
+    else:
+        return False
```

### Comparing `python-seispy-1.3.3/setup.py` & `python-seispy-1.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 packages = find_packages()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
-VERSION = "1.3.3"
+VERSION = "1.3.4"
 setup(name='python-seispy',
       version=VERSION,
       author='Mijian Xu',
       long_description=long_description,
       long_description_content_type="text/markdown",
       author_email='gomijianxu@gmail.com',
       license='GPLv3',
@@ -20,15 +20,16 @@
       install_requires=[
                 'numpy>=1.19.0',
                 'scipy>=1.9.1',
                 'matplotlib>=3.5.0',
                 'pandas>=1.0.0',
                 'obspy>=1.2.1',
                 'pyside6>=6.2.0',
-                'scikits.bootstrap>=1.0.0'],
+                'scikits.bootstrap>=1.0.0',
+                'pyproj'],
       entry_points={'console_scripts': ['gen_rayp_lib=seispy.psrayp:gen_rayp_lib',
                                         'prf=seispy.scripts:prf',
                                         'srf=seispy.scripts:srf',
                                         'setpar=seispy.rf:setpar',
                                         'rf2depth=seispy.rf2depth_makedata:rf2depth',
                                         'plotrt=seispy.scripts:plot_rt',
                                         'plotr=seispy.scripts:plot_r',
```

### Comparing `python-seispy-1.3.3/test/test_case01.py` & `python-seispy-1.3.4/test/test_case01.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.3/test/test_case02.py` & `python-seispy-1.3.4/test/test_case02.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.3/test/test_case03.py` & `python-seispy-1.3.4/test/test_case03.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,10 +38,19 @@
     ccp.cpara.adaptive = True
     ccp.cpara.stack_sta_list = 'ex-ccp/sta.lst'
     ccp.initial_profile()
     ccp.stack()
     ccp.save_stack_data(format='dat')
     os.remove(ccp.cpara.stackfile)
 
+def test_sub04():
+    ccp = CCPProfile('ex-ccp/ccp.cfg')
+    ccp.cpara.width = None
+    ccp.cpara.shape = 'circle'
+    ccp.initial_profile()
+    ccp.stack()
+    ccp.save_stack_data(format='dat')
+    os.remove(ccp.cpara.stackfile)
+
 if __name__ == '__main__':
     # test_download()
     test_sub01()
```

### Comparing `python-seispy-1.3.3/test/test_case04.py` & `python-seispy-1.3.4/test/test_case04.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.3/test/test_case05.py` & `python-seispy-1.3.4/test/test_case05.py`

 * *Files identical despite different names*

