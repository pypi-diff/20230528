# Comparing `tmp/gotify-tray-0.4.2.tar.gz` & `tmp/gotify-tray-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gotify-tray-0.4.2.tar", last modified: Sat Apr  8 12:33:42 2023, max compression
+gzip compressed data, was "gotify-tray-0.5.0.tar", last modified: Sat May 27 22:42:56 2023, max compression
```

## Comparing `gotify-tray-0.4.2.tar` & `gotify-tray-0.5.0.tar`

### file list

```diff
@@ -1,99 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:33:42.886032 gotify-tray-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-08 12:33:42.886032 gotify-tray-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:33:42.858031 gotify-tray-0.4.2/gotify_tray/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:33:42.862031 gotify-tray-0.4.2/gotify_tray/database/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/database/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/database/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/database/default_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/database/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/database/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:33:42.866031 gotify-tray-0.4.2/gotify_tray/gotify/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gotify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gotify/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gotify/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gotify/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:33:42.866031 gotify-tray-0.4.2/gotify_tray/gui/
--rw-r--r--   0 runner    (1001) docker     (123)    17974 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/MainApplication.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:33:42.866031 gotify-tray-0.4.2/gotify_tray/gui/designs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/designs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/designs/widget_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/designs/widget_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/designs/widget_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    18295 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/designs/widget_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:33:42.874031 gotify-tray-0.4.2/gotify_tray/gui/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   346772 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/images/gotify-small-macos.png
--rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/images/gotify-small.png
--rw-r--r--   0 runner    (1001) docker     (123)    73216 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/images/logo-macos.ico
--rw-r--r--   0 runner    (1001) docker     (123)   135098 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/images/logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)   339880 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/images/tray-error-macos.png
--rw-r--r--   0 runner    (1001) docker     (123)    17860 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/images/tray-error.png
--rw-r--r--   0 runner    (1001) docker     (123)   341637 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/images/tray-macos.png
--rw-r--r--   0 runner    (1001) docker     (123)   341277 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/images/tray-unread-macos.png
--rw-r--r--   0 runner    (1001) docker     (123)    17854 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/images/tray-unread.png
--rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/images/tray.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:33:42.874031 gotify-tray-0.4.2/gotify_tray/gui/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/models/ApplicationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/models/MessagesModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:33:42.874031 gotify-tray-0.4.2/gotify_tray/gui/themes/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/themes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:33:42.878032 gotify-tray-0.4.2/gotify_tray/gui/themes/dark_purple/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/themes/dark_purple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/themes/dark_purple/palette.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/themes/dark_purple/refresh.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/themes/dark_purple/status_active.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/themes/dark_purple/status_connecting.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/themes/dark_purple/status_error.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/themes/dark_purple/status_inactive.svg
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/themes/dark_purple/style.qss
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/themes/dark_purple/trashcan.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:33:42.878032 gotify-tray-0.4.2/gotify_tray/gui/themes/default/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/themes/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/themes/default/palette.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/themes/default/refresh.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/themes/default/status_active.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/themes/default/status_connecting.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/themes/default/status_error.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/themes/default/status_inactive.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/themes/default/style.qss
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/themes/default/trashcan.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:33:42.882032 gotify-tray-0.4.2/gotify_tray/gui/themes/light_purple/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/themes/light_purple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/themes/light_purple/palette.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/themes/light_purple/refresh.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/themes/light_purple/status_active.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/themes/light_purple/status_connecting.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/themes/light_purple/status_error.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/themes/light_purple/status_inactive.svg
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/themes/light_purple/style.qss
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/themes/light_purple/trashcan.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:33:42.886032 gotify-tray-0.4.2/gotify_tray/gui/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/widgets/ImagePopup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/widgets/MainWindow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/widgets/MessageWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/widgets/ServerInfoDialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/widgets/SettingsDialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/widgets/StatusWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/widgets/Tray.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/gui/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/gotify_tray/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:33:42.862031 gotify-tray-0.4.2/gotify_tray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-08 12:33:42.000000 gotify-tray-0.4.2/gotify_tray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-08 12:33:42.000000 gotify-tray-0.4.2/gotify_tray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 12:33:42.000000 gotify-tray-0.4.2/gotify_tray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-08 12:33:42.000000 gotify-tray-0.4.2/gotify_tray.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-08 12:33:42.000000 gotify-tray-0.4.2/gotify_tray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-08 12:33:42.000000 gotify-tray-0.4.2/gotify_tray.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 12:33:42.886032 gotify-tray-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-08 12:33:16.000000 gotify-tray-0.4.2/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:56.939483 gotify-tray-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-27 22:42:56.939483 gotify-tray-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:56.923482 gotify-tray-0.5.0/gotify_tray/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:56.923482 gotify-tray-0.5.0/gotify_tray/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/database/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/database/default_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/database/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/database/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:56.927482 gotify-tray-0.5.0/gotify_tray/gotify/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gotify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gotify/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gotify/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gotify/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:56.927482 gotify-tray-0.5.0/gotify_tray/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)    15871 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/MainApplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:56.927482 gotify-tray-0.5.0/gotify_tray/gui/designs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/designs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/designs/widget_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/designs/widget_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/designs/widget_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/designs/widget_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:56.931482 gotify-tray-0.5.0/gotify_tray/gui/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   346772 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/images/gotify-small-macos.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/images/gotify-small.png
+-rw-r--r--   0 runner    (1001) docker     (123)    73216 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/images/logo-macos.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   135098 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/images/logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   339880 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/images/tray-error-macos.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17860 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/images/tray-error.png
+-rw-r--r--   0 runner    (1001) docker     (123)   341637 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/images/tray-macos.png
+-rw-r--r--   0 runner    (1001) docker     (123)   341277 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/images/tray-unread-macos.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17854 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/images/tray-unread.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/images/tray.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:56.931482 gotify-tray-0.5.0/gotify_tray/gui/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/models/ApplicationModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/models/MessagesModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:56.935483 gotify-tray-0.5.0/gotify_tray/gui/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:56.935483 gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/refresh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/status_active.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/status_connecting.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/status_error.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/status_inactive.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/style.qss
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/trashcan.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:56.935483 gotify-tray-0.5.0/gotify_tray/gui/themes/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/default/palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/default/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:56.939483 gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/refresh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/status_active.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/status_connecting.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/status_error.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/status_inactive.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/style.qss
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/trashcan.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:56.939483 gotify-tray-0.5.0/gotify_tray/gui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/widgets/ImagePopup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/widgets/MainWindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/widgets/MessageWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/widgets/ServerInfoDialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/widgets/SettingsDialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/widgets/StatusWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/widgets/Tray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:56.923482 gotify-tray-0.5.0/gotify_tray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-27 22:42:56.000000 gotify-tray-0.5.0/gotify_tray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-27 22:42:56.000000 gotify-tray-0.5.0/gotify_tray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 22:42:56.000000 gotify-tray-0.5.0/gotify_tray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-27 22:42:56.000000 gotify-tray-0.5.0/gotify_tray.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-27 22:42:56.000000 gotify-tray-0.5.0/gotify_tray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-27 22:42:56.000000 gotify-tray-0.5.0/gotify_tray.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 22:42:56.939483 gotify-tray-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/version.txt
```

### Comparing `gotify-tray-0.4.2/LICENSE` & `gotify-tray-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/PKG-INFO` & `gotify-tray-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: gotify-tray
-Version: 0.4.2
+Version: 0.5.0
 Summary: A tray notification application for receiving messages from a Gotify server.
 Home-page: https://github.com/seird/gotify-tray
 Author: k.dries@protonmail.com
 Author-email: k.dries@protonmail.com
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8.0
+Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Gotify Tray
 
 
@@ -71,8 +69,8 @@
 ## Build instructions
 
 See [BUILDING](BUILDING.md).
 
 
 ## Requirements
 
-- python >=3.8
+- python >=3.10
```

### Comparing `gotify-tray-0.4.2/README.md` & `gotify-tray-0.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -52,8 +52,8 @@
 ## Build instructions
 
 See [BUILDING](BUILDING.md).
 
 
 ## Requirements
 
-- python >=3.8
+- python >=3.10
```

### Comparing `gotify-tray-0.4.2/gotify_tray/database/cache.py` & `gotify-tray-0.5.0/gotify_tray/database/cache.py`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/database/database.py` & `gotify-tray-0.5.0/gotify_tray/database/database.py`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/database/default_settings.py` & `gotify-tray-0.5.0/gotify_tray/database/default_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import os
 from pathlib import Path
 
 from ..__version__ import __title__
 
 
 DEFAULT_SETTINGS = {
-    "theme": "default",
+    "theme": "automatic",
     "message/check_missed/notify": True,
+    "locale": False,
     "logging/level": "Disabled",
     "export/path": os.path.join(
         Path.home(), f"{__title__.replace(' ', '-').lower()}-settings.bytes"
     ),
     "shortcuts/quit": "Ctrl+Q",
     "tray/notifications/priority": 5,
     "tray/notifications/duration_ms": 5000,
     "tray/notifications/icon/show": True,
     "tray/notifications/click": True,
     "tray/icon/unread": False,
     "watchdog/interval/s": 60,
+    "MessageWidget/height/min": 100,
     "MessageWidget/image/size": 33,
     "MessageWidget/content_image/W_percentage": 1.0,
     "MessageWidget/content_image/H_percentage": 0.5,
     "MessageWidget/priority_color": True,
     "MainWindow/label/size": 25,
     "MainWindow/button/size": 33,
     "MainWindow/application/icon/size": 40,
```

### Comparing `gotify-tray-0.4.2/gotify_tray/database/downloader.py` & `gotify-tray-0.5.0/gotify_tray/database/downloader.py`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/database/settings.py` & `gotify-tray-0.5.0/gotify_tray/database/settings.py`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/gotify/api.py` & `gotify-tray-0.5.0/gotify_tray/gotify/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import Callable, List, Optional, Union
+from typing import Callable
 
 import requests
 
 from .listener import Listener
 from .models import (
     GotifyApplicationModel,
     GotifyErrorModel,
@@ -18,20 +18,20 @@
 
 
 class GotifySession(object):
     def __init__(self, url: str, token: str):
         self.session = requests.Session()
         self.update_auth(url.rstrip("/"), token)
 
-    def update_auth(self, url: str = None, token: str = None):
+    def update_auth(self, url: str | None = None, token: str | None = None):
         if url:
             self.url = url
         if token:
             self.token = token
-        self.session.headers.update({"X-Gotify-Key": token})
+            self.session.headers.update({"X-Gotify-Key": token})
 
     def _get(self, endpoint: str = "/", **kwargs) -> requests.Response:
         return self.session.get(self.url + endpoint, **kwargs)
 
     def _post(self, endpoint: str = "/", **kwargs) -> requests.Response:
         return self.session.post(self.url + endpoint, **kwargs)
 
@@ -46,16 +46,16 @@
 
 
 class GotifyApplication(GotifySession):
     def __init__(self, url: str, application_token: str):
         super(GotifyApplication, self).__init__(url, application_token)
 
     def push(
-        self, title: str = "", message: str = "", priority: int = 0, extras: dict = None
-    ) -> Union[GotifyMessageModel, GotifyErrorModel]:
+        self, title: str = "", message: str = "", priority: int = 0, extras: dict | None = None
+    ) -> GotifyMessageModel | GotifyErrorModel:
         response = self._post(
             "/message",
             json={
                 "title": title,
                 "message": message,
                 "priority": priority,
                 "extras": extras,
@@ -73,37 +73,37 @@
 
 class GotifyClient(GotifySession):
 
     """
     Application
     """
 
-    def get_applications(self) -> Union[List[GotifyApplicationModel], GotifyErrorModel]:
+    def get_applications(self) -> list[GotifyApplicationModel] | GotifyErrorModel:
         response = self._get("/application")
         return (
             [GotifyApplicationModel(x) for x in response.json()]
             if response.ok
             else GotifyErrorModel(response)
         )
 
     def create_application(
         self, name: str, description: str = ""
-    ) -> Union[GotifyApplicationModel, GotifyErrorModel]:
+    ) -> GotifyApplicationModel | GotifyErrorModel:
         response = self._post(
             "/application", json={"name": name, "description": description}
         )
         return (
             GotifyApplicationModel(response.json())
             if response.ok
             else GotifyErrorModel(response)
         )
 
     def update_application(
         self, application_id: int, name: str, description: str = ""
-    ) -> Union[GotifyApplicationModel, GotifyErrorModel]:
+    ) -> GotifyApplicationModel | GotifyErrorModel:
         response = self._put(
             f"/application/{application_id}",
             json={"name": name, "description": description},
         )
         return (
             GotifyApplicationModel(response.json())
             if response.ok
@@ -111,15 +111,15 @@
         )
 
     def delete_application(self, application_id: int) -> bool:
         return self._delete(f"/application/{application_id}").ok
 
     def upload_application_image(
         self, application_id: int, img_path: str
-    ) -> Optional[Union[GotifyApplicationModel, GotifyErrorModel]]:
+    ) -> GotifyApplicationModel | GotifyErrorModel | None:
         try:
             with open(img_path, "rb") as f:
                 response = self._post(
                     f"/application/{application_id}/image", files={"file": f}
                 )
             return (
                 GotifyApplicationModel(response.json())
@@ -133,16 +133,16 @@
             return None
 
     """
     Message
     """
 
     def get_application_messages(
-        self, application_id: int, limit: int = 100, since: int = None
-    ) -> Union[GotifyPagedMessagesModel, GotifyErrorModel]:
+        self, application_id: int, limit: int = 100, since: int | None = None
+    ) -> GotifyPagedMessagesModel | GotifyErrorModel:
         response = self._get(
             f"/application/{application_id}/message",
             params={"limit": limit, "since": since},
         )
         if not response.ok:
             return GotifyErrorModel(response)
         j = response.json()
@@ -151,16 +151,16 @@
             paging=GotifyPagingModel(j["paging"]),
         )
 
     def delete_application_messages(self, application_id: int) -> bool:
         return self._delete(f"/application/{application_id}/message").ok
 
     def get_messages(
-        self, limit: int = 100, since: int = None
-    ) -> Union[GotifyPagedMessagesModel, GotifyErrorModel]:
+        self, limit: int = 100, since: int | None = None
+    ) -> GotifyPagedMessagesModel | GotifyErrorModel:
         response = self._get("/message", params={"limit": limit, "since": since})
         if not response.ok:
             return GotifyErrorModel(response)
         j = response.json()
         return GotifyPagedMessagesModel(
             messages=[GotifyMessageModel(m) for m in j["messages"]],
             paging=GotifyPagingModel(j["paging"]),
@@ -170,30 +170,30 @@
         return self._delete("/message").ok
 
     def delete_message(self, message_id: int) -> bool:
         return self._delete(f"/message/{message_id}").ok
 
     def listen(
         self,
-        opened_callback: Callable[[], None] = None,
-        closed_callback: Callable[[int, str], None] = None,
-        new_message_callback: Callable[[GotifyMessageModel], None] = None,
-        error_callback: Callable[[Exception], None] = None,
+        opened_callback: (Callable[[], None]) | None = None,
+        closed_callback: Callable[[int, str], None] | None = None,
+        new_message_callback: Callable[[GotifyMessageModel], None] | None = None,
+        error_callback: Callable[[Exception], None] | None = None,
     ):
         def dummy(*args):
             ...
 
         self.listener = Listener(self.url, self.token)
         self.listener.opened.connect(lambda: self.opened_callback(opened_callback))
         self.listener.closed.connect(closed_callback or dummy)
         self.listener.new_message.connect(new_message_callback or dummy)
         self.listener.error.connect(error_callback or dummy)
         self.listener.start()
 
-    def opened_callback(self, user_callback: Callable[[], None] = None):
+    def opened_callback(self, user_callback: Callable[[], None] | None = None):
         self.reset_wait_time()
         if user_callback:
             user_callback()
 
     def reconnect(self):
         if not self.is_listening():
             self.listener.start()
@@ -218,26 +218,26 @@
     def reset_wait_time(self):
         self.listener.reset_wait_time()
 
     """
     Health
     """
 
-    def health(self) -> Union[GotifyHealthModel, GotifyErrorModel]:
+    def health(self) -> GotifyHealthModel | GotifyErrorModel:
         response = self._get("/health")
         return (
             GotifyHealthModel(response.json())
             if response.ok
             else GotifyErrorModel(response)
         )
 
     """
     Version
     """
 
-    def version(self) -> Union[GotifyVersionModel, GotifyErrorModel]:
+    def version(self) -> GotifyVersionModel | GotifyErrorModel:
         response = self._get("/version")
         return (
             GotifyVersionModel(response.json())
             if response.ok
             else GotifyErrorModel(response)
         )
```

### Comparing `gotify-tray-0.4.2/gotify_tray/gotify/listener.py` & `gotify-tray-0.5.0/gotify_tray/gotify/listener.py`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/gotify/models.py` & `gotify-tray-0.5.0/gotify_tray/gotify/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import datetime
 from dateutil.parser import isoparse
 import logging
-from typing import List, Optional
 
 import requests
 
 
 logger = logging.getLogger("gotify-tray")
 
 
@@ -29,37 +28,37 @@
     internal: bool
     name: str
     token: str
 
 
 class GotifyPagingModel(AttributeDict):
     limit: int
-    next: Optional[str] = None
+    next: str | None = None
     since: int
     size: int
 
 
 class GotifyMessageModel(AttributeDict):
     appid: int
     date: datetime.datetime
-    extras: Optional[dict] = None
+    extras: dict | None = None
     id: int
     message: str
-    priority: Optional[int] = None
-    title: Optional[str] = None
+    priority: int | None = None
+    title: str | None = None
 
     def __init__(self, d: dict, *args, **kwargs):
         d.update(
             {"date": isoparse(d["date"]).astimezone(local_timezone)}
         )
         super(GotifyMessageModel, self).__init__(d, *args, **kwargs)
 
 
 class GotifyPagedMessagesModel(AttributeDict):
-    messages: List[GotifyMessageModel]
+    messages: list[GotifyMessageModel]
     paging: GotifyPagingModel
 
 
 class GotifyHealthModel(AttributeDict):
     database: str
     health: str
```

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/MainApplication.py` & `gotify-tray-0.5.0/gotify_tray/gui/MainApplication.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import getpass
 import logging
 import os
 import platform
 import sys
 import tempfile
-from typing import List, Union
 
 from gotify_tray import gotify
 from gotify_tray.__version__ import __title__
 from gotify_tray.database import Downloader, Settings
 from gotify_tray.tasks import (
     ClearCacheTask,
     DeleteApplicationMessagesTask,
     DeleteAllMessagesTask,
     DeleteMessageTask,
     GetApplicationsTask,
     GetApplicationMessagesTask,
     GetMessagesTask,
     ProcessMessageTask,
-    ProcessMessagesTask,
     ServerConnectionWatchdogTask,
 )
 from gotify_tray.gui.themes import set_theme
 from gotify_tray.utils import get_icon, verify_server
 from PyQt6 import QtCore, QtGui, QtWidgets
 
 from ..__version__ import __title__
@@ -47,17 +45,15 @@
 
 def init_logger(logger: logging.Logger):
     if (level := settings.value("logging/level", type=str)) != "Disabled":
         logger.setLevel(level)
     else:
         logging.disable()
 
-    logdir = QtCore.QStandardPaths.standardLocations(
-        QtCore.QStandardPaths.StandardLocation.AppDataLocation
-    )[0]
+    logdir = QtCore.QStandardPaths.standardLocations(QtCore.QStandardPaths.StandardLocation.AppDataLocation)[0]
     if not os.path.exists(logdir):
         os.mkdir(logdir)
     logging.basicConfig(
         filename=os.path.join(logdir, f"{title}.log"),
         format="%(levelname)s > %(name)s > %(asctime)s > %(filename)20s:%(lineno)3s - %(funcName)20s() > %(message)s",
     )
 
@@ -72,29 +68,29 @@
         )
 
         self.downloader = Downloader()
 
         self.messages_model = MessagesModel()
         self.application_model = ApplicationModel()
 
-        self.main_window = MainWindow(self.application_model, self.messages_model)
+        self.main_window = MainWindow(self, self.application_model, self.messages_model)
         self.main_window.show()  # The initial .show() is necessary to get the correct sizes when adding MessageWigets
         QtCore.QTimer.singleShot(0, self.main_window.hide)
 
         self.refresh_applications()
 
         self.tray = Tray()
         self.tray.show()
 
         self.first_connect = True
 
         self.gotify_client.listen(
-            new_message_callback=self.new_message_callback,
             opened_callback=self.listener_opened_callback,
             closed_callback=self.listener_closed_callback,
+            new_message_callback=self.new_message_callback,
             error_callback=self.listener_error_callback,
         )
 
         self.watchdog = ServerConnectionWatchdogTask(self.gotify_client)
 
         self.link_callbacks()
         self.init_shortcuts()
@@ -104,37 +100,25 @@
     def refresh_applications(self):
         self.messages_model.clear()
         self.application_model.clear()
 
         self.application_model.setItem(0, 0, ApplicationAllMessagesItem())
 
         self.get_applications_task = GetApplicationsTask(self.gotify_client)
-        self.get_applications_task.success.connect(
-            self.get_applications_success_callback
-        )
-        self.get_applications_task.started.connect(
-            self.main_window.disable_applications
-        )
-        self.get_applications_task.finished.connect(
-            self.main_window.enable_applications
-        )
+        self.get_applications_task.success.connect(self.get_applications_success_callback)
+        self.get_applications_task.started.connect(self.main_window.disable_applications)
+        self.get_applications_task.finished.connect(self.main_window.enable_applications)
         self.get_applications_task.start()
 
     def get_applications_success_callback(
-        self, applications: List[gotify.GotifyApplicationModel],
+        self, applications: list[gotify.GotifyApplicationModel],
     ):
         for i, application in enumerate(applications):
-            icon = QtGui.QIcon(
-                self.downloader.get_filename(
-                    f"{self.gotify_client.url}/{application.image}"
-                )
-            )
-            self.application_model.setItem(
-                i + 1, 0, ApplicationModelItem(application, icon),
-            )
+            icon = QtGui.QIcon(self.downloader.get_filename(f"{self.gotify_client.url}/{application.image}"))
+            self.application_model.setItem(i + 1, 0, ApplicationModelItem(application, icon))
 
     def update_last_id(self, i: int):
         if i > settings.value("message/last", type=int):
             settings.setValue("message/last", i)
 
     def listener_opened_callback(self):
         self.main_window.set_active()
@@ -149,179 +133,121 @@
             last_id = settings.value("message/last", type=int)
             ids = []
 
             page.messages.reverse()
             for message in page.messages:
                 if message.id > last_id:
                     if settings.value("message/check_missed/notify", type=bool):
-                        self.new_message_callback(message)
+                        self.new_message_callback(message, process=False)
                     else:
-                        self.add_message_to_model(message)
+                        self.add_message_to_model(message, process=False)
                     ids.append(message.id)
 
             if ids:
                 self.update_last_id(max(ids))
 
         self.get_missed_messages_task = GetMessagesTask(self.gotify_client)
         self.get_missed_messages_task.success.connect(get_missed_messages_callback)
         self.get_missed_messages_task.start()
 
     def listener_closed_callback(self, close_status_code: int, close_msg: str):
         self.main_window.set_connecting()
         self.tray.set_icon_error()
         self.gotify_client.increase_wait_time()
-        QtCore.QTimer.singleShot(
-            self.gotify_client.get_wait_time() * 1000, self.gotify_client.reconnect
-        )
+        QtCore.QTimer.singleShot(self.gotify_client.get_wait_time() * 1000, self.gotify_client.reconnect)
 
     def listener_error_callback(self, exception: Exception):
         self.main_window.set_connecting()
         self.tray.set_icon_error()
 
     def reconnect_callback(self):
         if not self.gotify_client.is_listening():
             self.gotify_client.listener.reset_wait_time()
             self.gotify_client.reconnect()
         else:
             self.gotify_client.stop(reset_wait=True)
 
-    def insert_message(
-        self,
-        row: int,
-        message: gotify.GotifyMessageModel,
-        application: gotify.GotifyApplicationModel,
-    ):
-        """Insert a message gotify message into the messages model. Also add the message widget to the listview
-
-        Args:
-            row (int): >=0: insert message at specified position, <0: append message to the end of the model
-            message (gotify.GotifyMessageModel): message
-            application (gotify.GotifyApplicationModel): application
+    def abort_get_messages_task(self):
         """
-        self.update_last_id(message.id)
-        message_item = MessagesModelItem(message)
-
-        if row >= 0:
-            self.messages_model.insertRow(row, message_item)
-        else:
-            self.messages_model.appendRow(message_item)
-
-        self.main_window.insert_message_widget(
-            message_item,
-            self.downloader.get_filename(
-                f"{self.gotify_client.url}/{application.image}"
-            ),
-        )
-
-    def get_messages_finished_callback(self, page: gotify.GotifyPagedMessagesModel):
-        """Process messages before inserting them into the main window
+        Abort any tasks that will result in new messages getting appended to messages_model
         """
+        aborted_tasks = []
+        for s in ["get_application_messages_task", "get_messages_task"]:
+            if task := getattr(self, s, None):
+                task.abort()
+                aborted_tasks.append(task)
+        
+        for task in aborted_tasks:
+            task.wait()
 
-        def insert_helper(message: gotify.GotifyMessageModel):
-            if item := self.application_model.itemFromId(message.appid):
-                self.insert_message(
-                    -1, message, item.data(ApplicationItemDataRole.ApplicationRole)
-                )
-                self.processEvents()
-
-        self.process_messages_task = ProcessMessagesTask(page)
-        self.process_messages_task.message_processed.connect(insert_helper)
-        self.process_messages_task.start()
-
-    def application_selection_changed_callback(
-        self, item: Union[ApplicationModelItem, ApplicationAllMessagesItem]
-    ):
+    def application_selection_changed_callback(self, item: ApplicationModelItem | ApplicationAllMessagesItem):
+        self.abort_get_messages_task()
         self.messages_model.clear()
 
         if isinstance(item, ApplicationModelItem):
-            self.get_application_messages_task = GetApplicationMessagesTask(
-                item.data(ApplicationItemDataRole.ApplicationRole).id,
-                self.gotify_client,
-            )
-            self.get_application_messages_task.success.connect(
-                self.get_messages_finished_callback
-            )
+            self.get_application_messages_task = GetApplicationMessagesTask(item.data(ApplicationItemDataRole.ApplicationRole).id, self.gotify_client)
+            self.get_application_messages_task.message.connect(self.messages_model.append_message)
             self.get_application_messages_task.start()
 
         elif isinstance(item, ApplicationAllMessagesItem):
             self.get_messages_task = GetMessagesTask(self.gotify_client)
-            self.get_messages_task.success.connect(self.get_messages_finished_callback)
+            self.get_messages_task.message.connect(self.messages_model.append_message)
             self.get_messages_task.start()
 
-    def add_message_to_model(self, message: gotify.GotifyMessageModel):
-        if application_item := self.application_model.itemFromId(message.appid):
+    def add_message_to_model(self, message: gotify.GotifyMessageModel, process: bool = True):
+        if self.application_model.itemFromId(message.appid):
             application_index = self.main_window.currentApplicationIndex()
-            if selected_application_item := self.application_model.itemFromIndex(
-                application_index
-            ):
+            if selected_application_item := self.application_model.itemFromIndex(application_index):
 
                 def insert_message_helper():
                     if isinstance(selected_application_item, ApplicationModelItem):
                         # A single application is selected
+                        # -> Only insert the message if the appid matches the selected appid
                         if (
-                            message.appid
-                            == selected_application_item.data(
-                                ApplicationItemDataRole.ApplicationRole
-                            ).id
+                            message.appid 
+                            == selected_application_item.data(ApplicationItemDataRole.ApplicationRole).id
                         ):
-                            self.insert_message(
-                                0,
-                                message,
-                                application_item.data(
-                                    ApplicationItemDataRole.ApplicationRole
-                                ),
-                            )
-                    elif isinstance(
-                        selected_application_item, ApplicationAllMessagesItem
-                    ):
+                            self.messages_model.insert_message(0, message)
+                    elif isinstance(selected_application_item, ApplicationAllMessagesItem):
                         # "All messages' is selected
-                        self.insert_message(
-                            0,
-                            message,
-                            application_item.data(
-                                ApplicationItemDataRole.ApplicationRole
-                            ),
-                        )
-
-                self.process_message_task = ProcessMessageTask(message)
-                self.process_message_task.finished.connect(insert_message_helper)
-                self.process_message_task.start()
+                        self.messages_model.insert_message(0, message)
+
+                if process:
+                    self.process_message_task = ProcessMessageTask(message)
+                    self.process_message_task.finished.connect(insert_message_helper)
+                    self.process_message_task.start()
+                else:
+                    insert_message_helper()
         else:
-            logger.error(
-                f"App id {message.appid} could not be found. Refreshing applications."
-            )
+            logger.error(f"App id {message.appid} could not be found. Refreshing applications.")
             self.refresh_applications()
 
-    def new_message_callback(self, message: gotify.GotifyMessageModel):
-        self.add_message_to_model(message)
+    def new_message_callback(self, message: gotify.GotifyMessageModel, process: bool = True):
+        self.add_message_to_model(message, process=process)
 
         # Change the tray icon to show there are unread notifications
         if (
             settings.value("tray/icon/unread", type=bool)
             and not self.main_window.isActiveWindow()
         ):
             self.tray.set_icon_unread()
 
-        # Show a notification
+        # Don't show a notification if it's low priority or the window is active
         if (
             message.priority < settings.value("tray/notifications/priority", type=int)
             or self.main_window.isActiveWindow()
         ):
             return
 
-        if settings.value("tray/notifications/icon/show", type=bool):
-            if application_item := self.application_model.itemFromId(message.appid):
-                image_url = f"{self.gotify_client.url}/{application_item.data(ApplicationItemDataRole.ApplicationRole).image}"
-                icon = QtGui.QIcon(self.downloader.get_filename(image_url))
-            else:
-                logger.error(
-                    f"MainWindow.new_message_callback: App id {message.appid} could not be found. Refreshing applications."
-                )
-                self.refresh_applications()
-                icon = QtWidgets.QSystemTrayIcon.MessageIcon.Information
+        # Get the application icon
+        if (
+            settings.value("tray/notifications/icon/show", type=bool)
+            and (application_item := self.application_model.itemFromId(message.appid))
+        ):
+            icon = application_item.icon()
         else:
             icon = QtWidgets.QSystemTrayIcon.MessageIcon.Information
 
         self.tray.showMessage(
             message.title,
             message.message,
             icon,
@@ -332,15 +258,15 @@
         self.delete_message_task = DeleteMessageTask(
             message_item.data(MessageItemDataRole.MessageRole).id, self.gotify_client
         )
         self.messages_model.removeRow(message_item.row())
         self.delete_message_task.start()
 
     def delete_all_messages_callback(
-        self, item: Union[ApplicationModelItem, ApplicationAllMessagesItem]
+        self, item: ApplicationModelItem | ApplicationAllMessagesItem
     ):
         if isinstance(item, ApplicationModelItem):
             self.delete_application_messages_task = DeleteApplicationMessagesTask(
                 item.data(ApplicationItemDataRole.ApplicationRole).id,
                 self.gotify_client,
             )
             self.delete_application_messages_task.start()
@@ -371,25 +297,21 @@
         set_theme(self, theme)
 
         # Update the main window icons
         self.main_window.set_icons()
 
         # Update the message widget icons
         for r in range(self.messages_model.rowCount()):
-            message_widget: MessageWidget = self.main_window.listView_messages.indexWidget(
-                self.messages_model.index(r, 0)
-            )
+            message_widget: MessageWidget = self.main_window.listView_messages.indexWidget(self.messages_model.index(r, 0))
             message_widget.set_icons()
 
     def settings_callback(self):
-        settings_dialog = SettingsDialog()
+        settings_dialog = SettingsDialog(self)
         settings_dialog.quit_requested.connect(self.quit)
-        settings_dialog.theme_change_requested.connect(
-            self.theme_change_requested_callback
-        )
+        settings_dialog.theme_change_requested.connect(self.theme_change_requested_callback)
         accepted = settings_dialog.exec()
 
         if accepted and settings_dialog.settings_changed:
             settings_dialog.apply_settings()
 
         if settings_dialog.server_changed:
             # Restart the listener
@@ -424,36 +346,36 @@
         self.tray.actionShowWindow.triggered.connect(self.main_window.bring_to_front)
         self.tray.actionReconnect.triggered.connect(self.reconnect_callback)
         self.tray.messageClicked.connect(self.tray_notification_clicked_callback)
         self.tray.activated.connect(self.tray_activated_callback)
 
         self.main_window.refresh.connect(self.refresh_applications)
         self.main_window.delete_all.connect(self.delete_all_messages_callback)
-        self.main_window.application_selection_changed.connect(
-            self.application_selection_changed_callback
-        )
+        self.main_window.application_selection_changed.connect(self.application_selection_changed_callback)
         self.main_window.delete_message.connect(self.delete_message_callback)
         self.main_window.image_popup.connect(self.image_popup_callback)
         self.main_window.hidden.connect(self.main_window_hidden_callback)
         self.main_window.activated.connect(self.tray.revert_icon)
+        
+        self.styleHints().colorSchemeChanged.connect(lambda _: self.theme_change_requested_callback(settings.value("theme", type=str)))
 
-        self.watchdog.closed.connect(lambda: self.listener_closed_callback(None, None))
+        self.messages_model.rowsInserted.connect(self.main_window.display_message_widgets)
+
+        self.watchdog.closed.connect(lambda: self.listener_closed_callback(0, 0))
 
     def init_shortcuts(self):
         self.shortcut_quit = QtGui.QShortcut(
             QtGui.QKeySequence.fromString(settings.value("shortcuts/quit", type=str)),
             self.main_window,
         )
         self.shortcut_quit.activated.connect(self.quit)
 
     def acquire_lock(self) -> bool:
         temp_dir = tempfile.gettempdir()
-        lock_filename = os.path.join(
-            temp_dir, __title__ + "-" + getpass.getuser() + ".lock"
-        )
+        lock_filename = os.path.join(temp_dir, __title__ + "-" + getpass.getuser() + ".lock")
         self.lock_file = QtCore.QLockFile(lock_filename)
         self.lock_file.setStaleLockTime(0)
         return self.lock_file.tryLock()
 
     def quit(self) -> None:
         self.main_window.store_state()
```

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/designs/widget_main.py` & `gotify-tray-0.5.0/gotify_tray/gui/designs/widget_main.py`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/designs/widget_message.py` & `gotify-tray-0.5.0/gotify_tray/gui/designs/widget_message.py`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/designs/widget_server.py` & `gotify-tray-0.5.0/gotify_tray/gui/designs/widget_server.py`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/designs/widget_settings.py` & `gotify-tray-0.5.0/gotify_tray/gui/designs/widget_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from PyQt6 import QtCore, QtGui, QtWidgets
 
 
 class Ui_Dialog(object):
     def setupUi(self, Dialog):
         Dialog.setObjectName("Dialog")
-        Dialog.resize(402, 392)
+        Dialog.resize(415, 450)
         self.gridLayout = QtWidgets.QGridLayout(Dialog)
         self.gridLayout.setObjectName("gridLayout")
         self.buttonBox = QtWidgets.QDialogButtonBox(Dialog)
         self.buttonBox.setOrientation(QtCore.Qt.Orientation.Horizontal)
         self.buttonBox.setStandardButtons(QtWidgets.QDialogButtonBox.StandardButton.Apply|QtWidgets.QDialogButtonBox.StandardButton.Cancel|QtWidgets.QDialogButtonBox.StandardButton.Ok)
         self.buttonBox.setObjectName("buttonBox")
         self.gridLayout.addWidget(self.buttonBox, 1, 0, 1, 1)
@@ -77,14 +77,17 @@
         self.horizontalLayout_3.addWidget(self.combo_theme)
         spacerItem1 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
         self.horizontalLayout_3.addItem(spacerItem1)
         self.verticalLayout_2.addLayout(self.horizontalLayout_3)
         self.cb_priority_colors = QtWidgets.QCheckBox(self.groupBox_2)
         self.cb_priority_colors.setObjectName("cb_priority_colors")
         self.verticalLayout_2.addWidget(self.cb_priority_colors)
+        self.cb_locale = QtWidgets.QCheckBox(self.groupBox_2)
+        self.cb_locale.setObjectName("cb_locale")
+        self.verticalLayout_2.addWidget(self.cb_locale)
         self.verticalLayout_4.addWidget(self.groupBox_2)
         self.groupBox_server_info = QtWidgets.QGroupBox(self.tab_general)
         self.groupBox_server_info.setObjectName("groupBox_server_info")
         self.gridLayout_3 = QtWidgets.QGridLayout(self.groupBox_server_info)
         self.gridLayout_3.setObjectName("gridLayout_3")
         self.pb_change_server_info = QtWidgets.QPushButton(self.groupBox_server_info)
         self.pb_change_server_info.setObjectName("pb_change_server_info")
@@ -236,14 +239,15 @@
         self.label_notification_priority.setText(_translate("Dialog", "Minimum priority to show notifications:"))
         self.cb_tray_icon_unread.setText(_translate("Dialog", "Change the tray icon color when there are unread notifications"))
         self.groupBox_2.setTitle(_translate("Dialog", "Interface"))
         self.label_theme.setText(_translate("Dialog", "Theme:"))
         self.cb_priority_colors.setToolTip(_translate("Dialog", "4..7   -> medium\n"
 "8..10 -> high"))
         self.cb_priority_colors.setText(_translate("Dialog", "Show message priority colors"))
+        self.cb_locale.setText(_translate("Dialog", "Display date in the system locale format"))
         self.groupBox_server_info.setTitle(_translate("Dialog", "Server info"))
         self.pb_change_server_info.setText(_translate("Dialog", "Change server info"))
         self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_general), _translate("Dialog", "General"))
         self.pb_reset_fonts.setText(_translate("Dialog", "Reset all fonts"))
         self.groupBox_fonts_message.setTitle(_translate("Dialog", "Message"))
         self.pb_font_message_title.setText(_translate("Dialog", "Title"))
         self.pb_font_message_date.setText(_translate("Dialog", "Date"))
```

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/images/gotify-small-macos.png` & `gotify-tray-0.5.0/gotify_tray/gui/images/gotify-small-macos.png`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/images/gotify-small.png` & `gotify-tray-0.5.0/gotify_tray/gui/images/gotify-small.png`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/images/logo-macos.ico` & `gotify-tray-0.5.0/gotify_tray/gui/images/logo-macos.ico`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/images/logo.ico` & `gotify-tray-0.5.0/gotify_tray/gui/images/logo.ico`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/images/tray-error-macos.png` & `gotify-tray-0.5.0/gotify_tray/gui/images/tray-error-macos.png`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/images/tray-error.png` & `gotify-tray-0.5.0/gotify_tray/gui/images/tray-error.png`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/images/tray-macos.png` & `gotify-tray-0.5.0/gotify_tray/gui/images/tray-macos.png`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/images/tray-unread-macos.png` & `gotify-tray-0.5.0/gotify_tray/gui/images/tray-unread-macos.png`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/images/tray-unread.png` & `gotify-tray-0.5.0/gotify_tray/gui/images/tray-unread.png`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/images/tray.png` & `gotify-tray-0.5.0/gotify_tray/gui/images/tray.png`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/models/ApplicationModel.py` & `gotify-tray-0.5.0/gotify_tray/gui/models/ApplicationModel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import enum
 
-from typing import Optional, Union
 from PyQt6 import QtCore, QtGui
 from gotify_tray import gotify
 from gotify_tray.database import Settings
 
 
 settings = Settings("gotify-tray")
 
@@ -14,15 +13,15 @@
     IconRole = QtCore.Qt.ItemDataRole.UserRole + 2
 
 
 class ApplicationModelItem(QtGui.QStandardItem):
     def __init__(
         self,
         application: gotify.GotifyApplicationModel,
-        icon: Optional[QtGui.QIcon] = None,
+        icon: QtGui.QIcon | None = None,
         *args,
         **kwargs,
     ):
         super(ApplicationModelItem, self).__init__(application.name)
         self.setDropEnabled(False)
         self.setData(application, ApplicationItemDataRole.ApplicationRole)
         self.setData(icon, ApplicationItemDataRole.IconRole)
@@ -51,32 +50,30 @@
             font.fromString(s)
             self.setFont(font)
 
 
 class ApplicationModel(QtGui.QStandardItemModel):
     def __init__(self):
         super(ApplicationModel, self).__init__()
-        self.setItemPrototype(
-            ApplicationModelItem(gotify.GotifyApplicationModel({"name": ""}), None)
-        )
+        self.setItemPrototype(ApplicationModelItem(gotify.GotifyApplicationModel({"name": ""}), None))
 
     def setItem(
         self,
         row: int,
         column: int,
-        item: Union[ApplicationModelItem, ApplicationAllMessagesItem],
+        item: ApplicationModelItem | ApplicationAllMessagesItem,
     ) -> None:
         super(ApplicationModel, self).setItem(row, column, item)
 
     def itemFromIndex(
         self, index: QtCore.QModelIndex
-    ) -> Union[ApplicationModelItem, ApplicationAllMessagesItem]:
+    ) -> ApplicationModelItem | ApplicationAllMessagesItem:
         return super(ApplicationModel, self).itemFromIndex(index)
 
-    def itemFromId(self, appid: int) -> Optional[ApplicationModelItem]:
+    def itemFromId(self, appid: int) -> ApplicationModelItem | None:
         for row in range(self.rowCount()):
             item = self.item(row, 0)
             if not isinstance(item, ApplicationModelItem):
                 continue
             if item.data(ApplicationItemDataRole.ApplicationRole).id == appid:
                 return item
         return None
```

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/models/MessagesModel.py` & `gotify-tray-0.5.0/gotify_tray/gui/models/MessagesModel.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,41 @@
 import enum
 
 from typing import cast
 from PyQt6 import QtCore, QtGui
 from gotify_tray import gotify
+from gotify_tray.database import Settings
+
+
+settings = Settings("gotify-tray")
 
 
 class MessageItemDataRole(enum.IntEnum):
     MessageRole = QtCore.Qt.ItemDataRole.UserRole + 1
 
 
 class MessagesModelItem(QtGui.QStandardItem):
     def __init__(self, message: gotify.GotifyMessageModel, *args, **kwargs):
         super(MessagesModelItem, self).__init__()
         self.setData(message, MessageItemDataRole.MessageRole)
 
 
 class MessagesModel(QtGui.QStandardItemModel):
+    def update_last_id(self, i: int):
+        if i > settings.value("message/last", type=int):
+            settings.setValue("message/last", i)
+
+    def insert_message(self, row: int, message: gotify.GotifyMessageModel):
+        self.update_last_id(message.id)
+        message_item = MessagesModelItem(message)
+        self.insertRow(row, message_item)
+    
+    def append_message(self, message: gotify.GotifyMessageModel):
+        self.update_last_id(message.id)
+        message_item = MessagesModelItem(message)
+        self.appendRow(message_item)
+
     def setItem(self, row: int, column: int, item: MessagesModelItem) -> None:
         super(MessagesModel, self).setItem(row, column, item)
 
     def itemFromIndex(self, index: QtCore.QModelIndex) -> MessagesModelItem:
         return cast(MessagesModelItem, super(MessagesModel, self).itemFromIndex(index))
```

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/themes/dark_purple/palette.py` & `gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/palette.py`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/themes/dark_purple/refresh.svg` & `gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/refresh.svg`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/themes/dark_purple/status_active.svg` & `gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/status_active.svg`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/themes/dark_purple/status_connecting.svg` & `gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/status_connecting.svg`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/themes/dark_purple/status_error.svg` & `gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/status_error.svg`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/themes/dark_purple/status_inactive.svg` & `gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/status_inactive.svg`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/themes/dark_purple/style.qss` & `gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/style.qss`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,48 @@
 QPushButton:!default:hover {
-    background: #441b85;
+    background: #5c24b6;
 }
 
 QPushButton:default:hover, QPushButton:checked:hover {
-    background: #441b85;
+    background: #5c24b6;
 }
 
-QToolTip {
-    color: #BFBFBF;
-    background-color: #5522a8;
+ServerInfoDialog QPushButton[state="success"] {
+    background-color: #6400FF00;
+    color: black;
+}
+
+ServerInfoDialog QPushButton[state="success"]:!default:hover {
+    background: #6400FF00;
+}
+
+ServerInfoDialog QPushButton[state="failed"] {
+    background-color: #64FF0000;
+    color: black;
 }
 
-QListView[objectName^="listView_applications"] {
-    background-color: #2E2E30;
+ServerInfoDialog QPushButton[state="failed"]:!default:hover {
+    background: #64FF0000;
 }
 
-MessageWidget QFrame {
-    background-color: #2E2E30;
+ServerInfoDialog QLineEdit[state="success"] {}
+
+ServerInfoDialog QLineEdit[state="failed"] {
+    border: 1px solid red;
+}
+
+QToolTip {
+    color: #BFBFBF;
+    background-color: #5522a8;
 }
 
 MessageWidget QPushButton {
     border: 0px;
 }
 
 MessageWidget QPushButton:!default:hover {
-    background: #7249b5;
+    background: #9662ea;
 }
 
 MessageWidget QPushButton:!default:pressed {
-    background: #5c3b91;
-}
-
-QCheckBox::indicator:unchecked {
-    border: 2px solid #4A4A4A;
+    background: #7a4dc2;
 }
```

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/themes/default/refresh.svg` & `gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/refresh.svg`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/themes/default/status_active.svg` & `gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/status_active.svg`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/themes/default/status_connecting.svg` & `gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/status_connecting.svg`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/themes/default/status_error.svg` & `gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/status_error.svg`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/themes/default/status_inactive.svg` & `gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/status_inactive.svg`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/themes/light_purple/palette.py` & `gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/palette.py`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/widgets/ImagePopup.py` & `gotify-tray-0.5.0/gotify_tray/gui/widgets/ImagePopup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from gotify_tray.database import Settings
 
 
 settings = Settings("gotify-tray")
 
 
 class ImagePopup(QtWidgets.QLabel):
-    def __init__(self, filename: str, pos: QtCore.QPoint, link: str = None):
+    def __init__(self, filename: str, pos: QtCore.QPoint, link: str | None = None):
         """Create and show a pop-up image under the cursor
 
         Args:
             filename (str): The path to the image to display
             pos (QtCore.QPoint): The location at which the image should be displayed
             link (str, optional): The URL of the image. Defaults to None.
         """
```

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/widgets/MainWindow.py` & `gotify-tray-0.5.0/gotify_tray/gui/widgets/MainWindow.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,16 @@
     MessagesModelItem,
 )
 from . import MessageWidget
 
 from gotify_tray.__version__ import __title__
 from gotify_tray.database import Settings
 from gotify_tray.gui.themes import get_theme_file
+from gotify_tray.gui.models import MessageItemDataRole
+from gotify_tray import gotify
 
 
 settings = Settings("gotify-tray")
 
 
 class MainWindow(QtWidgets.QMainWindow, Ui_MainWindow):
     refresh = QtCore.pyqtSignal()
@@ -22,36 +24,39 @@
     delete_message = QtCore.pyqtSignal(MessagesModelItem)
     application_selection_changed = QtCore.pyqtSignal(QtGui.QStandardItem)
     image_popup = QtCore.pyqtSignal(str, QtCore.QPoint)
     hidden = QtCore.pyqtSignal()
     activated = QtCore.pyqtSignal()
 
     def __init__(
-        self, application_model: ApplicationModel, messages_model: MessagesModel
+        self, app: QtWidgets.QApplication,
+        application_model: ApplicationModel, messages_model: MessagesModel
     ):
         super(MainWindow, self).__init__()
         self.setupUi(self)
 
         self.installEventFilter(self)
 
         self.setWindowTitle(__title__)
 
+        self.app = app
+
         self.application_model = application_model
         self.messages_model = messages_model
 
         self.listView_applications.setModel(application_model)
         self.listView_messages.setModel(messages_model)
 
         # Do not expand the applications listview when resizing
         self.splitter.setStretchFactor(0, 0)
         self.splitter.setStretchFactor(1, 1)
 
         # Do not collapse the message list
         self.splitter.setCollapsible(1, False)
-        self.status_widget = StatusWidget()
+        self.status_widget = StatusWidget(app)
         self.horizontalLayout.insertWidget(0, self.status_widget)
 
         self.set_icons()
 
         font_title = QtGui.QFont()
         if s := settings.value("MainWindow/font/application", type=str):
             font_title.fromString(s)
@@ -66,16 +71,16 @@
 
         self.restore_state()
 
         self.link_callbacks()
 
     def set_icons(self):
         # Set button icons
-        self.pb_refresh.setIcon(QtGui.QIcon(get_theme_file("refresh.svg")))
-        self.pb_delete_all.setIcon(QtGui.QIcon(get_theme_file("trashcan.svg")))
+        self.pb_refresh.setIcon(QtGui.QIcon(get_theme_file(self.app, "refresh.svg")))
+        self.pb_delete_all.setIcon(QtGui.QIcon(get_theme_file(self.app, "trashcan.svg")))
 
         # Resize the labels and icons
         size = settings.value("MainWindow/label/size", type=int)
         self.status_widget.setFixedSize(QtCore.QSize(size, size))
 
         size = settings.value("MainWindow/button/size", type=int)
         self.pb_refresh.setFixedSize(QtCore.QSize(size, size))
@@ -97,25 +102,28 @@
 
     def set_inactive(self):
         self.status_widget.set_inactive()
 
     def set_error(self):
         self.status_widget.set_error()
 
-    def insert_message_widget(
-        self, message_item: MessagesModelItem, image_path: str = ""
-    ):
-        message_widget = MessageWidget(
-            self.listView_messages, message_item, image_path=image_path
-        )
-        self.listView_messages.setIndexWidget(
-            self.messages_model.indexFromItem(message_item), message_widget
-        )
-        message_widget.deletion_requested.connect(self.delete_message.emit)
-        message_widget.image_popup.connect(self.image_popup.emit)
+    def display_message_widgets(self, parent: QtCore.QModelIndex, first: int, last: int):
+        for i in range(first, last+1):
+            if index := self.messages_model.index(i, 0, parent):
+                message_item = self.messages_model.itemFromIndex(index)
+
+                message: gotify.GotifyMessageModel = self.messages_model.data(index, MessageItemDataRole.MessageRole)
+
+                application_item = self.application_model.itemFromId(message.appid)
+                
+                message_widget = MessageWidget(self.app, self.listView_messages, message_item, icon=application_item.icon())
+                message_widget.deletion_requested.connect(self.delete_message.emit)
+                message_widget.image_popup.connect(self.image_popup.emit)
+                
+                self.listView_messages.setIndexWidget(self.messages_model.indexFromItem(message_item), message_widget)
 
     def currentApplicationIndex(self) -> QtCore.QModelIndex:
         return self.listView_applications.selectionModel().currentIndex()
 
     def application_selection_changed_callback(
         self, current: QtCore.QModelIndex, previous: QtCore.QModelIndex
     ):
@@ -180,14 +188,15 @@
         if state := settings.value("MainWindow/state", type=QtCore.QByteArray):
             self.restoreState(state)
         if splitter := settings.value("MainWindow/splitter", type=QtCore.QByteArray):
             self.splitter.restoreState(splitter)
 
     def closeEvent(self, e: QtGui.QCloseEvent) -> None:
         self.hide()
+        e.ignore()
         self.hidden.emit()
 
     def eventFilter(self, object: QtCore.QObject, event: QtCore.QEvent) -> bool:
         if event.type() == QtCore.QEvent.Type.WindowActivate:
             self.activated.emit()
 
         return super().eventFilter(object, event)
```

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/widgets/MessageWidget.py` & `gotify-tray-0.5.0/gotify_tray/gui/widgets/MessageWidget.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,70 +16,68 @@
 
 class MessageWidget(QtWidgets.QWidget, Ui_Form):
     deletion_requested = QtCore.pyqtSignal(MessagesModelItem)
     image_popup = QtCore.pyqtSignal(str, QtCore.QPoint)
 
     def __init__(
         self,
+        app: QtWidgets.QApplication,
         parent: QtWidgets.QWidget,
         message_item: MessagesModelItem,
-        image_path: str = "",
+        icon: QtGui.QIcon | None = None,
     ):
-        super(MessageWidget, self).__init__()
-        self.parent = parent
+        super(MessageWidget, self).__init__(parent)
+        self.app = app
+        self._parent = parent
         self.setupUi(self)
         self.setAutoFillBackground(True)
         self.message_item = message_item
         message: GotifyMessageModel = message_item.data(MessageItemDataRole.MessageRole)
 
         # Fonts
         self.set_fonts()
 
         # Display the message priority as a color
         self.set_priority_color(message.priority)
 
         # Display message contents
         self.label_title.setText(message.title)
-        self.label_date.setText(message.date.strftime("%Y-%m-%d, %H:%M"))
+        self.label_date.setText(message.date.strftime("%x, %X" if settings.value("locale", type=bool) else "%Y-%m-%d, %H:%M"))
 
-        if markdown := (
-            message.get("extras", {}).get("client::display", {}).get("contentType")
-            == "text/markdown"
-        ):
+        if message.get("extras", {}).get("client::display", {}).get("contentType") == "text/markdown":
             self.label_message.setTextFormat(QtCore.Qt.TextFormat.MarkdownText)
 
         # If the message is only an image URL, then instead of showing the message,
         # download the image and show it in the message label
         if image_url := get_image(message.message):
             downloader = Downloader()
             filename = downloader.get_filename(image_url)
             self.set_message_image(filename)
         else:
             self.label_message.setText(convert_links(message.message))
 
         # Show the application icon
-        if image_path:
+        if icon:
             image_size = settings.value("MessageWidget/image/size", type=int)
-            self.label_image.setFixedSize(QtCore.QSize(image_size, image_size))
-            pixmap = QtGui.QPixmap(image_path).scaled(
-                image_size,
-                image_size,
-                aspectRatioMode=QtCore.Qt.AspectRatioMode.KeepAspectRatioByExpanding,
-                transformMode=QtCore.Qt.TransformationMode.SmoothTransformation,
-            )
+            pixmap = icon.pixmap(QtCore.QSize(image_size, image_size))
             self.label_image.setPixmap(pixmap)
         else:
             self.label_image.hide()
 
         # Set MessagesModelItem's size hint based on the size of this widget
         self.gridLayout_frame.setContentsMargins(0, 0, 5, 0)
         self.gridLayout.setContentsMargins(4, 5, 4, 0)
         self.adjustSize()
         size_hint = self.message_item.sizeHint()
-        self.message_item.setSizeHint(QtCore.QSize(size_hint.width(), self.height()))
+        self.message_item.setSizeHint(
+            QtCore.QSize(
+                size_hint.width(),
+                max(settings.value("MessageWidget/height/min", type=int), self.height())
+            )
+        )
 
         self.set_icons()
 
         self.link_callbacks()
 
     def set_fonts(self):
         font_title = QtGui.QFont()
@@ -100,28 +98,25 @@
             font_content.fromString(s)
 
         self.label_title.setFont(font_title)
         self.label_date.setFont(font_date)
         self.label_message.setFont(font_content)
 
     def set_icons(self):
-        self.pb_delete.setIcon(QtGui.QIcon(get_theme_file("trashcan.svg")))
+        self.pb_delete.setIcon(QtGui.QIcon(get_theme_file(self.app, "trashcan.svg")))
         self.pb_delete.setIconSize(QtCore.QSize(24, 24))
 
     def set_message_image(self, filename: str):
         pixmap = QtGui.QPixmap(filename)
 
         # Make sure the image fits within the listView
-        W = settings.value("MessageWidget/content_image/W_percentage", type=float) * (
-            self.parent.width() - self.label_image.width()
-        )
-        H = (
-            settings.value("MessageWidget/content_image/H_percentage", type=float)
-            * self.parent.height()
-        )
+        W = settings.value("MessageWidget/content_image/W_percentage", type=float)
+        H = settings.value("MessageWidget/content_image/H_percentage", type=float)
+        W *= self._parent.width() - self.label_image.width()
+        H *= self._parent.height()
 
         if pixmap.width() > W or pixmap.height() > H:
             pixmap = pixmap.scaled(
                 QtCore.QSize(int(W), int(H)),
                 aspectRatioMode=QtCore.Qt.AspectRatioMode.KeepAspectRatio,
                 transformMode=QtCore.Qt.TransformationMode.SmoothTransformation,
             )
@@ -144,11 +139,9 @@
 
         qurl = QtCore.QUrl(link)
         _, ext = os.path.splitext(qurl.fileName())
         if ext in settings.value("ImagePopup/extensions", type=list):
             self.image_popup.emit(link, QtGui.QCursor.pos())
 
     def link_callbacks(self):
-        self.pb_delete.clicked.connect(
-            lambda: self.deletion_requested.emit(self.message_item)
-        )
+        self.pb_delete.clicked.connect(lambda: self.deletion_requested.emit(self.message_item))
         self.label_message.linkHovered.connect(self.link_hovered_callback)
```

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/widgets/ServerInfoDialog.py` & `gotify-tray-0.5.0/gotify_tray/gui/widgets/ServerInfoDialog.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,17 +15,15 @@
     def __init__(self, url: str = "", token: str = "", enable_import: bool = True):
         super(ServerInfoDialog, self).__init__()
         self.setupUi(self)
         self.setWindowTitle("Server info")
         self.line_url.setPlaceholderText("https://gotify.example.com")
         self.line_url.setText(url)
         self.line_token.setText(token)
-        self.buttonBox.button(QtWidgets.QDialogButtonBox.StandardButton.Ok).setDisabled(
-            True
-        )
+        self.buttonBox.button(QtWidgets.QDialogButtonBox.StandardButton.Ok).setDisabled(True)
         self.pb_import.setVisible(enable_import)
         self.link_callbacks()
 
     def test_server_info(self):
         self.pb_test.setStyleSheet("")
         self.line_url.setStyleSheet("")
         self.line_token.setStyleSheet("")
@@ -33,47 +31,57 @@
 
         url = self.line_url.text()
         client_token = self.line_token.text()
         if not url or not client_token:
             return
 
         self.pb_test.setDisabled(True)
-        self.buttonBox.button(QtWidgets.QDialogButtonBox.StandardButton.Ok).setDisabled(
-            True
-        )
+        self.buttonBox.button(QtWidgets.QDialogButtonBox.StandardButton.Ok).setDisabled(True)
 
         self.task = VerifyServerInfoTask(url, client_token)
         self.task.success.connect(self.server_info_success)
         self.task.incorrect_token.connect(self.incorrect_token_callback)
         self.task.incorrect_url.connect(self.incorrect_url_callback)
         self.task.start()
 
+    def update_widget_state(self, widget: QtWidgets.QWidget, state: str):
+        widget.setProperty("state", state)
+        widget.style().unpolish(widget)
+        widget.style().polish(widget)
+        widget.update()
+
     def server_info_success(self, version: GotifyVersionModel):
         self.pb_test.setEnabled(True)
         self.label_server_info.setText(f"Version: {version.version}")
-        self.pb_test.setStyleSheet("background-color: rgba(0, 255, 0, 100);")
-        self.buttonBox.button(QtWidgets.QDialogButtonBox.StandardButton.Ok).setEnabled(
-            True
-        )
+        self.update_widget_state(self.pb_test, "success")
+        self.update_widget_state(self.line_token, "success")
+        self.update_widget_state(self.line_url, "success")
+        self.buttonBox.button(QtWidgets.QDialogButtonBox.StandardButton.Ok).setEnabled(True)
         self.buttonBox.button(QtWidgets.QDialogButtonBox.StandardButton.Ok).setFocus()
 
     def incorrect_token_callback(self, version: GotifyVersionModel):
         self.pb_test.setEnabled(True)
         self.label_server_info.setText(f"Version: {version.version}")
-        self.pb_test.setStyleSheet("background-color: rgba(255, 0, 0, 100);")
-        self.line_token.setStyleSheet("border: 1px solid red;")
+        self.update_widget_state(self.pb_test, "failed")
+        self.update_widget_state(self.line_token, "failed")
+        self.update_widget_state(self.line_url, "success")
         self.line_token.setFocus()
 
     def incorrect_url_callback(self):
         self.pb_test.setEnabled(True)
         self.label_server_info.clear()
-        self.pb_test.setStyleSheet("background-color: rgba(255, 0, 0, 100);")
-        self.line_url.setStyleSheet("border: 1px solid red;")
+        self.update_widget_state(self.pb_test, "failed")
+        self.update_widget_state(self.line_token, "success")
+        self.update_widget_state(self.line_url, "failed")
         self.line_url.setFocus()
 
+    def input_changed_callback(self):
+        self.buttonBox.button(QtWidgets.QDialogButtonBox.StandardButton.Ok).setDisabled(True)
+        self.update_widget_state(self.pb_test, "")
+
     def import_success_callback(self):
         self.line_url.setText(settings.value("Server/url", type=str))
         self.line_token.setText(settings.value("Server/client_token"))
 
     def import_callback(self):
         fname = QtWidgets.QFileDialog.getOpenFileName(
             self, "Import Settings", settings.value("export/path", type=str), "*",
@@ -81,18 +89,10 @@
         if fname and os.path.exists(fname):
             self.import_settings_task = ImportSettingsTask(fname)
             self.import_settings_task.success.connect(self.import_success_callback)
             self.import_settings_task.start()
 
     def link_callbacks(self):
         self.pb_test.clicked.connect(self.test_server_info)
-        self.line_url.textChanged.connect(
-            lambda: self.buttonBox.button(
-                QtWidgets.QDialogButtonBox.StandardButton.Ok
-            ).setDisabled(True)
-        )
-        self.line_token.textChanged.connect(
-            lambda: self.buttonBox.button(
-                QtWidgets.QDialogButtonBox.StandardButton.Ok
-            ).setDisabled(True)
-        )
+        self.line_url.textChanged.connect(self.input_changed_callback)
+        self.line_token.textChanged.connect(self.input_changed_callback)
         self.pb_import.clicked.connect(self.import_callback)
```

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/widgets/SettingsDialog.py` & `gotify-tray-0.5.0/gotify_tray/gui/widgets/SettingsDialog.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,64 +23,53 @@
 settings = Settings("gotify-tray")
 
 
 class SettingsDialog(QtWidgets.QDialog, Ui_Dialog):
     quit_requested = QtCore.pyqtSignal()
     theme_change_requested = QtCore.pyqtSignal(str)
 
-    def __init__(self):
+    def __init__(self, app: QtWidgets.QApplication):
         super(SettingsDialog, self).__init__()
         self.setupUi(self)
         self.setWindowTitle("Settings")
+        
+        self.app = app
 
         self.settings_changed = False
         self.changes_applied = False
         self.server_changed = False
 
         self.initUI()
 
         self.link_callbacks()
 
     def initUI(self):
-        self.buttonBox.button(
-            QtWidgets.QDialogButtonBox.StandardButton.Apply
-        ).setEnabled(False)
+        self.buttonBox.button(QtWidgets.QDialogButtonBox.StandardButton.Apply).setEnabled(False)
 
         # Notifications
-        self.spin_priority.setValue(
-            settings.value("tray/notifications/priority", type=int)
-        )
+        self.spin_priority.setValue(settings.value("tray/notifications/priority", type=int))
 
-        self.spin_duration.setValue(
-            settings.value("tray/notifications/duration_ms", type=int)
-        )
+        self.spin_duration.setValue(settings.value("tray/notifications/duration_ms", type=int))
         if platform.system() == "Windows":
             # The notification duration setting is ignored by windows
             self.label_notification_duration.hide()
             self.spin_duration.hide()
             self.label_notification_duration_ms.hide()
 
-        self.cb_notify.setChecked(
-            settings.value("message/check_missed/notify", type=bool)
-        )
+        self.cb_notify.setChecked(settings.value("message/check_missed/notify", type=bool))
 
-        self.cb_notification_click.setChecked(
-            settings.value("tray/notifications/click", type=bool)
-        )
+        self.cb_notification_click.setChecked(settings.value("tray/notifications/click", type=bool))
 
-        self.cb_tray_icon_unread.setChecked(
-            settings.value("tray/icon/unread", type=bool)
-        )
+        self.cb_tray_icon_unread.setChecked(settings.value("tray/icon/unread", type=bool))
 
         # Interface
         self.combo_theme.addItems(get_themes())
         self.combo_theme.setCurrentText(settings.value("theme", type=str))
-        self.cb_priority_colors.setChecked(
-            settings.value("MessageWidget/priority_color", type=bool)
-        )
+        self.cb_priority_colors.setChecked(settings.value("MessageWidget/priority_color", type=bool))
+        self.cb_locale.setChecked(settings.value("locale", type=bool))
 
         # Logging
         self.combo_logging.addItems(
             [
                 logging.getLevelName(logging.ERROR),
                 logging.getLevelName(logging.WARNING),
                 logging.getLevelName(logging.INFO),
@@ -90,59 +79,54 @@
         )
         self.combo_logging.setCurrentText(settings.value("logging/level", type=str))
 
         # Fonts
         self.add_message_widget()
 
         # Advanced
-        self.groupbox_image_popup.setChecked(
-            settings.value("ImagePopup/enabled", type=bool)
-        )
+        self.groupbox_image_popup.setChecked(settings.value("ImagePopup/enabled", type=bool))
         self.spin_popup_w.setValue(settings.value("ImagePopup/w", type=int))
         self.spin_popup_h.setValue(settings.value("ImagePopup/h", type=int))
         self.label_cache.setText("0 MB")
         self.compute_cache_size()
 
     def add_message_widget(self):
         self.message_widget = MessageWidget(
+            self.app,
             self,
             MessagesModelItem(
                 GotifyMessageModel(
                     {
                         "date": "2021-01-01T11:11:00.928224+01:00",
                         "message": "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin luctus.",
                         "title": "Title",
                         "priority": 4,
                     }
                 )
             ),
-            get_icon("gotify-small"),
+            QtGui.QIcon(get_icon("gotify-small")),
         )
         self.layout_fonts_message.addWidget(self.message_widget)
 
     def compute_cache_size(self):
         self.cache_size_task = CacheSizeTask()
         self.cache_size_task.size.connect(lambda size: self.label_cache.setText(f"{round(size/1e6, 1)} MB"))
         self.cache_size_task.start()
 
     def change_server_info_callback(self):
         self.server_changed = verify_server(force_new=True, enable_import=False)
 
     def settings_changed_callback(self, *args, **kwargs):
         self.settings_changed = True
-        self.buttonBox.button(
-            QtWidgets.QDialogButtonBox.StandardButton.Apply
-        ).setEnabled(True)
+        self.buttonBox.button(QtWidgets.QDialogButtonBox.StandardButton.Apply).setEnabled(True)
 
     def change_font_callback(self, name: str):
         label: QtWidgets.QLabel = getattr(self.message_widget, "label_" + name)
 
-        font, accepted = QtWidgets.QFontDialog.getFont(
-            label.font(), self, f"Select a {name} font"
-        )
+        font, accepted = QtWidgets.QFontDialog.getFont(label.font(), self, f"Select a {name} font")
 
         if accepted:
             self.settings_changed_callback()
             label.setFont(font)
 
     def export_callback(self):
         fname = QtWidgets.QFileDialog.getSaveFileName(
@@ -198,50 +182,41 @@
 
     def clear_cache_callback(self):
         self.clear_cache_task = ClearCacheTask()
         self.clear_cache_task.start()
         self.label_cache.setText("0 MB")
 
     def link_callbacks(self):
-        self.buttonBox.button(
-            QtWidgets.QDialogButtonBox.StandardButton.Apply
-        ).clicked.connect(self.apply_settings)
+        self.buttonBox.button(QtWidgets.QDialogButtonBox.StandardButton.Apply).clicked.connect(self.apply_settings)
 
         # Notifications
         self.spin_priority.valueChanged.connect(self.settings_changed_callback)
         self.spin_duration.valueChanged.connect(self.settings_changed_callback)
         self.cb_notify.stateChanged.connect(self.settings_changed_callback)
         self.cb_notification_click.stateChanged.connect(self.settings_changed_callback)
         self.cb_tray_icon_unread.stateChanged.connect(self.settings_changed_callback)
 
         # Interface
         self.combo_theme.currentTextChanged.connect(self.settings_changed_callback)
         self.cb_priority_colors.stateChanged.connect(self.settings_changed_callback)
+        self.cb_locale.stateChanged.connect(self.settings_changed_callback)
 
         # Server info
         self.pb_change_server_info.clicked.connect(self.change_server_info_callback)
 
         # Logging
         self.combo_logging.currentTextChanged.connect(self.settings_changed_callback)
-        self.pb_open_log.clicked.connect(
-            lambda: open_file(logger.root.handlers[0].baseFilename)
-        )
+        self.pb_open_log.clicked.connect(lambda: open_file(logger.root.handlers[0].baseFilename))
 
         # Fonts
         self.pb_reset_fonts.clicked.connect(self.reset_fonts_callback)
 
-        self.pb_font_message_title.clicked.connect(
-            lambda: self.change_font_callback("title")
-        )
-        self.pb_font_message_date.clicked.connect(
-            lambda: self.change_font_callback("date")
-        )
-        self.pb_font_message_content.clicked.connect(
-            lambda: self.change_font_callback("message")
-        )
+        self.pb_font_message_title.clicked.connect(lambda: self.change_font_callback("title"))
+        self.pb_font_message_date.clicked.connect(lambda: self.change_font_callback("date"))
+        self.pb_font_message_content.clicked.connect(lambda: self.change_font_callback("message"))
 
         # Advanced
         self.pb_export.clicked.connect(self.export_callback)
         self.pb_import.clicked.connect(self.import_callback)
         self.pb_reset.clicked.connect(self.reset_callback)
         self.groupbox_image_popup.toggled.connect(self.settings_changed_callback)
         self.spin_popup_w.valueChanged.connect(self.settings_changed_callback)
@@ -250,51 +225,40 @@
         self.pb_open_cache_dir.clicked.connect(lambda: open_file(Cache().directory()))
 
     def apply_settings(self):
         # Priority
         settings.setValue("tray/notifications/priority", self.spin_priority.value())
         settings.setValue("tray/notifications/duration_ms", self.spin_duration.value())
         settings.setValue("message/check_missed/notify", self.cb_notify.isChecked())
-        settings.setValue(
-            "tray/notifications/click", self.cb_notification_click.isChecked()
-        )
+        settings.setValue("tray/notifications/click", self.cb_notification_click.isChecked())
         settings.setValue("tray/icon/unread", self.cb_tray_icon_unread.isChecked())
 
         # Interface
         current_theme = settings.value("theme", type=str)
         selected_theme = self.combo_theme.currentText()
         if current_theme != selected_theme:
             settings.setValue("theme", selected_theme)
             self.theme_change_requested.emit(selected_theme)
 
-        settings.setValue(
-            "MessageWidget/priority_color", self.cb_priority_colors.isChecked()
-        )
+        settings.setValue("MessageWidget/priority_color", self.cb_priority_colors.isChecked())
+        settings.setValue("locale", self.cb_locale.isChecked())
 
         # Logging
         selected_level = self.combo_logging.currentText()
         settings.setValue("logging/level", selected_level)
         if selected_level == "Disabled":
             logging.disable(logging.CRITICAL)
         else:
             logging.disable(logging.NOTSET)
             logger.setLevel(selected_level)
 
         # Fonts
-        settings.setValue(
-            "MessageWidget/font/title",
-            self.message_widget.label_title.font().toString(),
-        )
-        settings.setValue(
-            "MessageWidget/font/date", self.message_widget.label_date.font().toString()
-        )
-        settings.setValue(
-            "MessageWidget/font/message",
-            self.message_widget.label_message.font().toString(),
-        )
+        settings.setValue("MessageWidget/font/title", self.message_widget.label_title.font().toString())
+        settings.setValue("MessageWidget/font/date", self.message_widget.label_date.font().toString())
+        settings.setValue("MessageWidget/font/message", self.message_widget.label_message.font().toString())
 
         # Advanced
         settings.setValue("ImagePopup/enabled", self.groupbox_image_popup.isChecked())
         settings.setValue("ImagePopup/w", self.spin_popup_w.value())
         settings.setValue("ImagePopup/h", self.spin_popup_h.value())
 
         self.settings_changed = False
```

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/widgets/StatusWidget.py` & `gotify-tray-0.5.0/gotify_tray/gui/widgets/StatusWidget.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 from gotify_tray.gui.themes import get_theme_file
 
 
 settings = Settings("gotify-tray")
 
 
 class StatusWidget(QtWidgets.QLabel):
-    def __init__(self):
+    def __init__(self, app: QtWidgets.QApplication):
         super(StatusWidget, self).__init__()
+        self.app = app
         self.setFixedSize(QtCore.QSize(20, 20))
         self.setScaledContents(True)
         self.set_connecting()
         self.image = None
 
     def set_status(self, image: str):
         self.image = image
-        self.setPixmap(QtGui.QPixmap(get_theme_file(image)))
+        self.setPixmap(QtGui.QPixmap(get_theme_file(self.app, image)))
 
     def set_active(self):
         self.setToolTip("Listening for new messages")
         self.set_status("status_active.svg")
 
     def set_connecting(self):
         self.setToolTip("Connecting...")
```

### Comparing `gotify-tray-0.4.2/gotify_tray/gui/widgets/Tray.py` & `gotify-tray-0.5.0/gotify_tray/gui/widgets/Tray.py`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.4.2/gotify_tray/tasks.py` & `gotify-tray-0.5.0/gotify_tray/tasks.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,37 +4,44 @@
 import time
 import os
 
 from functools import reduce
 from PyQt6 import QtCore
 from PyQt6.QtCore import pyqtSignal
 
-from gotify_tray.database import Cache, Downloader, Settings
+from gotify_tray.database import Cache, Settings
 from gotify_tray.gotify.api import GotifyClient
 from gotify_tray.gotify.models import GotifyVersionModel
-from gotify_tray.utils import get_image
+from gotify_tray.utils import process_messages
 
 from . import gotify
 
 
 settings = Settings("gotify-tray")
 logger = logging.getLogger("gotify-tray")
 
 
 class BaseTask(QtCore.QThread):
     failed = pyqtSignal()
 
     def __init__(self):
         super(BaseTask, self).__init__()
         self.running = False
+        self._abort = False
 
     @abc.abstractmethod
     def task(self):
         ...
 
+    def abort(self):
+        self._abort = True
+
+    def abort_requested(self) -> bool:
+        return self._abort
+
     def run(self):
         self.running = True
         try:
             self.task()
         except Exception as e:
             logger.error(f"{self.__class__.__name__} failed: {e}")
             self.failed.emit()
@@ -93,46 +100,69 @@
         if isinstance(result, gotify.GotifyErrorModel):
             self.error.emit(result)
         else:
             self.success.emit(result)
 
 
 class GetApplicationMessagesTask(BaseTask):
-    success = pyqtSignal(gotify.GotifyPagedMessagesModel)
+    message = pyqtSignal(gotify.GotifyMessageModel)
     error = pyqtSignal(gotify.GotifyErrorModel)
 
     def __init__(self, appid: int, gotify_client: gotify.GotifyClient):
         super(GetApplicationMessagesTask, self).__init__()
         self.appid = appid
         self.gotify_client = gotify_client
 
     def task(self):
         result = self.gotify_client.get_application_messages(self.appid)
         if isinstance(result, gotify.GotifyErrorModel):
             self.error.emit(result)
         else:
-            self.success.emit(result)
+            for message in process_messages(result.messages):
+                if self.abort_requested():
+                    return
+                self.message.emit(message)
+                
+                # Prevent locking up the UI when there are a lot of messages ready at the same time
+                # -- side effect: switching application while the previous messages are still being inserted causes mixing of messages
+                time.sleep(0.001)
 
 
 class GetMessagesTask(BaseTask):
+    message = pyqtSignal(gotify.GotifyMessageModel)
     success = pyqtSignal(gotify.GotifyPagedMessagesModel)
     error = pyqtSignal(gotify.GotifyErrorModel)
 
     def __init__(self, gotify_client: gotify.GotifyClient):
         super(GetMessagesTask, self).__init__()
         self.gotify_client = gotify_client
 
     def task(self):
         result = self.gotify_client.get_messages()
         if isinstance(result, gotify.GotifyErrorModel):
             self.error.emit(result)
         else:
+            for message in process_messages(result.messages):
+                if self.abort_requested():
+                    return
+                self.message.emit(message)
+                time.sleep(0.001)
             self.success.emit(result)
 
 
+class ProcessMessageTask(BaseTask):
+    def __init__(self, message: gotify.GotifyMessageModel):
+        super(ProcessMessageTask, self).__init__()
+        self.message = message
+
+    def task(self):
+        for _ in process_messages([self.message]):
+            pass
+
+
 class VerifyServerInfoTask(BaseTask):
     success = pyqtSignal(GotifyVersionModel)
     incorrect_token = pyqtSignal(GotifyVersionModel)
     incorrect_url = pyqtSignal()
 
     def __init__(self, url: str, client_token: str):
         super(VerifyServerInfoTask, self).__init__()
@@ -172,17 +202,15 @@
         self.gotify_client = gotify_client
 
     def task(self):
         while True:
             time.sleep(settings.value("watchdog/interval/s", type=int))
             if not self.gotify_client.is_listening():
                 self.closed.emit()
-                logger.debug(
-                    "ServerConnectionWatchdogTask: gotify_client is not listening"
-                )
+                logger.debug("ServerConnectionWatchdogTask: gotify_client is not listening")
 
 
 class ExportSettingsTask(BaseTask):
     success = pyqtSignal()
 
     def __init__(self, path: str):
         super(ExportSettingsTask, self).__init__()
@@ -201,43 +229,14 @@
         self.path = path
 
     def task(self):
         settings.load(self.path)
         self.success.emit()
 
 
-class ProcessMessageTask(BaseTask):
-    def __init__(self, message: gotify.GotifyMessageModel):
-        super(ProcessMessageTask, self).__init__()
-        self.message = message
-
-    def task(self):
-        if image_url := get_image(self.message.message):
-            downloader = Downloader()
-            downloader.get_filename(image_url)
-
-
-class ProcessMessagesTask(BaseTask):
-    message_processed = pyqtSignal(gotify.GotifyMessageModel)
-
-    def __init__(self, page: gotify.GotifyPagedMessagesModel):
-        super(ProcessMessagesTask, self).__init__()
-        self.page = page
-
-    def task(self):
-        downloader = Downloader()
-        for message in self.page.messages:
-            if image_url := get_image(message.message):
-                downloader.get_filename(image_url)
-            self.message_processed.emit(message)
-
-            # Prevent locking up the UI when there are a lot of messages with images ready at the same time
-            time.sleep(0.001)
-
-
 class CacheSizeTask(BaseTask):
     size = pyqtSignal(int)
 
     def task(self):        
         cache_dir = Cache().directory()
         if os.path.exists(cache_dir):
             cache_size_bytes = reduce(lambda x, f: x + os.path.getsize(f), glob.glob(os.path.join(cache_dir, "*")), 0)
```

### Comparing `gotify-tray-0.4.2/gotify_tray/utils.py` & `gotify-tray-0.5.0/gotify_tray/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import os
 import platform
 import re
 import subprocess
 
 from pathlib import Path
-from typing import Optional
+from typing import Iterator
+
+from gotify_tray import gotify
+from gotify_tray.database import Downloader
 
 
 def verify_server(force_new: bool = False, enable_import: bool = True) -> bool:
     from gotify_tray.gui import ServerInfoDialog
     from gotify_tray.database import Settings
 
     settings = Settings("gotify-tray")
@@ -24,14 +27,22 @@
             return True
         else:
             return False
     else:
         return True
 
 
+def process_messages(messages: list[gotify.GotifyMessageModel]) -> Iterator[gotify.GotifyMessageModel]:
+    downloader = Downloader()
+    for message in messages:
+        if image_url := get_image(message.message):
+            downloader.get_filename(image_url)
+        yield message
+
+
 def convert_links(text):
     _link = re.compile(
         r'(?:(https://|http://)|(www\.))(\S+\b/?)([!"#$%&\'()*+,\-./:;<=>?@[\\\]^_`{|}~]*)(\s|$)',
         re.I,
     )
 
     def replace(match):
@@ -41,15 +52,15 @@
         return '<a href="http://{1}{2}" rel="nofollow">{0}{1}{2}</a>{3}{4}'.format(
             protocol, www_lead, *groups[2:]
         )
 
     return _link.sub(replace, text)
 
 
-def get_image(s: str) -> Optional[str]:
+def get_image(s: str) -> str | None:
     """If `s` contains only an image URL, this function returns that URL.
         This function also extracts a URL in the `![](<url>)` markdown image format.
     """
     s = s.strip()
 
     # Return True if 's' is a url and has an image extension
     RE = r'(?:(https://|http://)|(www\.))(\S+\b/?)([!"#$%&\'()*+,\-./:;<=>?@[\\\]^_`{|}~]*).(jpg|jpeg|png|bmp|gif)(\s|$)'
```

### Comparing `gotify-tray-0.4.2/gotify_tray.egg-info/PKG-INFO` & `gotify-tray-0.5.0/gotify_tray.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: gotify-tray
-Version: 0.4.2
+Version: 0.5.0
 Summary: A tray notification application for receiving messages from a Gotify server.
 Home-page: https://github.com/seird/gotify-tray
 Author: k.dries@protonmail.com
 Author-email: k.dries@protonmail.com
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8.0
+Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Gotify Tray
 
 
@@ -71,8 +69,8 @@
 ## Build instructions
 
 See [BUILDING](BUILDING.md).
 
 
 ## Requirements
 
-- python >=3.8
+- python >=3.10
```

### Comparing `gotify-tray-0.4.2/gotify_tray.egg-info/SOURCES.txt` & `gotify-tray-0.5.0/gotify_tray.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -53,21 +53,15 @@
 gotify_tray/gui/themes/dark_purple/status_connecting.svg
 gotify_tray/gui/themes/dark_purple/status_error.svg
 gotify_tray/gui/themes/dark_purple/status_inactive.svg
 gotify_tray/gui/themes/dark_purple/style.qss
 gotify_tray/gui/themes/dark_purple/trashcan.svg
 gotify_tray/gui/themes/default/__init__.py
 gotify_tray/gui/themes/default/palette.py
-gotify_tray/gui/themes/default/refresh.svg
-gotify_tray/gui/themes/default/status_active.svg
-gotify_tray/gui/themes/default/status_connecting.svg
-gotify_tray/gui/themes/default/status_error.svg
-gotify_tray/gui/themes/default/status_inactive.svg
 gotify_tray/gui/themes/default/style.qss
-gotify_tray/gui/themes/default/trashcan.svg
 gotify_tray/gui/themes/light_purple/__init__.py
 gotify_tray/gui/themes/light_purple/palette.py
 gotify_tray/gui/themes/light_purple/refresh.svg
 gotify_tray/gui/themes/light_purple/status_active.svg
 gotify_tray/gui/themes/light_purple/status_connecting.svg
 gotify_tray/gui/themes/light_purple/status_error.svg
 gotify_tray/gui/themes/light_purple/status_inactive.svg
```

### Comparing `gotify-tray-0.4.2/setup.py` & `gotify-tray-0.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 # Package meta-data.
 NAME = 'gotify-tray'
 DESCRIPTION = 'A tray notification application for receiving messages from a Gotify server.'
 URL = 'https://github.com/seird/gotify-tray'
 EMAIL = "k.dries@protonmail.com"
-REQUIRES_PYTHON = '>=3.8.0'
+REQUIRES_PYTHON = '>=3.10.0'
 with open("version.txt", "r") as f:
     VERSION = f.read()
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests', 'PyQt6', 'websocket-client', 'python-dateutil'
 ]
@@ -80,12 +80,10 @@
     license='GPLv3',
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10'
     ]
 )
```

