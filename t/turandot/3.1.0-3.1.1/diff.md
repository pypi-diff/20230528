# Comparing `tmp/turandot-3.1.0.tar.gz` & `tmp/turandot-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turandot-3.1.0.tar", last modified: Thu Dec 29 18:18:54 2022, max compression
+gzip compressed data, was "turandot-3.1.1.tar", last modified: Sun May 28 14:14:31 2023, max compression
```

## Comparing `turandot-3.1.0.tar` & `turandot-3.1.1.tar`

### file list

```diff
@@ -1,162 +1,159 @@
-drwxrwxr-x   0 dinu      (1000) dinu      (1000)        0 2022-12-29 18:18:54.075728 turandot-3.1.0/
--rw-rw-r--   0 dinu      (1000) dinu      (1000)    35075 2022-08-08 14:24:30.000000 turandot-3.1.0/LICENSE.txt
--rw-rw-r--   0 dinu      (1000) dinu      (1000)       21 2022-08-08 14:24:30.000000 turandot-3.1.0/MANIFEST.in
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     2048 2022-12-29 18:18:54.075728 turandot-3.1.0/PKG-INFO
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1073 2022-08-08 14:24:30.000000 turandot-3.1.0/README.md
--rw-rw-r--   0 dinu      (1000) dinu      (1000)       38 2022-12-29 18:18:54.075728 turandot-3.1.0/setup.cfg
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1945 2022-12-29 18:16:13.000000 turandot-3.1.0/setup.py
-drwxrwxr-x   0 dinu      (1000) dinu      (1000)        0 2022-12-29 18:18:54.011727 turandot-3.1.0/turandot/
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      294 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/__init__.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1705 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/__main__.py
-drwxrwxr-x   0 dinu      (1000) dinu      (1000)        0 2022-12-29 18:18:54.023727 turandot-3.1.0/turandot/assets/
--rw-rw-r--   0 dinu      (1000) dinu      (1000)        0 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/assets/__init__.py
-drwxrwxr-x   0 dinu      (1000) dinu      (1000)        0 2022-12-29 18:18:54.023727 turandot-3.1.0/turandot/assets/__pycache__/
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      153 2022-08-20 11:17:20.000000 turandot-3.1.0/turandot/assets/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      836 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/assets/about.txt
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     2538 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/assets/default.yaml
-drwxrwxr-x   0 dinu      (1000) dinu      (1000)        0 2022-12-29 18:18:54.023727 turandot-3.1.0/turandot/assets/extract/
--rw-rw-r--   0 dinu      (1000) dinu      (1000)        0 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/assets/extract/__init__.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1250 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/assets/extract/__main__.py
-drwxrwxr-x   0 dinu      (1000) dinu      (1000)        0 2022-12-29 18:18:54.043727 turandot-3.1.0/turandot/assets/extract/__pycache__/
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      161 2022-11-16 19:53:27.000000 turandot-3.1.0/turandot/assets/extract/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1348 2022-11-16 20:16:27.000000 turandot-3.1.0/turandot/assets/extract/__pycache__/__main__.cpython-310.pyc
--rw-rw-r--   0 dinu      (1000) dinu      (1000)       90 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/assets/gtk4.css
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      233 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/assets/turandot.desktop
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     9430 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/assets/turandot.png
--rw-rw-r--   0 dinu      (1000) dinu      (1000)       74 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/assets/turandot.sh
--rw-rw-r--   0 dinu      (1000) dinu      (1000)    20902 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/assets/turandot.svg
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      243 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/assets/uninstall.sh
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      235 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/assets/update.sh
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     2836 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/assets/windows_fonts.conf
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      568 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/exceptions.py
-drwxrwxr-x   0 dinu      (1000) dinu      (1000)        0 2022-12-29 18:18:54.051728 turandot-3.1.0/turandot/gtk4/
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      154 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/__init__.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1018 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/__main__.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1113 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/catcher.py
-drwxrwxr-x   0 dinu      (1000) dinu      (1000)        0 2022-12-29 18:18:54.051728 turandot-3.1.0/turandot/gtk4/controllers/
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      441 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/controllers/__init__.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      178 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/controllers/basecontroller.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     2992 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/controllers/conversionupdater.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     6713 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/controllers/convertercontroller.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     2943 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/controllers/cslcontroller.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      814 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/controllers/headerbarcontroller.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     3855 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/controllers/templatecontroller.py
-drwxrwxr-x   0 dinu      (1000) dinu      (1000)        0 2022-12-29 18:18:54.055728 turandot-3.1.0/turandot/gtk4/dialogs/
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      333 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/dialogs/__init__.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1507 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/dialogs/aboutdialog.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1613 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/dialogs/confirmationdialog.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1624 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/dialogs/errordialog.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     2774 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/dialogs/filechooser.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     3106 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/dialogs/settingsdialog.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      953 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/dialogs/templateeditor.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      992 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/enumlocalization.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     2987 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/filefilters.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      281 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/guithread.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     4792 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/mainwindow.py
-drwxrwxr-x   0 dinu      (1000) dinu      (1000)        0 2022-12-29 18:18:54.055728 turandot-3.1.0/turandot/gtk4/presentations/
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      377 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/presentations/__init__.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      670 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/presentations/enumdropdown.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1027 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/presentations/observerdropdown.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1728 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/presentations/observerlistviews.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     5197 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/presentations/settingspresentation.py
-drwxrwxr-x   0 dinu      (1000) dinu      (1000)        0 2022-12-29 18:18:54.055728 turandot-3.1.0/turandot/gtk4/representations/
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      194 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/representations/__init__.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      654 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/representations/dbobservables.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      508 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/representations/observerbase.py
-drwxrwxr-x   0 dinu      (1000) dinu      (1000)        0 2022-12-29 18:18:54.055728 turandot-3.1.0/turandot/gtk4/views/
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      277 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/views/__init__.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     8328 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/views/convertertab.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     3151 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/views/csltab.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      845 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/views/headerbarview.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     4641 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/views/templatetab.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      747 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/gtk4/views/viewcomponent.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      280 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/meta.py
-drwxrwxr-x   0 dinu      (1000) dinu      (1000)        0 2022-12-29 18:18:54.055728 turandot-3.1.0/turandot/model/
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1571 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/model/__init__.py
-drwxrwxr-x   0 dinu      (1000) dinu      (1000)        0 2022-12-29 18:18:54.055728 turandot-3.1.0/turandot/model/config/
--rw-rw-r--   0 dinu      (1000) dinu      (1000)        1 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/model/config/__init__.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     2241 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/model/config/config.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1789 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/model/config/configdict.py
-drwxrwxr-x   0 dinu      (1000) dinu      (1000)        0 2022-12-29 18:18:54.059728 turandot-3.1.0/turandot/model/converter/
--rw-rw-r--   0 dinu      (1000) dinu      (1000)        0 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/model/converter/__init__.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     3596 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/model/converter/applytemplate.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     3801 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/model/converter/conversionprocessor.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     3594 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/model/converter/converterbase.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1183 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/model/converter/converterchain.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     3577 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/model/converter/convtohtml.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     2716 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/model/converter/copytemplate.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      841 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/model/converter/frontendstrategy.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     4051 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/model/converter/gatherdata.py
-drwxrwxr-x   0 dinu      (1000) dinu      (1000)        0 2022-12-29 18:18:54.059728 turandot-3.1.0/turandot/model/converter/optional/
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      160 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/model/converter/optional/__init__.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1020 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/model/converter/optional/tocpagination.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1587 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/model/converter/optional/unifiedmath.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     3150 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/model/converter/weasytopdf.py
-drwxrwxr-x   0 dinu      (1000) dinu      (1000)        0 2022-12-29 18:18:54.063728 turandot-3.1.0/turandot/model/datastructures/
--rw-rw-r--   0 dinu      (1000) dinu      (1000)        0 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/model/datastructures/__init__.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1448 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/model/datastructures/baseasset.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1392 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/model/datastructures/companiondata.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1717 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/model/datastructures/conversionjob.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1509 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/model/datastructures/cslasset.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1255 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/model/datastructures/dbasset.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1075 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/model/datastructures/enums.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     2123 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/model/datastructures/queuemsg.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      646 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/model/datastructures/sourceasset.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      256 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/model/datastructures/textasset.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     4205 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/model/datastructures/tmplasset.py
-drwxrwxr-x   0 dinu      (1000) dinu      (1000)        0 2022-12-29 18:18:54.063728 turandot-3.1.0/turandot/model/sql/
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      222 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/model/sql/__init__.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)       82 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/model/sql/base.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1491 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/model/sql/engine.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     4473 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/model/sql/repository.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      811 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/model/sql/tables.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1112 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/model/util.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     2432 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/model/zoteroconnector.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1225 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/sysinfo.py
-drwxrwxr-x   0 dinu      (1000) dinu      (1000)        0 2022-12-29 18:18:54.067728 turandot-3.1.0/turandot/ttk/
--rw-rw-r--   0 dinu      (1000) dinu      (1000)       91 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ttk/__init__.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1206 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ttk/__main__.py
-drwxrwxr-x   0 dinu      (1000) dinu      (1000)        0 2022-12-29 18:18:54.067728 turandot-3.1.0/turandot/ttk/controllers/
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      591 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ttk/controllers/__init__.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1277 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ttk/controllers/aboutcontroller.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      238 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ttk/controllers/basecontroller.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     4300 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ttk/controllers/conversionupdater.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     4852 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ttk/controllers/convertercontroller.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     7532 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ttk/controllers/dbdropdowncontroller.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      871 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ttk/controllers/exceptioncontroller.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     3992 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ttk/controllers/exportcontroller.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     3033 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/ttk/controllers/settingscontroller.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      593 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ttk/filetypes.py
-drwxrwxr-x   0 dinu      (1000) dinu      (1000)        0 2022-12-29 18:18:54.071728 turandot-3.1.0/turandot/ttk/presentations/
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      644 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ttk/presentations/__init__.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     5979 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ttk/presentations/configpresentations.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      788 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/ttk/presentations/dbfedpicker.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1969 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ttk/presentations/dropdownobservables.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     2138 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ttk/presentations/dropdownobservers.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      594 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ttk/presentations/enumcombobox.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1923 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ttk/presentations/kvcombobox.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      434 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ttk/tkcatcher.py
-drwxrwxr-x   0 dinu      (1000) dinu      (1000)        0 2022-12-29 18:18:54.071728 turandot-3.1.0/turandot/ttk/view/
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      159 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ttk/view/__init__.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      574 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ttk/view/abouttab.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     6302 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ttk/view/convertertab.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     2607 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ttk/view/csltab.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     4709 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ttk/view/processframe.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     2075 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ttk/view/settingstab.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1402 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ttk/view/styles.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     3702 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ttk/view/templatetab.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     4805 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/ttk/view/ttkview.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      355 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ttk/view/viewcomponent.py
-drwxrwxr-x   0 dinu      (1000) dinu      (1000)        0 2022-12-29 18:18:54.075728 turandot-3.1.0/turandot/ui/
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      330 2022-12-29 18:16:13.000000 turandot-3.1.0/turandot/ui/__init__.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      780 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ui/background.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1246 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ui/enumtranslations.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1266 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ui/exceptioncatcher.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      220 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ui/frontend.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      968 2022-08-08 14:24:30.000000 turandot-3.1.0/turandot/ui/utils.py
-drwxrwxr-x   0 dinu      (1000) dinu      (1000)        0 2022-12-29 18:18:54.015727 turandot-3.1.0/turandot.egg-info/
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     2048 2022-12-29 18:18:53.000000 turandot-3.1.0/turandot.egg-info/PKG-INFO
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     4889 2022-12-29 18:18:53.000000 turandot-3.1.0/turandot.egg-info/SOURCES.txt
--rw-rw-r--   0 dinu      (1000) dinu      (1000)        1 2022-12-29 18:18:53.000000 turandot-3.1.0/turandot.egg-info/dependency_links.txt
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      299 2022-12-29 18:18:53.000000 turandot-3.1.0/turandot.egg-info/requires.txt
--rw-rw-r--   0 dinu      (1000) dinu      (1000)        9 2022-12-29 18:18:53.000000 turandot-3.1.0/turandot.egg-info/top_level.txt
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2023-05-28 14:14:31.457069 turandot-3.1.1/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)    35075 2023-02-28 11:23:16.000000 turandot-3.1.1/LICENSE.txt
+-rw-r--r--   0 dinu      (1000) dinu      (1000)       21 2023-02-28 11:23:16.000000 turandot-3.1.1/MANIFEST.in
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2028 2023-05-28 14:14:31.457069 turandot-3.1.1/PKG-INFO
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1073 2023-02-28 11:23:16.000000 turandot-3.1.1/README.md
+-rw-r--r--   0 dinu      (1000) dinu      (1000)       38 2023-05-28 14:14:31.457069 turandot-3.1.1/setup.cfg
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1945 2023-05-28 13:29:04.000000 turandot-3.1.1/setup.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2023-05-28 14:14:31.442069 turandot-3.1.1/turandot/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      294 2023-05-28 13:29:04.000000 turandot-3.1.1/turandot/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1705 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/__main__.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2023-05-28 14:14:31.443069 turandot-3.1.1/turandot/assets/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)        0 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/assets/__init__.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2023-05-28 14:14:31.444069 turandot-3.1.1/turandot/assets/__pycache__/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      169 2023-05-28 13:16:13.000000 turandot-3.1.1/turandot/assets/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      836 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/assets/about.txt
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2538 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/assets/default.yaml
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2023-05-28 14:14:31.444069 turandot-3.1.1/turandot/assets/extract/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)        0 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/assets/extract/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1250 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/assets/extract/__main__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)       90 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/assets/gtk4.css
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      233 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/assets/turandot.desktop
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     9430 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/assets/turandot.png
+-rw-r--r--   0 dinu      (1000) dinu      (1000)       74 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/assets/turandot.sh
+-rw-r--r--   0 dinu      (1000) dinu      (1000)    20902 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/assets/turandot.svg
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      243 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/assets/uninstall.sh
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      235 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/assets/update.sh
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2836 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/assets/windows_fonts.conf
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      568 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/exceptions.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2023-05-28 14:14:31.444069 turandot-3.1.1/turandot/gtk4/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      154 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1018 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/__main__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1113 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/catcher.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2023-05-28 14:14:31.445069 turandot-3.1.1/turandot/gtk4/controllers/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      441 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/controllers/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      178 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/controllers/basecontroller.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2992 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/controllers/conversionupdater.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     6713 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/controllers/convertercontroller.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2943 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/controllers/cslcontroller.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      814 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/controllers/headerbarcontroller.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     3855 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/controllers/templatecontroller.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2023-05-28 14:14:31.446069 turandot-3.1.1/turandot/gtk4/dialogs/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      333 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/dialogs/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1507 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/dialogs/aboutdialog.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1613 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/dialogs/confirmationdialog.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1624 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/dialogs/errordialog.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2774 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/dialogs/filechooser.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     3106 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/dialogs/settingsdialog.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      953 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/dialogs/templateeditor.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      992 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/enumlocalization.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2987 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/filefilters.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      281 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/guithread.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     4792 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/mainwindow.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2023-05-28 14:14:31.446069 turandot-3.1.1/turandot/gtk4/presentations/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      377 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/presentations/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      670 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/presentations/enumdropdown.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1027 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/presentations/observerdropdown.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1728 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/presentations/observerlistviews.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     5197 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/presentations/settingspresentation.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2023-05-28 14:14:31.446069 turandot-3.1.1/turandot/gtk4/representations/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      194 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/representations/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      654 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/representations/dbobservables.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      508 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/representations/observerbase.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2023-05-28 14:14:31.447069 turandot-3.1.1/turandot/gtk4/views/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      277 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/views/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     8328 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/views/convertertab.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     3151 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/views/csltab.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      845 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/views/headerbarview.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     4641 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/views/templatetab.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      747 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/gtk4/views/viewcomponent.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      280 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/meta.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2023-05-28 14:14:31.448069 turandot-3.1.1/turandot/model/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1571 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/__init__.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2023-05-28 14:14:31.448069 turandot-3.1.1/turandot/model/config/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)        1 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/config/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2241 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/config/config.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1789 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/config/configdict.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2023-05-28 14:14:31.450069 turandot-3.1.1/turandot/model/converter/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)        0 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/converter/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     3596 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/converter/applytemplate.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     3801 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/converter/conversionprocessor.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     3594 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/converter/converterbase.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1183 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/converter/converterchain.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     3577 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/converter/convtohtml.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2716 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/converter/copytemplate.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      841 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/converter/frontendstrategy.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     4051 2023-05-28 14:12:28.000000 turandot-3.1.1/turandot/model/converter/gatherdata.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2023-05-28 14:14:31.450069 turandot-3.1.1/turandot/model/converter/optional/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      160 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/converter/optional/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1020 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/converter/optional/tocpagination.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1587 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/converter/optional/unifiedmath.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     3150 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/converter/weasytopdf.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2023-05-28 14:14:31.451069 turandot-3.1.1/turandot/model/datastructures/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)        0 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/datastructures/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1448 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/datastructures/baseasset.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1392 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/datastructures/companiondata.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1717 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/datastructures/conversionjob.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1509 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/datastructures/cslasset.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1255 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/datastructures/dbasset.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1075 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/datastructures/enums.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2123 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/datastructures/queuemsg.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      646 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/datastructures/sourceasset.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      256 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/datastructures/textasset.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     4205 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/datastructures/tmplasset.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2023-05-28 14:14:31.452069 turandot-3.1.1/turandot/model/sql/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      222 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/sql/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)       82 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/sql/base.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1491 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/sql/engine.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     4475 2023-05-28 13:28:06.000000 turandot-3.1.1/turandot/model/sql/repository.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      811 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/model/sql/tables.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1170 2023-05-28 14:13:52.000000 turandot-3.1.1/turandot/model/util.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2436 2023-05-28 14:09:13.000000 turandot-3.1.1/turandot/model/zoteroconnector.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1225 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/sysinfo.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2023-05-28 14:14:31.452069 turandot-3.1.1/turandot/ttk/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)       91 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1206 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/__main__.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2023-05-28 14:14:31.454069 turandot-3.1.1/turandot/ttk/controllers/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      591 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/controllers/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1277 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/controllers/aboutcontroller.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      238 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/controllers/basecontroller.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     4300 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/controllers/conversionupdater.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     4852 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/controllers/convertercontroller.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     7532 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/controllers/dbdropdowncontroller.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      871 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/controllers/exceptioncontroller.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     3992 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/controllers/exportcontroller.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     3033 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/controllers/settingscontroller.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      593 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/filetypes.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2023-05-28 14:14:31.455069 turandot-3.1.1/turandot/ttk/presentations/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      644 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/presentations/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     5979 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/presentations/configpresentations.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      788 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/presentations/dbfedpicker.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1969 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/presentations/dropdownobservables.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2138 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/presentations/dropdownobservers.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      594 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/presentations/enumcombobox.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1923 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/presentations/kvcombobox.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      434 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/tkcatcher.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2023-05-28 14:14:31.456069 turandot-3.1.1/turandot/ttk/view/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      159 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/view/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      574 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/view/abouttab.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     6302 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/view/convertertab.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2607 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/view/csltab.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     4709 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/view/processframe.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2075 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/view/settingstab.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1402 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/view/styles.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     3702 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/view/templatetab.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     4805 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/view/ttkview.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      355 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ttk/view/viewcomponent.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2023-05-28 14:14:31.457069 turandot-3.1.1/turandot/ui/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      330 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ui/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      780 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ui/background.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1246 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ui/enumtranslations.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1266 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ui/exceptioncatcher.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      220 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ui/frontend.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      968 2023-02-28 11:23:16.000000 turandot-3.1.1/turandot/ui/utils.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2023-05-28 14:14:31.442069 turandot-3.1.1/turandot.egg-info/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2028 2023-05-28 14:14:31.000000 turandot-3.1.1/turandot.egg-info/PKG-INFO
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     4767 2023-05-28 14:14:31.000000 turandot-3.1.1/turandot.egg-info/SOURCES.txt
+-rw-r--r--   0 dinu      (1000) dinu      (1000)        1 2023-05-28 14:14:31.000000 turandot-3.1.1/turandot.egg-info/dependency_links.txt
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      299 2023-05-28 14:14:31.000000 turandot-3.1.1/turandot.egg-info/requires.txt
+-rw-r--r--   0 dinu      (1000) dinu      (1000)        9 2023-05-28 14:14:31.000000 turandot-3.1.1/turandot.egg-info/top_level.txt
```

### Comparing `turandot-3.1.0/LICENSE.txt` & `turandot-3.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/PKG-INFO` & `turandot-3.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: turandot
-Version: 3.1.0
+Version: 3.1.1
 Summary: Turandot Markdown Converter
 Home-page: https://turandot.readthedocs.io
 Author: Martin Obrist
 Author-email: dev@obrist.email
 License: GPLv3
 Project-URL: Documentation, https://turandot.readthedocs.io
 Project-URL: Source Code, https://gitlab.com/dinuthehuman/turandot
 Project-URL: Issue Tracker, https://gitlab.com/dinuthehuman/turandot/-/issues
 Keywords: markdown,citeproc
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.10, <4
@@ -41,9 +40,7 @@
 - Available as deb package with a Windows installer in progress
 
 ## Links
 
 - [Full documentation](https://turandot.readthedocs.io) (work in progress)
 - [Source Code](https://gitlab.com/dinuthehuman/turandot)
 - [Issue Tracker](https://gitlab.com/dinuthehuman/turandot/-/issues)
-
-
```

### Comparing `turandot-3.1.0/README.md` & `turandot-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/setup.py` & `turandot-3.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='turandot',
-    version='3.1.0',
+    version='3.1.1',
     description='Turandot Markdown Converter',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
     author='Martin Obrist',
     author_email='dev@obrist.email',
     url='https://turandot.readthedocs.io',
```

### Comparing `turandot-3.1.0/turandot/__main__.py` & `turandot-3.1.1/turandot/__main__.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/assets/about.txt` & `turandot-3.1.1/turandot/assets/about.txt`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/assets/default.yaml` & `turandot-3.1.1/turandot/assets/default.yaml`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/assets/extract/__main__.py` & `turandot-3.1.1/turandot/assets/extract/__main__.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/assets/turandot.png` & `turandot-3.1.1/turandot/assets/turandot.png`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/assets/turandot.svg` & `turandot-3.1.1/turandot/assets/turandot.svg`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/assets/windows_fonts.conf` & `turandot-3.1.1/turandot/assets/windows_fonts.conf`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/exceptions.py` & `turandot-3.1.1/turandot/exceptions.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/gtk4/__main__.py` & `turandot-3.1.1/turandot/gtk4/__main__.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/gtk4/catcher.py` & `turandot-3.1.1/turandot/gtk4/catcher.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/gtk4/controllers/conversionupdater.py` & `turandot-3.1.1/turandot/gtk4/controllers/conversionupdater.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/gtk4/controllers/convertercontroller.py` & `turandot-3.1.1/turandot/gtk4/controllers/convertercontroller.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/gtk4/controllers/cslcontroller.py` & `turandot-3.1.1/turandot/gtk4/controllers/cslcontroller.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/gtk4/controllers/headerbarcontroller.py` & `turandot-3.1.1/turandot/gtk4/controllers/headerbarcontroller.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/gtk4/controllers/templatecontroller.py` & `turandot-3.1.1/turandot/gtk4/controllers/templatecontroller.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/gtk4/dialogs/aboutdialog.py` & `turandot-3.1.1/turandot/gtk4/dialogs/aboutdialog.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/gtk4/dialogs/confirmationdialog.py` & `turandot-3.1.1/turandot/gtk4/dialogs/confirmationdialog.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/gtk4/dialogs/errordialog.py` & `turandot-3.1.1/turandot/gtk4/dialogs/errordialog.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/gtk4/dialogs/filechooser.py` & `turandot-3.1.1/turandot/gtk4/dialogs/filechooser.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/gtk4/dialogs/settingsdialog.py` & `turandot-3.1.1/turandot/gtk4/dialogs/settingsdialog.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/gtk4/dialogs/templateeditor.py` & `turandot-3.1.1/turandot/gtk4/dialogs/templateeditor.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/gtk4/enumlocalization.py` & `turandot-3.1.1/turandot/gtk4/enumlocalization.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/gtk4/filefilters.py` & `turandot-3.1.1/turandot/gtk4/filefilters.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/gtk4/mainwindow.py` & `turandot-3.1.1/turandot/gtk4/mainwindow.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/gtk4/presentations/enumdropdown.py` & `turandot-3.1.1/turandot/gtk4/presentations/enumdropdown.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/gtk4/presentations/observerdropdown.py` & `turandot-3.1.1/turandot/gtk4/presentations/observerdropdown.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/gtk4/presentations/observerlistviews.py` & `turandot-3.1.1/turandot/gtk4/presentations/observerlistviews.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/gtk4/presentations/settingspresentation.py` & `turandot-3.1.1/turandot/gtk4/presentations/settingspresentation.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/gtk4/representations/dbobservables.py` & `turandot-3.1.1/turandot/gtk4/representations/dbobservables.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/gtk4/views/convertertab.py` & `turandot-3.1.1/turandot/gtk4/views/convertertab.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/gtk4/views/csltab.py` & `turandot-3.1.1/turandot/gtk4/views/csltab.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/gtk4/views/headerbarview.py` & `turandot-3.1.1/turandot/gtk4/views/headerbarview.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/gtk4/views/templatetab.py` & `turandot-3.1.1/turandot/gtk4/views/templatetab.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/gtk4/views/viewcomponent.py` & `turandot-3.1.1/turandot/gtk4/views/viewcomponent.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/model/__init__.py` & `turandot-3.1.1/turandot/model/__init__.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/model/config/config.py` & `turandot-3.1.1/turandot/model/config/config.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/model/config/configdict.py` & `turandot-3.1.1/turandot/model/config/configdict.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/model/converter/applytemplate.py` & `turandot-3.1.1/turandot/model/converter/applytemplate.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/model/converter/conversionprocessor.py` & `turandot-3.1.1/turandot/model/converter/conversionprocessor.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/model/converter/converterbase.py` & `turandot-3.1.1/turandot/model/converter/converterbase.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/model/converter/converterchain.py` & `turandot-3.1.1/turandot/model/converter/converterchain.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/model/converter/convtohtml.py` & `turandot-3.1.1/turandot/model/converter/convtohtml.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/model/converter/copytemplate.py` & `turandot-3.1.1/turandot/model/converter/copytemplate.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/model/converter/frontendstrategy.py` & `turandot-3.1.1/turandot/model/converter/frontendstrategy.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/model/converter/gatherdata.py` & `turandot-3.1.1/turandot/model/converter/gatherdata.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/model/converter/optional/tocpagination.py` & `turandot-3.1.1/turandot/model/converter/optional/tocpagination.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/model/converter/optional/unifiedmath.py` & `turandot-3.1.1/turandot/model/converter/optional/unifiedmath.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/model/converter/weasytopdf.py` & `turandot-3.1.1/turandot/model/converter/weasytopdf.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/model/datastructures/baseasset.py` & `turandot-3.1.1/turandot/model/datastructures/baseasset.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/model/datastructures/companiondata.py` & `turandot-3.1.1/turandot/model/datastructures/companiondata.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/model/datastructures/conversionjob.py` & `turandot-3.1.1/turandot/model/datastructures/conversionjob.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/model/datastructures/cslasset.py` & `turandot-3.1.1/turandot/model/datastructures/cslasset.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/model/datastructures/dbasset.py` & `turandot-3.1.1/turandot/model/datastructures/dbasset.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/model/datastructures/enums.py` & `turandot-3.1.1/turandot/model/datastructures/enums.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/model/datastructures/queuemsg.py` & `turandot-3.1.1/turandot/model/datastructures/queuemsg.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/model/datastructures/sourceasset.py` & `turandot-3.1.1/turandot/model/datastructures/sourceasset.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/model/datastructures/tmplasset.py` & `turandot-3.1.1/turandot/model/datastructures/tmplasset.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/model/sql/engine.py` & `turandot-3.1.1/turandot/model/sql/engine.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/model/sql/repository.py` & `turandot-3.1.1/turandot/model/sql/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,9 +113,9 @@
             return Path(row.last_path)
         except NoResultFound:
             return Path.home()
 
     def set_file_select_persist(self, selector_id: str, path: Path):
         with self.engine.create_session() as session:
             dbmodel = DbFileSelectPersistence(input_id=selector_id, last_path=str(path))
-            session.add(dbmodel)
+            session.merge(dbmodel)
             session.commit()
```

### Comparing `turandot-3.1.0/turandot/model/sql/tables.py` & `turandot-3.1.1/turandot/model/sql/tables.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/model/util.py` & `turandot-3.1.1/turandot/model/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import os
 from pathlib import Path
 from importlib import resources
+from importlib.resources import files
+
+from turandot import assets
 
 
 class ModelUtils:
     """Static helper functions for the model"""
 
     @staticmethod
     def get_config_dir() -> Path:
@@ -22,12 +25,12 @@
 
     @staticmethod
     def get_config_file() -> Path:
         return ModelUtils.get_config_dir() / "config3.yaml"
 
     @staticmethod
     def get_asset_content(filename: str) -> str:
-        return resources.read_text("turandot.assets", filename)
+        return files(assets).joinpath(filename).read_text()
 
     @staticmethod
     def get_asset_bytes(filename: str) -> bytes:
-        return resources.read_binary("turandot.assets", filename)
+        return files(assets).joinpath(filename).read_bytes()
```

### Comparing `turandot-3.1.0/turandot/model/zoteroconnector.py` & `turandot-3.1.1/turandot/model/zoteroconnector.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from enum import Enum
 from turandot import TurandotConnectionException
 from turandot.model import ConfigDict
 
 
 class ZoteroDataFormat(Enum):
     BIBTEX = "biblatex"
-    CSLJSON = "csljson"
+    CSLJSON = "json"
 
 
 class ZoteroConnector:
     """Connect to Zoteros BetterBibtex extension to get bibliographic data"""
 
     def __init__(self, config: ConfigDict):
         self.hostname = config.get_key(['api', 'zotero', 'host'], "localhost")
@@ -46,15 +46,15 @@
     def get_bib_data(self, libid: int, form: ZoteroDataFormat) -> str:
         """
         Get bibliographic data from Zotero
         :param libid: Library to get data from
         :param form: Format: JSON or Bibtex
         :return: Bibliographic data in text format
         """
-        endpoint = "/better-bibtex/library?/{}/library.{}".format(libid, form.value)
+        endpoint = "/better-bibtex/export/library?/{}/library.{}".format(libid, form.value)
         url = self._assemble_url(endpoint)
         try:
             response = requests.get(url)
             return response.content.decode()
         except requests.exceptions.ConnectionError:
             raise self.connection_error
```

### Comparing `turandot-3.1.0/turandot/sysinfo.py` & `turandot-3.1.1/turandot/sysinfo.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/ttk/__main__.py` & `turandot-3.1.1/turandot/ttk/__main__.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/ttk/controllers/__init__.py` & `turandot-3.1.1/turandot/ttk/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/ttk/controllers/aboutcontroller.py` & `turandot-3.1.1/turandot/ttk/controllers/aboutcontroller.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/ttk/controllers/conversionupdater.py` & `turandot-3.1.1/turandot/ttk/controllers/conversionupdater.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/ttk/controllers/convertercontroller.py` & `turandot-3.1.1/turandot/ttk/controllers/convertercontroller.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/ttk/controllers/dbdropdowncontroller.py` & `turandot-3.1.1/turandot/ttk/controllers/dbdropdowncontroller.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/ttk/controllers/exceptioncontroller.py` & `turandot-3.1.1/turandot/ttk/controllers/exceptioncontroller.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/ttk/controllers/exportcontroller.py` & `turandot-3.1.1/turandot/ttk/controllers/exportcontroller.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/ttk/controllers/settingscontroller.py` & `turandot-3.1.1/turandot/ttk/controllers/settingscontroller.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/ttk/filetypes.py` & `turandot-3.1.1/turandot/ttk/filetypes.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/ttk/presentations/__init__.py` & `turandot-3.1.1/turandot/ttk/presentations/__init__.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/ttk/presentations/configpresentations.py` & `turandot-3.1.1/turandot/ttk/presentations/configpresentations.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/ttk/presentations/dbfedpicker.py` & `turandot-3.1.1/turandot/ttk/presentations/dbfedpicker.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/ttk/presentations/dropdownobservables.py` & `turandot-3.1.1/turandot/ttk/presentations/dropdownobservables.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/ttk/presentations/dropdownobservers.py` & `turandot-3.1.1/turandot/ttk/presentations/dropdownobservers.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/ttk/presentations/enumcombobox.py` & `turandot-3.1.1/turandot/ttk/presentations/enumcombobox.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/ttk/presentations/kvcombobox.py` & `turandot-3.1.1/turandot/ttk/presentations/kvcombobox.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/ttk/view/abouttab.py` & `turandot-3.1.1/turandot/ttk/view/abouttab.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/ttk/view/convertertab.py` & `turandot-3.1.1/turandot/ttk/view/convertertab.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/ttk/view/csltab.py` & `turandot-3.1.1/turandot/ttk/view/csltab.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/ttk/view/processframe.py` & `turandot-3.1.1/turandot/ttk/view/processframe.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/ttk/view/settingstab.py` & `turandot-3.1.1/turandot/ttk/view/settingstab.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/ttk/view/styles.py` & `turandot-3.1.1/turandot/ttk/view/styles.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/ttk/view/templatetab.py` & `turandot-3.1.1/turandot/ttk/view/templatetab.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/ttk/view/ttkview.py` & `turandot-3.1.1/turandot/ttk/view/ttkview.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/ui/background.py` & `turandot-3.1.1/turandot/ui/background.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/ui/enumtranslations.py` & `turandot-3.1.1/turandot/ui/enumtranslations.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/ui/exceptioncatcher.py` & `turandot-3.1.1/turandot/ui/exceptioncatcher.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot/ui/utils.py` & `turandot-3.1.1/turandot/ui/utils.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.0/turandot.egg-info/PKG-INFO` & `turandot-3.1.1/turandot.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: turandot
-Version: 3.1.0
+Version: 3.1.1
 Summary: Turandot Markdown Converter
 Home-page: https://turandot.readthedocs.io
 Author: Martin Obrist
 Author-email: dev@obrist.email
 License: GPLv3
 Project-URL: Documentation, https://turandot.readthedocs.io
 Project-URL: Source Code, https://gitlab.com/dinuthehuman/turandot
 Project-URL: Issue Tracker, https://gitlab.com/dinuthehuman/turandot/-/issues
 Keywords: markdown,citeproc
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.10, <4
@@ -41,9 +40,7 @@
 - Available as deb package with a Windows installer in progress
 
 ## Links
 
 - [Full documentation](https://turandot.readthedocs.io) (work in progress)
 - [Source Code](https://gitlab.com/dinuthehuman/turandot)
 - [Issue Tracker](https://gitlab.com/dinuthehuman/turandot/-/issues)
-
-
```

### Comparing `turandot-3.1.0/turandot.egg-info/SOURCES.txt` & `turandot-3.1.1/turandot.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,17 @@
 turandot/assets/turandot.desktop
 turandot/assets/turandot.png
 turandot/assets/turandot.sh
 turandot/assets/turandot.svg
 turandot/assets/uninstall.sh
 turandot/assets/update.sh
 turandot/assets/windows_fonts.conf
-turandot/assets/__pycache__/__init__.cpython-310.pyc
+turandot/assets/__pycache__/__init__.cpython-311.pyc
 turandot/assets/extract/__init__.py
 turandot/assets/extract/__main__.py
-turandot/assets/extract/__pycache__/__init__.cpython-310.pyc
-turandot/assets/extract/__pycache__/__main__.cpython-310.pyc
 turandot/gtk4/__init__.py
 turandot/gtk4/__main__.py
 turandot/gtk4/catcher.py
 turandot/gtk4/enumlocalization.py
 turandot/gtk4/filefilters.py
 turandot/gtk4/guithread.py
 turandot/gtk4/mainwindow.py
```

