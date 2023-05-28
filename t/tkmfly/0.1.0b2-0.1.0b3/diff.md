# Comparing `tmp/tkmfly-0.1.0b2.tar.gz` & `tmp/tkmfly-0.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkmfly-0.1.0b2.tar", max compression
+gzip compressed data, was "tkmfly-0.1.0b3.tar", max compression
```

## Comparing `tkmfly-0.1.0b2.tar` & `tkmfly-0.1.0b3.tar`

### file list

```diff
@@ -1,89 +1,125 @@
--rw-r--r--   0        0        0      294 2023-05-27 12:46:56.355240 tkmfly-0.1.0b2/pyproject.toml
--rw-r--r--   0        0        0      996 2023-05-26 23:57:55.185069 tkmfly-0.1.0b2/README.md
--rw-r--r--   0        0        0      326 2023-05-27 12:46:46.430498 tkmfly-0.1.0b2/tkmfly/__init__.py
--rw-r--r--   0        0        0     2236 2023-05-19 12:56:40.594230 tkmfly-0.1.0b2/tkmfly/core.py
--rw-r--r--   0        0        0     1233 2023-05-26 23:09:11.462165 tkmfly-0.1.0b2/tkmfly/datefield/__init__.py
--rw-r--r--   0        0        0     2576 2023-05-26 23:09:11.811654 tkmfly-0.1.0b2/tkmfly/datefield/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    12619 2023-05-26 23:09:11.812654 tkmfly-0.1.0b2/tkmfly/datefield/__pycache__/pkgIndex.cpython-311.pyc
--rw-r--r--   0        0        0    12954 2023-05-26 23:09:11.466673 tkmfly-0.1.0b2/tkmfly/datefield/pkgIndex.py
--rw-r--r--   0        0        0     5339 2023-05-26 23:12:13.060020 tkmfly-0.1.0b2/tkmfly/history/__init__.py
--rw-r--r--   0        0        0     8854 2023-05-26 23:19:59.494590 tkmfly-0.1.0b2/tkmfly/history/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3351 2023-05-26 23:11:33.122621 tkmfly-0.1.0b2/tkmfly/history/__pycache__/pkgIndex.cpython-311.pyc
--rw-r--r--   0        0        0     3317 2023-05-26 23:10:48.026539 tkmfly-0.1.0b2/tkmfly/history/pkgIndex.py
--rw-r--r--   0        0        0      899 2023-05-26 10:17:24.710900 tkmfly-0.1.0b2/tkmfly/notifywindow/__init__.py
--rw-r--r--   0        0        0     2358 2023-05-26 10:17:25.218284 tkmfly-0.1.0b2/tkmfly/notifywindow/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4177 2023-05-26 10:17:25.219284 tkmfly-0.1.0b2/tkmfly/notifywindow/__pycache__/pkgIndex.cpython-311.pyc
--rw-r--r--   0        0        0     4128 2023-05-26 10:15:08.058584 tkmfly-0.1.0b2/tkmfly/notifywindow/pkgIndex.py
--rw-r--r--   0        0        0      676 2023-05-26 23:27:44.237391 tkmfly-0.1.0b2/tkmfly/tkmdi/__init__.py
--rw-r--r--   0        0        0      933 2023-05-26 23:27:44.393937 tkmfly-0.1.0b2/tkmfly/tkmdi/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0       94 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/activehorztab.gif
--rw-r--r--   0        0        0       88 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/activeverttab.gif
--rw-r--r--   0        0        0       72 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/backwards.gif
--rw-r--r--   0        0        0      111 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/ballstick.gif
--rw-r--r--   0        0        0     1020 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/ballstick2.gif
--rw-r--r--   0        0        0      104 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/circle.gif
--rw-r--r--   0        0        0       61 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/close.gif
--rw-r--r--   0        0        0      853 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/corner.gif
--rw-r--r--   0        0        0       97 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/cut.gif
--rw-r--r--   0        0        0       70 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/down.gif
--rw-r--r--   0        0        0      135 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/draw.gif
--rw-r--r--   0        0        0      124 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/end.gif
--rw-r--r--   0        0        0      120 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/folder.gif
--rw-r--r--   0        0        0       67 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/horzsep.gif
--rw-r--r--   0        0        0       79 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/horztab.gif
--rw-r--r--   0        0        0      255 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/info.gif
--rw-r--r--   0        0        0       72 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/left.gif
--rw-r--r--   0        0        0       64 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/maximize.gif
--rw-r--r--   0        0        0       54 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/minimize.gif
--rw-r--r--   0        0        0       75 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/minusnode.gif
--rw-r--r--   0        0        0      105 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/new.gif
--rw-r--r--   0        0        0       40 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/nothing.gif
--rw-r--r--   0        0        0      132 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/open.gif
--rw-r--r--   0        0        0      125 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/openfolder.gif
--rw-r--r--   0        0        0       76 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/pause.gif
--rw-r--r--   0        0        0      109 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/play.gif
--rw-r--r--   0        0        0       79 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/plusnode.gif
--rw-r--r--   0        0        0       96 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/rect.gif
--rw-r--r--   0        0        0       70 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/restore.gif
--rw-r--r--   0        0        0      124 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/rewind.gif
--rw-r--r--   0        0        0      109 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/right.gif
--rw-r--r--   0        0        0       93 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/rotate.gif
--rw-r--r--   0        0        0       91 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/rotz.gif
--rw-r--r--   0        0        0      115 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/save.gif
--rw-r--r--   0        0        0      883 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/select.gif
--rw-r--r--   0        0        0      926 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/sphere.gif
--rw-r--r--   0        0        0     1236 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/sphere2.gif
--rw-r--r--   0        0        0      103 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/stick.gif
--rw-r--r--   0        0        0      611 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/stick2.gif
--rw-r--r--   0        0        0       75 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/stop.gif
--rw-r--r--   0        0        0      103 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/surface.gif
--rw-r--r--   0        0        0       85 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/tk.gif
--rw-r--r--   0        0        0      920 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/toscreen.gif
--rw-r--r--   0        0        0      139 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/toselection.gif
--rw-r--r--   0        0        0      881 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/trans.gif
--rw-r--r--   0        0        0       79 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/up.gif
--rw-r--r--   0        0        0       64 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/vertsep.gif
--rw-r--r--   0        0        0       72 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/verttab.gif
--rw-r--r--   0        0        0      871 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/wire.gif
--rw-r--r--   0        0        0      573 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/wire2.gif
--rw-r--r--   0        0        0       91 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/zclip.gif
--rw-r--r--   0        0        0      924 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/zoom.gif
--rw-r--r--   0        0        0      916 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/zoomToArea.gif
--rw-r--r--   0        0        0    10684 2023-05-27 00:03:28.083145 tkmfly-0.1.0b2/tkmfly/tkmdi/Widgets/__pycache__/FlatButtons.cpython-311.pyc
--rw-r--r--   0        0        0      171 2023-05-26 23:27:44.397534 tkmfly-0.1.0b2/tkmfly/tkmdi/Widgets/__pycache__/iconPath.cpython-311.pyc
--rw-r--r--   0        0        0    40355 2023-05-26 23:27:44.899919 tkmfly-0.1.0b2/tkmfly/tkmdi/Widgets/__pycache__/MDI.cpython-311.pyc
--rw-r--r--   0        0        0     6988 2023-05-27 00:03:28.076605 tkmfly-0.1.0b2/tkmfly/tkmdi/Widgets/__pycache__/ProgressBar.cpython-311.pyc
--rw-r--r--   0        0        0    14492 2023-05-27 00:03:28.089807 tkmfly-0.1.0b2/tkmfly/tkmdi/Widgets/__pycache__/Toolbar.cpython-311.pyc
--rw-r--r--   0        0        0    14971 2023-05-27 00:03:28.096936 tkmfly-0.1.0b2/tkmfly/tkmdi/Widgets/__pycache__/Tree.cpython-311.pyc
--rw-r--r--   0        0        0     5908 2023-05-26 23:27:44.257384 tkmfly-0.1.0b2/tkmfly/tkmdi/Widgets/FlatButtons.py
--rw-r--r--   0        0        0       51 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Widgets/iconPath.py
--rw-r--r--   0        0        0    24007 2023-05-26 23:27:44.247321 tkmfly-0.1.0b2/tkmfly/tkmdi/Widgets/MDI.py
--rw-r--r--   0        0        0     3170 2015-11-12 22:41:02.000000 tkmfly-0.1.0b2/tkmfly/tkmdi/Widgets/ProgressBar.py
--rw-r--r--   0        0        0     8636 2023-05-26 23:27:44.238812 tkmfly-0.1.0b2/tkmfly/tkmdi/Widgets/Toolbar.py
--rw-r--r--   0        0        0     7917 2023-05-26 23:27:44.232887 tkmfly-0.1.0b2/tkmfly/tkmdi/Widgets/Tree.py
--rw-r--r--   0        0        0     2036 2023-05-26 23:06:14.575524 tkmfly-0.1.0b2/tkmfly/tooltip/__init__.py
--rw-r--r--   0        0        0     3942 2023-05-26 23:06:15.078979 tkmfly-0.1.0b2/tkmfly/tooltip/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    18587 2023-05-26 23:06:15.080978 tkmfly-0.1.0b2/tkmfly/tooltip/__pycache__/pkgIndex.cpython-311.pyc
--rw-r--r--   0        0        0    19169 2023-05-26 23:05:54.789763 tkmfly-0.1.0b2/tkmfly/tooltip/pkgIndex.py
--rw-r--r--   0        0        0     6551 2023-05-26 23:55:52.145047 tkmfly-0.1.0b2/tkmfly/ttree.py
--rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 tkmfly-0.1.0b2/PKG-INFO
+-rw-r--r--   0        0        0      362 2023-05-28 09:54:44.624552 tkmfly-0.1.0b3/pyproject.toml
+-rw-r--r--   0        0        0      996 2023-05-26 23:57:55.185069 tkmfly-0.1.0b3/README.md
+-rw-r--r--   0        0        0      743 2023-05-28 09:45:28.427564 tkmfly-0.1.0b3/tkmfly/__init__.py
+-rw-r--r--   0        0        0     8776 2000-10-08 11:36:14.000000 tkmfly-0.1.0b3/tkmfly/_mkwidgets/Aclock.tcl
+-rw-r--r--   0        0        0     7959 2000-10-08 12:25:22.000000 tkmfly-0.1.0b3/tkmfly/_mkwidgets/Calendar.tcl
+-rw-r--r--   0        0        0     8431 2001-07-10 13:11:34.000000 tkmfly-0.1.0b3/tkmfly/_mkwidgets/Combobox.tcl
+-rw-r--r--   0        0        0    23297 2001-07-11 07:46:44.000000 tkmfly-0.1.0b3/tkmfly/_mkwidgets/Document.tcl
+-rw-r--r--   0        0        0    35855 2001-07-11 12:47:44.000000 tkmfly-0.1.0b3/tkmfly/_mkwidgets/Gridcontrol.tcl
+-rw-r--r--   0        0        0     2205 2000-10-17 11:08:12.000000 tkmfly-0.1.0b3/tkmfly/_mkwidgets/Ibutton.tcl
+-rw-r--r--   0        0        0    39251 2000-10-25 09:45:54.000000 tkmfly-0.1.0b3/tkmfly/_mkwidgets/Iconbox.tcl
+-rw-r--r--   0        0        0    33462 2001-07-12 09:28:42.000000 tkmfly-0.1.0b3/tkmfly/_mkwidgets/Listcontrol.tcl
+-rw-r--r--   0        0        0    26895 2001-07-11 07:54:00.000000 tkmfly-0.1.0b3/tkmfly/_mkwidgets/metawidget.tcl
+-rw-r--r--   0        0        0    30205 2003-07-08 13:35:52.000000 tkmfly-0.1.0b3/tkmfly/_mkwidgets/mkWidgets13.htm
+-rw-r--r--   0        0        0    65292 2003-07-08 13:35:54.000000 tkmfly-0.1.0b3/tkmfly/_mkwidgets/mkWidgetsCol13.htm
+-rw-r--r--   0        0        0    10122 2001-07-08 05:58:14.000000 tkmfly-0.1.0b3/tkmfly/_mkwidgets/Pane.tcl
+-rw-r--r--   0        0        0     1018 2001-07-11 12:36:48.000000 tkmfly-0.1.0b3/tkmfly/_mkwidgets/pkgIndex.tcl
+-rw-r--r--   0        0        0     3193 2000-10-25 13:42:14.000000 tkmfly-0.1.0b3/tkmfly/_mkwidgets/Progressbar.tcl
+-rw-r--r--   0        0        0      237 2000-03-26 13:12:28.000000 tkmfly-0.1.0b3/tkmfly/_mkwidgets/ReadMe.txt
+-rw-r--r--   0        0        0     6133 2000-10-25 14:02:00.000000 tkmfly-0.1.0b3/tkmfly/_mkwidgets/Scrollbox.tcl
+-rw-r--r--   0        0        0     3872 2000-10-26 12:39:18.000000 tkmfly-0.1.0b3/tkmfly/_mkwidgets/Spinentry.tcl
+-rw-r--r--   0        0        0     6365 2000-10-26 13:09:12.000000 tkmfly-0.1.0b3/tkmfly/_mkwidgets/Statusbar.tcl
+-rw-r--r--   0        0        0    12759 2001-07-08 06:42:04.000000 tkmfly-0.1.0b3/tkmfly/_mkwidgets/Tabcontrol.tcl
+-rw-r--r--   0        0        0     3693 2000-10-26 13:54:28.000000 tkmfly-0.1.0b3/tkmfly/_mkwidgets/Textframe.tcl
+-rw-r--r--   0        0        0    13012 2001-07-06 16:07:24.000000 tkmfly-0.1.0b3/tkmfly/_mkwidgets/Toolbar.tcl
+-rw-r--r--   0        0        0     4221 2000-03-20 12:51:28.000000 tkmfly-0.1.0b3/tkmfly/_mkwidgets/Tooltip.tcl
+-rw-r--r--   0        0        0    35987 2001-07-06 16:09:24.000000 tkmfly-0.1.0b3/tkmfly/_mkwidgets/Treecontrol.tcl
+-rw-r--r--   0        0        0     3744 2001-07-11 12:36:34.000000 tkmfly-0.1.0b3/tkmfly/_mkwidgets/Window.tcl
+-rw-r--r--   0        0        0     2236 2023-05-19 12:56:40.594230 tkmfly-0.1.0b3/tkmfly/core.py
+-rw-r--r--   0        0        0     1233 2023-05-26 23:09:11.462165 tkmfly-0.1.0b3/tkmfly/datefield/__init__.py
+-rw-r--r--   0        0        0     2576 2023-05-26 23:09:11.811654 tkmfly-0.1.0b3/tkmfly/datefield/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    12619 2023-05-26 23:09:11.812654 tkmfly-0.1.0b3/tkmfly/datefield/__pycache__/pkgIndex.cpython-311.pyc
+-rw-r--r--   0        0        0    12954 2023-05-26 23:09:11.466673 tkmfly-0.1.0b3/tkmfly/datefield/pkgIndex.py
+-rw-r--r--   0        0        0     5339 2023-05-26 23:12:13.060020 tkmfly-0.1.0b3/tkmfly/history/__init__.py
+-rw-r--r--   0        0        0     8854 2023-05-26 23:19:59.494590 tkmfly-0.1.0b3/tkmfly/history/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3351 2023-05-26 23:11:33.122621 tkmfly-0.1.0b3/tkmfly/history/__pycache__/pkgIndex.cpython-311.pyc
+-rw-r--r--   0        0        0     3317 2023-05-26 23:10:48.026539 tkmfly-0.1.0b3/tkmfly/history/pkgIndex.py
+-rw-r--r--   0        0        0      569 2023-05-28 09:40:18.309311 tkmfly-0.1.0b3/tkmfly/mdi.py
+-rw-r--r--   0        0        0    18968 2023-05-28 09:45:28.407537 tkmfly-0.1.0b3/tkmfly/mkwidgets/__init__.py
+-rw-r--r--   0        0        0    19467 2023-05-28 09:45:28.577648 tkmfly-0.1.0b3/tkmfly/mkwidgets/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2337 2023-05-28 09:49:47.865964 tkmfly-0.1.0b3/tkmfly/mkwidgets/__pycache__/calendar.cpython-311.pyc
+-rw-r--r--   0        0        0     2451 2023-05-28 09:45:28.580652 tkmfly-0.1.0b3/tkmfly/mkwidgets/__pycache__/document.cpython-311.pyc
+-rw-r--r--   0        0        0     8657 2023-05-28 09:45:28.582646 tkmfly-0.1.0b3/tkmfly/mkwidgets/__pycache__/toolbar.cpython-311.pyc
+-rw-r--r--   0        0        0     1742 2023-05-28 09:45:28.584152 tkmfly-0.1.0b3/tkmfly/mkwidgets/__pycache__/window.cpython-311.pyc
+-rw-r--r--   0        0        0      830 2023-05-28 09:49:47.748095 tkmfly-0.1.0b3/tkmfly/mkwidgets/calendar.py
+-rw-r--r--   0        0        0     1143 2023-05-28 09:45:28.422048 tkmfly-0.1.0b3/tkmfly/mkwidgets/document.py
+-rw-r--r--   0        0        0     5645 2023-05-28 09:45:28.417052 tkmfly-0.1.0b3/tkmfly/mkwidgets/toolbar.py
+-rw-r--r--   0        0        0      754 2023-05-28 09:45:28.412537 tkmfly-0.1.0b3/tkmfly/mkwidgets/window.py
+-rw-r--r--   0        0        0      899 2023-05-26 10:17:24.710900 tkmfly-0.1.0b3/tkmfly/notifywindow/__init__.py
+-rw-r--r--   0        0        0     2358 2023-05-26 10:17:25.218284 tkmfly-0.1.0b3/tkmfly/notifywindow/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4177 2023-05-26 10:17:25.219284 tkmfly-0.1.0b3/tkmfly/notifywindow/__pycache__/pkgIndex.cpython-311.pyc
+-rw-r--r--   0        0        0     4128 2023-05-26 10:15:08.058584 tkmfly-0.1.0b3/tkmfly/notifywindow/pkgIndex.py
+-rw-r--r--   0        0        0      676 2023-05-26 23:27:44.237391 tkmfly-0.1.0b3/tkmfly/tkmdi/__init__.py
+-rw-r--r--   0        0        0      933 2023-05-26 23:27:44.393937 tkmfly-0.1.0b3/tkmfly/tkmdi/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0       94 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/activehorztab.gif
+-rw-r--r--   0        0        0       88 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/activeverttab.gif
+-rw-r--r--   0        0        0       72 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/backwards.gif
+-rw-r--r--   0        0        0      111 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/ballstick.gif
+-rw-r--r--   0        0        0     1020 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/ballstick2.gif
+-rw-r--r--   0        0        0      104 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/circle.gif
+-rw-r--r--   0        0        0       61 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/close.gif
+-rw-r--r--   0        0        0      853 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/corner.gif
+-rw-r--r--   0        0        0       97 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/cut.gif
+-rw-r--r--   0        0        0       70 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/down.gif
+-rw-r--r--   0        0        0      135 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/draw.gif
+-rw-r--r--   0        0        0      124 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/end.gif
+-rw-r--r--   0        0        0      120 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/folder.gif
+-rw-r--r--   0        0        0       67 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/horzsep.gif
+-rw-r--r--   0        0        0       79 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/horztab.gif
+-rw-r--r--   0        0        0      255 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/info.gif
+-rw-r--r--   0        0        0       72 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/left.gif
+-rw-r--r--   0        0        0       64 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/maximize.gif
+-rw-r--r--   0        0        0       54 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/minimize.gif
+-rw-r--r--   0        0        0       75 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/minusnode.gif
+-rw-r--r--   0        0        0      105 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/new.gif
+-rw-r--r--   0        0        0       40 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/nothing.gif
+-rw-r--r--   0        0        0      132 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/open.gif
+-rw-r--r--   0        0        0      125 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/openfolder.gif
+-rw-r--r--   0        0        0       76 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/pause.gif
+-rw-r--r--   0        0        0      109 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/play.gif
+-rw-r--r--   0        0        0       79 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/plusnode.gif
+-rw-r--r--   0        0        0       96 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/rect.gif
+-rw-r--r--   0        0        0       70 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/restore.gif
+-rw-r--r--   0        0        0      124 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/rewind.gif
+-rw-r--r--   0        0        0      109 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/right.gif
+-rw-r--r--   0        0        0       93 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/rotate.gif
+-rw-r--r--   0        0        0       91 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/rotz.gif
+-rw-r--r--   0        0        0      115 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/save.gif
+-rw-r--r--   0        0        0      883 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/select.gif
+-rw-r--r--   0        0        0      926 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/sphere.gif
+-rw-r--r--   0        0        0     1236 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/sphere2.gif
+-rw-r--r--   0        0        0      103 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/stick.gif
+-rw-r--r--   0        0        0      611 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/stick2.gif
+-rw-r--r--   0        0        0       75 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/stop.gif
+-rw-r--r--   0        0        0      103 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/surface.gif
+-rw-r--r--   0        0        0       85 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/tk.gif
+-rw-r--r--   0        0        0      920 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/toscreen.gif
+-rw-r--r--   0        0        0      139 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/toselection.gif
+-rw-r--r--   0        0        0      881 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/trans.gif
+-rw-r--r--   0        0        0       79 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/up.gif
+-rw-r--r--   0        0        0       64 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/vertsep.gif
+-rw-r--r--   0        0        0       72 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/verttab.gif
+-rw-r--r--   0        0        0      871 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/wire.gif
+-rw-r--r--   0        0        0      573 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/wire2.gif
+-rw-r--r--   0        0        0       91 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/zclip.gif
+-rw-r--r--   0        0        0      924 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/zoom.gif
+-rw-r--r--   0        0        0      916 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/zoomToArea.gif
+-rw-r--r--   0        0        0    10684 2023-05-27 00:03:28.083145 tkmfly-0.1.0b3/tkmfly/tkmdi/Widgets/__pycache__/FlatButtons.cpython-311.pyc
+-rw-r--r--   0        0        0      171 2023-05-26 23:27:44.397534 tkmfly-0.1.0b3/tkmfly/tkmdi/Widgets/__pycache__/iconPath.cpython-311.pyc
+-rw-r--r--   0        0        0    40355 2023-05-26 23:27:44.899919 tkmfly-0.1.0b3/tkmfly/tkmdi/Widgets/__pycache__/MDI.cpython-311.pyc
+-rw-r--r--   0        0        0     6988 2023-05-27 00:03:28.076605 tkmfly-0.1.0b3/tkmfly/tkmdi/Widgets/__pycache__/ProgressBar.cpython-311.pyc
+-rw-r--r--   0        0        0    14492 2023-05-27 00:03:28.089807 tkmfly-0.1.0b3/tkmfly/tkmdi/Widgets/__pycache__/Toolbar.cpython-311.pyc
+-rw-r--r--   0        0        0    14971 2023-05-27 00:03:28.096936 tkmfly-0.1.0b3/tkmfly/tkmdi/Widgets/__pycache__/Tree.cpython-311.pyc
+-rw-r--r--   0        0        0     5908 2023-05-26 23:27:44.257384 tkmfly-0.1.0b3/tkmfly/tkmdi/Widgets/FlatButtons.py
+-rw-r--r--   0        0        0       51 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Widgets/iconPath.py
+-rw-r--r--   0        0        0    24007 2023-05-26 23:27:44.247321 tkmfly-0.1.0b3/tkmfly/tkmdi/Widgets/MDI.py
+-rw-r--r--   0        0        0     3170 2015-11-12 22:41:02.000000 tkmfly-0.1.0b3/tkmfly/tkmdi/Widgets/ProgressBar.py
+-rw-r--r--   0        0        0     8636 2023-05-26 23:27:44.238812 tkmfly-0.1.0b3/tkmfly/tkmdi/Widgets/Toolbar.py
+-rw-r--r--   0        0        0     7917 2023-05-26 23:27:44.232887 tkmfly-0.1.0b3/tkmfly/tkmdi/Widgets/Tree.py
+-rw-r--r--   0        0        0     5370 2023-05-20 14:38:16.735308 tkmfly-0.1.0b3/tkmfly/toolbar.py
+-rw-r--r--   0        0        0     2036 2023-05-26 23:06:14.575524 tkmfly-0.1.0b3/tkmfly/tooltip/__init__.py
+-rw-r--r--   0        0        0     3942 2023-05-26 23:06:15.078979 tkmfly-0.1.0b3/tkmfly/tooltip/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    18587 2023-05-26 23:06:15.080978 tkmfly-0.1.0b3/tkmfly/tooltip/__pycache__/pkgIndex.cpython-311.pyc
+-rw-r--r--   0        0        0    19169 2023-05-26 23:05:54.789763 tkmfly-0.1.0b3/tkmfly/tooltip/pkgIndex.py
+-rw-r--r--   0        0        0     6551 2023-05-26 23:55:52.145047 tkmfly-0.1.0b3/tkmfly/ttree.py
+-rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 tkmfly-0.1.0b3/PKG-INFO
```

### Comparing `tkmfly-0.1.0b2/README.md` & `tkmfly-0.1.0b3/README.md`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/core.py` & `tkmfly-0.1.0b3/tkmfly/core.py`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/datefield/__init__.py` & `tkmfly-0.1.0b3/tkmfly/datefield/__init__.py`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/datefield/__pycache__/__init__.cpython-311.pyc` & `tkmfly-0.1.0b3/tkmfly/datefield/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/datefield/__pycache__/pkgIndex.cpython-311.pyc` & `tkmfly-0.1.0b3/tkmfly/datefield/__pycache__/pkgIndex.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/datefield/pkgIndex.py` & `tkmfly-0.1.0b3/tkmfly/datefield/pkgIndex.py`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/history/__init__.py` & `tkmfly-0.1.0b3/tkmfly/history/__init__.py`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/history/__pycache__/__init__.cpython-311.pyc` & `tkmfly-0.1.0b3/tkmfly/history/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/history/__pycache__/pkgIndex.cpython-311.pyc` & `tkmfly-0.1.0b3/tkmfly/history/__pycache__/pkgIndex.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/history/pkgIndex.py` & `tkmfly-0.1.0b3/tkmfly/history/pkgIndex.py`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/notifywindow/__init__.py` & `tkmfly-0.1.0b3/tkmfly/notifywindow/__init__.py`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/notifywindow/__pycache__/__init__.cpython-311.pyc` & `tkmfly-0.1.0b3/tkmfly/notifywindow/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/notifywindow/__pycache__/pkgIndex.cpython-311.pyc` & `tkmfly-0.1.0b3/tkmfly/notifywindow/__pycache__/pkgIndex.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/notifywindow/pkgIndex.py` & `tkmfly-0.1.0b3/tkmfly/notifywindow/pkgIndex.py`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/tkmdi/__init__.py` & `tkmfly-0.1.0b3/tkmfly/tkmdi/__init__.py`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/tkmdi/__pycache__/__init__.cpython-311.pyc` & `tkmfly-0.1.0b3/tkmfly/tkmdi/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/ballstick2.gif` & `tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/ballstick2.gif`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/corner.gif` & `tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/corner.gif`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/select.gif` & `tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/select.gif`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/sphere.gif` & `tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/sphere.gif`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/sphere2.gif` & `tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/sphere2.gif`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/stick2.gif` & `tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/stick2.gif`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/toscreen.gif` & `tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/toscreen.gif`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/trans.gif` & `tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/trans.gif`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/wire.gif` & `tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/wire.gif`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/wire2.gif` & `tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/wire2.gif`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/zoom.gif` & `tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/zoom.gif`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/tkmdi/Icons/zoomToArea.gif` & `tkmfly-0.1.0b3/tkmfly/tkmdi/Icons/zoomToArea.gif`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/tkmdi/Widgets/__pycache__/FlatButtons.cpython-311.pyc` & `tkmfly-0.1.0b3/tkmfly/tkmdi/Widgets/__pycache__/FlatButtons.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/tkmdi/Widgets/__pycache__/MDI.cpython-311.pyc` & `tkmfly-0.1.0b3/tkmfly/tkmdi/Widgets/__pycache__/MDI.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/tkmdi/Widgets/__pycache__/ProgressBar.cpython-311.pyc` & `tkmfly-0.1.0b3/tkmfly/tkmdi/Widgets/__pycache__/ProgressBar.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/tkmdi/Widgets/__pycache__/Toolbar.cpython-311.pyc` & `tkmfly-0.1.0b3/tkmfly/tkmdi/Widgets/__pycache__/Toolbar.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/tkmdi/Widgets/__pycache__/Tree.cpython-311.pyc` & `tkmfly-0.1.0b3/tkmfly/tkmdi/Widgets/__pycache__/Tree.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/tkmdi/Widgets/FlatButtons.py` & `tkmfly-0.1.0b3/tkmfly/tkmdi/Widgets/FlatButtons.py`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/tkmdi/Widgets/MDI.py` & `tkmfly-0.1.0b3/tkmfly/tkmdi/Widgets/MDI.py`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/tkmdi/Widgets/ProgressBar.py` & `tkmfly-0.1.0b3/tkmfly/tkmdi/Widgets/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/tkmdi/Widgets/Toolbar.py` & `tkmfly-0.1.0b3/tkmfly/tkmdi/Widgets/Toolbar.py`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/tkmdi/Widgets/Tree.py` & `tkmfly-0.1.0b3/tkmfly/tkmdi/Widgets/Tree.py`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/tooltip/__init__.py` & `tkmfly-0.1.0b3/tkmfly/tooltip/__init__.py`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/tooltip/__pycache__/__init__.cpython-311.pyc` & `tkmfly-0.1.0b3/tkmfly/tooltip/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/tooltip/__pycache__/pkgIndex.cpython-311.pyc` & `tkmfly-0.1.0b3/tkmfly/tooltip/__pycache__/pkgIndex.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/tooltip/pkgIndex.py` & `tkmfly-0.1.0b3/tkmfly/tooltip/pkgIndex.py`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/tkmfly/ttree.py` & `tkmfly-0.1.0b3/tkmfly/ttree.py`

 * *Files identical despite different names*

### Comparing `tkmfly-0.1.0b2/PKG-INFO` & `tkmfly-0.1.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkmfly
-Version: 0.1.0b2
+Version: 0.1.0b3
 Summary: 
 Author: XiangQinxi
 Author-email: 1379773753@qq.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

