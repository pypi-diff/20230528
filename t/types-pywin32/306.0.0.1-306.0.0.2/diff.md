# Comparing `tmp/types-pywin32-306.0.0.1.tar.gz` & `tmp/types-pywin32-306.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pywin32-306.0.0.1.tar", last modified: Mon Mar 27 18:24:57 2023, max compression
+gzip compressed data, was "types-pywin32-306.0.0.2.tar", last modified: Sun May 28 06:18:12 2023, max compression
```

## Comparing `types-pywin32-306.0.0.1.tar` & `types-pywin32-306.0.0.2.tar`

### file list

```diff
@@ -1,415 +1,415 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.639531 types-pywin32-306.0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-03-27 18:24:57.639531 types-pywin32-306.0.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.607531 types-pywin32-306.0.0.1/_win32typing-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/_win32typing-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)   210273 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/_win32typing-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.607531 types-pywin32-306.0.0.1/afxres-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/afxres-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/afxres-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.607531 types-pywin32-306.0.0.1/commctrl-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/commctrl-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/commctrl-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.611531 types-pywin32-306.0.0.1/dde-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/dde-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/dde-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.611531 types-pywin32-306.0.0.1/isapi-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/isapi-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/isapi-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/isapi-stubs/isapicon.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/isapi-stubs/simple.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/isapi-stubs/threaded_extension.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.611531 types-pywin32-306.0.0.1/mmapfile-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/mmapfile-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/mmapfile-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.611531 types-pywin32-306.0.0.1/mmsystem-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/mmsystem-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/mmsystem-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.611531 types-pywin32-306.0.0.1/ntsecuritycon-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/ntsecuritycon-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/ntsecuritycon-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.611531 types-pywin32-306.0.0.1/odbc-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/odbc-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/odbc-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.611531 types-pywin32-306.0.0.1/perfmon-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/perfmon-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/perfmon-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.611531 types-pywin32-306.0.0.1/pythoncom-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/pythoncom-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)    16434 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/pythoncom-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.611531 types-pywin32-306.0.0.1/pythonwin-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/pythonwin-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/pythonwin-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/pythonwin-stubs/dde.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11981 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/pythonwin-stubs/win32ui.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/pythonwin-stubs/win32uiole.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.611531 types-pywin32-306.0.0.1/pywintypes-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/pywintypes-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/pywintypes-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.611531 types-pywin32-306.0.0.1/regutil-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/regutil-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/regutil-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.611531 types-pywin32-306.0.0.1/servicemanager-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/servicemanager-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/servicemanager-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:24:57.639531 types-pywin32-306.0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.611531 types-pywin32-306.0.0.1/sspicon-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/sspicon-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/sspicon-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.611531 types-pywin32-306.0.0.1/timer-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/timer-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/timer-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.611531 types-pywin32-306.0.0.1/types_pywin32.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-03-27 18:24:57.000000 types-pywin32-306.0.0.1/types_pywin32.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-03-27 18:24:57.000000 types-pywin32-306.0.0.1/types_pywin32.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:24:57.000000 types-pywin32-306.0.0.1/types_pywin32.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-03-27 18:24:57.000000 types-pywin32-306.0.0.1/types_pywin32.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.611531 types-pywin32-306.0.0.1/win2kras-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win2kras-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win2kras-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.615531 types-pywin32-306.0.0.1/win32-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/_wincerapi.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.619531 types-pywin32-306.0.0.1/win32-stubs/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/lib/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/lib/afxres.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    35998 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/lib/commctrl.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22380 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/lib/mmsystem.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16244 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/lib/ntsecuritycon.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/lib/pywintypes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/lib/regutil.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13870 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/lib/sspicon.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/lib/win2kras.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   101683 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/lib/win32con.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    54316 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/lib/win32cryptcon.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/lib/win32evtlogutil.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/lib/win32gui_struct.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    33390 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/lib/win32inetcon.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/lib/win32netcon.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/lib/win32pdhquery.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/lib/win32serviceutil.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/lib/win32timezone.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    77893 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/lib/winerror.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17966 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/lib/winioctlcon.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    31295 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/lib/winnt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/lib/winperf.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/lib/winxptheme.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/mmapfile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/odbc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/perfmon.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/servicemanager.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/timer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/win32api.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/win32clipboard.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/win32console.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/win32cred.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/win32crypt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/win32event.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/win32evtlog.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16761 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/win32file.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    24668 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/win32gui.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/win32help.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/win32inet.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/win32job.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/win32lz.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/win32net.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/win32pdh.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/win32pipe.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/win32print.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/win32process.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/win32profile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/win32ras.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20333 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/win32security.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/win32service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/win32trace.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/win32transaction.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/win32ts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/win32wnet.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32-stubs/winxpgui.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.619531 types-pywin32-306.0.0.1/win32api-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32api-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32api-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.619531 types-pywin32-306.0.0.1/win32clipboard-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32clipboard-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32clipboard-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.619531 types-pywin32-306.0.0.1/win32com-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32com-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.619531 types-pywin32-306.0.0.1/win32com-stubs/adsi/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/adsi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/adsi/adsi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/adsi/adsicon.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.619531 types-pywin32-306.0.0.1/win32com-stubs/authorization/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/authorization/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/authorization/authorization.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.619531 types-pywin32-306.0.0.1/win32com-stubs/axcontrol/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/axcontrol/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/axcontrol/axcontrol.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.619531 types-pywin32-306.0.0.1/win32com-stubs/axdebug/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/axdebug/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/axdebug/adb.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/axdebug/axdebug.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/axdebug/codecontainer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/axdebug/contexts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/axdebug/debugger.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/axdebug/documents.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/axdebug/expressions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/axdebug/gateways.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/axdebug/stackframe.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/axdebug/util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.623531 types-pywin32-306.0.0.1/win32com-stubs/axscript/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/axscript/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/axscript/asputil.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/axscript/axscript.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.623531 types-pywin32-306.0.0.1/win32com-stubs/axscript/client/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/axscript/client/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/axscript/client/error.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.623531 types-pywin32-306.0.0.1/win32com-stubs/axscript/server/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/axscript/server/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/axscript/server/axsite.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/axscript/server/error.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.623531 types-pywin32-306.0.0.1/win32com-stubs/bits/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/bits/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/bits/bits.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.623531 types-pywin32-306.0.0.1/win32com-stubs/client/
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/client/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/client/build.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/client/dynamic.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/client/gencache.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.623531 types-pywin32-306.0.0.1/win32com-stubs/directsound/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/directsound/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/directsound/directsound.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.623531 types-pywin32-306.0.0.1/win32com-stubs/ifilter/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/ifilter/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/ifilter/ifilter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/ifilter/ifiltercon.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.623531 types-pywin32-306.0.0.1/win32com-stubs/internet/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/internet/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/internet/inetcon.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/internet/internet.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.623531 types-pywin32-306.0.0.1/win32com-stubs/mapi/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/mapi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/mapi/_exchdapi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/mapi/emsabtags.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/mapi/exchange.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/mapi/mapi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/mapi/mapitags.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/mapi/mapiutil.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/olectl.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.623531 types-pywin32-306.0.0.1/win32com-stubs/propsys/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/propsys/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/propsys/propsys.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/propsys/pscon.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.623531 types-pywin32-306.0.0.1/win32com-stubs/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/server/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/server/connect.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/server/dispatcher.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/server/exception.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/server/policy.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/server/util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.623531 types-pywin32-306.0.0.1/win32com-stubs/shell/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/shell/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/shell/shell.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/shell/shellcon.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/storagecon.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.623531 types-pywin32-306.0.0.1/win32com-stubs/taskscheduler/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/taskscheduler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/taskscheduler/taskscheduler.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/universal.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32com-stubs/util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.623531 types-pywin32-306.0.0.1/win32comext-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32comext-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.623531 types-pywin32-306.0.0.1/win32comext-stubs/adsi/
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/adsi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/adsi/adsi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10322 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/adsi/adsicon.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.627531 types-pywin32-306.0.0.1/win32comext-stubs/authorization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/authorization/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/authorization/authorization.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.627531 types-pywin32-306.0.0.1/win32comext-stubs/axcontrol/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/axcontrol/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/axcontrol/axcontrol.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.627531 types-pywin32-306.0.0.1/win32comext-stubs/axdebug/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/axdebug/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/axdebug/adb.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/axdebug/axdebug.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/axdebug/codecontainer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/axdebug/contexts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/axdebug/debugger.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/axdebug/documents.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/axdebug/expressions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/axdebug/gateways.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/axdebug/stackframe.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/axdebug/util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.627531 types-pywin32-306.0.0.1/win32comext-stubs/axscript/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/axscript/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/axscript/asputil.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/axscript/axscript.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.627531 types-pywin32-306.0.0.1/win32comext-stubs/axscript/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/axscript/client/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/axscript/client/error.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/axscript/client/pyscript.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.627531 types-pywin32-306.0.0.1/win32comext-stubs/axscript/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/axscript/server/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/axscript/server/axsite.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/axscript/server/error.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.627531 types-pywin32-306.0.0.1/win32comext-stubs/bits/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/bits/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/bits/bits.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.627531 types-pywin32-306.0.0.1/win32comext-stubs/directsound/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/directsound/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/directsound/directsound.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.627531 types-pywin32-306.0.0.1/win32comext-stubs/ifilter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/ifilter/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/ifilter/ifilter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/ifilter/ifiltercon.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.627531 types-pywin32-306.0.0.1/win32comext-stubs/internet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/internet/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/internet/inetcon.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/internet/internet.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.631531 types-pywin32-306.0.0.1/win32comext-stubs/mapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/mapi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/mapi/_exchdapi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    34766 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/mapi/emsabtags.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/mapi/exchange.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8993 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/mapi/mapi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    26668 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/mapi/mapitags.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/mapi/mapiutil.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.631531 types-pywin32-306.0.0.1/win32comext-stubs/propsys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/propsys/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/propsys/propsys.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23479 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/propsys/pscon.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.631531 types-pywin32-306.0.0.1/win32comext-stubs/shell/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/shell/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18642 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/shell/shell.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    34194 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/shell/shellcon.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.631531 types-pywin32-306.0.0.1/win32comext-stubs/taskscheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/taskscheduler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-03-27 18:21:24.000000 types-pywin32-306.0.0.1/win32comext-stubs/taskscheduler/taskscheduler.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.631531 types-pywin32-306.0.0.1/win32con-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32con-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32con-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.631531 types-pywin32-306.0.0.1/win32console-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32console-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32console-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.631531 types-pywin32-306.0.0.1/win32cred-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32cred-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32cred-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.631531 types-pywin32-306.0.0.1/win32crypt-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32crypt-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32crypt-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.631531 types-pywin32-306.0.0.1/win32cryptcon-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32cryptcon-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32cryptcon-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.631531 types-pywin32-306.0.0.1/win32event-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32event-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32event-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.631531 types-pywin32-306.0.0.1/win32evtlog-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32evtlog-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32evtlog-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.631531 types-pywin32-306.0.0.1/win32evtlogutil-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32evtlogutil-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32evtlogutil-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.631531 types-pywin32-306.0.0.1/win32file-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32file-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32file-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.631531 types-pywin32-306.0.0.1/win32gui-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32gui-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32gui-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.631531 types-pywin32-306.0.0.1/win32gui_struct-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32gui_struct-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32gui_struct-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.631531 types-pywin32-306.0.0.1/win32help-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32help-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32help-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.631531 types-pywin32-306.0.0.1/win32inet-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32inet-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32inet-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.631531 types-pywin32-306.0.0.1/win32inetcon-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32inetcon-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32inetcon-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.631531 types-pywin32-306.0.0.1/win32job-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32job-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32job-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.635531 types-pywin32-306.0.0.1/win32lz-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32lz-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32lz-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.635531 types-pywin32-306.0.0.1/win32net-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32net-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32net-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.635531 types-pywin32-306.0.0.1/win32netcon-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32netcon-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32netcon-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.635531 types-pywin32-306.0.0.1/win32pdh-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32pdh-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32pdh-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.635531 types-pywin32-306.0.0.1/win32pdhquery-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32pdhquery-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32pdhquery-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.635531 types-pywin32-306.0.0.1/win32pipe-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32pipe-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32pipe-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.635531 types-pywin32-306.0.0.1/win32print-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32print-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32print-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.635531 types-pywin32-306.0.0.1/win32process-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32process-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32process-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.635531 types-pywin32-306.0.0.1/win32profile-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32profile-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32profile-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.635531 types-pywin32-306.0.0.1/win32ras-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32ras-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32ras-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.635531 types-pywin32-306.0.0.1/win32security-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32security-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32security-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.635531 types-pywin32-306.0.0.1/win32service-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32service-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32service-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.635531 types-pywin32-306.0.0.1/win32serviceutil-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32serviceutil-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32serviceutil-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.635531 types-pywin32-306.0.0.1/win32timezone-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32timezone-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32timezone-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.635531 types-pywin32-306.0.0.1/win32trace-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32trace-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32trace-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.635531 types-pywin32-306.0.0.1/win32transaction-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32transaction-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32transaction-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.635531 types-pywin32-306.0.0.1/win32ts-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32ts-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32ts-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.635531 types-pywin32-306.0.0.1/win32ui-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32ui-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32ui-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.635531 types-pywin32-306.0.0.1/win32uiole-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32uiole-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32uiole-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.639531 types-pywin32-306.0.0.1/win32wnet-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32wnet-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/win32wnet-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.639531 types-pywin32-306.0.0.1/winerror-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/winerror-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/winerror-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.639531 types-pywin32-306.0.0.1/winioctlcon-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/winioctlcon-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/winioctlcon-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.639531 types-pywin32-306.0.0.1/winnt-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/winnt-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/winnt-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.639531 types-pywin32-306.0.0.1/winperf-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/winperf-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/winperf-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.639531 types-pywin32-306.0.0.1/winxpgui-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/winxpgui-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/winxpgui-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:57.639531 types-pywin32-306.0.0.1/winxptheme-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/winxptheme-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-27 18:24:56.000000 types-pywin32-306.0.0.1/winxptheme-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.278519 types-pywin32-306.0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-28 06:18:12.278519 types-pywin32-306.0.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.226519 types-pywin32-306.0.0.2/_win32typing-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/_win32typing-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)   210273 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/_win32typing-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.226519 types-pywin32-306.0.0.2/afxres-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/afxres-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/afxres-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.226519 types-pywin32-306.0.0.2/commctrl-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/commctrl-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/commctrl-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.230519 types-pywin32-306.0.0.2/dde-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/dde-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/dde-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.230519 types-pywin32-306.0.0.2/isapi-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/isapi-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/isapi-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/isapi-stubs/isapicon.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/isapi-stubs/simple.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/isapi-stubs/threaded_extension.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.230519 types-pywin32-306.0.0.2/mmapfile-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/mmapfile-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/mmapfile-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.230519 types-pywin32-306.0.0.2/mmsystem-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/mmsystem-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/mmsystem-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.230519 types-pywin32-306.0.0.2/ntsecuritycon-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/ntsecuritycon-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/ntsecuritycon-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.230519 types-pywin32-306.0.0.2/odbc-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/odbc-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/odbc-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.230519 types-pywin32-306.0.0.2/perfmon-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/perfmon-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/perfmon-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.230519 types-pywin32-306.0.0.2/pythoncom-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/pythoncom-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    16434 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/pythoncom-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.230519 types-pywin32-306.0.0.2/pythonwin-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/pythonwin-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/pythonwin-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/pythonwin-stubs/dde.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11981 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/pythonwin-stubs/win32ui.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/pythonwin-stubs/win32uiole.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.230519 types-pywin32-306.0.0.2/pywintypes-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/pywintypes-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/pywintypes-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.234519 types-pywin32-306.0.0.2/regutil-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/regutil-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/regutil-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.234519 types-pywin32-306.0.0.2/servicemanager-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/servicemanager-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/servicemanager-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 06:18:12.278519 types-pywin32-306.0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.234519 types-pywin32-306.0.0.2/sspicon-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/sspicon-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/sspicon-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.234519 types-pywin32-306.0.0.2/timer-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/timer-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/timer-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.234519 types-pywin32-306.0.0.2/types_pywin32.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-28 06:18:12.000000 types-pywin32-306.0.0.2/types_pywin32.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-05-28 06:18:12.000000 types-pywin32-306.0.0.2/types_pywin32.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 06:18:12.000000 types-pywin32-306.0.0.2/types_pywin32.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-28 06:18:12.000000 types-pywin32-306.0.0.2/types_pywin32.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.234519 types-pywin32-306.0.0.2/win2kras-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win2kras-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win2kras-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.238519 types-pywin32-306.0.0.2/win32-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/_wincerapi.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.242519 types-pywin32-306.0.0.2/win32-stubs/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/lib/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/lib/afxres.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    35998 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/lib/commctrl.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22380 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/lib/mmsystem.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16244 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/lib/ntsecuritycon.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/lib/pywintypes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/lib/regutil.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13870 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/lib/sspicon.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/lib/win2kras.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   101683 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/lib/win32con.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    54316 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/lib/win32cryptcon.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/lib/win32evtlogutil.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/lib/win32gui_struct.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    33390 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/lib/win32inetcon.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/lib/win32netcon.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/lib/win32pdhquery.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/lib/win32serviceutil.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/lib/win32timezone.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    77893 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/lib/winerror.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17966 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/lib/winioctlcon.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    31295 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/lib/winnt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/lib/winperf.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/lib/winxptheme.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/mmapfile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/odbc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/perfmon.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/servicemanager.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/timer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/win32api.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/win32clipboard.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/win32console.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/win32cred.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/win32crypt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/win32event.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/win32evtlog.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16761 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/win32file.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    24668 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/win32gui.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/win32help.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/win32inet.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/win32job.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/win32lz.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/win32net.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/win32pdh.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/win32pipe.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/win32print.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/win32process.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/win32profile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/win32ras.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20333 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/win32security.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/win32service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/win32trace.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/win32transaction.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/win32ts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/win32wnet.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32-stubs/winxpgui.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.246519 types-pywin32-306.0.0.2/win32api-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32api-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32api-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.246519 types-pywin32-306.0.0.2/win32clipboard-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32clipboard-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32clipboard-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.246519 types-pywin32-306.0.0.2/win32com-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32com-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.246519 types-pywin32-306.0.0.2/win32com-stubs/adsi/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/adsi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/adsi/adsi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/adsi/adsicon.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.246519 types-pywin32-306.0.0.2/win32com-stubs/authorization/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/authorization/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/authorization/authorization.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.246519 types-pywin32-306.0.0.2/win32com-stubs/axcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/axcontrol/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/axcontrol/axcontrol.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.250519 types-pywin32-306.0.0.2/win32com-stubs/axdebug/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/axdebug/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/axdebug/adb.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/axdebug/axdebug.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/axdebug/codecontainer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/axdebug/contexts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/axdebug/debugger.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/axdebug/documents.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/axdebug/expressions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/axdebug/gateways.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/axdebug/stackframe.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/axdebug/util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.250519 types-pywin32-306.0.0.2/win32com-stubs/axscript/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/axscript/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/axscript/asputil.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/axscript/axscript.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.250519 types-pywin32-306.0.0.2/win32com-stubs/axscript/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/axscript/client/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/axscript/client/error.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.250519 types-pywin32-306.0.0.2/win32com-stubs/axscript/server/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/axscript/server/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/axscript/server/axsite.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/axscript/server/error.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.250519 types-pywin32-306.0.0.2/win32com-stubs/bits/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/bits/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/bits/bits.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.250519 types-pywin32-306.0.0.2/win32com-stubs/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/client/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/client/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/client/dynamic.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/client/gencache.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.250519 types-pywin32-306.0.0.2/win32com-stubs/directsound/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/directsound/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/directsound/directsound.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.250519 types-pywin32-306.0.0.2/win32com-stubs/ifilter/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/ifilter/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/ifilter/ifilter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/ifilter/ifiltercon.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.254519 types-pywin32-306.0.0.2/win32com-stubs/internet/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/internet/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/internet/inetcon.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/internet/internet.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.254519 types-pywin32-306.0.0.2/win32com-stubs/mapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/mapi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/mapi/_exchdapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/mapi/emsabtags.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/mapi/exchange.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/mapi/mapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/mapi/mapitags.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/mapi/mapiutil.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/olectl.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.254519 types-pywin32-306.0.0.2/win32com-stubs/propsys/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/propsys/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/propsys/propsys.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/propsys/pscon.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.254519 types-pywin32-306.0.0.2/win32com-stubs/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/server/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/server/connect.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/server/dispatcher.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/server/exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/server/policy.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/server/util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.254519 types-pywin32-306.0.0.2/win32com-stubs/shell/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/shell/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/shell/shell.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/shell/shellcon.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/storagecon.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.254519 types-pywin32-306.0.0.2/win32com-stubs/taskscheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/taskscheduler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/taskscheduler/taskscheduler.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/universal.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32com-stubs/util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.254519 types-pywin32-306.0.0.2/win32comext-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32comext-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.258519 types-pywin32-306.0.0.2/win32comext-stubs/adsi/
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/adsi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/adsi/adsi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10322 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/adsi/adsicon.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.258519 types-pywin32-306.0.0.2/win32comext-stubs/authorization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/authorization/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/authorization/authorization.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.258519 types-pywin32-306.0.0.2/win32comext-stubs/axcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/axcontrol/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/axcontrol/axcontrol.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.258519 types-pywin32-306.0.0.2/win32comext-stubs/axdebug/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/axdebug/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/axdebug/adb.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/axdebug/axdebug.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/axdebug/codecontainer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/axdebug/contexts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/axdebug/debugger.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/axdebug/documents.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/axdebug/expressions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/axdebug/gateways.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/axdebug/stackframe.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/axdebug/util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.258519 types-pywin32-306.0.0.2/win32comext-stubs/axscript/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/axscript/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/axscript/asputil.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/axscript/axscript.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.258519 types-pywin32-306.0.0.2/win32comext-stubs/axscript/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/axscript/client/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/axscript/client/error.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/axscript/client/pyscript.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.258519 types-pywin32-306.0.0.2/win32comext-stubs/axscript/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/axscript/server/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/axscript/server/axsite.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/axscript/server/error.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.262519 types-pywin32-306.0.0.2/win32comext-stubs/bits/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/bits/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/bits/bits.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.262519 types-pywin32-306.0.0.2/win32comext-stubs/directsound/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/directsound/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/directsound/directsound.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.262519 types-pywin32-306.0.0.2/win32comext-stubs/ifilter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/ifilter/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/ifilter/ifilter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/ifilter/ifiltercon.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.262519 types-pywin32-306.0.0.2/win32comext-stubs/internet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/internet/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/internet/inetcon.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/internet/internet.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.262519 types-pywin32-306.0.0.2/win32comext-stubs/mapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/mapi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/mapi/_exchdapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    34766 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/mapi/emsabtags.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/mapi/exchange.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8993 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/mapi/mapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    26668 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/mapi/mapitags.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/mapi/mapiutil.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.262519 types-pywin32-306.0.0.2/win32comext-stubs/propsys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/propsys/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/propsys/propsys.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23479 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/propsys/pscon.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.262519 types-pywin32-306.0.0.2/win32comext-stubs/shell/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/shell/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18642 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/shell/shell.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    34194 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/shell/shellcon.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.262519 types-pywin32-306.0.0.2/win32comext-stubs/taskscheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/taskscheduler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-28 06:17:54.000000 types-pywin32-306.0.0.2/win32comext-stubs/taskscheduler/taskscheduler.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.266519 types-pywin32-306.0.0.2/win32con-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32con-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32con-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.266519 types-pywin32-306.0.0.2/win32console-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32console-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32console-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.266519 types-pywin32-306.0.0.2/win32cred-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32cred-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32cred-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.266519 types-pywin32-306.0.0.2/win32crypt-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32crypt-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32crypt-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.266519 types-pywin32-306.0.0.2/win32cryptcon-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32cryptcon-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32cryptcon-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.266519 types-pywin32-306.0.0.2/win32event-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32event-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32event-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.266519 types-pywin32-306.0.0.2/win32evtlog-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32evtlog-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32evtlog-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.266519 types-pywin32-306.0.0.2/win32evtlogutil-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32evtlogutil-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32evtlogutil-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.266519 types-pywin32-306.0.0.2/win32file-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32file-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32file-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.266519 types-pywin32-306.0.0.2/win32gui-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32gui-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32gui-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.270519 types-pywin32-306.0.0.2/win32gui_struct-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32gui_struct-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32gui_struct-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.270519 types-pywin32-306.0.0.2/win32help-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32help-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32help-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.270519 types-pywin32-306.0.0.2/win32inet-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32inet-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32inet-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.270519 types-pywin32-306.0.0.2/win32inetcon-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32inetcon-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32inetcon-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.270519 types-pywin32-306.0.0.2/win32job-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32job-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32job-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.270519 types-pywin32-306.0.0.2/win32lz-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32lz-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32lz-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.270519 types-pywin32-306.0.0.2/win32net-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32net-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32net-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.270519 types-pywin32-306.0.0.2/win32netcon-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32netcon-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32netcon-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.270519 types-pywin32-306.0.0.2/win32pdh-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32pdh-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32pdh-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.270519 types-pywin32-306.0.0.2/win32pdhquery-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32pdhquery-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32pdhquery-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.270519 types-pywin32-306.0.0.2/win32pipe-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32pipe-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32pipe-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.270519 types-pywin32-306.0.0.2/win32print-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32print-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32print-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.274519 types-pywin32-306.0.0.2/win32process-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32process-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32process-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.274519 types-pywin32-306.0.0.2/win32profile-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32profile-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32profile-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.274519 types-pywin32-306.0.0.2/win32ras-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32ras-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32ras-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.274519 types-pywin32-306.0.0.2/win32security-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32security-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32security-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.274519 types-pywin32-306.0.0.2/win32service-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32service-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32service-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.274519 types-pywin32-306.0.0.2/win32serviceutil-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32serviceutil-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32serviceutil-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.274519 types-pywin32-306.0.0.2/win32timezone-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32timezone-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32timezone-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.274519 types-pywin32-306.0.0.2/win32trace-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32trace-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32trace-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.274519 types-pywin32-306.0.0.2/win32transaction-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32transaction-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32transaction-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.274519 types-pywin32-306.0.0.2/win32ts-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32ts-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32ts-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.278519 types-pywin32-306.0.0.2/win32ui-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32ui-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32ui-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.278519 types-pywin32-306.0.0.2/win32uiole-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32uiole-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32uiole-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.278519 types-pywin32-306.0.0.2/win32wnet-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32wnet-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/win32wnet-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.278519 types-pywin32-306.0.0.2/winerror-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/winerror-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/winerror-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.278519 types-pywin32-306.0.0.2/winioctlcon-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/winioctlcon-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/winioctlcon-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.278519 types-pywin32-306.0.0.2/winnt-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/winnt-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/winnt-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.278519 types-pywin32-306.0.0.2/winperf-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/winperf-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/winperf-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.278519 types-pywin32-306.0.0.2/winxpgui-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/winxpgui-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/winxpgui-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:18:12.278519 types-pywin32-306.0.0.2/winxptheme-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/winxptheme-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-28 06:18:10.000000 types-pywin32-306.0.0.2/winxptheme-stubs/__init__.pyi
```

### Comparing `types-pywin32-306.0.0.1/CHANGELOG.md` & `types-pywin32-306.0.0.2/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+## 306.0.0.2 (2023-05-28)
+
+pywin32: add `HANDLEType` class (#10032)
+
+per http://timgolden.me.uk/pywin32-docs/PyHANDLE.html these objects actually have methods, they are not ints
+
+Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
+
 ## 306.0.0.1 (2023-03-27)
 
 Add default values for third-party stubs beginning with 'P' (#9957)
 
 ## 306.0.0.0 (2023-03-26)
 
 Bump pywin32 to 306.* (#9945)
```

### Comparing `types-pywin32-306.0.0.1/PKG-INFO` & `types-pywin32-306.0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pywin32
-Version: 306.0.0.1
+Version: 306.0.0.2
 Summary: Typing stubs for pywin32
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pywin32.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pywin32`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pywin32. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `d6a85e2c4820a69e504cdea1b446f3764cc3afec`.
```

### Comparing `types-pywin32-306.0.0.1/_win32typing-stubs/__init__.pyi` & `types-pywin32-306.0.0.2/_win32typing-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/isapi-stubs/isapicon.pyi` & `types-pywin32-306.0.0.2/isapi-stubs/isapicon.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/isapi-stubs/threaded_extension.pyi` & `types-pywin32-306.0.0.2/isapi-stubs/threaded_extension.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/pythoncom-stubs/__init__.pyi` & `types-pywin32-306.0.0.2/pythoncom-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/pythonwin-stubs/dde.pyi` & `types-pywin32-306.0.0.2/pythonwin-stubs/dde.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/pythonwin-stubs/win32ui.pyi` & `types-pywin32-306.0.0.2/pythonwin-stubs/win32ui.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/pythonwin-stubs/win32uiole.pyi` & `types-pywin32-306.0.0.2/pythonwin-stubs/win32uiole.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/setup.py` & `types-pywin32-306.0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,32 +12,32 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pywin32`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pywin32. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `d6a85e2c4820a69e504cdea1b446f3764cc3afec`.
 '''.lstrip()
 
 setup(name=name,
-      version="306.0.0.1",
+      version="306.0.0.2",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pywin32.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
-      packages=['win32service-stubs', 'winioctlcon-stubs', '_win32typing-stubs', 'win32api-stubs', 'win32event-stubs', 'win32help-stubs', 'win32security-stubs', 'win32inet-stubs', 'win32clipboard-stubs', 'pythonwin-stubs', 'win32crypt-stubs', 'win32cryptcon-stubs', 'mmapfile-stubs', 'win32evtlog-stubs', 'win32trace-stubs', 'win32cred-stubs', 'sspicon-stubs', 'pythoncom-stubs', 'win32serviceutil-stubs', 'winxpgui-stubs', 'pywintypes-stubs', 'dde-stubs', 'win32pipe-stubs', 'win32wnet-stubs', 'win32pdh-stubs', 'winxptheme-stubs', 'win32print-stubs', 'win32gui_struct-stubs', 'win32gui-stubs', 'timer-stubs', 'odbc-stubs', 'win32com-stubs', 'win32profile-stubs', 'win32file-stubs', 'afxres-stubs', 'winnt-stubs', 'win32-stubs', 'win32netcon-stubs', 'win32inetcon-stubs', 'win32ui-stubs', 'win32con-stubs', 'win32timezone-stubs', 'commctrl-stubs', 'win32lz-stubs', 'win2kras-stubs', 'win32net-stubs', 'isapi-stubs', 'win32ts-stubs', 'winerror-stubs', 'win32job-stubs', 'ntsecuritycon-stubs', 'perfmon-stubs', 'win32evtlogutil-stubs', 'win32transaction-stubs', 'win32ras-stubs', 'win32pdhquery-stubs', 'mmsystem-stubs', 'regutil-stubs', 'win32uiole-stubs', 'win32console-stubs', 'win32process-stubs', 'win32comext-stubs', 'servicemanager-stubs', 'winperf-stubs'],
-      package_data={'win32service-stubs': ['__init__.pyi', 'METADATA.toml'], 'winioctlcon-stubs': ['__init__.pyi', 'METADATA.toml'], '_win32typing-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32api-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32event-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32help-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32security-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32inet-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32clipboard-stubs': ['__init__.pyi', 'METADATA.toml'], 'pythonwin-stubs': ['__init__.pyi', 'dde.pyi', 'win32ui.pyi', 'win32uiole.pyi', 'METADATA.toml'], 'win32crypt-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32cryptcon-stubs': ['__init__.pyi', 'METADATA.toml'], 'mmapfile-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32evtlog-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32trace-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32cred-stubs': ['__init__.pyi', 'METADATA.toml'], 'sspicon-stubs': ['__init__.pyi', 'METADATA.toml'], 'pythoncom-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32serviceutil-stubs': ['__init__.pyi', 'METADATA.toml'], 'winxpgui-stubs': ['__init__.pyi', 'METADATA.toml'], 'pywintypes-stubs': ['__init__.pyi', 'METADATA.toml'], 'dde-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32pipe-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32wnet-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32pdh-stubs': ['__init__.pyi', 'METADATA.toml'], 'winxptheme-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32print-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32gui_struct-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32gui-stubs': ['__init__.pyi', 'METADATA.toml'], 'timer-stubs': ['__init__.pyi', 'METADATA.toml'], 'odbc-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32com-stubs': ['__init__.pyi', 'adsi/__init__.pyi', 'adsi/adsi.pyi', 'adsi/adsicon.pyi', 'authorization/__init__.pyi', 'authorization/authorization.pyi', 'axcontrol/__init__.pyi', 'axcontrol/axcontrol.pyi', 'axdebug/__init__.pyi', 'axdebug/adb.pyi', 'axdebug/axdebug.pyi', 'axdebug/codecontainer.pyi', 'axdebug/contexts.pyi', 'axdebug/debugger.pyi', 'axdebug/documents.pyi', 'axdebug/expressions.pyi', 'axdebug/gateways.pyi', 'axdebug/stackframe.pyi', 'axdebug/util.pyi', 'axscript/__init__.pyi', 'axscript/asputil.pyi', 'axscript/axscript.pyi', 'axscript/client/__init__.pyi', 'axscript/client/error.pyi', 'axscript/server/__init__.pyi', 'axscript/server/axsite.pyi', 'axscript/server/error.pyi', 'bits/__init__.pyi', 'bits/bits.pyi', 'client/__init__.pyi', 'client/build.pyi', 'client/dynamic.pyi', 'client/gencache.pyi', 'directsound/__init__.pyi', 'directsound/directsound.pyi', 'ifilter/__init__.pyi', 'ifilter/ifilter.pyi', 'ifilter/ifiltercon.pyi', 'internet/__init__.pyi', 'internet/inetcon.pyi', 'internet/internet.pyi', 'mapi/__init__.pyi', 'mapi/_exchdapi.pyi', 'mapi/emsabtags.pyi', 'mapi/exchange.pyi', 'mapi/mapi.pyi', 'mapi/mapitags.pyi', 'mapi/mapiutil.pyi', 'olectl.pyi', 'propsys/__init__.pyi', 'propsys/propsys.pyi', 'propsys/pscon.pyi', 'server/__init__.pyi', 'server/connect.pyi', 'server/dispatcher.pyi', 'server/exception.pyi', 'server/policy.pyi', 'server/util.pyi', 'shell/__init__.pyi', 'shell/shell.pyi', 'shell/shellcon.pyi', 'storagecon.pyi', 'taskscheduler/__init__.pyi', 'taskscheduler/taskscheduler.pyi', 'universal.pyi', 'util.pyi', 'METADATA.toml'], 'win32profile-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32file-stubs': ['__init__.pyi', 'METADATA.toml'], 'afxres-stubs': ['__init__.pyi', 'METADATA.toml'], 'winnt-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32-stubs': ['__init__.pyi', '_wincerapi.pyi', 'lib/__init__.pyi', 'lib/afxres.pyi', 'lib/commctrl.pyi', 'lib/mmsystem.pyi', 'lib/ntsecuritycon.pyi', 'lib/pywintypes.pyi', 'lib/regutil.pyi', 'lib/sspicon.pyi', 'lib/win2kras.pyi', 'lib/win32con.pyi', 'lib/win32cryptcon.pyi', 'lib/win32evtlogutil.pyi', 'lib/win32gui_struct.pyi', 'lib/win32inetcon.pyi', 'lib/win32netcon.pyi', 'lib/win32pdhquery.pyi', 'lib/win32serviceutil.pyi', 'lib/win32timezone.pyi', 'lib/winerror.pyi', 'lib/winioctlcon.pyi', 'lib/winnt.pyi', 'lib/winperf.pyi', 'lib/winxptheme.pyi', 'mmapfile.pyi', 'odbc.pyi', 'perfmon.pyi', 'servicemanager.pyi', 'timer.pyi', 'win32api.pyi', 'win32clipboard.pyi', 'win32console.pyi', 'win32cred.pyi', 'win32crypt.pyi', 'win32event.pyi', 'win32evtlog.pyi', 'win32file.pyi', 'win32gui.pyi', 'win32help.pyi', 'win32inet.pyi', 'win32job.pyi', 'win32lz.pyi', 'win32net.pyi', 'win32pdh.pyi', 'win32pipe.pyi', 'win32print.pyi', 'win32process.pyi', 'win32profile.pyi', 'win32ras.pyi', 'win32security.pyi', 'win32service.pyi', 'win32trace.pyi', 'win32transaction.pyi', 'win32ts.pyi', 'win32wnet.pyi', 'winxpgui.pyi', 'METADATA.toml'], 'win32netcon-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32inetcon-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32ui-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32con-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32timezone-stubs': ['__init__.pyi', 'METADATA.toml'], 'commctrl-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32lz-stubs': ['__init__.pyi', 'METADATA.toml'], 'win2kras-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32net-stubs': ['__init__.pyi', 'METADATA.toml'], 'isapi-stubs': ['__init__.pyi', 'isapicon.pyi', 'simple.pyi', 'threaded_extension.pyi', 'METADATA.toml'], 'win32ts-stubs': ['__init__.pyi', 'METADATA.toml'], 'winerror-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32job-stubs': ['__init__.pyi', 'METADATA.toml'], 'ntsecuritycon-stubs': ['__init__.pyi', 'METADATA.toml'], 'perfmon-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32evtlogutil-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32transaction-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32ras-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32pdhquery-stubs': ['__init__.pyi', 'METADATA.toml'], 'mmsystem-stubs': ['__init__.pyi', 'METADATA.toml'], 'regutil-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32uiole-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32console-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32process-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32comext-stubs': ['__init__.pyi', 'adsi/__init__.pyi', 'adsi/adsi.pyi', 'adsi/adsicon.pyi', 'authorization/__init__.pyi', 'authorization/authorization.pyi', 'axcontrol/__init__.pyi', 'axcontrol/axcontrol.pyi', 'axdebug/__init__.pyi', 'axdebug/adb.pyi', 'axdebug/axdebug.pyi', 'axdebug/codecontainer.pyi', 'axdebug/contexts.pyi', 'axdebug/debugger.pyi', 'axdebug/documents.pyi', 'axdebug/expressions.pyi', 'axdebug/gateways.pyi', 'axdebug/stackframe.pyi', 'axdebug/util.pyi', 'axscript/__init__.pyi', 'axscript/asputil.pyi', 'axscript/axscript.pyi', 'axscript/client/__init__.pyi', 'axscript/client/error.pyi', 'axscript/client/pyscript.pyi', 'axscript/server/__init__.pyi', 'axscript/server/axsite.pyi', 'axscript/server/error.pyi', 'bits/__init__.pyi', 'bits/bits.pyi', 'directsound/__init__.pyi', 'directsound/directsound.pyi', 'ifilter/__init__.pyi', 'ifilter/ifilter.pyi', 'ifilter/ifiltercon.pyi', 'internet/__init__.pyi', 'internet/inetcon.pyi', 'internet/internet.pyi', 'mapi/__init__.pyi', 'mapi/_exchdapi.pyi', 'mapi/emsabtags.pyi', 'mapi/exchange.pyi', 'mapi/mapi.pyi', 'mapi/mapitags.pyi', 'mapi/mapiutil.pyi', 'propsys/__init__.pyi', 'propsys/propsys.pyi', 'propsys/pscon.pyi', 'shell/__init__.pyi', 'shell/shell.pyi', 'shell/shellcon.pyi', 'taskscheduler/__init__.pyi', 'taskscheduler/taskscheduler.pyi', 'METADATA.toml'], 'servicemanager-stubs': ['__init__.pyi', 'METADATA.toml'], 'winperf-stubs': ['__init__.pyi', 'METADATA.toml']},
+      packages=['win32security-stubs', 'win32pdhquery-stubs', 'winnt-stubs', 'win32cred-stubs', 'win32comext-stubs', 'win32cryptcon-stubs', 'timer-stubs', 'win32pdh-stubs', 'win32con-stubs', 'winxpgui-stubs', 'win32process-stubs', 'win32serviceutil-stubs', 'pythonwin-stubs', 'win32ras-stubs', 'win32evtlog-stubs', 'pywintypes-stubs', 'win32ts-stubs', 'win32timezone-stubs', '_win32typing-stubs', 'win32api-stubs', 'regutil-stubs', 'win32com-stubs', 'win32service-stubs', 'dde-stubs', 'win32file-stubs', 'win32gui_struct-stubs', 'sspicon-stubs', 'afxres-stubs', 'win32wnet-stubs', 'winerror-stubs', 'win32clipboard-stubs', 'pythoncom-stubs', 'win32trace-stubs', 'winioctlcon-stubs', 'win32inetcon-stubs', 'win32profile-stubs', 'win32event-stubs', 'win32netcon-stubs', 'perfmon-stubs', 'win32-stubs', 'win32evtlogutil-stubs', 'win32job-stubs', 'servicemanager-stubs', 'isapi-stubs', 'mmapfile-stubs', 'win32help-stubs', 'win2kras-stubs', 'win32gui-stubs', 'win32print-stubs', 'winperf-stubs', 'commctrl-stubs', 'win32pipe-stubs', 'win32uiole-stubs', 'winxptheme-stubs', 'win32ui-stubs', 'win32console-stubs', 'mmsystem-stubs', 'ntsecuritycon-stubs', 'win32transaction-stubs', 'win32lz-stubs', 'win32net-stubs', 'win32crypt-stubs', 'odbc-stubs', 'win32inet-stubs'],
+      package_data={'win32security-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32pdhquery-stubs': ['__init__.pyi', 'METADATA.toml'], 'winnt-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32cred-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32comext-stubs': ['__init__.pyi', 'adsi/__init__.pyi', 'adsi/adsi.pyi', 'adsi/adsicon.pyi', 'authorization/__init__.pyi', 'authorization/authorization.pyi', 'axcontrol/__init__.pyi', 'axcontrol/axcontrol.pyi', 'axdebug/__init__.pyi', 'axdebug/adb.pyi', 'axdebug/axdebug.pyi', 'axdebug/codecontainer.pyi', 'axdebug/contexts.pyi', 'axdebug/debugger.pyi', 'axdebug/documents.pyi', 'axdebug/expressions.pyi', 'axdebug/gateways.pyi', 'axdebug/stackframe.pyi', 'axdebug/util.pyi', 'axscript/__init__.pyi', 'axscript/asputil.pyi', 'axscript/axscript.pyi', 'axscript/client/__init__.pyi', 'axscript/client/error.pyi', 'axscript/client/pyscript.pyi', 'axscript/server/__init__.pyi', 'axscript/server/axsite.pyi', 'axscript/server/error.pyi', 'bits/__init__.pyi', 'bits/bits.pyi', 'directsound/__init__.pyi', 'directsound/directsound.pyi', 'ifilter/__init__.pyi', 'ifilter/ifilter.pyi', 'ifilter/ifiltercon.pyi', 'internet/__init__.pyi', 'internet/inetcon.pyi', 'internet/internet.pyi', 'mapi/__init__.pyi', 'mapi/_exchdapi.pyi', 'mapi/emsabtags.pyi', 'mapi/exchange.pyi', 'mapi/mapi.pyi', 'mapi/mapitags.pyi', 'mapi/mapiutil.pyi', 'propsys/__init__.pyi', 'propsys/propsys.pyi', 'propsys/pscon.pyi', 'shell/__init__.pyi', 'shell/shell.pyi', 'shell/shellcon.pyi', 'taskscheduler/__init__.pyi', 'taskscheduler/taskscheduler.pyi', 'METADATA.toml'], 'win32cryptcon-stubs': ['__init__.pyi', 'METADATA.toml'], 'timer-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32pdh-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32con-stubs': ['__init__.pyi', 'METADATA.toml'], 'winxpgui-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32process-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32serviceutil-stubs': ['__init__.pyi', 'METADATA.toml'], 'pythonwin-stubs': ['__init__.pyi', 'dde.pyi', 'win32ui.pyi', 'win32uiole.pyi', 'METADATA.toml'], 'win32ras-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32evtlog-stubs': ['__init__.pyi', 'METADATA.toml'], 'pywintypes-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32ts-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32timezone-stubs': ['__init__.pyi', 'METADATA.toml'], '_win32typing-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32api-stubs': ['__init__.pyi', 'METADATA.toml'], 'regutil-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32com-stubs': ['__init__.pyi', 'adsi/__init__.pyi', 'adsi/adsi.pyi', 'adsi/adsicon.pyi', 'authorization/__init__.pyi', 'authorization/authorization.pyi', 'axcontrol/__init__.pyi', 'axcontrol/axcontrol.pyi', 'axdebug/__init__.pyi', 'axdebug/adb.pyi', 'axdebug/axdebug.pyi', 'axdebug/codecontainer.pyi', 'axdebug/contexts.pyi', 'axdebug/debugger.pyi', 'axdebug/documents.pyi', 'axdebug/expressions.pyi', 'axdebug/gateways.pyi', 'axdebug/stackframe.pyi', 'axdebug/util.pyi', 'axscript/__init__.pyi', 'axscript/asputil.pyi', 'axscript/axscript.pyi', 'axscript/client/__init__.pyi', 'axscript/client/error.pyi', 'axscript/server/__init__.pyi', 'axscript/server/axsite.pyi', 'axscript/server/error.pyi', 'bits/__init__.pyi', 'bits/bits.pyi', 'client/__init__.pyi', 'client/build.pyi', 'client/dynamic.pyi', 'client/gencache.pyi', 'directsound/__init__.pyi', 'directsound/directsound.pyi', 'ifilter/__init__.pyi', 'ifilter/ifilter.pyi', 'ifilter/ifiltercon.pyi', 'internet/__init__.pyi', 'internet/inetcon.pyi', 'internet/internet.pyi', 'mapi/__init__.pyi', 'mapi/_exchdapi.pyi', 'mapi/emsabtags.pyi', 'mapi/exchange.pyi', 'mapi/mapi.pyi', 'mapi/mapitags.pyi', 'mapi/mapiutil.pyi', 'olectl.pyi', 'propsys/__init__.pyi', 'propsys/propsys.pyi', 'propsys/pscon.pyi', 'server/__init__.pyi', 'server/connect.pyi', 'server/dispatcher.pyi', 'server/exception.pyi', 'server/policy.pyi', 'server/util.pyi', 'shell/__init__.pyi', 'shell/shell.pyi', 'shell/shellcon.pyi', 'storagecon.pyi', 'taskscheduler/__init__.pyi', 'taskscheduler/taskscheduler.pyi', 'universal.pyi', 'util.pyi', 'METADATA.toml'], 'win32service-stubs': ['__init__.pyi', 'METADATA.toml'], 'dde-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32file-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32gui_struct-stubs': ['__init__.pyi', 'METADATA.toml'], 'sspicon-stubs': ['__init__.pyi', 'METADATA.toml'], 'afxres-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32wnet-stubs': ['__init__.pyi', 'METADATA.toml'], 'winerror-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32clipboard-stubs': ['__init__.pyi', 'METADATA.toml'], 'pythoncom-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32trace-stubs': ['__init__.pyi', 'METADATA.toml'], 'winioctlcon-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32inetcon-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32profile-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32event-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32netcon-stubs': ['__init__.pyi', 'METADATA.toml'], 'perfmon-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32-stubs': ['__init__.pyi', '_wincerapi.pyi', 'lib/__init__.pyi', 'lib/afxres.pyi', 'lib/commctrl.pyi', 'lib/mmsystem.pyi', 'lib/ntsecuritycon.pyi', 'lib/pywintypes.pyi', 'lib/regutil.pyi', 'lib/sspicon.pyi', 'lib/win2kras.pyi', 'lib/win32con.pyi', 'lib/win32cryptcon.pyi', 'lib/win32evtlogutil.pyi', 'lib/win32gui_struct.pyi', 'lib/win32inetcon.pyi', 'lib/win32netcon.pyi', 'lib/win32pdhquery.pyi', 'lib/win32serviceutil.pyi', 'lib/win32timezone.pyi', 'lib/winerror.pyi', 'lib/winioctlcon.pyi', 'lib/winnt.pyi', 'lib/winperf.pyi', 'lib/winxptheme.pyi', 'mmapfile.pyi', 'odbc.pyi', 'perfmon.pyi', 'servicemanager.pyi', 'timer.pyi', 'win32api.pyi', 'win32clipboard.pyi', 'win32console.pyi', 'win32cred.pyi', 'win32crypt.pyi', 'win32event.pyi', 'win32evtlog.pyi', 'win32file.pyi', 'win32gui.pyi', 'win32help.pyi', 'win32inet.pyi', 'win32job.pyi', 'win32lz.pyi', 'win32net.pyi', 'win32pdh.pyi', 'win32pipe.pyi', 'win32print.pyi', 'win32process.pyi', 'win32profile.pyi', 'win32ras.pyi', 'win32security.pyi', 'win32service.pyi', 'win32trace.pyi', 'win32transaction.pyi', 'win32ts.pyi', 'win32wnet.pyi', 'winxpgui.pyi', 'METADATA.toml'], 'win32evtlogutil-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32job-stubs': ['__init__.pyi', 'METADATA.toml'], 'servicemanager-stubs': ['__init__.pyi', 'METADATA.toml'], 'isapi-stubs': ['__init__.pyi', 'isapicon.pyi', 'simple.pyi', 'threaded_extension.pyi', 'METADATA.toml'], 'mmapfile-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32help-stubs': ['__init__.pyi', 'METADATA.toml'], 'win2kras-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32gui-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32print-stubs': ['__init__.pyi', 'METADATA.toml'], 'winperf-stubs': ['__init__.pyi', 'METADATA.toml'], 'commctrl-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32pipe-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32uiole-stubs': ['__init__.pyi', 'METADATA.toml'], 'winxptheme-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32ui-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32console-stubs': ['__init__.pyi', 'METADATA.toml'], 'mmsystem-stubs': ['__init__.pyi', 'METADATA.toml'], 'ntsecuritycon-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32transaction-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32lz-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32net-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32crypt-stubs': ['__init__.pyi', 'METADATA.toml'], 'odbc-stubs': ['__init__.pyi', 'METADATA.toml'], 'win32inet-stubs': ['__init__.pyi', 'METADATA.toml']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-pywin32-306.0.0.1/types_pywin32.egg-info/PKG-INFO` & `types-pywin32-306.0.0.2/types_pywin32.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pywin32
-Version: 306.0.0.1
+Version: 306.0.0.2
 Summary: Typing stubs for pywin32
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pywin32.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pywin32`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pywin32. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `d6a85e2c4820a69e504cdea1b446f3764cc3afec`.
```

### Comparing `types-pywin32-306.0.0.1/types_pywin32.egg-info/SOURCES.txt` & `types-pywin32-306.0.0.2/types_pywin32.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/types_pywin32.egg-info/top_level.txt` & `types-pywin32-306.0.0.2/types_pywin32.egg-info/top_level.txt`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/_wincerapi.pyi` & `types-pywin32-306.0.0.2/win32-stubs/_wincerapi.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/lib/afxres.pyi` & `types-pywin32-306.0.0.2/win32-stubs/lib/afxres.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/lib/commctrl.pyi` & `types-pywin32-306.0.0.2/win32-stubs/lib/commctrl.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/lib/mmsystem.pyi` & `types-pywin32-306.0.0.2/win32-stubs/lib/mmsystem.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/lib/ntsecuritycon.pyi` & `types-pywin32-306.0.0.2/win32-stubs/lib/ntsecuritycon.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/lib/pywintypes.pyi` & `types-pywin32-306.0.0.2/win32-stubs/lib/pywintypes.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 # Can't generate with stubgen because:
 # "KeyError: 'pywintypes'"
 from _typeshed import Incomplete
 from datetime import datetime
-from typing_extensions import Literal
+from typing import NoReturn
+from typing_extensions import Literal, Never
 
 import _win32typing
 
 class error(Exception):
     winerror: int
     funcname: str
     strerror: str
     def __init__(self, winerror: int, funcname: str, strerror: str): ...
 
 class com_error(Exception): ...
 class UnicodeType(str): ...
 
+class HANDLEType:
+    def __init__(self, *args: Never, **kwargs: Never) -> NoReturn: ...
+    @property
+    def handle(self) -> int: ...
+    def Close(self) -> None: ...
+    def close(self) -> None: ...
+    def Detach(self) -> None: ...
+    def __int__(self) -> int: ...
+
 class TimeType(datetime):
     Format = datetime.strftime
 
 IIDType = _win32typing.PyIID
 
 def DosDateTimeToTime() -> _win32typing.PyTime: ...
 def Unicode() -> str: ...
@@ -28,15 +38,15 @@
 def IID(iidString: str, is_bytes: bool = ...) -> _win32typing.PyIID: ...
 def Time(timeRepr) -> _win32typing.PyTime: ...
 def CreateGuid() -> _win32typing.PyIID: ...
 def ACL(__bufSize: int = ...) -> _win32typing.PyACL: ...
 def SID(buffer, idAuthority, subAuthorities, bufSize=...) -> _win32typing.PySID: ...
 def SECURITY_ATTRIBUTES() -> _win32typing.PySECURITY_ATTRIBUTES: ...
 def SECURITY_DESCRIPTOR() -> _win32typing.PySECURITY_DESCRIPTOR: ...
-def HANDLE() -> int: ...
+def HANDLE() -> HANDLEType: ...
 def HKEY() -> _win32typing.PyHKEY: ...
 def WAVEFORMATEX() -> _win32typing.PyWAVEFORMATEX: ...
 def TimeStamp(*args, **kwargs): ...  # incomplete
 
 FALSE: Literal[False]
 TRUE: Literal[True]
 WAVE_FORMAT_PCM: int
```

### Comparing `types-pywin32-306.0.0.1/win32-stubs/lib/regutil.pyi` & `types-pywin32-306.0.0.2/win32-stubs/lib/regutil.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/lib/sspicon.pyi` & `types-pywin32-306.0.0.2/win32-stubs/lib/sspicon.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/lib/win2kras.pyi` & `types-pywin32-306.0.0.2/win32-stubs/lib/win2kras.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/lib/win32con.pyi` & `types-pywin32-306.0.0.2/win32-stubs/lib/win32con.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/lib/win32cryptcon.pyi` & `types-pywin32-306.0.0.2/win32-stubs/lib/win32cryptcon.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/lib/win32evtlogutil.pyi` & `types-pywin32-306.0.0.2/win32-stubs/lib/win32evtlogutil.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/lib/win32gui_struct.pyi` & `types-pywin32-306.0.0.2/win32-stubs/lib/win32gui_struct.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/lib/win32inetcon.pyi` & `types-pywin32-306.0.0.2/win32-stubs/lib/win32inetcon.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/lib/win32netcon.pyi` & `types-pywin32-306.0.0.2/win32-stubs/lib/win32netcon.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/lib/win32pdhquery.pyi` & `types-pywin32-306.0.0.2/win32-stubs/lib/win32pdhquery.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/lib/win32serviceutil.pyi` & `types-pywin32-306.0.0.2/win32-stubs/lib/win32serviceutil.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/lib/win32timezone.pyi` & `types-pywin32-306.0.0.2/win32-stubs/lib/win32timezone.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/lib/winerror.pyi` & `types-pywin32-306.0.0.2/win32-stubs/lib/winerror.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/lib/winioctlcon.pyi` & `types-pywin32-306.0.0.2/win32-stubs/lib/winioctlcon.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/lib/winnt.pyi` & `types-pywin32-306.0.0.2/win32-stubs/lib/winnt.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/lib/winperf.pyi` & `types-pywin32-306.0.0.2/win32-stubs/lib/winperf.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/lib/winxptheme.pyi` & `types-pywin32-306.0.0.2/win32-stubs/lib/winxptheme.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/odbc.pyi` & `types-pywin32-306.0.0.2/win32-stubs/odbc.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/servicemanager.pyi` & `types-pywin32-306.0.0.2/win32-stubs/servicemanager.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/win32api.pyi` & `types-pywin32-306.0.0.2/win32-stubs/win32api.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/win32clipboard.pyi` & `types-pywin32-306.0.0.2/win32-stubs/win32clipboard.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/win32console.pyi` & `types-pywin32-306.0.0.2/win32-stubs/win32console.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/win32cred.pyi` & `types-pywin32-306.0.0.2/win32-stubs/win32cred.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/win32crypt.pyi` & `types-pywin32-306.0.0.2/win32-stubs/win32crypt.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/win32event.pyi` & `types-pywin32-306.0.0.2/win32-stubs/win32event.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/win32evtlog.pyi` & `types-pywin32-306.0.0.2/win32-stubs/win32evtlog.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/win32file.pyi` & `types-pywin32-306.0.0.2/win32-stubs/win32file.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/win32gui.pyi` & `types-pywin32-306.0.0.2/win32-stubs/win32gui.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/win32help.pyi` & `types-pywin32-306.0.0.2/win32-stubs/win32help.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/win32inet.pyi` & `types-pywin32-306.0.0.2/win32-stubs/win32inet.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/win32job.pyi` & `types-pywin32-306.0.0.2/win32-stubs/win32job.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/win32net.pyi` & `types-pywin32-306.0.0.2/win32-stubs/win32net.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/win32pdh.pyi` & `types-pywin32-306.0.0.2/win32-stubs/win32pdh.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/win32pipe.pyi` & `types-pywin32-306.0.0.2/win32-stubs/win32pipe.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/win32print.pyi` & `types-pywin32-306.0.0.2/win32-stubs/win32print.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/win32process.pyi` & `types-pywin32-306.0.0.2/win32-stubs/win32process.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/win32profile.pyi` & `types-pywin32-306.0.0.2/win32-stubs/win32profile.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/win32ras.pyi` & `types-pywin32-306.0.0.2/win32-stubs/win32ras.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/win32security.pyi` & `types-pywin32-306.0.0.2/win32-stubs/win32security.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/win32service.pyi` & `types-pywin32-306.0.0.2/win32-stubs/win32service.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/win32trace.pyi` & `types-pywin32-306.0.0.2/win32-stubs/win32trace.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/win32transaction.pyi` & `types-pywin32-306.0.0.2/win32-stubs/win32transaction.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/win32ts.pyi` & `types-pywin32-306.0.0.2/win32-stubs/win32ts.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32-stubs/win32wnet.pyi` & `types-pywin32-306.0.0.2/win32-stubs/win32wnet.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32com-stubs/client/__init__.pyi` & `types-pywin32-306.0.0.2/win32com-stubs/client/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32com-stubs/client/build.pyi` & `types-pywin32-306.0.0.2/win32com-stubs/client/build.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32com-stubs/client/dynamic.pyi` & `types-pywin32-306.0.0.2/win32com-stubs/client/dynamic.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32com-stubs/olectl.pyi` & `types-pywin32-306.0.0.2/win32com-stubs/olectl.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32com-stubs/server/connect.pyi` & `types-pywin32-306.0.0.2/win32com-stubs/server/connect.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32com-stubs/server/dispatcher.pyi` & `types-pywin32-306.0.0.2/win32com-stubs/server/dispatcher.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32com-stubs/server/exception.pyi` & `types-pywin32-306.0.0.2/win32com-stubs/server/exception.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32com-stubs/server/policy.pyi` & `types-pywin32-306.0.0.2/win32com-stubs/server/policy.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32com-stubs/server/util.pyi` & `types-pywin32-306.0.0.2/win32com-stubs/server/util.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32com-stubs/storagecon.pyi` & `types-pywin32-306.0.0.2/win32com-stubs/storagecon.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32com-stubs/universal.pyi` & `types-pywin32-306.0.0.2/win32com-stubs/universal.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/adsi/__init__.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/adsi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/adsi/adsi.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/adsi/adsi.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/adsi/adsicon.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/adsi/adsicon.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/axcontrol/axcontrol.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/axcontrol/axcontrol.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/axdebug/adb.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/axdebug/adb.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/axdebug/axdebug.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/axdebug/axdebug.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/axdebug/codecontainer.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/axdebug/codecontainer.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/axdebug/contexts.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/axdebug/contexts.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/axdebug/debugger.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/axdebug/debugger.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/axdebug/documents.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/axdebug/documents.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/axdebug/expressions.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/axdebug/expressions.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/axdebug/gateways.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/axdebug/gateways.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/axdebug/stackframe.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/axdebug/stackframe.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/axscript/axscript.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/axscript/axscript.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/axscript/client/error.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/axscript/client/error.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/axscript/server/axsite.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/axscript/server/axsite.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/bits/bits.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/bits/bits.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/directsound/directsound.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/directsound/directsound.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/ifilter/ifilter.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/ifilter/ifilter.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/ifilter/ifiltercon.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/ifilter/ifiltercon.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/internet/inetcon.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/internet/inetcon.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/internet/internet.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/internet/internet.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/mapi/_exchdapi.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/mapi/_exchdapi.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/mapi/emsabtags.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/mapi/emsabtags.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/mapi/mapi.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/mapi/mapi.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/mapi/mapitags.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/mapi/mapitags.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/mapi/mapiutil.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/mapi/mapiutil.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/propsys/propsys.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/propsys/propsys.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/propsys/pscon.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/propsys/pscon.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/shell/shell.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/shell/shell.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/shell/shellcon.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/shell/shellcon.pyi`

 * *Files identical despite different names*

### Comparing `types-pywin32-306.0.0.1/win32comext-stubs/taskscheduler/taskscheduler.pyi` & `types-pywin32-306.0.0.2/win32comext-stubs/taskscheduler/taskscheduler.pyi`

 * *Files identical despite different names*

