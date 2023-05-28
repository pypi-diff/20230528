# Comparing `tmp/slixmpp-1.8.3.tar.gz` & `tmp/slixmpp-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slixmpp-1.8.3.tar", last modified: Sun Nov 13 10:53:19 2022, max compression
+gzip compressed data, was "slixmpp-1.8.4.tar", last modified: Sun May 28 11:03:13 2023, max compression
```

## Comparing `slixmpp-1.8.3.tar` & `slixmpp-1.8.4.tar`

### file list

```diff
@@ -1,896 +1,877 @@
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.607339 slixmpp-1.8.3/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     7133 2020-12-11 21:20:33.000000 slixmpp-1.8.3/LICENSE
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      215 2016-10-26 15:31:18.000000 slixmpp-1.8.3/MANIFEST.in
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     6234 2022-11-13 10:53:19.607339 slixmpp-1.8.3/PKG-INFO
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     5444 2020-12-11 21:20:33.000000 slixmpp-1.8.3/README.rst
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.373985 slixmpp-1.8.3/docs/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4594 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/Makefile
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.357317 slixmpp-1.8.3/docs/_build/
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.360650 slixmpp-1.8.3/docs/_build/html/
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.373985 slixmpp-1.8.3/docs/_build/html/_images/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    27645 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/_build/html/_images/arch_layers.png
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.383986 slixmpp-1.8.3/docs/_build/html/_static/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     6850 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/_build/html/_static/agogo.css
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1128 2020-03-05 16:54:43.000000 slixmpp-1.8.3/docs/_build/html/_static/alert_info_32.png
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      944 2020-03-05 16:54:43.000000 slixmpp-1.8.3/docs/_build/html/_static/alert_warning_32.png
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     8359 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/_build/html/_static/basic.css
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)       82 2020-03-05 16:54:43.000000 slixmpp-1.8.3/docs/_build/html/_static/bg-page.png
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      165 2020-03-05 16:54:43.000000 slixmpp-1.8.3/docs/_build/html/_static/bullet_orange.png
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3500 2016-10-01 15:14:37.000000 slixmpp-1.8.3/docs/_build/html/_static/comment-bright.png
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3578 2016-10-01 15:14:37.000000 slixmpp-1.8.3/docs/_build/html/_static/comment-close.png
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3445 2016-10-01 15:14:37.000000 slixmpp-1.8.3/docs/_build/html/_static/comment.png
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4040 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/_build/html/_static/default.css
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      347 2016-10-01 15:14:37.000000 slixmpp-1.8.3/docs/_build/html/_static/down-pressed.png
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      347 2016-10-01 15:14:37.000000 slixmpp-1.8.3/docs/_build/html/_static/down.png
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      286 2020-03-05 16:54:43.000000 slixmpp-1.8.3/docs/_build/html/_static/file.png
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.390653 slixmpp-1.8.3/docs/_build/html/_static/fonts/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)   161252 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/_build/html/_static/fonts/OFLGoudyStMTT-Italic.ttf
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)   173520 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/_build/html/_static/fonts/OFLGoudyStMTT.ttf
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)   121352 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/_build/html/_static/fonts/YanoneKaffeesatz-Bold.ttf
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)   129136 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/_build/html/_static/fonts/YanoneKaffeesatz-Light.ttf
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)   128564 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/_build/html/_static/fonts/YanoneKaffeesatz-Regular.ttf
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)   129060 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/_build/html/_static/fonts/YanoneKaffeesatz-Thin.ttf
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     8203 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/_build/html/_static/haiku.css
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    16588 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/_build/html/_static/header.png
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.390653 slixmpp-1.8.3/docs/_build/html/_static/images/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    27645 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/_build/html/_static/images/arch_layers.png
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2812 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/_build/html/_static/images/from_&yet.png
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4081 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/_build/html/_static/ir_black.css
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)       90 2020-03-05 16:54:43.000000 slixmpp-1.8.3/docs/_build/html/_static/minus.png
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4141 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/_build/html/_static/nature.css
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    22763 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/_build/html/_static/noise_dk.png
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)       90 2020-03-05 16:54:43.000000 slixmpp-1.8.3/docs/_build/html/_static/plus.png
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4081 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/_build/html/_static/pygments.css
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     6083 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/_build/html/_static/sphinxdoc.css
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      345 2016-10-01 15:14:37.000000 slixmpp-1.8.3/docs/_build/html/_static/up-pressed.png
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      345 2016-10-01 15:14:37.000000 slixmpp-1.8.3/docs/_build/html/_static/up.png
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.360650 slixmpp-1.8.3/docs/_static/
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.393987 slixmpp-1.8.3/docs/_static/images/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    27645 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/_static/images/arch_layers.png
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2812 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/_static/images/from_&yet.png
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.397320 slixmpp-1.8.3/docs/api/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2741 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/api/api.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)       96 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/api/basexmpp.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      106 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/api/clientxmpp.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      121 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/api/componentxmpp.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      185 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/api/exceptions.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      263 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/api/index.rst
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.407321 slixmpp-1.8.3/docs/api/plugins/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1228 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/api/plugins/index.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      391 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0004.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      302 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0009.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1404 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/api/plugins/xep_0012.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      346 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0013.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      316 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0020.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1359 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/api/plugins/xep_0027.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      787 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/api/plugins/xep_0030.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      330 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0033.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      336 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/api/plugins/xep_0045.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2575 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/api/plugins/xep_0047.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      316 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0049.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      308 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0050.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1180 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/api/plugins/xep_0054.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      304 2022-09-23 09:29:09.000000 slixmpp-1.8.3/docs/api/plugins/xep_0055.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      392 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/api/plugins/xep_0059.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      699 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0060.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1772 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/api/plugins/xep_0065.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      310 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0066.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      342 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0070.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      294 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0071.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1817 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/api/plugins/xep_0077.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      332 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0079.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      304 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0080.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      214 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0082.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      300 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0084.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      326 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0085.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      326 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0086.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      310 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0092.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      198 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/api/plugins/xep_0100.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      184 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0106.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      296 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0107.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      304 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0108.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1769 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/api/plugins/xep_0115.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      296 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0118.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      320 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0122.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1139 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/api/plugins/xep_0128.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      350 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0131.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      204 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0133.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      322 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0152.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1314 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/api/plugins/xep_0153.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      224 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0163.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      304 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0172.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      328 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0184.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      312 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0186.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      310 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0191.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      300 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0196.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      312 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0198.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      296 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0199.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      300 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0202.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      310 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0203.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      326 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0221.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      248 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0222.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      250 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0223.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      296 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0224.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1198 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/api/plugins/xep_0231.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      308 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0235.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      322 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0249.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      210 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0256.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      372 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0257.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      324 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0258.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      308 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0279.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      308 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0280.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      312 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0297.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      364 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0300.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      324 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0308.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      358 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/api/plugins/xep_0313.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      954 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/api/plugins/xep_0319.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      514 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0332.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      302 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0333.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      326 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0334.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      308 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0335.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      324 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0352.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      328 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0353.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      311 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/api/plugins/xep_0356.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      334 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0359.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      401 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/api/plugins/xep_0363.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      294 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0369.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      306 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0377.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      332 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0380.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      306 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0394.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      302 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0403.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      294 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0404.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      292 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0405.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      370 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0421.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      312 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0422.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      314 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0424.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      314 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0425.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      316 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0428.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      326 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0437.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      306 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0439.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      354 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/api/plugins/xep_0441.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      312 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/api/plugins/xep_0444.rst
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.410655 slixmpp-1.8.3/docs/api/stanza/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      106 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/api/stanza/index.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)       96 2020-12-11 21:20:33.000000 slixmpp-1.8.3/docs/api/stanza/iq.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      110 2020-12-11 21:20:33.000000 slixmpp-1.8.3/docs/api/stanza/message.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      100 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/api/stanza/presence.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      105 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/api/stanza/rootstanza.rst
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.410655 slixmpp-1.8.3/docs/api/xmlstream/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      387 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/api/xmlstream/handler.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)       94 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/api/xmlstream/jid.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      601 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/api/xmlstream/matcher.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4323 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/api/xmlstream/stanzabase.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1919 2020-12-11 21:20:33.000000 slixmpp-1.8.3/docs/api/xmlstream/tostring.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      114 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/api/xmlstream/xmlstream.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     5514 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/architecture.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     7614 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/conf.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1731 2020-05-02 14:26:20.000000 slixmpp-1.8.3/docs/differences.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    18324 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/event_index.rst
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.413988 slixmpp-1.8.3/docs/getting_started/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2258 2020-05-02 14:26:20.000000 slixmpp-1.8.3/docs/getting_started/component.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    13814 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/getting_started/echobot.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      179 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/getting_started/index.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     5933 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/getting_started/iq.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     6816 2020-12-11 21:20:33.000000 slixmpp-1.8.3/docs/getting_started/muc.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)       60 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/getting_started/presence.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)       62 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/getting_started/scheduler.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3604 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/getting_started/sendlogout.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1348 2021-02-03 11:48:15.000000 slixmpp-1.8.3/docs/glossary.rst
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.420656 slixmpp-1.8.3/docs/howto/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    25410 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/howto/create_plugin.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)       54 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/howto/features.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     9016 2022-02-16 11:41:52.000000 slixmpp-1.8.3/docs/howto/guide_xep_0030.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      100 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/howto/handlersmatchers.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      243 2022-02-27 23:09:52.000000 slixmpp-1.8.3/docs/howto/index.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2990 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/howto/internal_api.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    91601 2020-12-11 21:20:33.000000 slixmpp-1.8.3/docs/howto/make_plugin_extension_for_message_and_iq.pl.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    87716 2020-12-11 21:20:33.000000 slixmpp-1.8.3/docs/howto/make_plugin_extension_for_message_and_iq.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1679 2022-02-27 23:09:52.000000 slixmpp-1.8.3/docs/howto/remove_process.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)       60 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/howto/sasl.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    11552 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/howto/stanzas.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1913 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/howto/xeps.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    10764 2022-02-27 23:09:52.000000 slixmpp-1.8.3/docs/howto/xmpp_tdg.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     5974 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/index.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)       74 2020-12-11 21:20:33.000000 slixmpp-1.8.3/docs/license.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4513 2016-10-26 15:31:18.000000 slixmpp-1.8.3/docs/make.bat
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      110 2021-07-13 11:33:10.000000 slixmpp-1.8.3/docs/sleekxmpp.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4363 2022-02-16 11:41:52.000000 slixmpp-1.8.3/docs/using_asyncio.rst
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.437324 slixmpp-1.8.3/examples/
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     6462 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/IoT_TestDevice.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     6279 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/adhoc_provider.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     6122 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/adhoc_user.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     4845 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/admin_commands.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     3016 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/confirm_answer.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     4176 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/confirm_ask.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.440657 slixmpp-1.8.3/examples/custom_stanzas/
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     4467 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/custom_stanzas/custom_stanza_provider.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     4418 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/custom_stanzas/custom_stanza_user.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1881 2016-10-26 15:31:18.000000 slixmpp-1.8.3/examples/custom_stanzas/stanza.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     5695 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/disco_browser.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     5477 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/download_avatars.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     3739 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/echo_client.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     3653 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/echo_component.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     4483 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/gtalk_custom_domain.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2851 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/http_over_xmpp.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     4955 2022-03-21 16:42:50.000000 slixmpp-1.8.3/examples/http_upload.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.440657 slixmpp-1.8.3/examples/ibb_transfer/
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     3638 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/ibb_transfer/ibb_receiver.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     4176 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/ibb_transfer/ibb_sender.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     3116 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/mam.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     4030 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/markup.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     3346 2021-02-03 11:48:15.000000 slixmpp-1.8.3/examples/migrate_roster.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     5849 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/mix.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     6327 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/muc.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     3672 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/ping.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     6876 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/pubsub_client.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     4480 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/pubsub_events.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     5137 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/register_account.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     4412 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/roster_browser.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)      754 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/rpc_async.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     1076 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/rpc_client_side.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     1083 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/rpc_server_side.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.440657 slixmpp-1.8.3/examples/s5b_transfer/
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     2793 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/s5b_transfer/s5b_receiver.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     3971 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/s5b_transfer/s5b_sender.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     3527 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/send_client.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     4438 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/set_avatar.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     7209 2021-07-13 11:33:10.000000 slixmpp-1.8.3/examples/thirdparty_auth.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     3204 2020-05-02 15:14:27.000000 slixmpp-1.8.3/examples/user_location.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     3947 2020-05-02 15:14:27.000000 slixmpp-1.8.3/examples/user_tune.py
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     1902 2021-07-13 11:33:10.000000 slixmpp-1.8.3/run_tests.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)       38 2022-11-13 10:53:19.607339 slixmpp-1.8.3/setup.cfg
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     3308 2022-03-21 16:42:50.000000 slixmpp-1.8.3/setup.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.447325 slixmpp-1.8.3/slixmpp/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      994 2022-11-11 17:26:23.000000 slixmpp-1.8.3/slixmpp/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     8890 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/api.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    31808 2022-06-02 11:48:28.000000 slixmpp-1.8.3/slixmpp/basexmpp.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    12665 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/clientxmpp.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4889 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/componentxmpp.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3709 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/exceptions.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.450658 slixmpp-1.8.3/slixmpp/features/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      313 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/features/__init__.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.450658 slixmpp-1.8.3/slixmpp/features/feature_bind/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      349 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/features/feature_bind/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2029 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/features/feature_bind/bind.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      407 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/features/feature_bind/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.450658 slixmpp-1.8.3/slixmpp/features/feature_mechanisms/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      571 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/features/feature_mechanisms/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     8980 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/features/feature_mechanisms/mechanisms.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.453992 slixmpp-1.8.3/slixmpp/features/feature_mechanisms/stanza/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      655 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/features/feature_mechanisms/stanza/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      513 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/features/feature_mechanisms/stanza/abort.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1220 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/features/feature_mechanisms/stanza/auth.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      827 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/features/feature_mechanisms/stanza/challenge.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2369 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/features/feature_mechanisms/stanza/failure.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1201 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/features/feature_mechanisms/stanza/mechanisms.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      825 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/features/feature_mechanisms/stanza/response.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      822 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/features/feature_mechanisms/stanza/success.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.453992 slixmpp-1.8.3/slixmpp/features/feature_preapproval/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      391 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/features/feature_preapproval/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1208 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/features/feature_preapproval/preapproval.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      407 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/features/feature_preapproval/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.453992 slixmpp-1.8.3/slixmpp/features/feature_rosterver/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      379 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/features/feature_rosterver/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1135 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/features/feature_rosterver/rosterver.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      400 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/features/feature_rosterver/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.453992 slixmpp-1.8.3/slixmpp/features/feature_sasl2mechanisms/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      626 2022-08-29 18:37:42.000000 slixmpp-1.8.3/slixmpp/features/feature_sasl2mechanisms/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     9052 2022-08-29 18:45:14.000000 slixmpp-1.8.3/slixmpp/features/feature_sasl2mechanisms/mechanisms.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.457326 slixmpp-1.8.3/slixmpp/features/feature_sasl2mechanisms/stanza/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      725 2022-08-29 18:38:44.000000 slixmpp-1.8.3/slixmpp/features/feature_sasl2mechanisms/stanza/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      501 2022-08-29 18:39:06.000000 slixmpp-1.8.3/slixmpp/features/feature_sasl2mechanisms/stanza/abort.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1207 2022-08-29 18:39:21.000000 slixmpp-1.8.3/slixmpp/features/feature_sasl2mechanisms/stanza/auth.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      815 2022-08-29 18:39:38.000000 slixmpp-1.8.3/slixmpp/features/feature_sasl2mechanisms/stanza/challenge.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2357 2022-08-29 18:39:52.000000 slixmpp-1.8.3/slixmpp/features/feature_sasl2mechanisms/stanza/failure.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1189 2022-08-29 18:40:19.000000 slixmpp-1.8.3/slixmpp/features/feature_sasl2mechanisms/stanza/mechanisms.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      813 2022-08-29 18:41:12.000000 slixmpp-1.8.3/slixmpp/features/feature_sasl2mechanisms/stanza/response.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      811 2022-08-29 18:42:14.000000 slixmpp-1.8.3/slixmpp/features/feature_sasl2mechanisms/stanza/success.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.457326 slixmpp-1.8.3/slixmpp/features/feature_session/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      367 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/features/feature_session/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1641 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/features/feature_session/session.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      821 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/features/feature_session/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.457326 slixmpp-1.8.3/slixmpp/features/feature_starttls/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      366 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/features/feature_starttls/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1362 2022-04-05 19:56:37.000000 slixmpp-1.8.3/slixmpp/features/feature_starttls/stanza.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2094 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/features/feature_starttls/starttls.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    12830 2022-09-23 09:29:09.000000 slixmpp-1.8.3/slixmpp/jid.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.467326 slixmpp-1.8.3/slixmpp/plugins/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4826 2022-09-23 09:29:09.000000 slixmpp-1.8.3/slixmpp/plugins/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    12027 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/plugins/base.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4649 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/gmail_notify.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.467326 slixmpp-1.8.3/slixmpp/plugins/google/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1185 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/google/__init__.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.467326 slixmpp-1.8.3/slixmpp/plugins/google/auth/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      275 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/google/auth/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1473 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/google/auth/auth.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1440 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/google/auth/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.467326 slixmpp-1.8.3/slixmpp/plugins/google/gmail/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      281 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/google/gmail/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2822 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/google/gmail/notifications.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2743 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/google/gmail/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.467326 slixmpp-1.8.3/slixmpp/plugins/google/nosave/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      283 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/google/nosave/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2573 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/google/nosave/nosave.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1439 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/google/nosave/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.467326 slixmpp-1.8.3/slixmpp/plugins/google/settings/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      291 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/google/settings/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1842 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/google/settings/settings.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3417 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/google/settings/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.467326 slixmpp-1.8.3/slixmpp/plugins/xep_0004/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      422 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0004/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1630 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0004/dataforms.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.470660 slixmpp-1.8.3/slixmpp/plugins/xep_0004/stanza/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      299 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0004/stanza/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     6122 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0004/stanza/field.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     8619 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0004/stanza/form.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.470660 slixmpp-1.8.3/slixmpp/plugins/xep_0009/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      432 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0009/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     5745 2022-02-08 20:42:25.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0009/binding.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    26798 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0009/remote.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     8601 2022-02-08 20:42:25.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0009/rpc.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.470660 slixmpp-1.8.3/slixmpp/plugins/xep_0009/stanza/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1585 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0009/stanza/RPC.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      264 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0009/stanza/__init__.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.473994 slixmpp-1.8.3/slixmpp/plugins/xep_0012/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      367 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0012/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     6076 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0012/last_activity.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      711 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0012/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.473994 slixmpp-1.8.3/slixmpp/plugins/xep_0013/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      354 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0013/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3797 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0013/offline.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1284 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0013/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.473994 slixmpp-1.8.3/slixmpp/plugins/xep_0016/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      400 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0016/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4398 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0016/privacy.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3068 2016-10-26 15:31:18.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0016/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.473994 slixmpp-1.8.3/slixmpp/plugins/xep_0020/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      423 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0020/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      996 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0020/feature_negotiation.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      391 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0020/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.477327 slixmpp-1.8.3/slixmpp/plugins/xep_0027/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      362 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0027/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     6355 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0027/gpg.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1318 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0027/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.477327 slixmpp-1.8.3/slixmpp/plugins/xep_0030/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      468 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0030/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    31625 2022-09-23 09:29:09.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0030/disco.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.477327 slixmpp-1.8.3/slixmpp/plugins/xep_0030/stanza/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      292 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0030/stanza/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    10456 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0030/stanza/info.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4645 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0030/stanza/items.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    17152 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0030/static.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.480661 slixmpp-1.8.3/slixmpp/plugins/xep_0033/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      413 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0033/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      920 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0033/addresses.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3652 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0033/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.480661 slixmpp-1.8.3/slixmpp/plugins/xep_0045/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      410 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0045/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    27696 2022-07-12 11:32:44.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0045/muc.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     7576 2021-12-28 17:35:33.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0045/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.480661 slixmpp-1.8.3/slixmpp/plugins/xep_0047/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      463 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0047/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     8175 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0047/ibb.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1819 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0047/stanza.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     6330 2022-02-08 20:42:25.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0047/stream.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.483994 slixmpp-1.8.3/slixmpp/plugins/xep_0048/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      377 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0048/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2340 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0048/bookmarks.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1940 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0048/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.483994 slixmpp-1.8.3/slixmpp/plugins/xep_0049/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      367 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0049/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1762 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0049/private_storage.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      360 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0049/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.487328 slixmpp-1.8.3/slixmpp/plugins/xep_0050/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      354 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0050/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    22530 2022-11-11 17:26:23.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0050/adhoc.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     5658 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0050/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.487328 slixmpp-1.8.3/slixmpp/plugins/xep_0054/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      361 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0054/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    15166 2018-04-23 21:52:28.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0054/stanza.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     5148 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0054/vcard_temp.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.490662 slixmpp-1.8.3/slixmpp/plugins/xep_0055/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      107 2022-09-23 09:29:09.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0055/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2804 2022-09-23 09:29:09.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0055/search.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      231 2022-09-23 09:29:09.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0055/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.490662 slixmpp-1.8.3/slixmpp/plugins/xep_0059/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      371 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0059/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     8098 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0059/rsm.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3816 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0059/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.490662 slixmpp-1.8.3/slixmpp/plugins/xep_0060/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      347 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0060/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    21323 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0060/pubsub.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.493995 slixmpp-1.8.3/slixmpp/plugins/xep_0060/stanza/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      386 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0060/stanza/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      770 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0060/stanza/base.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     7543 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0060/stanza/pubsub.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3033 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0060/stanza/pubsub_errors.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4208 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0060/stanza/pubsub_event.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3919 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0060/stanza/pubsub_owner.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.497329 slixmpp-1.8.3/slixmpp/plugins/xep_0065/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      240 2016-10-26 15:31:18.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0065/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    10313 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0065/proxy.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     7670 2018-08-07 21:35:31.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0065/socks5.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1272 2016-10-26 15:31:18.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0065/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.497329 slixmpp-1.8.3/slixmpp/plugins/xep_0066/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      405 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0066/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4818 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0066/oob.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      610 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0066/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.497329 slixmpp-1.8.3/slixmpp/plugins/xep_0070/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      339 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0070/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2573 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0070/confirm.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      375 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0070/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.497329 slixmpp-1.8.3/slixmpp/plugins/xep_0071/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      356 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0071/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2769 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0071/stanza.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      777 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0071/xhtml_im.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.500663 slixmpp-1.8.3/slixmpp/plugins/xep_0077/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      375 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0077/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     8975 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0077/register.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2137 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0077/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.500663 slixmpp-1.8.3/slixmpp/plugins/xep_0078/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      415 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0078/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4290 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0078/legacyauth.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1143 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0078/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.500663 slixmpp-1.8.3/slixmpp/plugins/xep_0079/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      475 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0079/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2540 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0079/amp.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2589 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0079/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.500663 slixmpp-1.8.3/slixmpp/plugins/xep_0080/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      361 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0080/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4051 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0080/geoloc.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     7983 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0080/stanza.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     6923 2022-07-12 11:43:12.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0082.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.503996 slixmpp-1.8.3/slixmpp/plugins/xep_0084/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      406 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0084/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3986 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0084/avatar.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2773 2022-09-23 09:29:09.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0084/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.503996 slixmpp-1.8.3/slixmpp/plugins/xep_0085/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      360 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0085/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1638 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0085/chat_states.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2036 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0085/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.503996 slixmpp-1.8.3/slixmpp/plugins/xep_0086/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      365 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0086/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1439 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0086/legacy_error.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3077 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0086/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.503996 slixmpp-1.8.3/slixmpp/plugins/xep_0091/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      409 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0091/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      710 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0091/legacy_delay.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1200 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0091/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.507330 slixmpp-1.8.3/slixmpp/plugins/xep_0092/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      400 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0092/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1152 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0092/stanza.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2494 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0092/version.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.507330 slixmpp-1.8.3/slixmpp/plugins/xep_0095/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      405 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0095/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      623 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0095/stanza.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     7300 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0095/stream_initiation.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.507330 slixmpp-1.8.3/slixmpp/plugins/xep_0096/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      403 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0096/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1764 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0096/file_transfer.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1256 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0096/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.507330 slixmpp-1.8.3/slixmpp/plugins/xep_0100/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      145 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0100/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     9137 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0100/gateway.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      584 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0106.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.507330 slixmpp-1.8.3/slixmpp/plugins/xep_0107/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      403 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0107/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2197 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0107/stanza.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1952 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0107/user_mood.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.510663 slixmpp-1.8.3/slixmpp/plugins/xep_0108/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      411 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0108/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3458 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0108/stanza.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1965 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0108/user_activity.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.510663 slixmpp-1.8.3/slixmpp/plugins/xep_0115/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      413 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0115/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    13457 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0115/caps.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      431 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0115/stanza.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     5291 2022-09-23 09:29:09.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0115/static.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.510663 slixmpp-1.8.3/slixmpp/plugins/xep_0118/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      403 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0118/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      644 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0118/stanza.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2364 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0118/user_tune.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.510663 slixmpp-1.8.3/slixmpp/plugins/xep_0122/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      199 2016-10-26 15:31:18.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0122/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      533 2016-10-26 15:31:18.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0122/data_validation.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2806 2020-12-11 21:20:33.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0122/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.513997 slixmpp-1.8.3/slixmpp/plugins/xep_0128/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      375 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0128/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3301 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0128/extended_disco.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1971 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0128/static.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.513997 slixmpp-1.8.3/slixmpp/plugins/xep_0131/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      400 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0131/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1276 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0131/headers.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1531 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0131/stanza.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1881 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0133.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4149 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0138.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.513997 slixmpp-1.8.3/slixmpp/plugins/xep_0152/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      410 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0152/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2164 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0152/reachability.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      686 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0152/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.513997 slixmpp-1.8.3/slixmpp/plugins/xep_0153/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      369 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0153/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      736 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0153/stanza.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     6400 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0153/vcard_avatar.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4628 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0163.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.513997 slixmpp-1.8.3/slixmpp/plugins/xep_0172/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      403 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0172/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1819 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0172/stanza.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1990 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0172/user_nick.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.513997 slixmpp-1.8.3/slixmpp/plugins/xep_0184/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      373 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0184/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3862 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0184/receipt.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2008 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0184/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.517331 slixmpp-1.8.3/slixmpp/plugins/xep_0186/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      421 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0186/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1190 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0186/invisible_command.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      508 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0186/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.517331 slixmpp-1.8.3/slixmpp/plugins/xep_0191/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      375 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0191/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2726 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0191/blocking.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1278 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0191/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.517331 slixmpp-1.8.3/slixmpp/plugins/xep_0196/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      407 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0196/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      499 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0196/stanza.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2810 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0196/user_gaming.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.517331 slixmpp-1.8.3/slixmpp/plugins/xep_0198/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      607 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0198/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3525 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0198/stanza.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    12148 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0198/stream_management.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.520664 slixmpp-1.8.3/slixmpp/plugins/xep_0199/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      332 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0199/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     6995 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0199/ping.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      735 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0199/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.520664 slixmpp-1.8.3/slixmpp/plugins/xep_0202/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      400 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0202/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3234 2022-07-12 11:43:12.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0202/stanza.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2587 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0202/time.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.520664 slixmpp-1.8.3/slixmpp/plugins/xep_0203/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      396 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0203/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1076 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0203/delay.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1343 2022-07-12 11:43:12.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0203/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.520664 slixmpp-1.8.3/slixmpp/plugins/xep_0221/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      401 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0221/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      636 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0221/media.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      939 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0221/stanza.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3649 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0222.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3643 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0223.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.523998 slixmpp-1.8.3/slixmpp/plugins/xep_0224/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      404 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0224/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2142 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0224/attention.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      923 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0224/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.523998 slixmpp-1.8.3/slixmpp/plugins/xep_0231/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      387 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0231/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     5639 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0231/bob.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      943 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0231/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.523998 slixmpp-1.8.3/slixmpp/plugins/xep_0235/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      396 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0235/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      779 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0235/oauth.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2840 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0235/stanza.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      511 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0242.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.527331 slixmpp-1.8.3/slixmpp/plugins/xep_0249/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      343 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0249/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2674 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0249/invite.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1141 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0249/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.527331 slixmpp-1.8.3/slixmpp/plugins/xep_0256/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      332 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0256/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      646 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0256/last_activity_presence.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2244 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0256.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.527331 slixmpp-1.8.3/slixmpp/plugins/xep_0257/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      493 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0257/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2467 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0257/client_cert_management.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2520 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0257/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.527331 slixmpp-1.8.3/slixmpp/plugins/xep_0258/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      572 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0258/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1213 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0258/security_labels.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3749 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0258/stanza.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      479 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0270.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.530665 slixmpp-1.8.3/slixmpp/plugins/xep_0279/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      400 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0279/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1109 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0279/ipcheck.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      626 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0279/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.530665 slixmpp-1.8.3/slixmpp/plugins/xep_0280/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      503 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0280/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2888 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0280/carbons.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1521 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0280/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.530665 slixmpp-1.8.3/slixmpp/plugins/xep_0297/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      404 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0297/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2057 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0297/forwarded.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      971 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0297/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.530665 slixmpp-1.8.3/slixmpp/plugins/xep_0300/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      377 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0300/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2611 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0300/hash.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      870 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0300/stanza.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      523 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0302.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.530665 slixmpp-1.8.3/slixmpp/plugins/xep_0308/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      357 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0308/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1375 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0308/correction.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      362 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0308/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.533999 slixmpp-1.8.3/slixmpp/plugins/xep_0313/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      417 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0313/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     9499 2022-02-27 23:09:52.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0313/mam.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     9974 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0313/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.533999 slixmpp-1.8.3/slixmpp/plugins/xep_0319/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      394 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0319/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2980 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0319/idle.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      685 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0319/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.533999 slixmpp-1.8.3/slixmpp/plugins/xep_0323/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      506 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0323/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    10004 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0323/device.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    30142 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0323/sensordata.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.533999 slixmpp-1.8.3/slixmpp/plugins/xep_0323/stanza/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      367 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0323/stanza/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      348 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0323/stanza/base.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    25419 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0323/stanza/sensordata.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2054 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0323/timerreset.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.537332 slixmpp-1.8.3/slixmpp/plugins/xep_0325/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      503 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0325/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    22903 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0325/control.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4501 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0325/device.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.537332 slixmpp-1.8.3/slixmpp/plugins/xep_0325/stanza/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      364 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0325/stanza/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      348 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0325/stanza/base.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    16180 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0325/stanza/control.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.540666 slixmpp-1.8.3/slixmpp/plugins/xep_0332/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      431 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0332/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     5586 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0332/http.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.540666 slixmpp-1.8.3/slixmpp/plugins/xep_0332/stanza/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      446 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0332/stanza/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      740 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0332/stanza/data.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2187 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0332/stanza/request.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2185 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0332/stanza/response.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.540666 slixmpp-1.8.3/slixmpp/plugins/xep_0333/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      374 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0333/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2873 2022-05-28 09:36:38.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0333/markers.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      726 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0333/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.540666 slixmpp-1.8.3/slixmpp/plugins/xep_0334/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      386 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0334/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      786 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0334/hints.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      741 2016-10-26 15:31:18.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0334/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.540666 slixmpp-1.8.3/slixmpp/plugins/xep_0335/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      401 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0335/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      578 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0335/json_containers.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      616 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0335/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.544000 slixmpp-1.8.3/slixmpp/plugins/xep_0352/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      384 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0352/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2111 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0352/csi.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      806 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0352/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.544000 slixmpp-1.8.3/slixmpp/plugins/xep_0353/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      379 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0353/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3660 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0353/jingle_message.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1504 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0353/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.544000 slixmpp-1.8.3/slixmpp/plugins/xep_0356/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      237 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0356/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4692 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0356/privilege.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1273 2022-07-12 11:32:44.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0356/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.544000 slixmpp-1.8.3/slixmpp/plugins/xep_0359/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      352 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0359/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      693 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0359/stanza.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      559 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0359/stanzaid.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.544000 slixmpp-1.8.3/slixmpp/plugins/xep_0363/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      453 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0363/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     7838 2022-09-23 09:29:09.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0363/http_upload.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1136 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0363/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.547333 slixmpp-1.8.3/slixmpp/plugins/xep_0369/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      352 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0369/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    10921 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0369/mix_core.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2632 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0369/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.547333 slixmpp-1.8.3/slixmpp/plugins/xep_0377/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      347 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0377/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1062 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0377/spam_reporting.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1866 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0377/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.547333 slixmpp-1.8.3/slixmpp/plugins/xep_0380/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      363 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0380/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2137 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0380/eme.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      377 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0380/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.547333 slixmpp-1.8.3/slixmpp/plugins/xep_0382/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      351 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0382/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      873 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0382/spoiler.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      486 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0382/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.550667 slixmpp-1.8.3/slixmpp/plugins/xep_0394/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      401 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0394/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     5858 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0394/markup.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3177 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0394/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.550667 slixmpp-1.8.3/slixmpp/plugins/xep_0403/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      356 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0403/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1155 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0403/mix_presence.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      792 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0403/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.550667 slixmpp-1.8.3/slixmpp/plugins/xep_0404/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      362 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0404/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3321 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0404/mix_anon.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      940 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0404/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.550667 slixmpp-1.8.3/slixmpp/plugins/xep_0405/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      351 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0405/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3882 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0405/mix_pam.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1328 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0405/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.550667 slixmpp-1.8.3/slixmpp/plugins/xep_0421/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      366 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0421/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1053 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0421/occupant_id.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1239 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0421/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.554000 slixmpp-1.8.3/slixmpp/plugins/xep_0422/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      353 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0422/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      741 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0422/fastening.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      912 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0422/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.554000 slixmpp-1.8.3/slixmpp/plugins/xep_0424/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      354 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0424/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2474 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0424/retraction.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      821 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0424/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.554000 slixmpp-1.8.3/slixmpp/plugins/xep_0425/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      354 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0425/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1677 2022-02-08 20:42:25.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0425/moderation.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1232 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0425/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.554000 slixmpp-1.8.3/slixmpp/plugins/xep_0428/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      352 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0428/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      541 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0428/fallback.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      491 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0428/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.554000 slixmpp-1.8.3/slixmpp/plugins/xep_0437/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      276 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0437/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1986 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0437/rai.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1120 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0437/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.557334 slixmpp-1.8.3/slixmpp/plugins/xep_0439/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      357 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0439/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4243 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0439/quickresponse.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      938 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0439/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.557334 slixmpp-1.8.3/slixmpp/plugins/xep_0441/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      377 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0441/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2407 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0441/mam_prefs.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2510 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0441/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.557334 slixmpp-1.8.3/slixmpp/plugins/xep_0444/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      282 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0444/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2012 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0444/reactions.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1699 2022-09-23 09:29:09.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0444/stanza.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.557334 slixmpp-1.8.3/slixmpp/plugins/xep_0454/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     5289 2022-03-21 16:42:50.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0454/__init__.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.560668 slixmpp-1.8.3/slixmpp/plugins/xep_0461/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      126 2022-09-23 09:29:09.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0461/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1383 2022-09-23 09:29:09.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0461/reply.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1357 2022-09-23 09:29:09.000000 slixmpp-1.8.3/slixmpp/plugins/xep_0461/stanza.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     6540 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/pluginsdict.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)        0 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/py.typed
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.560668 slixmpp-1.8.3/slixmpp/roster/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      283 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/roster/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    20424 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/roster/item.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     7098 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/roster/multi.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    11677 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/roster/single.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.564001 slixmpp-1.8.3/slixmpp/stanza/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      578 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/stanza/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1008 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/stanza/atom.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     6071 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/stanza/error.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      593 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/stanza/handshake.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      341 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/stanza/htmlim.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     9744 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/stanza/iq.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     6839 2022-06-02 11:48:28.000000 slixmpp-1.8.3/slixmpp/stanza/message.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     5471 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/stanza/presence.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3150 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/stanza/rootstanza.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4627 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/stanza/roster.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      350 2022-04-05 16:14:52.000000 slixmpp-1.8.3/slixmpp/stanza/starttls.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3249 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/stanza/stream_error.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1334 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/stanza/stream_features.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)   171762 2022-08-20 16:29:48.000000 slixmpp-1.8.3/slixmpp/stringprep.c
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3499 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/stringprep.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2432 2016-10-26 15:31:18.000000 slixmpp-1.8.3/slixmpp/stringprep.pyx
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.567335 slixmpp-1.8.3/slixmpp/test/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      321 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/test/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1913 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/test/integration.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4721 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/test/livesocket.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     6774 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/test/mocksocket.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    30299 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/test/slixtest.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.567335 slixmpp-1.8.3/slixmpp/thirdparty/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      138 2022-07-12 11:43:12.000000 slixmpp-1.8.3/slixmpp/thirdparty/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    35683 2016-10-26 15:31:18.000000 slixmpp-1.8.3/slixmpp/thirdparty/gnupg.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2942 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/thirdparty/orderedset.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1823 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/types.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.570669 slixmpp-1.8.3/slixmpp/util/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      496 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/util/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4708 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/util/cache.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3103 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/util/misc_ops.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.570669 slixmpp-1.8.3/slixmpp/util/sasl/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      391 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/util/sasl/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     5488 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/util/sasl/client.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    17279 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/util/sasl/mechanisms.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4283 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/util/stringprep_profiles.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      303 2022-11-12 20:39:31.000000 slixmpp-1.8.3/slixmpp/version.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.574002 slixmpp-1.8.3/slixmpp/xmlstream/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      593 2022-01-02 21:37:53.000000 slixmpp-1.8.3/slixmpp/xmlstream/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     6563 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/xmlstream/cert.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.577336 slixmpp-1.8.3/slixmpp/xmlstream/handler/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      599 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/xmlstream/handler/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2991 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/xmlstream/handler/base.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3373 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/xmlstream/handler/callback.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2346 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/xmlstream/handler/collector.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3567 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/xmlstream/handler/coroutine_callback.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3218 2021-12-14 16:10:08.000000 slixmpp-1.8.3/slixmpp/xmlstream/handler/waiter.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1087 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/xmlstream/handler/xmlcallback.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      849 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/xmlstream/handler/xmlwaiter.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.580669 slixmpp-1.8.3/slixmpp/xmlstream/matcher/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      587 2021-07-13 11:33:10.000000 slixmpp-1.8.3/slixmpp/xmlstream/matcher/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      795 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/xmlstream/matcher/base.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      798 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/xmlstream/matcher/id.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1561 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/xmlstream/matcher/idsender.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1113 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/xmlstream/matcher/many.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1636 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/xmlstream/matcher/stanzapath.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3870 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/xmlstream/matcher/xmlmask.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1255 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/xmlstream/matcher/xpath.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    12064 2022-09-23 09:29:09.000000 slixmpp-1.8.3/slixmpp/xmlstream/resolver.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    61335 2022-04-05 17:38:16.000000 slixmpp-1.8.3/slixmpp/xmlstream/stanzabase.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     6637 2021-07-16 19:38:52.000000 slixmpp-1.8.3/slixmpp/xmlstream/tostring.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    56767 2022-11-12 20:36:07.000000 slixmpp-1.8.3/slixmpp/xmlstream/xmlstream.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.450658 slixmpp-1.8.3/slixmpp.egg-info/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     6234 2022-11-13 10:53:19.000000 slixmpp-1.8.3/slixmpp.egg-info/PKG-INFO
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    25137 2022-11-13 10:53:19.000000 slixmpp-1.8.3/slixmpp.egg-info/SOURCES.txt
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)        1 2022-11-13 10:53:19.000000 slixmpp-1.8.3/slixmpp.egg-info/dependency_links.txt
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      187 2022-11-13 10:53:19.000000 slixmpp-1.8.3/slixmpp.egg-info/requires.txt
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3332 2022-11-13 10:53:19.000000 slixmpp-1.8.3/slixmpp.egg-info/top_level.txt
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2022-11-13 10:53:19.607339 slixmpp-1.8.3/tests/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)        0 2016-10-26 15:31:18.000000 slixmpp-1.8.3/tests/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1817 2016-10-26 15:31:18.000000 slixmpp-1.8.3/tests/live_multiple_streams.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3419 2016-10-26 15:31:18.000000 slixmpp-1.8.3/tests/live_test.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2343 2020-05-02 14:26:20.000000 slixmpp-1.8.3/tests/test_cache.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2611 2018-10-15 13:51:15.000000 slixmpp-1.8.3/tests/test_events.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    11108 2016-10-26 15:31:18.000000 slixmpp-1.8.3/tests/test_jid.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      493 2020-12-11 21:20:33.000000 slixmpp-1.8.3/tests/test_overall.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4192 2016-10-26 15:31:18.000000 slixmpp-1.8.3/tests/test_plugins.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2686 2020-05-02 14:26:20.000000 slixmpp-1.8.3/tests/test_stanza_base.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    36816 2021-07-13 11:33:10.000000 slixmpp-1.8.3/tests/test_stanza_element.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2516 2018-10-15 13:51:15.000000 slixmpp-1.8.3/tests/test_stanza_error.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4298 2018-10-15 13:51:15.000000 slixmpp-1.8.3/tests/test_stanza_gmail.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2398 2018-10-15 13:51:15.000000 slixmpp-1.8.3/tests/test_stanza_iq.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1867 2021-07-13 11:33:10.000000 slixmpp-1.8.3/tests/test_stanza_message.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2428 2021-07-13 11:33:10.000000 slixmpp-1.8.3/tests/test_stanza_presence.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3009 2018-10-15 13:51:15.000000 slixmpp-1.8.3/tests/test_stanza_roster.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     8144 2020-12-11 21:20:33.000000 slixmpp-1.8.3/tests/test_stanza_xep_0004.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    11638 2016-10-26 15:31:18.000000 slixmpp-1.8.3/tests/test_stanza_xep_0009.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    17641 2018-10-15 13:51:15.000000 slixmpp-1.8.3/tests/test_stanza_xep_0030.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3861 2016-10-26 15:31:18.000000 slixmpp-1.8.3/tests/test_stanza_xep_0033.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4806 2021-02-03 11:48:15.000000 slixmpp-1.8.3/tests/test_stanza_xep_0045.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2563 2016-10-26 15:31:18.000000 slixmpp-1.8.3/tests/test_stanza_xep_0047.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3598 2018-10-15 13:51:15.000000 slixmpp-1.8.3/tests/test_stanza_xep_0050.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1765 2022-09-23 09:29:09.000000 slixmpp-1.8.3/tests/test_stanza_xep_0055.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2882 2018-10-15 13:51:15.000000 slixmpp-1.8.3/tests/test_stanza_xep_0059.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    24602 2021-07-13 11:33:10.000000 slixmpp-1.8.3/tests/test_stanza_xep_0060.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1568 2016-10-26 15:31:18.000000 slixmpp-1.8.3/tests/test_stanza_xep_0085.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     6535 2016-10-26 15:31:18.000000 slixmpp-1.8.3/tests/test_stanza_xep_0122.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      993 2016-10-26 15:31:18.000000 slixmpp-1.8.3/tests/test_stanza_xep_0184.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1524 2018-04-23 21:52:28.000000 slixmpp-1.8.3/tests/test_stanza_xep_0300.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3612 2021-07-13 11:33:10.000000 slixmpp-1.8.3/tests/test_stanza_xep_0313.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    14275 2016-10-26 15:31:18.000000 slixmpp-1.8.3/tests/test_stanza_xep_0323.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     8587 2016-10-26 15:31:18.000000 slixmpp-1.8.3/tests/test_stanza_xep_0325.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1398 2022-07-12 11:32:44.000000 slixmpp-1.8.3/tests/test_stanza_xep_0356.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3598 2020-12-11 21:20:33.000000 slixmpp-1.8.3/tests/test_stanza_xep_0369.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1481 2020-05-24 19:33:49.000000 slixmpp-1.8.3/tests/test_stanza_xep_0377.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1038 2018-04-23 21:52:28.000000 slixmpp-1.8.3/tests/test_stanza_xep_0380.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      887 2021-07-13 11:33:10.000000 slixmpp-1.8.3/tests/test_stanza_xep_0403.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1801 2020-12-11 21:20:33.000000 slixmpp-1.8.3/tests/test_stanza_xep_0405.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      857 2020-05-28 23:02:31.000000 slixmpp-1.8.3/tests/test_stanza_xep_0421.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      876 2020-12-11 21:20:33.000000 slixmpp-1.8.3/tests/test_stanza_xep_0422.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1112 2021-07-13 11:33:10.000000 slixmpp-1.8.3/tests/test_stanza_xep_0424.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1316 2020-12-11 21:20:33.000000 slixmpp-1.8.3/tests/test_stanza_xep_0425.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      650 2020-12-11 21:20:33.000000 slixmpp-1.8.3/tests/test_stanza_xep_0437.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1669 2020-12-11 21:20:33.000000 slixmpp-1.8.3/tests/test_stanza_xep_0439.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2288 2022-03-16 15:11:48.000000 slixmpp-1.8.3/tests/test_stanza_xep_0444.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1332 2022-09-23 09:29:09.000000 slixmpp-1.8.3/tests/test_stanza_xep_0461.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1682 2016-10-26 15:31:18.000000 slixmpp-1.8.3/tests/test_stream.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     6371 2016-10-26 15:31:18.000000 slixmpp-1.8.3/tests/test_stream_exceptions.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1883 2016-10-26 15:31:18.000000 slixmpp-1.8.3/tests/test_stream_filters.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     6455 2018-10-15 13:51:15.000000 slixmpp-1.8.3/tests/test_stream_handlers.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    10512 2019-04-27 11:58:48.000000 slixmpp-1.8.3/tests/test_stream_presence.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     9271 2018-10-15 13:51:15.000000 slixmpp-1.8.3/tests/test_stream_roster.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    20304 2021-07-13 11:33:10.000000 slixmpp-1.8.3/tests/test_stream_xep_0030.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4545 2021-07-13 11:33:10.000000 slixmpp-1.8.3/tests/test_stream_xep_0047.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    40851 2021-07-13 11:33:10.000000 slixmpp-1.8.3/tests/test_stream_xep_0050.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     5608 2022-09-23 09:29:09.000000 slixmpp-1.8.3/tests/test_stream_xep_0055.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    25585 2021-07-13 11:33:10.000000 slixmpp-1.8.3/tests/test_stream_xep_0060.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      984 2016-10-26 15:31:18.000000 slixmpp-1.8.3/tests/test_stream_xep_0066.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4114 2021-07-13 11:33:10.000000 slixmpp-1.8.3/tests/test_stream_xep_0077.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1702 2018-10-15 13:51:15.000000 slixmpp-1.8.3/tests/test_stream_xep_0085.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1906 2016-10-26 15:31:18.000000 slixmpp-1.8.3/tests/test_stream_xep_0092.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    14283 2021-07-13 11:33:10.000000 slixmpp-1.8.3/tests/test_stream_xep_0100.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     3675 2016-10-26 15:31:18.000000 slixmpp-1.8.3/tests/test_stream_xep_0128.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1623 2019-07-20 13:15:56.000000 slixmpp-1.8.3/tests/test_stream_xep_0249.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    11431 2021-07-13 11:33:10.000000 slixmpp-1.8.3/tests/test_stream_xep_0313.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    44827 2020-05-02 14:26:20.000000 slixmpp-1.8.3/tests/test_stream_xep_0323.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    12134 2016-10-26 15:31:18.000000 slixmpp-1.8.3/tests/test_stream_xep_0325.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4029 2022-07-12 11:32:44.000000 slixmpp-1.8.3/tests/test_stream_xep_0356.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     6145 2021-07-13 11:33:10.000000 slixmpp-1.8.3/tests/test_stream_xep_0405.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1507 2022-09-23 09:29:09.000000 slixmpp-1.8.3/tests/test_stream_xep_0461.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4071 2018-10-15 13:51:15.000000 slixmpp-1.8.3/tests/test_tostring.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1203 2022-03-21 16:42:50.000000 slixmpp-1.8.3/tests/test_xep_0454.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.982864 slixmpp-1.8.4/
+-rw-r--r--   0 mathieui  (1000) users      (100)     7133 2023-05-28 11:03:05.000000 slixmpp-1.8.4/LICENSE
+-rw-r--r--   0 mathieui  (1000) users      (100)      215 2023-05-28 11:03:05.000000 slixmpp-1.8.4/MANIFEST.in
+-rw-r--r--   0 mathieui  (1000) users      (100)     6234 2023-05-28 11:03:13.982864 slixmpp-1.8.4/PKG-INFO
+-rw-r--r--   0 mathieui  (1000) users      (100)     5444 2023-05-28 11:03:05.000000 slixmpp-1.8.4/README.rst
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.902864 slixmpp-1.8.4/docs/
+-rw-r--r--   0 mathieui  (1000) users      (100)     4594 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/Makefile
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.892864 slixmpp-1.8.4/docs/_static/
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.902864 slixmpp-1.8.4/docs/_static/images/
+-rw-r--r--   0 mathieui  (1000) users      (100)    27645 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/_static/images/arch_layers.png
+-rw-r--r--   0 mathieui  (1000) users      (100)     2812 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/_static/images/from_&yet.png
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.902864 slixmpp-1.8.4/docs/api/
+-rw-r--r--   0 mathieui  (1000) users      (100)     2741 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/api.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)       96 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/basexmpp.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      106 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/clientxmpp.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      121 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/componentxmpp.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      185 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/exceptions.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      263 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/index.rst
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.912864 slixmpp-1.8.4/docs/api/plugins/
+-rw-r--r--   0 mathieui  (1000) users      (100)     1228 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/index.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      391 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0004.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      302 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0009.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)     1404 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0012.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      346 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0013.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      316 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0020.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)     1359 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0027.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      787 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0030.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      330 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0033.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      336 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0045.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)     2575 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0047.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      316 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0049.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      308 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0050.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)     1180 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0054.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      304 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0055.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      392 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0059.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      699 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0060.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)     1772 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0065.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      310 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0066.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      342 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0070.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      294 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0071.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)     1817 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0077.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      332 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0079.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      304 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0080.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      214 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0082.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      300 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0084.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      326 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0085.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      326 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0086.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      310 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0092.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      198 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0100.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      184 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0106.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      296 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0107.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      304 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0108.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)     1769 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0115.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      296 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0118.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      320 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0122.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)     1139 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0128.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      350 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0131.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      204 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0133.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      322 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0152.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)     1314 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0153.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      224 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0163.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      304 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0172.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      328 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0184.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      312 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0186.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      310 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0191.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      300 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0196.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      312 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0198.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      296 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0199.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      300 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0202.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      310 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0203.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      326 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0221.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      248 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0222.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      250 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0223.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      296 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0224.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)     1198 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0231.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      308 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0235.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      322 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0249.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      210 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0256.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      372 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0257.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      324 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0258.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      308 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0279.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      308 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0280.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      295 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0292.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      312 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0297.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      364 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0300.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      324 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0308.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      358 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0313.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      954 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0319.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      514 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0332.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      302 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0333.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      326 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0334.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      308 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0335.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      324 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0352.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      328 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0353.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      311 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0356.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      334 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0359.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      401 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0363.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      294 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0369.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      306 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0377.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      332 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0380.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      306 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0394.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      302 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0403.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      294 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0404.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      292 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0405.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      370 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0421.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      312 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0422.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      314 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0424.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      314 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0425.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      316 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0428.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      326 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0437.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      306 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0439.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      354 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0441.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      312 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/plugins/xep_0444.rst
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.916197 slixmpp-1.8.4/docs/api/stanza/
+-rw-r--r--   0 mathieui  (1000) users      (100)      106 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/stanza/index.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)       96 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/stanza/iq.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      110 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/stanza/message.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      100 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/stanza/presence.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      105 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/stanza/rootstanza.rst
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.916197 slixmpp-1.8.4/docs/api/xmlstream/
+-rw-r--r--   0 mathieui  (1000) users      (100)      387 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/xmlstream/handler.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)       94 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/xmlstream/jid.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      601 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/xmlstream/matcher.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)     4323 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/xmlstream/stanzabase.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)     1919 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/xmlstream/tostring.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      114 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/api/xmlstream/xmlstream.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)     5514 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/architecture.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)     7614 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/conf.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1731 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/differences.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)    18324 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/event_index.rst
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.916197 slixmpp-1.8.4/docs/getting_started/
+-rw-r--r--   0 mathieui  (1000) users      (100)     2258 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/getting_started/component.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)    13814 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/getting_started/echobot.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      179 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/getting_started/index.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)     5933 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/getting_started/iq.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)     6816 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/getting_started/muc.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)       60 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/getting_started/presence.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)       62 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/getting_started/scheduler.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)     3604 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/getting_started/sendlogout.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)     1348 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/glossary.rst
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.919530 slixmpp-1.8.4/docs/howto/
+-rw-r--r--   0 mathieui  (1000) users      (100)    25410 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/howto/create_plugin.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)       54 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/howto/features.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)     9016 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/howto/guide_xep_0030.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      100 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/howto/handlersmatchers.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)      243 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/howto/index.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)     2990 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/howto/internal_api.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)    91601 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/howto/make_plugin_extension_for_message_and_iq.pl.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)    87716 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/howto/make_plugin_extension_for_message_and_iq.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)     1679 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/howto/remove_process.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)       60 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/howto/sasl.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)    11552 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/howto/stanzas.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)     1913 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/howto/xeps.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)    10764 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/howto/xmpp_tdg.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)     5974 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/index.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)       74 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/license.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)     4513 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/make.bat
+-rw-r--r--   0 mathieui  (1000) users      (100)      110 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/sleekxmpp.rst
+-rw-r--r--   0 mathieui  (1000) users      (100)     4363 2023-05-28 11:03:05.000000 slixmpp-1.8.4/docs/using_asyncio.rst
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.922864 slixmpp-1.8.4/examples/
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     6462 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/IoT_TestDevice.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     6279 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/adhoc_provider.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     6122 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/adhoc_user.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     4845 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/admin_commands.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     3016 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/confirm_answer.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     4176 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/confirm_ask.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.922864 slixmpp-1.8.4/examples/custom_stanzas/
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     4467 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/custom_stanzas/custom_stanza_provider.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     4418 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/custom_stanzas/custom_stanza_user.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1881 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/custom_stanzas/stanza.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     5695 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/disco_browser.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     5477 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/download_avatars.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     3739 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/echo_client.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     3653 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/echo_component.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     4483 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/gtalk_custom_domain.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2851 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/http_over_xmpp.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     4955 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/http_upload.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.922864 slixmpp-1.8.4/examples/ibb_transfer/
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     3638 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/ibb_transfer/ibb_receiver.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     4176 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/ibb_transfer/ibb_sender.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     3116 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/mam.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     4030 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/markup.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     3346 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/migrate_roster.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     5849 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/mix.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     6327 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/muc.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     3672 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/ping.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     6876 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/pubsub_client.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     4480 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/pubsub_events.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     5137 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/register_account.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     4412 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/roster_browser.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)      754 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/rpc_async.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     1076 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/rpc_client_side.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     1083 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/rpc_server_side.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.922864 slixmpp-1.8.4/examples/s5b_transfer/
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     2793 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/s5b_transfer/s5b_receiver.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     3971 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/s5b_transfer/s5b_sender.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     3527 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/send_client.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     4438 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/set_avatar.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     7209 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/thirdparty_auth.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     3204 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/user_location.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     3947 2023-05-28 11:03:05.000000 slixmpp-1.8.4/examples/user_tune.py
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     1902 2023-05-28 11:03:05.000000 slixmpp-1.8.4/run_tests.py
+-rw-r--r--   0 mathieui  (1000) users      (100)       38 2023-05-28 11:03:13.982864 slixmpp-1.8.4/setup.cfg
+-rwxr-xr-x   0 mathieui  (1000) users      (100)     3308 2023-05-28 11:03:05.000000 slixmpp-1.8.4/setup.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.922864 slixmpp-1.8.4/slixmpp/
+-rw-r--r--   0 mathieui  (1000) users      (100)      994 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     8890 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/api.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    31808 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/basexmpp.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    12665 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/clientxmpp.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     5597 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/componentxmpp.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     4882 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/exceptions.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.922864 slixmpp-1.8.4/slixmpp/features/
+-rw-r--r--   0 mathieui  (1000) users      (100)      313 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/features/__init__.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.926197 slixmpp-1.8.4/slixmpp/features/feature_bind/
+-rw-r--r--   0 mathieui  (1000) users      (100)      349 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/features/feature_bind/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2029 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/features/feature_bind/bind.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      407 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/features/feature_bind/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.926197 slixmpp-1.8.4/slixmpp/features/feature_mechanisms/
+-rw-r--r--   0 mathieui  (1000) users      (100)      571 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/features/feature_mechanisms/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     8980 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/features/feature_mechanisms/mechanisms.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.926197 slixmpp-1.8.4/slixmpp/features/feature_mechanisms/stanza/
+-rw-r--r--   0 mathieui  (1000) users      (100)      655 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/features/feature_mechanisms/stanza/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      513 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/features/feature_mechanisms/stanza/abort.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1220 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/features/feature_mechanisms/stanza/auth.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      827 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/features/feature_mechanisms/stanza/challenge.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2369 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/features/feature_mechanisms/stanza/failure.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1201 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/features/feature_mechanisms/stanza/mechanisms.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      825 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/features/feature_mechanisms/stanza/response.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      822 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/features/feature_mechanisms/stanza/success.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.926197 slixmpp-1.8.4/slixmpp/features/feature_preapproval/
+-rw-r--r--   0 mathieui  (1000) users      (100)      391 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/features/feature_preapproval/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1208 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/features/feature_preapproval/preapproval.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      407 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/features/feature_preapproval/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.926197 slixmpp-1.8.4/slixmpp/features/feature_rosterver/
+-rw-r--r--   0 mathieui  (1000) users      (100)      379 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/features/feature_rosterver/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1135 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/features/feature_rosterver/rosterver.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      400 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/features/feature_rosterver/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.926197 slixmpp-1.8.4/slixmpp/features/feature_session/
+-rw-r--r--   0 mathieui  (1000) users      (100)      367 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/features/feature_session/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1641 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/features/feature_session/session.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      821 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/features/feature_session/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.926197 slixmpp-1.8.4/slixmpp/features/feature_starttls/
+-rw-r--r--   0 mathieui  (1000) users      (100)      366 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/features/feature_starttls/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1362 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/features/feature_starttls/stanza.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2094 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/features/feature_starttls/starttls.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    13047 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/jid.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.929531 slixmpp-1.8.4/slixmpp/plugins/
+-rw-r--r--   0 mathieui  (1000) users      (100)     5103 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    12027 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/base.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     4649 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/gmail_notify.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.929531 slixmpp-1.8.4/slixmpp/plugins/google/
+-rw-r--r--   0 mathieui  (1000) users      (100)     1185 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/google/__init__.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.929531 slixmpp-1.8.4/slixmpp/plugins/google/auth/
+-rw-r--r--   0 mathieui  (1000) users      (100)      275 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/google/auth/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1473 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/google/auth/auth.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1440 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/google/auth/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.929531 slixmpp-1.8.4/slixmpp/plugins/google/gmail/
+-rw-r--r--   0 mathieui  (1000) users      (100)      281 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/google/gmail/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2822 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/google/gmail/notifications.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2743 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/google/gmail/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.929531 slixmpp-1.8.4/slixmpp/plugins/google/nosave/
+-rw-r--r--   0 mathieui  (1000) users      (100)      283 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/google/nosave/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2573 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/google/nosave/nosave.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1439 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/google/nosave/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.929531 slixmpp-1.8.4/slixmpp/plugins/google/settings/
+-rw-r--r--   0 mathieui  (1000) users      (100)      291 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/google/settings/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1842 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/google/settings/settings.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3417 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/google/settings/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.929531 slixmpp-1.8.4/slixmpp/plugins/xep_0004/
+-rw-r--r--   0 mathieui  (1000) users      (100)      422 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0004/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1630 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0004/dataforms.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.929531 slixmpp-1.8.4/slixmpp/plugins/xep_0004/stanza/
+-rw-r--r--   0 mathieui  (1000) users      (100)      299 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0004/stanza/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     6122 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0004/stanza/field.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     8619 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0004/stanza/form.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.929531 slixmpp-1.8.4/slixmpp/plugins/xep_0009/
+-rw-r--r--   0 mathieui  (1000) users      (100)      432 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0009/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     5745 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0009/binding.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    26798 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0009/remote.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     8601 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0009/rpc.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.932864 slixmpp-1.8.4/slixmpp/plugins/xep_0009/stanza/
+-rw-r--r--   0 mathieui  (1000) users      (100)     1585 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0009/stanza/RPC.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      264 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0009/stanza/__init__.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.932864 slixmpp-1.8.4/slixmpp/plugins/xep_0012/
+-rw-r--r--   0 mathieui  (1000) users      (100)      367 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0012/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     6076 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0012/last_activity.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      711 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0012/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.932864 slixmpp-1.8.4/slixmpp/plugins/xep_0013/
+-rw-r--r--   0 mathieui  (1000) users      (100)      354 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0013/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3797 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0013/offline.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1284 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0013/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.932864 slixmpp-1.8.4/slixmpp/plugins/xep_0016/
+-rw-r--r--   0 mathieui  (1000) users      (100)      400 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0016/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     4398 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0016/privacy.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3068 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0016/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.932864 slixmpp-1.8.4/slixmpp/plugins/xep_0020/
+-rw-r--r--   0 mathieui  (1000) users      (100)      423 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0020/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      996 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0020/feature_negotiation.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      391 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0020/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.932864 slixmpp-1.8.4/slixmpp/plugins/xep_0027/
+-rw-r--r--   0 mathieui  (1000) users      (100)      362 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0027/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     6416 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0027/gpg.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1318 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0027/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.932864 slixmpp-1.8.4/slixmpp/plugins/xep_0030/
+-rw-r--r--   0 mathieui  (1000) users      (100)      468 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0030/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    31793 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0030/disco.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.932864 slixmpp-1.8.4/slixmpp/plugins/xep_0030/stanza/
+-rw-r--r--   0 mathieui  (1000) users      (100)      292 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0030/stanza/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    10456 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0030/stanza/info.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     4645 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0030/stanza/items.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    17152 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0030/static.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.932864 slixmpp-1.8.4/slixmpp/plugins/xep_0033/
+-rw-r--r--   0 mathieui  (1000) users      (100)      413 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0033/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      920 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0033/addresses.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3652 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0033/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.932864 slixmpp-1.8.4/slixmpp/plugins/xep_0045/
+-rw-r--r--   0 mathieui  (1000) users      (100)      410 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0045/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    27671 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0045/muc.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     7576 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0045/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.936197 slixmpp-1.8.4/slixmpp/plugins/xep_0047/
+-rw-r--r--   0 mathieui  (1000) users      (100)      463 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0047/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     8175 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0047/ibb.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1819 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0047/stanza.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     6330 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0047/stream.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.936197 slixmpp-1.8.4/slixmpp/plugins/xep_0048/
+-rw-r--r--   0 mathieui  (1000) users      (100)      377 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0048/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2340 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0048/bookmarks.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1940 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0048/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.936197 slixmpp-1.8.4/slixmpp/plugins/xep_0049/
+-rw-r--r--   0 mathieui  (1000) users      (100)      367 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0049/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1762 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0049/private_storage.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      360 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0049/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.936197 slixmpp-1.8.4/slixmpp/plugins/xep_0050/
+-rw-r--r--   0 mathieui  (1000) users      (100)      354 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0050/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    22759 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0050/adhoc.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     5658 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0050/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.936197 slixmpp-1.8.4/slixmpp/plugins/xep_0054/
+-rw-r--r--   0 mathieui  (1000) users      (100)      361 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0054/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    15166 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0054/stanza.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     5236 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0054/vcard_temp.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.936197 slixmpp-1.8.4/slixmpp/plugins/xep_0055/
+-rw-r--r--   0 mathieui  (1000) users      (100)      107 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0055/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2804 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0055/search.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      231 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0055/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.936197 slixmpp-1.8.4/slixmpp/plugins/xep_0059/
+-rw-r--r--   0 mathieui  (1000) users      (100)      371 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0059/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     8098 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0059/rsm.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3816 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0059/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.936197 slixmpp-1.8.4/slixmpp/plugins/xep_0060/
+-rw-r--r--   0 mathieui  (1000) users      (100)      347 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0060/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    21323 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0060/pubsub.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.936197 slixmpp-1.8.4/slixmpp/plugins/xep_0060/stanza/
+-rw-r--r--   0 mathieui  (1000) users      (100)      386 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0060/stanza/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      770 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0060/stanza/base.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     7543 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0060/stanza/pubsub.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3033 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0060/stanza/pubsub_errors.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     4208 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0060/stanza/pubsub_event.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3919 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0060/stanza/pubsub_owner.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.936197 slixmpp-1.8.4/slixmpp/plugins/xep_0065/
+-rw-r--r--   0 mathieui  (1000) users      (100)      240 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0065/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    10313 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0065/proxy.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     7670 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0065/socks5.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1272 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0065/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.939531 slixmpp-1.8.4/slixmpp/plugins/xep_0066/
+-rw-r--r--   0 mathieui  (1000) users      (100)      405 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0066/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     4818 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0066/oob.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      610 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0066/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.939531 slixmpp-1.8.4/slixmpp/plugins/xep_0070/
+-rw-r--r--   0 mathieui  (1000) users      (100)      339 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0070/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2573 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0070/confirm.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      375 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0070/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.939531 slixmpp-1.8.4/slixmpp/plugins/xep_0071/
+-rw-r--r--   0 mathieui  (1000) users      (100)      356 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0071/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2769 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0071/stanza.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      777 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0071/xhtml_im.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.939531 slixmpp-1.8.4/slixmpp/plugins/xep_0077/
+-rw-r--r--   0 mathieui  (1000) users      (100)      375 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0077/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     8975 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0077/register.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2137 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0077/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.939531 slixmpp-1.8.4/slixmpp/plugins/xep_0078/
+-rw-r--r--   0 mathieui  (1000) users      (100)      415 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0078/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     4290 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0078/legacyauth.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1143 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0078/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.939531 slixmpp-1.8.4/slixmpp/plugins/xep_0079/
+-rw-r--r--   0 mathieui  (1000) users      (100)      475 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0079/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2540 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0079/amp.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2589 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0079/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.939531 slixmpp-1.8.4/slixmpp/plugins/xep_0080/
+-rw-r--r--   0 mathieui  (1000) users      (100)      361 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0080/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     4051 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0080/geoloc.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     7983 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0080/stanza.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     6923 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0082.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.939531 slixmpp-1.8.4/slixmpp/plugins/xep_0084/
+-rw-r--r--   0 mathieui  (1000) users      (100)      406 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0084/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3986 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0084/avatar.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2773 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0084/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.939531 slixmpp-1.8.4/slixmpp/plugins/xep_0085/
+-rw-r--r--   0 mathieui  (1000) users      (100)      360 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0085/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1638 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0085/chat_states.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2036 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0085/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.939531 slixmpp-1.8.4/slixmpp/plugins/xep_0086/
+-rw-r--r--   0 mathieui  (1000) users      (100)      365 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0086/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1439 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0086/legacy_error.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3077 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0086/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.942864 slixmpp-1.8.4/slixmpp/plugins/xep_0091/
+-rw-r--r--   0 mathieui  (1000) users      (100)      409 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0091/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      710 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0091/legacy_delay.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1200 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0091/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.942864 slixmpp-1.8.4/slixmpp/plugins/xep_0092/
+-rw-r--r--   0 mathieui  (1000) users      (100)      400 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0092/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1152 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0092/stanza.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2494 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0092/version.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.942864 slixmpp-1.8.4/slixmpp/plugins/xep_0095/
+-rw-r--r--   0 mathieui  (1000) users      (100)      405 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0095/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      623 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0095/stanza.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     7300 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0095/stream_initiation.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.942864 slixmpp-1.8.4/slixmpp/plugins/xep_0096/
+-rw-r--r--   0 mathieui  (1000) users      (100)      403 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0096/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1764 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0096/file_transfer.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1256 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0096/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.942864 slixmpp-1.8.4/slixmpp/plugins/xep_0100/
+-rw-r--r--   0 mathieui  (1000) users      (100)      145 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0100/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     9137 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0100/gateway.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      584 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0106.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.942864 slixmpp-1.8.4/slixmpp/plugins/xep_0107/
+-rw-r--r--   0 mathieui  (1000) users      (100)      403 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0107/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2197 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0107/stanza.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1952 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0107/user_mood.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.942864 slixmpp-1.8.4/slixmpp/plugins/xep_0108/
+-rw-r--r--   0 mathieui  (1000) users      (100)      411 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0108/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3458 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0108/stanza.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1965 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0108/user_activity.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.942864 slixmpp-1.8.4/slixmpp/plugins/xep_0115/
+-rw-r--r--   0 mathieui  (1000) users      (100)      413 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0115/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    13463 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0115/caps.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      431 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0115/stanza.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     5291 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0115/static.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.942864 slixmpp-1.8.4/slixmpp/plugins/xep_0118/
+-rw-r--r--   0 mathieui  (1000) users      (100)      403 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0118/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      644 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0118/stanza.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2364 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0118/user_tune.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.942864 slixmpp-1.8.4/slixmpp/plugins/xep_0122/
+-rw-r--r--   0 mathieui  (1000) users      (100)      199 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0122/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      533 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0122/data_validation.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2806 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0122/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.946197 slixmpp-1.8.4/slixmpp/plugins/xep_0128/
+-rw-r--r--   0 mathieui  (1000) users      (100)      375 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0128/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3301 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0128/extended_disco.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1971 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0128/static.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.946197 slixmpp-1.8.4/slixmpp/plugins/xep_0131/
+-rw-r--r--   0 mathieui  (1000) users      (100)      400 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0131/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1276 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0131/headers.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1531 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0131/stanza.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1881 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0133.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     4149 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0138.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.946197 slixmpp-1.8.4/slixmpp/plugins/xep_0152/
+-rw-r--r--   0 mathieui  (1000) users      (100)      410 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0152/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2164 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0152/reachability.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      686 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0152/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.946197 slixmpp-1.8.4/slixmpp/plugins/xep_0153/
+-rw-r--r--   0 mathieui  (1000) users      (100)      369 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0153/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      736 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0153/stanza.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     6400 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0153/vcard_avatar.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     4628 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0163.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.946197 slixmpp-1.8.4/slixmpp/plugins/xep_0172/
+-rw-r--r--   0 mathieui  (1000) users      (100)      403 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0172/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1819 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0172/stanza.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1990 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0172/user_nick.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.946197 slixmpp-1.8.4/slixmpp/plugins/xep_0184/
+-rw-r--r--   0 mathieui  (1000) users      (100)      373 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0184/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3862 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0184/receipt.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2008 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0184/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.946197 slixmpp-1.8.4/slixmpp/plugins/xep_0186/
+-rw-r--r--   0 mathieui  (1000) users      (100)      421 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0186/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1190 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0186/invisible_command.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      508 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0186/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.946197 slixmpp-1.8.4/slixmpp/plugins/xep_0191/
+-rw-r--r--   0 mathieui  (1000) users      (100)      375 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0191/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2726 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0191/blocking.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1278 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0191/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.946197 slixmpp-1.8.4/slixmpp/plugins/xep_0196/
+-rw-r--r--   0 mathieui  (1000) users      (100)      407 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0196/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      499 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0196/stanza.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2810 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0196/user_gaming.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.946197 slixmpp-1.8.4/slixmpp/plugins/xep_0198/
+-rw-r--r--   0 mathieui  (1000) users      (100)      607 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0198/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3525 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0198/stanza.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    12148 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0198/stream_management.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.949531 slixmpp-1.8.4/slixmpp/plugins/xep_0199/
+-rw-r--r--   0 mathieui  (1000) users      (100)      332 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0199/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     6995 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0199/ping.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      735 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0199/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.949531 slixmpp-1.8.4/slixmpp/plugins/xep_0202/
+-rw-r--r--   0 mathieui  (1000) users      (100)      400 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0202/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3234 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0202/stanza.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2587 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0202/time.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.949531 slixmpp-1.8.4/slixmpp/plugins/xep_0203/
+-rw-r--r--   0 mathieui  (1000) users      (100)      396 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0203/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1076 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0203/delay.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1343 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0203/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.949531 slixmpp-1.8.4/slixmpp/plugins/xep_0221/
+-rw-r--r--   0 mathieui  (1000) users      (100)      401 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0221/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      636 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0221/media.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      939 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0221/stanza.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3649 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0222.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3643 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0223.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.949531 slixmpp-1.8.4/slixmpp/plugins/xep_0224/
+-rw-r--r--   0 mathieui  (1000) users      (100)      404 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0224/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2142 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0224/attention.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      923 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0224/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.949531 slixmpp-1.8.4/slixmpp/plugins/xep_0231/
+-rw-r--r--   0 mathieui  (1000) users      (100)      387 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0231/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     5639 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0231/bob.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      943 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0231/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.949531 slixmpp-1.8.4/slixmpp/plugins/xep_0234/
+-rw-r--r--   0 mathieui  (1000) users      (100)      141 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0234/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      398 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0234/jingle_file_transfer.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      917 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0234/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.949531 slixmpp-1.8.4/slixmpp/plugins/xep_0235/
+-rw-r--r--   0 mathieui  (1000) users      (100)      396 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0235/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      779 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0235/oauth.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2840 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0235/stanza.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      511 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0242.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.949531 slixmpp-1.8.4/slixmpp/plugins/xep_0249/
+-rw-r--r--   0 mathieui  (1000) users      (100)      343 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0249/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2674 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0249/invite.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1141 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0249/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.949531 slixmpp-1.8.4/slixmpp/plugins/xep_0256/
+-rw-r--r--   0 mathieui  (1000) users      (100)      332 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0256/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      646 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0256/last_activity_presence.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2244 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0256.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.952864 slixmpp-1.8.4/slixmpp/plugins/xep_0257/
+-rw-r--r--   0 mathieui  (1000) users      (100)      493 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0257/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2467 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0257/client_cert_management.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2520 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0257/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.952864 slixmpp-1.8.4/slixmpp/plugins/xep_0258/
+-rw-r--r--   0 mathieui  (1000) users      (100)      572 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0258/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1213 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0258/security_labels.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3749 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0258/stanza.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      479 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0270.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.952864 slixmpp-1.8.4/slixmpp/plugins/xep_0279/
+-rw-r--r--   0 mathieui  (1000) users      (100)      400 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0279/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1109 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0279/ipcheck.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      626 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0279/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.952864 slixmpp-1.8.4/slixmpp/plugins/xep_0280/
+-rw-r--r--   0 mathieui  (1000) users      (100)      503 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0280/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2888 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0280/carbons.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1521 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0280/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.952864 slixmpp-1.8.4/slixmpp/plugins/xep_0292/
+-rw-r--r--   0 mathieui  (1000) users      (100)      113 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0292/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3782 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0292/stanza.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3125 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0292/vcard4.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.952864 slixmpp-1.8.4/slixmpp/plugins/xep_0297/
+-rw-r--r--   0 mathieui  (1000) users      (100)      404 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0297/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2057 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0297/forwarded.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      971 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0297/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.952864 slixmpp-1.8.4/slixmpp/plugins/xep_0300/
+-rw-r--r--   0 mathieui  (1000) users      (100)      377 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0300/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2611 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0300/hash.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      870 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0300/stanza.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      523 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0302.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.952864 slixmpp-1.8.4/slixmpp/plugins/xep_0308/
+-rw-r--r--   0 mathieui  (1000) users      (100)      357 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0308/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1375 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0308/correction.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      362 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0308/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.952864 slixmpp-1.8.4/slixmpp/plugins/xep_0313/
+-rw-r--r--   0 mathieui  (1000) users      (100)      417 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0313/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     9499 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0313/mam.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     9974 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0313/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.952864 slixmpp-1.8.4/slixmpp/plugins/xep_0319/
+-rw-r--r--   0 mathieui  (1000) users      (100)      394 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0319/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2980 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0319/idle.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      685 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0319/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.956198 slixmpp-1.8.4/slixmpp/plugins/xep_0323/
+-rw-r--r--   0 mathieui  (1000) users      (100)      506 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0323/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    10004 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0323/device.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    30142 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0323/sensordata.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.956198 slixmpp-1.8.4/slixmpp/plugins/xep_0323/stanza/
+-rw-r--r--   0 mathieui  (1000) users      (100)      367 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0323/stanza/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      348 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0323/stanza/base.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    25419 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0323/stanza/sensordata.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2054 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0323/timerreset.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.956198 slixmpp-1.8.4/slixmpp/plugins/xep_0325/
+-rw-r--r--   0 mathieui  (1000) users      (100)      503 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0325/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    22903 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0325/control.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     4501 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0325/device.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.956198 slixmpp-1.8.4/slixmpp/plugins/xep_0325/stanza/
+-rw-r--r--   0 mathieui  (1000) users      (100)      364 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0325/stanza/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      348 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0325/stanza/base.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    16180 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0325/stanza/control.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.956198 slixmpp-1.8.4/slixmpp/plugins/xep_0332/
+-rw-r--r--   0 mathieui  (1000) users      (100)      431 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0332/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     5586 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0332/http.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.956198 slixmpp-1.8.4/slixmpp/plugins/xep_0332/stanza/
+-rw-r--r--   0 mathieui  (1000) users      (100)      446 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0332/stanza/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      740 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0332/stanza/data.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2187 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0332/stanza/request.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2185 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0332/stanza/response.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.956198 slixmpp-1.8.4/slixmpp/plugins/xep_0333/
+-rw-r--r--   0 mathieui  (1000) users      (100)      374 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0333/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2873 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0333/markers.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      726 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0333/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.956198 slixmpp-1.8.4/slixmpp/plugins/xep_0334/
+-rw-r--r--   0 mathieui  (1000) users      (100)      386 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0334/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      786 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0334/hints.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      741 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0334/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.956198 slixmpp-1.8.4/slixmpp/plugins/xep_0335/
+-rw-r--r--   0 mathieui  (1000) users      (100)      401 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0335/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      578 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0335/json_containers.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      616 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0335/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.959531 slixmpp-1.8.4/slixmpp/plugins/xep_0352/
+-rw-r--r--   0 mathieui  (1000) users      (100)      384 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0352/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2111 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0352/csi.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      806 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0352/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.959531 slixmpp-1.8.4/slixmpp/plugins/xep_0353/
+-rw-r--r--   0 mathieui  (1000) users      (100)      379 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0353/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3660 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0353/jingle_message.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1504 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0353/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.959531 slixmpp-1.8.4/slixmpp/plugins/xep_0356/
+-rw-r--r--   0 mathieui  (1000) users      (100)      237 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0356/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     4692 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0356/privilege.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1273 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0356/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.959531 slixmpp-1.8.4/slixmpp/plugins/xep_0359/
+-rw-r--r--   0 mathieui  (1000) users      (100)      352 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0359/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      693 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0359/stanza.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      559 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0359/stanzaid.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.959531 slixmpp-1.8.4/slixmpp/plugins/xep_0363/
+-rw-r--r--   0 mathieui  (1000) users      (100)      453 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0363/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     7838 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0363/http_upload.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1136 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0363/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.959531 slixmpp-1.8.4/slixmpp/plugins/xep_0369/
+-rw-r--r--   0 mathieui  (1000) users      (100)      352 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0369/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    10921 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0369/mix_core.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2632 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0369/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.959531 slixmpp-1.8.4/slixmpp/plugins/xep_0372/
+-rw-r--r--   0 mathieui  (1000) users      (100)      131 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0372/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      471 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0372/references.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      230 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0372/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.959531 slixmpp-1.8.4/slixmpp/plugins/xep_0377/
+-rw-r--r--   0 mathieui  (1000) users      (100)      347 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0377/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1139 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0377/spam_reporting.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      807 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0377/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.959531 slixmpp-1.8.4/slixmpp/plugins/xep_0380/
+-rw-r--r--   0 mathieui  (1000) users      (100)      363 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0380/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2137 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0380/eme.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      377 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0380/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.962864 slixmpp-1.8.4/slixmpp/plugins/xep_0382/
+-rw-r--r--   0 mathieui  (1000) users      (100)      351 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0382/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      873 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0382/spoiler.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      486 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0382/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.962864 slixmpp-1.8.4/slixmpp/plugins/xep_0385/
+-rw-r--r--   0 mathieui  (1000) users      (100)      296 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0385/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1960 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0385/sims.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      273 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0385/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.962864 slixmpp-1.8.4/slixmpp/plugins/xep_0394/
+-rw-r--r--   0 mathieui  (1000) users      (100)      401 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0394/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     5858 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0394/markup.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3177 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0394/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.962864 slixmpp-1.8.4/slixmpp/plugins/xep_0402/
+-rw-r--r--   0 mathieui  (1000) users      (100)      130 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0402/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      330 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0402/bookmarks.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      863 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0402/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.962864 slixmpp-1.8.4/slixmpp/plugins/xep_0403/
+-rw-r--r--   0 mathieui  (1000) users      (100)      356 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0403/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1155 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0403/mix_presence.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      792 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0403/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.962864 slixmpp-1.8.4/slixmpp/plugins/xep_0404/
+-rw-r--r--   0 mathieui  (1000) users      (100)      362 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0404/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3321 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0404/mix_anon.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      940 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0404/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.962864 slixmpp-1.8.4/slixmpp/plugins/xep_0405/
+-rw-r--r--   0 mathieui  (1000) users      (100)      351 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0405/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3882 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0405/mix_pam.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1328 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0405/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.962864 slixmpp-1.8.4/slixmpp/plugins/xep_0421/
+-rw-r--r--   0 mathieui  (1000) users      (100)      366 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0421/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1053 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0421/occupant_id.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1239 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0421/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.962864 slixmpp-1.8.4/slixmpp/plugins/xep_0422/
+-rw-r--r--   0 mathieui  (1000) users      (100)      353 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0422/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      741 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0422/fastening.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      912 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0422/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.962864 slixmpp-1.8.4/slixmpp/plugins/xep_0424/
+-rw-r--r--   0 mathieui  (1000) users      (100)      354 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0424/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2474 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0424/retraction.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      821 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0424/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.966198 slixmpp-1.8.4/slixmpp/plugins/xep_0425/
+-rw-r--r--   0 mathieui  (1000) users      (100)      354 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0425/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1677 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0425/moderation.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1232 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0425/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.966198 slixmpp-1.8.4/slixmpp/plugins/xep_0428/
+-rw-r--r--   0 mathieui  (1000) users      (100)      352 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0428/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      541 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0428/fallback.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      491 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0428/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.966198 slixmpp-1.8.4/slixmpp/plugins/xep_0437/
+-rw-r--r--   0 mathieui  (1000) users      (100)      276 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0437/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1986 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0437/rai.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1120 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0437/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.966198 slixmpp-1.8.4/slixmpp/plugins/xep_0439/
+-rw-r--r--   0 mathieui  (1000) users      (100)      357 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0439/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     4243 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0439/quickresponse.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      938 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0439/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.966198 slixmpp-1.8.4/slixmpp/plugins/xep_0441/
+-rw-r--r--   0 mathieui  (1000) users      (100)      377 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0441/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2407 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0441/mam_prefs.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2510 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0441/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.966198 slixmpp-1.8.4/slixmpp/plugins/xep_0444/
+-rw-r--r--   0 mathieui  (1000) users      (100)      282 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0444/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2012 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0444/reactions.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1699 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0444/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.966198 slixmpp-1.8.4/slixmpp/plugins/xep_0446/
+-rw-r--r--   0 mathieui  (1000) users      (100)      134 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0446/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      348 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0446/file_metadata.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      905 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0446/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.966198 slixmpp-1.8.4/slixmpp/plugins/xep_0447/
+-rw-r--r--   0 mathieui  (1000) users      (100)      295 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0447/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1776 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0447/sfs.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      469 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0447/stanza.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.966198 slixmpp-1.8.4/slixmpp/plugins/xep_0454/
+-rw-r--r--   0 mathieui  (1000) users      (100)     5289 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0454/__init__.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.966198 slixmpp-1.8.4/slixmpp/plugins/xep_0461/
+-rw-r--r--   0 mathieui  (1000) users      (100)      126 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0461/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1383 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0461/reply.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2390 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/plugins/xep_0461/stanza.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     6540 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/pluginsdict.py
+-rw-r--r--   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/py.typed
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.969531 slixmpp-1.8.4/slixmpp/roster/
+-rw-r--r--   0 mathieui  (1000) users      (100)      283 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/roster/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    20424 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/roster/item.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     7098 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/roster/multi.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    11677 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/roster/single.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.969531 slixmpp-1.8.4/slixmpp/stanza/
+-rw-r--r--   0 mathieui  (1000) users      (100)      578 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/stanza/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1008 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/stanza/atom.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     6071 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/stanza/error.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      593 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/stanza/handshake.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      341 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/stanza/htmlim.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     9744 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/stanza/iq.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     6891 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/stanza/message.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     5471 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/stanza/presence.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3215 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/stanza/rootstanza.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     4627 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/stanza/roster.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3249 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/stanza/stream_error.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1334 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/stanza/stream_features.py
+-rw-r--r--   0 mathieui  (1000) users      (100)   172010 2023-05-28 11:03:13.000000 slixmpp-1.8.4/slixmpp/stringprep.c
+-rw-r--r--   0 mathieui  (1000) users      (100)     3499 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/stringprep.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2432 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/stringprep.pyx
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.969531 slixmpp-1.8.4/slixmpp/test/
+-rw-r--r--   0 mathieui  (1000) users      (100)      321 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/test/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1913 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/test/integration.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     4721 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/test/livesocket.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     6774 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/test/mocksocket.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    30676 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/test/slixtest.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.969531 slixmpp-1.8.4/slixmpp/thirdparty/
+-rw-r--r--   0 mathieui  (1000) users      (100)      138 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/thirdparty/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    35683 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/thirdparty/gnupg.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2942 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/thirdparty/orderedset.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2490 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/types.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.969531 slixmpp-1.8.4/slixmpp/util/
+-rw-r--r--   0 mathieui  (1000) users      (100)      496 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/util/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     4708 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/util/cache.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3103 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/util/misc_ops.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.969531 slixmpp-1.8.4/slixmpp/util/sasl/
+-rw-r--r--   0 mathieui  (1000) users      (100)      391 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/util/sasl/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     5488 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/util/sasl/client.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    17279 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/util/sasl/mechanisms.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     4283 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/util/stringprep_profiles.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      303 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/version.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.972864 slixmpp-1.8.4/slixmpp/xmlstream/
+-rw-r--r--   0 mathieui  (1000) users      (100)      593 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/xmlstream/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     6563 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/xmlstream/cert.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.972864 slixmpp-1.8.4/slixmpp/xmlstream/handler/
+-rw-r--r--   0 mathieui  (1000) users      (100)      599 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/xmlstream/handler/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2991 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/xmlstream/handler/base.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3373 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/xmlstream/handler/callback.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2346 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/xmlstream/handler/collector.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3567 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/xmlstream/handler/coroutine_callback.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3218 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/xmlstream/handler/waiter.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1087 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/xmlstream/handler/xmlcallback.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      849 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/xmlstream/handler/xmlwaiter.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.972864 slixmpp-1.8.4/slixmpp/xmlstream/matcher/
+-rw-r--r--   0 mathieui  (1000) users      (100)      587 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/xmlstream/matcher/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      795 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/xmlstream/matcher/base.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      798 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/xmlstream/matcher/id.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1561 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/xmlstream/matcher/idsender.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1113 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/xmlstream/matcher/many.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1636 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/xmlstream/matcher/stanzapath.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3870 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/xmlstream/matcher/xmlmask.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1255 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/xmlstream/matcher/xpath.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    12064 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/xmlstream/resolver.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    61335 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/xmlstream/stanzabase.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     6637 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/xmlstream/tostring.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    56868 2023-05-28 11:03:05.000000 slixmpp-1.8.4/slixmpp/xmlstream/xmlstream.py
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.922864 slixmpp-1.8.4/slixmpp.egg-info/
+-rw-r--r--   0 mathieui  (1000) users      (100)     6234 2023-05-28 11:03:13.000000 slixmpp-1.8.4/slixmpp.egg-info/PKG-INFO
+-rw-r--r--   0 mathieui  (1000) users      (100)    24067 2023-05-28 11:03:13.000000 slixmpp-1.8.4/slixmpp.egg-info/SOURCES.txt
+-rw-r--r--   0 mathieui  (1000) users      (100)        1 2023-05-28 11:03:13.000000 slixmpp-1.8.4/slixmpp.egg-info/dependency_links.txt
+-rw-r--r--   0 mathieui  (1000) users      (100)      187 2023-05-28 11:03:13.000000 slixmpp-1.8.4/slixmpp.egg-info/requires.txt
+-rw-r--r--   0 mathieui  (1000) users      (100)     3418 2023-05-28 11:03:13.000000 slixmpp-1.8.4/slixmpp.egg-info/top_level.txt
+drwxr-xr-x   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:13.982864 slixmpp-1.8.4/tests/
+-rw-r--r--   0 mathieui  (1000) users      (100)        0 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/__init__.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1817 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/live_multiple_streams.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3366 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/live_test.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2343 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_cache.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2558 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_events.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    11108 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_jid.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      493 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_overall.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     4192 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_plugins.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2686 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_base.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    36816 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_element.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2516 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_error.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     4298 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_gmail.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2292 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_iq.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1867 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_message.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2428 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_presence.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3009 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_roster.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     8144 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0004.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    11638 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0009.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    17641 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0030.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3861 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0033.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     4806 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0045.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2563 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0047.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3598 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0050.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1765 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0055.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2882 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0059.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    24602 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0060.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1568 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0085.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     6535 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0122.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      993 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0184.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3312 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0292.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1524 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0300.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3612 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0313.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    14275 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0323.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     8587 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0325.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1398 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0356.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3598 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0369.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1537 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0377.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1038 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0380.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1249 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0402.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      887 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0403.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1801 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0405.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      857 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0421.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      876 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0422.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1112 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0424.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1316 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0425.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      650 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0437.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1669 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0439.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2288 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0444.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     2276 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stanza_xep_0461.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1629 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stream.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     6318 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stream_exceptions.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1830 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stream_filters.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     6402 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stream_handlers.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    10459 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stream_presence.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     9218 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stream_roster.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    20251 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stream_xep_0030.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     4492 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stream_xep_0047.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    40798 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stream_xep_0050.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     5555 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stream_xep_0055.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    25532 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stream_xep_0060.py
+-rw-r--r--   0 mathieui  (1000) users      (100)      931 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stream_xep_0066.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     4114 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stream_xep_0077.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1649 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stream_xep_0085.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1853 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stream_xep_0092.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    14213 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stream_xep_0100.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     3622 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stream_xep_0128.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1570 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stream_xep_0249.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    11378 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stream_xep_0313.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    44774 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stream_xep_0323.py
+-rw-r--r--   0 mathieui  (1000) users      (100)    12081 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stream_xep_0325.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     4029 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stream_xep_0356.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1939 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stream_xep_0385.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     6092 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stream_xep_0405.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1940 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stream_xep_0447.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1446 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_stream_xep_0461.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     4018 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_tostring.py
+-rw-r--r--   0 mathieui  (1000) users      (100)     1203 2023-05-28 11:03:05.000000 slixmpp-1.8.4/tests/test_xep_0454.py
```

### Comparing `slixmpp-1.8.3/LICENSE` & `slixmpp-1.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/PKG-INFO` & `slixmpp-1.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slixmpp
-Version: 1.8.3
+Version: 1.8.4
 Summary: Slixmpp is an elegant Python library for XMPP (aka Jabber).
 Home-page: https://lab.louiz.org/poezio/slixmpp
 Author: Florent Le Coz
 Author-email: louiz@louiz.org
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `slixmpp-1.8.3/README.rst` & `slixmpp-1.8.4/README.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/Makefile` & `slixmpp-1.8.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/_build/html/_images/arch_layers.png` & `slixmpp-1.8.4/docs/_static/images/arch_layers.png`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/_build/html/_static/images/from_&yet.png` & `slixmpp-1.8.4/docs/_static/images/from_&yet.png`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/api/api.rst` & `slixmpp-1.8.4/docs/api/api.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/api/plugins/index.rst` & `slixmpp-1.8.4/docs/api/plugins/index.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/api/plugins/xep_0012.rst` & `slixmpp-1.8.4/docs/api/plugins/xep_0012.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/api/plugins/xep_0027.rst` & `slixmpp-1.8.4/docs/api/plugins/xep_0027.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/api/plugins/xep_0030.rst` & `slixmpp-1.8.4/docs/api/plugins/xep_0030.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/api/plugins/xep_0047.rst` & `slixmpp-1.8.4/docs/api/plugins/xep_0047.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/api/plugins/xep_0054.rst` & `slixmpp-1.8.4/docs/api/plugins/xep_0054.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/api/plugins/xep_0060.rst` & `slixmpp-1.8.4/docs/api/plugins/xep_0060.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/api/plugins/xep_0065.rst` & `slixmpp-1.8.4/docs/api/plugins/xep_0065.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/api/plugins/xep_0077.rst` & `slixmpp-1.8.4/docs/api/plugins/xep_0077.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/api/plugins/xep_0115.rst` & `slixmpp-1.8.4/docs/api/plugins/xep_0115.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/api/plugins/xep_0128.rst` & `slixmpp-1.8.4/docs/api/plugins/xep_0128.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/api/plugins/xep_0153.rst` & `slixmpp-1.8.4/docs/api/plugins/xep_0153.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/api/plugins/xep_0231.rst` & `slixmpp-1.8.4/docs/api/plugins/xep_0231.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/api/plugins/xep_0319.rst` & `slixmpp-1.8.4/docs/api/plugins/xep_0319.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/api/plugins/xep_0332.rst` & `slixmpp-1.8.4/docs/api/plugins/xep_0332.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/api/xmlstream/matcher.rst` & `slixmpp-1.8.4/docs/api/xmlstream/matcher.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/api/xmlstream/stanzabase.rst` & `slixmpp-1.8.4/docs/api/xmlstream/stanzabase.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/api/xmlstream/tostring.rst` & `slixmpp-1.8.4/docs/api/xmlstream/tostring.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/architecture.rst` & `slixmpp-1.8.4/docs/architecture.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/conf.py` & `slixmpp-1.8.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/differences.rst` & `slixmpp-1.8.4/docs/differences.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/event_index.rst` & `slixmpp-1.8.4/docs/event_index.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/getting_started/component.rst` & `slixmpp-1.8.4/docs/getting_started/component.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/getting_started/echobot.rst` & `slixmpp-1.8.4/docs/getting_started/echobot.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/getting_started/iq.rst` & `slixmpp-1.8.4/docs/getting_started/iq.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/getting_started/muc.rst` & `slixmpp-1.8.4/docs/getting_started/muc.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/getting_started/sendlogout.rst` & `slixmpp-1.8.4/docs/getting_started/sendlogout.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/glossary.rst` & `slixmpp-1.8.4/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/howto/create_plugin.rst` & `slixmpp-1.8.4/docs/howto/create_plugin.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/howto/guide_xep_0030.rst` & `slixmpp-1.8.4/docs/howto/guide_xep_0030.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/howto/internal_api.rst` & `slixmpp-1.8.4/docs/howto/internal_api.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/howto/make_plugin_extension_for_message_and_iq.pl.rst` & `slixmpp-1.8.4/docs/howto/make_plugin_extension_for_message_and_iq.pl.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/howto/make_plugin_extension_for_message_and_iq.rst` & `slixmpp-1.8.4/docs/howto/make_plugin_extension_for_message_and_iq.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/howto/remove_process.rst` & `slixmpp-1.8.4/docs/howto/remove_process.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/howto/stanzas.rst` & `slixmpp-1.8.4/docs/howto/stanzas.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/howto/xeps.rst` & `slixmpp-1.8.4/docs/howto/xeps.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/howto/xmpp_tdg.rst` & `slixmpp-1.8.4/docs/howto/xmpp_tdg.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/index.rst` & `slixmpp-1.8.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/make.bat` & `slixmpp-1.8.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/docs/using_asyncio.rst` & `slixmpp-1.8.4/docs/using_asyncio.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/IoT_TestDevice.py` & `slixmpp-1.8.4/examples/IoT_TestDevice.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/adhoc_provider.py` & `slixmpp-1.8.4/examples/adhoc_provider.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/adhoc_user.py` & `slixmpp-1.8.4/examples/adhoc_user.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/admin_commands.py` & `slixmpp-1.8.4/examples/admin_commands.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/confirm_answer.py` & `slixmpp-1.8.4/examples/confirm_answer.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/confirm_ask.py` & `slixmpp-1.8.4/examples/confirm_ask.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/custom_stanzas/custom_stanza_provider.py` & `slixmpp-1.8.4/examples/custom_stanzas/custom_stanza_provider.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/custom_stanzas/custom_stanza_user.py` & `slixmpp-1.8.4/examples/custom_stanzas/custom_stanza_user.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/custom_stanzas/stanza.py` & `slixmpp-1.8.4/examples/custom_stanzas/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/disco_browser.py` & `slixmpp-1.8.4/examples/disco_browser.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/download_avatars.py` & `slixmpp-1.8.4/examples/download_avatars.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/echo_client.py` & `slixmpp-1.8.4/examples/echo_client.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/echo_component.py` & `slixmpp-1.8.4/examples/echo_component.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/gtalk_custom_domain.py` & `slixmpp-1.8.4/examples/gtalk_custom_domain.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/http_over_xmpp.py` & `slixmpp-1.8.4/examples/http_over_xmpp.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/http_upload.py` & `slixmpp-1.8.4/examples/http_upload.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/ibb_transfer/ibb_receiver.py` & `slixmpp-1.8.4/examples/ibb_transfer/ibb_receiver.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/ibb_transfer/ibb_sender.py` & `slixmpp-1.8.4/examples/ibb_transfer/ibb_sender.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/mam.py` & `slixmpp-1.8.4/examples/mam.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/markup.py` & `slixmpp-1.8.4/examples/markup.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/migrate_roster.py` & `slixmpp-1.8.4/examples/migrate_roster.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/mix.py` & `slixmpp-1.8.4/examples/mix.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/muc.py` & `slixmpp-1.8.4/examples/muc.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/ping.py` & `slixmpp-1.8.4/examples/ping.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/pubsub_client.py` & `slixmpp-1.8.4/examples/pubsub_client.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/pubsub_events.py` & `slixmpp-1.8.4/examples/pubsub_events.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/register_account.py` & `slixmpp-1.8.4/examples/register_account.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/roster_browser.py` & `slixmpp-1.8.4/examples/roster_browser.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/rpc_async.py` & `slixmpp-1.8.4/examples/rpc_async.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/rpc_client_side.py` & `slixmpp-1.8.4/examples/rpc_client_side.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/rpc_server_side.py` & `slixmpp-1.8.4/examples/rpc_server_side.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/s5b_transfer/s5b_receiver.py` & `slixmpp-1.8.4/examples/s5b_transfer/s5b_receiver.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/s5b_transfer/s5b_sender.py` & `slixmpp-1.8.4/examples/s5b_transfer/s5b_sender.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/send_client.py` & `slixmpp-1.8.4/examples/send_client.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/set_avatar.py` & `slixmpp-1.8.4/examples/set_avatar.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/thirdparty_auth.py` & `slixmpp-1.8.4/examples/thirdparty_auth.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/user_location.py` & `slixmpp-1.8.4/examples/user_location.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/examples/user_tune.py` & `slixmpp-1.8.4/examples/user_tune.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/run_tests.py` & `slixmpp-1.8.4/run_tests.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/setup.py` & `slixmpp-1.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/__init__.py` & `slixmpp-1.8.4/slixmpp/__init__.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/api.py` & `slixmpp-1.8.4/slixmpp/api.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/basexmpp.py` & `slixmpp-1.8.4/slixmpp/basexmpp.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,18 +275,18 @@
         contained in :attr:`plugin_whitelist`.
 
         Plugin configurations stored in :attr:`plugin_config` will be used.
         """
         if self.plugin_whitelist:
             plugin_list = self.plugin_whitelist
         else:
-            plugin_list = plugins.__all__
+            plugin_list = plugins.PLUGINS
 
         for plugin in plugin_list:
-            if plugin in plugins.__all__:
+            if plugin in plugins.PLUGINS:
                 self.register_plugin(plugin)
             else:
                 raise NameError("Plugin %s not in plugins.__all__." % plugin)
 
     def __getitem__(self, key):
         """Return a plugin given its name, if it has been registered."""
         if key in self.plugin:
```

### Comparing `slixmpp-1.8.3/slixmpp/clientxmpp.py` & `slixmpp-1.8.4/slixmpp/clientxmpp.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/componentxmpp.py` & `slixmpp-1.8.4/slixmpp/componentxmpp.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 # is specific to external server component connections.
 # Part of Slixmpp: The Slick XMPP Library
 # :copyright: (c) 2011 Nathanael C. Fritz
 # :license: MIT, see LICENSE for more details
 import logging
 import hashlib
 
+from slixmpp import Message, Iq, Presence
 from slixmpp.basexmpp import BaseXMPP
 from slixmpp.stanza import Handshake
+from slixmpp.stanza.error import Error
 from slixmpp.xmlstream import XMLStream
-from slixmpp.xmlstream import ET
 from slixmpp.xmlstream.matcher import MatchXPath
 from slixmpp.xmlstream.handler import Callback
-
+from slixmpp.xmlstream.stanzabase import register_stanza_plugin
 
 log = logging.getLogger(__name__)
 
 
 class ComponentXMPP(BaseXMPP):
 
     """
@@ -35,28 +36,38 @@
     :param plugin_whitelist: A list of approved plugins that
                     will be loaded when calling
                     :meth:`~slixmpp.basexmpp.BaseXMPP.register_plugins()`.
     :param use_jc_ns: Indicates if the ``'jabber:client'`` namespace
                       should be used instead of the standard
                       ``'jabber:component:accept'`` namespace.
                       Defaults to ``False``.
+    :param fix_error_ns: Fix the namespace of error stanzas.
+        If you use ``use_jc_ns`` namespace, you probably want that, but
+        it can be a problem if you use both a ClientXMPP and a ComponentXMPP
+        in the same interpreter. This is ``False`` by default for backwards
+        compatibility.
     """
 
-    def __init__(self, jid, secret, host=None, port=None, plugin_config=None, plugin_whitelist=None, use_jc_ns=False):
+    def __init__(self, jid, secret,
+                 host=None, port=None, plugin_config=None,
+                 plugin_whitelist=None, use_jc_ns=False,
+                 fix_error_ns=False):
 
         if not plugin_whitelist:
             plugin_whitelist = []
         if not plugin_config:
             plugin_config = {}
 
         if use_jc_ns:
             default_ns = 'jabber:client'
         else:
             default_ns = 'jabber:component:accept'
         BaseXMPP.__init__(self, jid, default_ns)
+        if fix_error_ns:
+            self._fix_error_ns()
 
         self.auto_authorize = None
         self.stream_header = '<stream:stream %s %s to="%s">' % (
                 'xmlns="jabber:component:accept"',
                 'xmlns:stream="%s"' % self.stream_ns,
                 jid)
         self.stream_footer = "</stream:stream>"
@@ -73,14 +84,19 @@
         self.register_handler(
                 Callback('Handshake',
                          MatchXPath('{jabber:component:accept}handshake'),
                          self._handle_handshake))
         self.add_event_handler('presence_probe',
                                self._handle_probe)
 
+    def _fix_error_ns(self):
+        Error.namespace = self.default_ns
+        for st in Message, Iq, Presence:
+            register_stanza_plugin(st, Error)
+
     def connect(self, host=None, port=None, use_ssl=False):
         """Connect to the server.
 
 
         :param host: The name of the desired server for the connection.
                      Defaults to :attr:`server_host`.
         :param port: Port to connect to on the server.
```

### Comparing `slixmpp-1.8.3/slixmpp/exceptions.py` & `slixmpp-1.8.4/slixmpp/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 
 # slixmpp.exceptions
 # ~~~~~~~~~~~~~~~~~~~~
 # Part of Slixmpp: The Slick XMPP Library
 # :copyright: (c) 2011 Nathanael C. Fritz
 # :license: MIT, see LICENSE for more details
 
+from typing import Dict, Optional
+
+from .types import ErrorConditions, ErrorTypes, JidStr
+
+
 class XMPPError(Exception):
 
     """
     A generic exception that may be raised while processing an XMPP stanza
     to indicate that an error response stanza should be sent.
 
     The exception method for stanza objects extending
@@ -33,20 +38,25 @@
                            the :class:`~xml.etree.ElementTree.Element`
                            constructor.
     :param clear: Indicates if the stanza's contents should be
                   removed before replying with an error.
                   Defaults to ``True``.
     """
 
-    def __init__(self, condition='undefined-condition', text='',
-                etype='cancel', extension=None, extension_ns=None,
-                extension_args=None, clear=True):
+    def __init__(self, condition: ErrorConditions='undefined-condition', text='',
+                etype: Optional[ErrorTypes]=None, extension=None, extension_ns=None,
+                extension_args=None, clear=True, by: Optional[JidStr] = None):
         if extension_args is None:
             extension_args = {}
+        if condition not in _DEFAULT_ERROR_TYPES:
+            raise ValueError("This is not a valid condition type", condition)
+        if etype is None:
+            etype = _DEFAULT_ERROR_TYPES[condition]
 
+        self.by = by
         self.condition = condition
         self.text = text
         self.etype = etype
         self.clear = clear
         self.extension = extension
         self.extension_ns = extension_ns
         self.extension_args = extension_args
@@ -106,7 +116,33 @@
     def __init__(self, pres):
         super().__init__(
             condition=pres['error']['condition'],
             text=pres['error']['text'],
             etype=pres['error']['type'],
         )
         self.presence = pres
+
+
+_DEFAULT_ERROR_TYPES: Dict[ErrorConditions, ErrorTypes] = {
+    "bad-request": "modify",
+    "conflict": "cancel",
+    "feature-not-implemented": "cancel",
+    "forbidden": "auth",
+    "gone": "modify",
+    "internal-server-error": "wait",
+    "item-not-found": "cancel",
+    "jid-malformed": "modify",
+    "not-acceptable": "modify",
+    "not-allowed": "cancel",
+    "not-authorized": "auth",
+    "payment-required": "auth",
+    "recipient-unavailable": "wait",
+    "redirect": "modify",
+    "registration-required": "auth",
+    "remote-server-not-found": "cancel",
+    "remote-server-timeout": "wait",
+    "resource-constraint": "wait",
+    "service-unavailable": "cancel",
+    "subscription-required": "auth",
+    "undefined-condition": "cancel",
+    "unexpected-request": "modify",
+}
```

### Comparing `slixmpp-1.8.3/slixmpp/features/feature_bind/bind.py` & `slixmpp-1.8.4/slixmpp/features/feature_bind/bind.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/features/feature_mechanisms/__init__.py` & `slixmpp-1.8.4/slixmpp/features/feature_mechanisms/__init__.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/features/feature_mechanisms/mechanisms.py` & `slixmpp-1.8.4/slixmpp/features/feature_mechanisms/mechanisms.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/features/feature_mechanisms/stanza/__init__.py` & `slixmpp-1.8.4/slixmpp/features/feature_mechanisms/stanza/__init__.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/features/feature_mechanisms/stanza/abort.py` & `slixmpp-1.8.4/slixmpp/features/feature_mechanisms/stanza/abort.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/features/feature_mechanisms/stanza/auth.py` & `slixmpp-1.8.4/slixmpp/features/feature_mechanisms/stanza/auth.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/features/feature_mechanisms/stanza/challenge.py` & `slixmpp-1.8.4/slixmpp/features/feature_mechanisms/stanza/challenge.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/features/feature_mechanisms/stanza/failure.py` & `slixmpp-1.8.4/slixmpp/features/feature_mechanisms/stanza/failure.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/features/feature_mechanisms/stanza/mechanisms.py` & `slixmpp-1.8.4/slixmpp/features/feature_mechanisms/stanza/mechanisms.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/features/feature_mechanisms/stanza/response.py` & `slixmpp-1.8.4/slixmpp/features/feature_mechanisms/stanza/response.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/features/feature_mechanisms/stanza/success.py` & `slixmpp-1.8.4/slixmpp/features/feature_mechanisms/stanza/success.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/features/feature_preapproval/preapproval.py` & `slixmpp-1.8.4/slixmpp/features/feature_preapproval/preapproval.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/features/feature_rosterver/rosterver.py` & `slixmpp-1.8.4/slixmpp/features/feature_rosterver/rosterver.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/features/feature_sasl2mechanisms/stanza/challenge.py` & `slixmpp-1.8.4/slixmpp/stanza/handshake.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,26 @@
-
 # Slixmpp: The Slick XMPP Library
-# Copyright (C) 2011  Nathanael C. Fritz
+# Copyright (C) 2021 Mathieu Pasquet
 # This file is part of Slixmpp.
 # See the file LICENSE for copying permission.
-import base64
 
-from slixmpp.util import bytes
 from slixmpp.xmlstream import StanzaBase
+from typing import Optional
 
 
-class SASL2Challenge(StanzaBase):
+class Handshake(StanzaBase):
 
     """
+    Jabber Component protocol handshake
     """
-
-    name = 'challenge'
-    namespace = 'urn:xmpp:sasl:1'
+    namespace = 'jabber:component:accept'
+    name = 'handshake'
     interfaces = {'value'}
-    plugin_attrib = name
 
-    def setup(self, xml):
-        StanzaBase.setup(self, xml)
-        self.xml.tag = self.tag_name()
-
-    def get_value(self):
-        return base64.b64decode(bytes(self.xml.text))
-
-    def set_value(self, values):
-        if values:
-            self.xml.text = bytes(base64.b64encode(values)).decode('utf-8')
-        else:
-            self.xml.text = '='
+    def set_value(self, value: str):
+        self.xml.text = value
+
+    def get_value(self) -> Optional[str]:
+        return self.xml.text
 
     def del_value(self):
         self.xml.text = ''
```

### Comparing `slixmpp-1.8.3/slixmpp/features/feature_sasl2mechanisms/stanza/response.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0300/stanza.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 
 # Slixmpp: The Slick XMPP Library
-# Copyright (C) 2011  Nathanael C. Fritz
+# Copyright (C) 2017 Emmanuel Gil Peyrot
 # This file is part of Slixmpp.
 # See the file LICENSE for copying permission.
-import base64
+from slixmpp.xmlstream import ElementBase
 
-from slixmpp.util import bytes
-from slixmpp.xmlstream import StanzaBase
 
-
-class SASL2Response(StanzaBase):
-
-    """
-    """
-
-    name = 'response'
-    namespace = 'urn:xmpp:sasl:1'
-    interfaces = {'value'}
-    plugin_attrib = name
-
-    def setup(self, xml):
-        StanzaBase.setup(self, xml)
-        self.xml.tag = self.tag_name()
+class Hash(ElementBase):
+    name = 'hash'
+    namespace = 'urn:xmpp:hashes:2'
+    plugin_attrib = 'hash'
+    interfaces = {'algo', 'value'}
+
+    allowed_algos = ['sha-1', 'sha-256', 'sha-512', 'sha3-256', 'sha3-512', 'BLAKE2b256', 'BLAKE2b512']
+
+    def set_algo(self, value):
+        if value in self.allowed_algos:
+            self._set_attr('algo', value)
+        elif value in [None, '']:
+            self._del_attr('algo')
+        else:
+            raise ValueError('Invalid algo: %s' % value)
 
     def get_value(self):
-        return base64.b64decode(bytes(self.xml.text))
+        return self.xml.text
 
-    def set_value(self, values):
-        if values:
-            self.xml.text = bytes(base64.b64encode(values)).decode('utf-8')
-        else:
-            self.xml.text = '='
+    def set_value(self, value):
+        self.xml.text = value
 
     def del_value(self):
         self.xml.text = ''
```

### Comparing `slixmpp-1.8.3/slixmpp/features/feature_sasl2mechanisms/stanza/success.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0231/stanza.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 
 # Slixmpp: The Slick XMPP Library
-# Copyright (C) 2011  Nathanael C. Fritz
+# Copyright (C) 2012 Nathanael C. Fritz
+# Emmanuel Gil Peyrot <linkmauve@linkmauve.fr>
 # This file is part of Slixmpp.
 # See the file LICENSE for copying permission.
 import base64
 
-from slixmpp.util import bytes
-from slixmpp.xmlstream import StanzaBase
-
 
-class SASL2Success(StanzaBase):
-
-    """
-    """
+from slixmpp.util import bytes
+from slixmpp.xmlstream import ElementBase
 
-    name = 'success'
-    namespace = 'urn:xmpp:sasl:1'
-    interfaces = {'value'}
-    plugin_attrib = name
 
-    def setup(self, xml):
-        StanzaBase.setup(self, xml)
-        self.xml.tag = self.tag_name()
+class BitsOfBinary(ElementBase):
+    name = 'data'
+    namespace = 'urn:xmpp:bob'
+    plugin_attrib = 'bob'
+    interfaces = {'cid', 'max_age', 'type', 'data'}
+
+    def get_max_age(self):
+        try:
+            return int(self._get_attr('max-age'))
+        except ValueError:
+            return None
+
+    def set_max_age(self, value):
+        if value is not None:
+            self._set_attr('max-age', str(value))
 
-    def get_value(self):
+    def get_data(self):
         return base64.b64decode(bytes(self.xml.text))
 
-    def set_value(self, values):
-        if values:
-            self.xml.text = bytes(base64.b64encode(values)).decode('utf-8')
-        else:
-            self.xml.text = '='
+    def set_data(self, value):
+        self.xml.text = bytes(base64.b64encode(value)).decode('utf-8')
 
-    def del_value(self):
+    def del_data(self):
         self.xml.text = ''
```

### Comparing `slixmpp-1.8.3/slixmpp/features/feature_session/session.py` & `slixmpp-1.8.4/slixmpp/features/feature_session/session.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/features/feature_session/stanza.py` & `slixmpp-1.8.4/slixmpp/features/feature_session/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/features/feature_starttls/stanza.py` & `slixmpp-1.8.4/slixmpp/features/feature_starttls/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/features/feature_starttls/starttls.py` & `slixmpp-1.8.4/slixmpp/features/feature_starttls/starttls.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/jid.py` & `slixmpp-1.8.4/slixmpp/jid.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,34 +299,39 @@
         :domain: The domain name portion of the JID.
         :server: Alias for ``domain``.
         :host: Alias for ``domain``.
         :resource: The resource portion of the JID.
 
     :param string jid:
         A string of the form ``'[user@]domain[/resource]'``.
+    :param bool bare:
+        If present, discard the provided resource.
 
     :raises InvalidJID:
     """
 
     __slots__ = ('_node', '_domain', '_resource', '_bare', '_full')
 
-    def __init__(self, jid: Optional[Union[str, 'JID']] = None):
+    def __init__(self, jid: Optional[Union[str, 'JID']] = None, bare: bool = False):
         if not jid:
             self._node = ''
             self._domain = ''
             self._resource = ''
             self._bare = ''
             self._full = ''
             return
         elif not isinstance(jid, JID):
-            self._node, self._domain, self._resource = _parse_jid(jid)
+            node, domain, resource = _parse_jid(jid)
+            self._node = node
+            self._domain = domain
+            self._resource = resource if not bare else ''
         else:
             self._node = jid._node
             self._domain = jid._domain
-            self._resource = jid._resource
+            self._resource = jid._resource if not bare else ''
         self._update_bare_full()
 
     def unescape(self):
         """Return an unescaped JID object.
 
         Using an unescaped JID is preferred for displaying JIDs
         to humans, and they should NOT be used for any other
```

### Comparing `slixmpp-1.8.3/slixmpp/plugins/__init__.py` & `slixmpp-1.8.4/slixmpp/plugins/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) 2010 Nathanael C. Fritz
 # This file is part of Slixmpp.
 # See the file LICENSE for copying permission.
 from slixmpp.plugins.base import PluginManager, PluginNotFound, BasePlugin
 from slixmpp.plugins.base import register_plugin, load_plugin
 
 
-__all__ = [
+PLUGINS = [
     # XEPS
     'xep_0004',  # Data Forms
     'xep_0009',  # Jabber-RPC
     'xep_0012',  # Last Activity
     'xep_0013',  # Flexible Offline Message Retrieval
 #   'xep_0016',  # Privacy Lists. Don’t automatically load
     'xep_0020',  # Feature Negotiation
@@ -75,14 +75,15 @@
     'xep_0249',  # Direct MUC Invitations
     'xep_0256',  # Last Activity in Presence
     'xep_0257',  # Client Certificate Management for SASL EXTERNAL
     'xep_0258',  # Security Labels in XMPP
 #   'xep_0270',  # XMPP Compliance Suites 2010. Don’t automatically load
     'xep_0279',  # Server IP Check
     'xep_0280',  # Message Carbons
+    'xep_0292',  # vCard4 Over XMPP
     'xep_0297',  # Stanza Forwarding
     'xep_0300',  # Use of Cryptographic Hash Functions in XMPP
 #   'xep_0302',  # XMPP Compliance Suites 2012. Don’t automatically load
     'xep_0308',  # Last Message Correction
     'xep_0313',  # Message Archive Management
     'xep_0319',  # Last User Interaction in Presence
 #   'xep_0323',  # IoT Systems Sensor Data. Don’t automatically load
@@ -97,20 +98,31 @@
     'xep_0359',  # Unique and Stable Stanza IDs
     'xep_0363',  # HTTP File Upload
     'xep_0369',  # MIX-CORE
     'xep_0377',  # Spam reporting
     'xep_0380',  # Explicit Message Encryption
     'xep_0382',  # Spoiler Messages
     'xep_0394',  # Message Markup
+    'xep_0402',  # PEP Native Bookmarks
     'xep_0403',  # MIX-Presence
     'xep_0404',  # MIX-Anon
     'xep_0405',  # MIX-PAM
     'xep_0421',  # Anonymous unique occupant identifiers for MUCs
     'xep_0422',  # Message Fastening
     'xep_0424',  # Message Retraction
     'xep_0425',  # Message Moderation
     'xep_0428',  # Message Fallback
     'xep_0437',  # Room Activity Indicators
     'xep_0439',  # Quick Response
     'xep_0441',  # Message Archive Management Preferences
     'xep_0444',  # Message Reactions
+    'xep_0461',  # Message Replies
+    # Meant to be imported by plugins
+]
+
+__all__ = PLUGINS + [
+    'PluginManager',
+    'PluginNotFound',
+    'BasePlugin',
+    'register_plugin',
+    'load_plugin',
 ]
```

### Comparing `slixmpp-1.8.3/slixmpp/plugins/base.py` & `slixmpp-1.8.4/slixmpp/plugins/base.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/gmail_notify.py` & `slixmpp-1.8.4/slixmpp/plugins/gmail_notify.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/google/__init__.py` & `slixmpp-1.8.4/slixmpp/plugins/google/__init__.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/google/auth/auth.py` & `slixmpp-1.8.4/slixmpp/plugins/google/auth/auth.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/google/auth/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/google/auth/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/google/gmail/notifications.py` & `slixmpp-1.8.4/slixmpp/plugins/google/gmail/notifications.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/google/gmail/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/google/gmail/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/google/nosave/nosave.py` & `slixmpp-1.8.4/slixmpp/plugins/google/nosave/nosave.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/google/nosave/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/google/nosave/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/google/settings/settings.py` & `slixmpp-1.8.4/slixmpp/plugins/google/settings/settings.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/google/settings/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/google/settings/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0004/dataforms.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0004/dataforms.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0004/stanza/field.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0004/stanza/field.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0004/stanza/form.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0004/stanza/form.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0009/binding.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0009/binding.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0009/remote.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0009/remote.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0009/rpc.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0009/rpc.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0009/stanza/RPC.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0009/stanza/RPC.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0012/last_activity.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0012/last_activity.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0012/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0012/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0013/offline.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0013/offline.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0013/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0013/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0016/privacy.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0016/privacy.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0016/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0016/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0020/feature_negotiation.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0020/feature_negotiation.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0027/gpg.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0027/gpg.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 from slixmpp.plugins.xep_0027 import stanza, Signed, Encrypted
 
 
 def _extract_data(data, kind):
     stripped = []
     begin_headers = False
     begin_data = False
+    if isinstance(data, bytes):
+        data = data.decode()
     for line in data.split('\n'):
         if not begin_headers and 'BEGIN PGP %s' % kind in line:
             begin_headers = True
             continue
         if begin_headers and line.strip() == '':
             begin_data = True
             continue
```

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0027/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0027/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0030/disco.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0030/disco.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,29 +303,29 @@
                 'itype': itype,
                 'lang': lang,
                 'local': local,
                 'cached': cached}
         return self.api['has_identity'](jid, node, ifrom, data)
 
     async def get_info_from_domain(self, domain=None, timeout=None,
-                                   cached=True, callback=None):
+                                   cached=True, callback=None, **iqkwargs):
         """Fetch disco#info of specified domain and one disco#items level below
         """
 
         if domain is None:
             domain = self.xmpp.boundjid.domain
 
         if not cached or domain not in self.domain_infos:
-            infos = [self.get_info(
-                domain, timeout=timeout)]
+            infos = [asyncio.create_task(self.get_info(
+                domain, timeout=timeout, **iqkwargs))]
             iq_items = await self.get_items(
-                domain, timeout=timeout)
+                domain, timeout=timeout, **iqkwargs)
             items = iq_items['disco_items']['items']
             infos += [
-                self.get_info(item[0], timeout=timeout)
+                asyncio.create_task(self.get_info(item[0], timeout=timeout, **iqkwargs))
                 for item in items]
             info_futures, _ = await asyncio.wait(
                 infos,
                 timeout=timeout,
             )
 
             self.domain_infos[domain] = [
@@ -453,17 +453,20 @@
                       no stanzas need to be sent.
                       Otherwise, a disco stanza must be sent to the
                       remove JID to retrieve the items.
         :param iterator: If True, return a result set iterator using
                          the XEP-0059 plugin, if the plugin is loaded.
                          Otherwise the parameter is ignored.
         """
+        if ifrom is None and self.xmpp.is_component:
+            ifrom = self.xmpp.boundjid.bare
+
         if local or local is None and jid is None:
             items = await self.api['get_items'](jid, node, ifrom, kwargs)
-            return self._wrap(kwargs.get('ifrom', None), jid, items)
+            return self._wrap(ifrom, jid, items)
 
         iq = self.xmpp.Iq()
         # Check dfrom parameter for backwards compatibility
         iq['from'] = ifrom or kwargs.get('dfrom', '')
         iq['to'] = jid
         iq['type'] = 'get'
         iq['disco_items']['node'] = node if node else ''
```

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0030/stanza/info.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0030/stanza/info.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0030/stanza/items.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0030/stanza/items.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0030/static.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0030/static.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0033/addresses.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0033/addresses.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0033/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0033/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0045/muc.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0045/muc.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,15 +319,14 @@
         presence_done: asyncio.Future = asyncio.Future()
         topic_received: asyncio.Future = asyncio.Future()
         history_buffer: List[Message] = []
         occupant_buffer: List[Presence] = []
 
         def add_message(msg: Message):
             delay = msg.get_plugin('delay', check=True)
-            print(delay)
             if delay is not None and delay['from'] == room:
                 history_buffer.append(msg)
 
         def add_occupant(pres: Presence):
             occupant_buffer.append(pres)
 
         catch_occupants = self.xmpp.event_handler("muc::%s::got_online" % room, add_occupant)
```

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0045/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0045/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0047/ibb.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0047/ibb.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0047/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0047/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0047/stream.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0047/stream.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0048/bookmarks.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0048/bookmarks.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0048/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0048/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0049/private_storage.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0049/private_storage.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0050/adhoc.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0050/adhoc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 # Slixmpp: The Slick XMPP Library
 # Copyright (C) 2011 Nathanael C. Fritz, Lance J.T. Stout
 # This file is part of Slixmpp.
 # See the file LICENSE for copying permission.
 import asyncio
+import functools
 import logging
 import time
 
 from slixmpp import Iq
 from slixmpp.exceptions import XMPPError
 from slixmpp.xmlstream.handler import Callback
 from slixmpp.xmlstream.matcher import StanzaPath
@@ -615,16 +616,22 @@
         elif iq['type'] == 'error':
             self.terminate_command(session)
 
         if iq['command']['status'] == 'completed':
             self.terminate_command(session)
 
 
+def _iscoroutine_or_partial_coroutine(handler):
+    return asyncio.iscoroutinefunction(handler) \
+        or isinstance(handler, functools.partial) \
+        and asyncio.iscoroutinefunction(handler.func)
+
+
 async def _await_if_needed(handler, *args):
     if handler is None:
         raise XMPPError("bad-request", text="The command is completed")
-    if asyncio.iscoroutinefunction(handler):
+    if _iscoroutine_or_partial_coroutine(handler):
         log.debug(f"%s is async", handler)
         return await handler(*args)
     else:
         log.debug(f"%s is sync", handler)
         return handler(*args)
```

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0050/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0050/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0054/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0054/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0054/vcard_temp.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0054/vcard_temp.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,16 +130,18 @@
 
     async def _handle_get_vcard(self, iq: Iq):
         if iq['type'] == 'result':
             await self.api['set_vcard'](jid=iq['from'], args=iq['vcard_temp'])
             return
         elif iq['type'] == 'get' and self.xmpp.is_component:
             vcard = await self.api['get_vcard'](iq['to'].bare, ifrom=iq['from'])
-            if isinstance(vcard, Iq):
-                vcard.send()
+            if vcard is None:
+                raise XMPPError("item-not-found")
+            elif isinstance(vcard, Iq):
+                await vcard.send()
             else:
                 iq = iq.reply()
                 iq.append(vcard)
                 iq.send()
         elif iq['type'] == 'set':
             raise XMPPError('service-unavailable')
```

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0055/search.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0055/search.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0059/rsm.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0059/rsm.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0059/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0059/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0060/pubsub.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0060/pubsub.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0060/stanza/base.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0060/stanza/base.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0060/stanza/pubsub.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0060/stanza/pubsub.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0060/stanza/pubsub_errors.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0060/stanza/pubsub_errors.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0060/stanza/pubsub_event.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0060/stanza/pubsub_event.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0060/stanza/pubsub_owner.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0060/stanza/pubsub_owner.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0065/proxy.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0065/proxy.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0065/socks5.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0065/socks5.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0065/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0065/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0066/oob.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0066/oob.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0066/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0066/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0070/confirm.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0070/confirm.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0071/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0071/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0071/xhtml_im.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0071/xhtml_im.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0077/register.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0077/register.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0077/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0077/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0078/legacyauth.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0078/legacyauth.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0078/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0078/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0079/amp.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0079/amp.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0079/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0079/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0080/geoloc.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0080/geoloc.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0080/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0080/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0082.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0082.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0084/avatar.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0084/avatar.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0084/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0084/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0085/chat_states.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0085/chat_states.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0085/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0085/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0086/legacy_error.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0086/legacy_error.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0086/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0086/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0091/legacy_delay.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0091/legacy_delay.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0091/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0091/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0092/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0092/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0092/version.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0092/version.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0095/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0095/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0095/stream_initiation.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0095/stream_initiation.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0096/file_transfer.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0096/file_transfer.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0096/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0096/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0100/gateway.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0100/gateway.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0106.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0106.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0107/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0107/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0107/user_mood.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0107/user_mood.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0108/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0108/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0108/user_activity.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0108/user_activity.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0115/caps.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0115/caps.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
             return
 
         ifrom = pres['to'] if self.xmpp.is_component else None
 
         if pres['caps']['hash'] not in self.hashes:
             try:
                 log.debug("Unknown caps hash: %s", pres['caps']['hash'])
-                self.xmpp['xep_0030'].get_info(jid=pres['from'], ifrom=ifrom)
+                await self.xmpp['xep_0030'].get_info(jid=pres['from'], ifrom=ifrom)
                 return
             except XMPPError:
                 return
 
         log.debug("New caps verification string: %s", ver)
         try:
             node = '%s#%s' % (pres['caps']['node'], ver)
```

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0115/static.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0115/static.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0118/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0118/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0118/user_tune.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0118/user_tune.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0122/data_validation.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0122/data_validation.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0122/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0122/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0128/extended_disco.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0128/extended_disco.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0128/static.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0128/static.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0131/headers.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0131/headers.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0131/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0131/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0133.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0133.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0138.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0138.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0152/reachability.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0152/reachability.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0152/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0152/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0153/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0153/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0153/vcard_avatar.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0153/vcard_avatar.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0163.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0163.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0172/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0172/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0172/user_nick.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0172/user_nick.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0184/receipt.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0184/receipt.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0184/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0184/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0186/invisible_command.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0186/invisible_command.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0191/blocking.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0191/blocking.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0191/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0191/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0196/user_gaming.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0196/user_gaming.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0198/__init__.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0198/__init__.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0198/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0198/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0198/stream_management.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0198/stream_management.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0199/ping.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0199/ping.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0199/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0199/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0202/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0202/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0202/time.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0202/time.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0203/delay.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0203/delay.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0203/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0203/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0221/media.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0221/media.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0221/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0221/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0222.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0222.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0223.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0223.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0224/attention.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0224/attention.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0224/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0224/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0231/bob.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0231/bob.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0235/oauth.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0235/oauth.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0235/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0235/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0249/invite.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0249/invite.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0249/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0249/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0256/last_activity_presence.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0256/last_activity_presence.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0256.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0256.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0257/client_cert_management.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0257/client_cert_management.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0257/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0257/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0258/__init__.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0258/__init__.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0258/security_labels.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0258/security_labels.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0258/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0258/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0279/ipcheck.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0279/ipcheck.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0279/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0279/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0280/carbons.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0280/carbons.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0280/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0280/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0297/forwarded.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0297/forwarded.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0297/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0297/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0300/hash.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0300/hash.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0302.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0302.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0308/correction.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0308/correction.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0313/mam.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0313/mam.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0313/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0313/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0319/idle.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0319/idle.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0319/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0319/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0323/device.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0323/device.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0323/sensordata.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0323/sensordata.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0323/stanza/sensordata.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0323/stanza/sensordata.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0323/timerreset.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0323/timerreset.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0325/control.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0325/control.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0325/device.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0325/device.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0325/stanza/control.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0325/stanza/control.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0332/http.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0332/http.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0332/stanza/data.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0332/stanza/data.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0332/stanza/request.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0332/stanza/request.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0332/stanza/response.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0332/stanza/response.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0333/markers.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0333/markers.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0333/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0333/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0334/hints.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0334/hints.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0334/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0334/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0335/json_containers.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0335/json_containers.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0335/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0335/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0352/csi.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0352/csi.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0352/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0352/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0353/jingle_message.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0353/jingle_message.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0353/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0353/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0356/privilege.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0356/privilege.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0356/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0356/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0359/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0359/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0359/stanzaid.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0359/stanzaid.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0363/http_upload.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0363/http_upload.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0363/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0363/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0369/mix_core.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0369/mix_core.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0369/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0369/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0377/spam_reporting.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0377/spam_reporting.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,14 +22,17 @@
     """XEP-0377: Spam reporting"""
 
     name = 'xep_0377'
     description = 'XEP-0377: Spam Reporting'
     dependencies = {'xep_0030', 'xep_0191'}
     stanza = stanza
 
+    SPAM = 'urn:xmpp:reporting:spam'
+    ABUSE = 'urn:xmpp:reporting:abuse'
+
     def plugin_init(self):
         register_stanza_plugin(Block, stanza.Report)
         register_stanza_plugin(stanza.Report, stanza.Text)
 
     def plugin_end(self):
         self.xmpp['xep_0030'].del_feature(feature=stanza.Report.namespace)
```

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0380/eme.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0380/eme.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0382/spoiler.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0382/spoiler.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0394/markup.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0394/markup.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0394/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0394/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0403/mix_presence.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0403/mix_presence.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0403/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0403/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0404/mix_anon.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0404/mix_anon.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0404/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0404/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0405/mix_pam.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0405/mix_pam.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0405/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0405/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0421/occupant_id.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0421/occupant_id.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0421/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0421/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0422/fastening.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0422/fastening.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0422/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0422/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0424/retraction.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0424/retraction.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0424/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0424/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0425/moderation.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0425/moderation.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0425/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0425/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0428/fallback.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0428/fallback.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0437/rai.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0437/rai.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0437/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0437/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0439/quickresponse.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0439/quickresponse.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0439/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0439/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0441/mam_prefs.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0441/mam_prefs.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0441/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0441/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0444/reactions.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0444/reactions.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0444/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0444/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0454/__init__.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0454/__init__.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0461/reply.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0461/reply.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/plugins/xep_0461/stanza.py` & `slixmpp-1.8.4/slixmpp/plugins/xep_0461/stanza.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,39 +9,72 @@
     name = "reply"
     plugin_attrib = "reply"
     interfaces = {"id", "to"}
 
 
 class FeatureFallBack(ElementBase):
     # should also be a multi attrib
-    namespace = "urn:xmpp:feature-fallback:0"
+    namespace = "urn:xmpp:fallback:0"
     name = "fallback"
     plugin_attrib = "feature_fallback"
     interfaces = {"for"}
 
-    def get_stripped_body(self):
+    def get_fallback_body(self):
         # only works for a single fallback_body attrib
         start = self["fallback_body"]["start"]
         end = self["fallback_body"]["end"]
         body = self.parent()["body"]
-        try:
-            start = int(start)
-            end = int(end)
-        except ValueError:
-            return body
+        if start <= end:
+            return body[start:end]
         else:
+            return ""
+
+    def get_stripped_body(self):
+        # only works for a single fallback_body attrib
+        start = self["fallback_body"]["start"]
+        end = self["fallback_body"]["end"]
+        body = self.parent()["body"]
+        if start <= end < len(body):
             return body[:start] + body[end:]
+        else:
+            return body
+
+    def add_quoted_fallback(self, fallback: str):
+        msg = self.parent()
+        quoted = "\n".join("> " + x.strip() for x in fallback.split("\n")) + "\n"
+        msg["body"] = quoted + msg["body"]
+        msg["feature_fallback"]["for"] = NS
+        msg["feature_fallback"]["fallback_body"]["start"] = 0
+        msg["feature_fallback"]["fallback_body"]["end"] = len(quoted)
 
 
 class FallBackBody(ElementBase):
     # According to https://xmpp.org/extensions/inbox/compatibility-fallback.html
     # this should be a multi_attrib *but* since it's a protoXEP, we'll see...
     namespace = FeatureFallBack.namespace
     name = "body"
     plugin_attrib = "fallback_body"
     interfaces = {"start", "end"}
 
+    def set_start(self, v: int):
+        self._set_attr("start", str(v))
+
+    def get_start(self):
+        try:
+            return int(self._get_attr("start"))
+        except ValueError:
+            return 0
+
+    def set_end(self, v: int):
+        self._set_attr("end", str(v))
+
+    def get_end(self):
+        try:
+            return int(self._get_attr("end"))
+        except ValueError:
+            return 0
+
 
 def register_plugins():
     register_stanza_plugin(Message, Reply)
     register_stanza_plugin(Message, FeatureFallBack)
     register_stanza_plugin(FeatureFallBack, FallBackBody)
```

### Comparing `slixmpp-1.8.3/slixmpp/pluginsdict.py` & `slixmpp-1.8.4/slixmpp/pluginsdict.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/roster/item.py` & `slixmpp-1.8.4/slixmpp/roster/item.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/roster/multi.py` & `slixmpp-1.8.4/slixmpp/roster/multi.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/roster/single.py` & `slixmpp-1.8.4/slixmpp/roster/single.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/stanza/__init__.py` & `slixmpp-1.8.4/slixmpp/stanza/__init__.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/stanza/atom.py` & `slixmpp-1.8.4/slixmpp/stanza/atom.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/stanza/error.py` & `slixmpp-1.8.4/slixmpp/stanza/error.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/stanza/iq.py` & `slixmpp-1.8.4/slixmpp/stanza/iq.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/stanza/message.py` & `slixmpp-1.8.4/slixmpp/stanza/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,15 @@
         :param bool clear: Indicates if existing content should be removed
                            before replying. Defaults to True.
 
         :rtype: :class:`~.Message`
         """
         new_message = StanzaBase.reply(self, clear)
 
-        if self['type'] == 'groupchat':
+        if not getattr(self.stream, "is_component", False) and self['type'] == 'groupchat':
             new_message['to'] = new_message['to'].bare
 
         new_message['thread'] = self['thread']
         new_message['parent_thread'] = self['parent_thread']
 
         del new_message['id']
         if self.stream is not None and self.stream.use_message_ids:
```

### Comparing `slixmpp-1.8.3/slixmpp/stanza/presence.py` & `slixmpp-1.8.4/slixmpp/stanza/presence.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/stanza/rootstanza.py` & `slixmpp-1.8.4/slixmpp/stanza/rootstanza.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,14 +59,16 @@
             # We raised this deliberately
             keep_id = self['id']
             reply = self.reply(clear=e.clear)
             reply['id'] = keep_id
             reply['error']['condition'] = e.condition
             reply['error']['text'] = e.text
             reply['error']['type'] = e.etype
+            if e.by:
+                reply["error"]["by"] = e.by
             if e.extension is not None:
                 # Extended error tag
                 extxml = ET.Element("{%s}%s" % (e.extension_ns, e.extension),
                                     e.extension_args)
                 reply['error'].append(extxml)
             reply.send()
         else:
```

### Comparing `slixmpp-1.8.3/slixmpp/stanza/roster.py` & `slixmpp-1.8.4/slixmpp/stanza/roster.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/stanza/stream_error.py` & `slixmpp-1.8.4/slixmpp/stanza/stream_error.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/stanza/stream_features.py` & `slixmpp-1.8.4/slixmpp/stanza/stream_features.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/stringprep.c` & `slixmpp-1.8.4/slixmpp/stringprep.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "libraries": [
             "idn"
@@ -21,16 +21,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -90,24 +90,28 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -215,15 +219,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -254,15 +258,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -564,35 +568,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1073,26 +1077,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1483,15 +1487,15 @@
  *     unicode_out = out.decode('utf-8')
  *     free(out)
  *     return unicode_out             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  if (!(likely(PyUnicode_CheckExact(__pyx_v_unicode_out))||((__pyx_v_unicode_out) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_unicode_out)->tp_name), 0))) __PYX_ERR(0, 42, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_v_unicode_out))||((__pyx_v_unicode_out) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_unicode_out)->tp_name), 0))) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_INCREF(__pyx_v_unicode_out);
   __pyx_r = ((PyObject*)__pyx_v_unicode_out);
   goto __pyx_L0;
 
   /* "slixmpp/stringprep.pyx":34
  * 
  * 
@@ -2200,15 +2204,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -2439,15 +2443,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_slixmpp__stringprep) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -3101,28 +3105,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -3285,15 +3289,15 @@
     }
     Py_XDECREF(owned_metaclass);
     return result;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -3670,15 +3674,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -3866,15 +3870,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `slixmpp-1.8.3/slixmpp/stringprep.py` & `slixmpp-1.8.4/slixmpp/stringprep.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/stringprep.pyx` & `slixmpp-1.8.4/slixmpp/stringprep.pyx`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/test/integration.py` & `slixmpp-1.8.4/slixmpp/test/integration.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/test/livesocket.py` & `slixmpp-1.8.4/slixmpp/test/livesocket.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/test/mocksocket.py` & `slixmpp-1.8.4/slixmpp/test/mocksocket.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/test/slixtest.py` & `slixmpp-1.8.4/slixmpp/test/slixtest.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 import unittest
 from queue import Queue
 from xml.parsers.expat import ExpatError
 
 from slixmpp.test import TestTransport
 from slixmpp import ClientXMPP, ComponentXMPP
 from slixmpp.stanza import Message, Iq, Presence
+from slixmpp.stanza.error import Error
 from slixmpp.xmlstream import ET
 from slixmpp.xmlstream import ElementBase
 from slixmpp.xmlstream.tostring import tostring, highlight
 from slixmpp.xmlstream.matcher import StanzaPath, MatcherId, MatchIDSender
 from slixmpp.xmlstream.matcher import MatchXMLMask, MatchXPath
+from slixmpp.xmlstream.stanzabase import register_stanza_plugin
 
 import asyncio
 
 
 class SlixTest(unittest.TestCase):
 
     """
@@ -318,14 +320,15 @@
                         Defaults to 5222.
             plugins  -- List of plugins to register. By default, all plugins
                         are loaded.
         """
         if not plugin_config:
             plugin_config = {}
 
+        self.mode = mode
         if mode == 'client':
             self.xmpp = ClientXMPP(jid, password,
                                    sasl_mech=sasl_mech,
                                    plugin_config=plugin_config)
         elif mode == 'component':
             self.xmpp = ComponentXMPP(jid, password,
                                       server, port,
@@ -736,7 +739,14 @@
                 if self.compare(child, child2):
                     break
             else:
                 return False
 
         # Everything matches
         return True
+
+    def tearDown(self):
+        self.stream_close()
+        if getattr(self, "mode", None) == "component":
+            Error.namespace = 'jabber:client'
+            for st in Message, Iq, Presence:
+                register_stanza_plugin(st, Error)
```

### Comparing `slixmpp-1.8.3/slixmpp/thirdparty/gnupg.py` & `slixmpp-1.8.4/slixmpp/thirdparty/gnupg.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/thirdparty/orderedset.py` & `slixmpp-1.8.4/slixmpp/thirdparty/orderedset.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/types.py` & `slixmpp-1.8.4/slixmpp/types.py`

 * *Files 26% similar despite different names*

```diff
@@ -79,12 +79,39 @@
 JidStr = Union[str, JID]
 OptJidStr = Optional[Union[str, JID]]
 
 MAMDefault = Literal['always', 'never', 'roster']
 
 FilterString = Literal['in', 'out', 'out_sync']
 
+ErrorTypes = Literal["modify", "cancel", "auth", "wait", "cancel"]
+
+ErrorConditions = Literal[
+    "bad-request",
+    "conflict",
+    "feature-not-implemented",
+    "forbidden",
+    "gone",
+    "internal-server-error",
+    "item-not-found",
+    "jid-malformed",
+    "not-acceptable",
+    "not-allowed",
+    "not-authorized",
+    "payment-required",
+    "recipient-unavailable",
+    "redirect",
+    "registration-required",
+    "remote-server-not-found",
+    "remote-server-timeout",
+    "resource-constraint",
+    "service-unavailable",
+    "subscription-required",
+    "undefined-condition",
+    "unexpected-request",
+]
+
 __all__ = [
-    'Protocol', 'TypedDict', 'Literal', 'OptJid', 'JidStr', 'MAMDefault',
+    'Protocol', 'TypedDict', 'Literal', 'OptJid', 'OptJidStr', 'JidStr', 'MAMDefault',
     'PresenceTypes', 'PresenceShows', 'MessageTypes', 'IqTypes', 'MucRole',
-    'MucAffiliation', 'FilterString',
+    'MucAffiliation', 'FilterString', 'ErrorConditions', 'ErrorTypes'
 ]
```

### Comparing `slixmpp-1.8.3/slixmpp/util/cache.py` & `slixmpp-1.8.4/slixmpp/util/cache.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/util/misc_ops.py` & `slixmpp-1.8.4/slixmpp/util/misc_ops.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/util/sasl/client.py` & `slixmpp-1.8.4/slixmpp/util/sasl/client.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/util/sasl/mechanisms.py` & `slixmpp-1.8.4/slixmpp/util/sasl/mechanisms.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/util/stringprep_profiles.py` & `slixmpp-1.8.4/slixmpp/util/stringprep_profiles.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/xmlstream/__init__.py` & `slixmpp-1.8.4/slixmpp/xmlstream/__init__.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/xmlstream/cert.py` & `slixmpp-1.8.4/slixmpp/xmlstream/cert.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/xmlstream/handler/__init__.py` & `slixmpp-1.8.4/slixmpp/xmlstream/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/xmlstream/handler/base.py` & `slixmpp-1.8.4/slixmpp/xmlstream/handler/base.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/xmlstream/handler/callback.py` & `slixmpp-1.8.4/slixmpp/xmlstream/handler/callback.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/xmlstream/handler/collector.py` & `slixmpp-1.8.4/slixmpp/xmlstream/handler/collector.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/xmlstream/handler/coroutine_callback.py` & `slixmpp-1.8.4/slixmpp/xmlstream/handler/coroutine_callback.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/xmlstream/handler/waiter.py` & `slixmpp-1.8.4/slixmpp/xmlstream/handler/waiter.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/xmlstream/handler/xmlcallback.py` & `slixmpp-1.8.4/slixmpp/xmlstream/handler/xmlcallback.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/xmlstream/handler/xmlwaiter.py` & `slixmpp-1.8.4/slixmpp/xmlstream/handler/xmlwaiter.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/xmlstream/matcher/__init__.py` & `slixmpp-1.8.4/slixmpp/xmlstream/matcher/__init__.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/xmlstream/matcher/base.py` & `slixmpp-1.8.4/slixmpp/xmlstream/matcher/base.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/xmlstream/matcher/id.py` & `slixmpp-1.8.4/slixmpp/xmlstream/matcher/id.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/xmlstream/matcher/idsender.py` & `slixmpp-1.8.4/slixmpp/xmlstream/matcher/idsender.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/xmlstream/matcher/many.py` & `slixmpp-1.8.4/slixmpp/xmlstream/matcher/many.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/xmlstream/matcher/stanzapath.py` & `slixmpp-1.8.4/slixmpp/xmlstream/matcher/stanzapath.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/xmlstream/matcher/xmlmask.py` & `slixmpp-1.8.4/slixmpp/xmlstream/matcher/xmlmask.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/xmlstream/matcher/xpath.py` & `slixmpp-1.8.4/slixmpp/xmlstream/matcher/xpath.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/xmlstream/resolver.py` & `slixmpp-1.8.4/slixmpp/xmlstream/resolver.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/xmlstream/stanzabase.py` & `slixmpp-1.8.4/slixmpp/xmlstream/stanzabase.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/xmlstream/tostring.py` & `slixmpp-1.8.4/slixmpp/xmlstream/tostring.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/slixmpp/xmlstream/xmlstream.py` & `slixmpp-1.8.4/slixmpp/xmlstream/xmlstream.py`

 * *Files 1% similar despite different names*

```diff
@@ -1335,14 +1335,16 @@
 
             passthrough = False
             if isinstance(data, Iq):
                 if data.get_plugin('bind', check=True):
                     passthrough = True
                 elif data.get_plugin('session', check=True):
                     passthrough = True
+                elif data.get_plugin('register', check=True):
+                    passthrough = True
             elif isinstance(data, Handshake):
                 passthrough = True
 
             if isinstance(data, (RootStanza, str)) and not passthrough:
                 self.__queued_stanzas.append((data, use_filters))
                 log.debug('NOT SENT: %s %s', type(data), data)
                 return
```

### Comparing `slixmpp-1.8.3/slixmpp.egg-info/PKG-INFO` & `slixmpp-1.8.4/slixmpp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slixmpp
-Version: 1.8.3
+Version: 1.8.4
 Summary: Slixmpp is an elegant Python library for XMPP (aka Jabber).
 Home-page: https://lab.louiz.org/poezio/slixmpp
 Author: Florent Le Coz
 Author-email: louiz@louiz.org
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `slixmpp-1.8.3/slixmpp.egg-info/SOURCES.txt` & `slixmpp-1.8.4/slixmpp.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -10,47 +10,14 @@
 docs/event_index.rst
 docs/glossary.rst
 docs/index.rst
 docs/license.rst
 docs/make.bat
 docs/sleekxmpp.rst
 docs/using_asyncio.rst
-docs/_build/html/_images/arch_layers.png
-docs/_build/html/_static/agogo.css
-docs/_build/html/_static/alert_info_32.png
-docs/_build/html/_static/alert_warning_32.png
-docs/_build/html/_static/basic.css
-docs/_build/html/_static/bg-page.png
-docs/_build/html/_static/bullet_orange.png
-docs/_build/html/_static/comment-bright.png
-docs/_build/html/_static/comment-close.png
-docs/_build/html/_static/comment.png
-docs/_build/html/_static/default.css
-docs/_build/html/_static/down-pressed.png
-docs/_build/html/_static/down.png
-docs/_build/html/_static/file.png
-docs/_build/html/_static/haiku.css
-docs/_build/html/_static/header.png
-docs/_build/html/_static/ir_black.css
-docs/_build/html/_static/minus.png
-docs/_build/html/_static/nature.css
-docs/_build/html/_static/noise_dk.png
-docs/_build/html/_static/plus.png
-docs/_build/html/_static/pygments.css
-docs/_build/html/_static/sphinxdoc.css
-docs/_build/html/_static/up-pressed.png
-docs/_build/html/_static/up.png
-docs/_build/html/_static/fonts/OFLGoudyStMTT-Italic.ttf
-docs/_build/html/_static/fonts/OFLGoudyStMTT.ttf
-docs/_build/html/_static/fonts/YanoneKaffeesatz-Bold.ttf
-docs/_build/html/_static/fonts/YanoneKaffeesatz-Light.ttf
-docs/_build/html/_static/fonts/YanoneKaffeesatz-Regular.ttf
-docs/_build/html/_static/fonts/YanoneKaffeesatz-Thin.ttf
-docs/_build/html/_static/images/arch_layers.png
-docs/_build/html/_static/images/from_&yet.png
 docs/_static/images/arch_layers.png
 docs/_static/images/from_&yet.png
 docs/api/api.rst
 docs/api/basexmpp.rst
 docs/api/clientxmpp.rst
 docs/api/componentxmpp.rst
 docs/api/exceptions.rst
@@ -114,14 +81,15 @@
 docs/api/plugins/xep_0235.rst
 docs/api/plugins/xep_0249.rst
 docs/api/plugins/xep_0256.rst
 docs/api/plugins/xep_0257.rst
 docs/api/plugins/xep_0258.rst
 docs/api/plugins/xep_0279.rst
 docs/api/plugins/xep_0280.rst
+docs/api/plugins/xep_0292.rst
 docs/api/plugins/xep_0297.rst
 docs/api/plugins/xep_0300.rst
 docs/api/plugins/xep_0308.rst
 docs/api/plugins/xep_0313.rst
 docs/api/plugins/xep_0319.rst
 docs/api/plugins/xep_0332.rst
 docs/api/plugins/xep_0333.rst
@@ -253,24 +221,14 @@
 slixmpp/features/feature_mechanisms/stanza/success.py
 slixmpp/features/feature_preapproval/__init__.py
 slixmpp/features/feature_preapproval/preapproval.py
 slixmpp/features/feature_preapproval/stanza.py
 slixmpp/features/feature_rosterver/__init__.py
 slixmpp/features/feature_rosterver/rosterver.py
 slixmpp/features/feature_rosterver/stanza.py
-slixmpp/features/feature_sasl2mechanisms/__init__.py
-slixmpp/features/feature_sasl2mechanisms/mechanisms.py
-slixmpp/features/feature_sasl2mechanisms/stanza/__init__.py
-slixmpp/features/feature_sasl2mechanisms/stanza/abort.py
-slixmpp/features/feature_sasl2mechanisms/stanza/auth.py
-slixmpp/features/feature_sasl2mechanisms/stanza/challenge.py
-slixmpp/features/feature_sasl2mechanisms/stanza/failure.py
-slixmpp/features/feature_sasl2mechanisms/stanza/mechanisms.py
-slixmpp/features/feature_sasl2mechanisms/stanza/response.py
-slixmpp/features/feature_sasl2mechanisms/stanza/success.py
 slixmpp/features/feature_session/__init__.py
 slixmpp/features/feature_session/session.py
 slixmpp/features/feature_session/stanza.py
 slixmpp/features/feature_starttls/__init__.py
 slixmpp/features/feature_starttls/stanza.py
 slixmpp/features/feature_starttls/starttls.py
 slixmpp/plugins/__init__.py
@@ -476,14 +434,17 @@
 slixmpp/plugins/xep_0221/stanza.py
 slixmpp/plugins/xep_0224/__init__.py
 slixmpp/plugins/xep_0224/attention.py
 slixmpp/plugins/xep_0224/stanza.py
 slixmpp/plugins/xep_0231/__init__.py
 slixmpp/plugins/xep_0231/bob.py
 slixmpp/plugins/xep_0231/stanza.py
+slixmpp/plugins/xep_0234/__init__.py
+slixmpp/plugins/xep_0234/jingle_file_transfer.py
+slixmpp/plugins/xep_0234/stanza.py
 slixmpp/plugins/xep_0235/__init__.py
 slixmpp/plugins/xep_0235/oauth.py
 slixmpp/plugins/xep_0235/stanza.py
 slixmpp/plugins/xep_0249/__init__.py
 slixmpp/plugins/xep_0249/invite.py
 slixmpp/plugins/xep_0249/stanza.py
 slixmpp/plugins/xep_0256/__init__.py
@@ -496,14 +457,17 @@
 slixmpp/plugins/xep_0258/stanza.py
 slixmpp/plugins/xep_0279/__init__.py
 slixmpp/plugins/xep_0279/ipcheck.py
 slixmpp/plugins/xep_0279/stanza.py
 slixmpp/plugins/xep_0280/__init__.py
 slixmpp/plugins/xep_0280/carbons.py
 slixmpp/plugins/xep_0280/stanza.py
+slixmpp/plugins/xep_0292/__init__.py
+slixmpp/plugins/xep_0292/stanza.py
+slixmpp/plugins/xep_0292/vcard4.py
 slixmpp/plugins/xep_0297/__init__.py
 slixmpp/plugins/xep_0297/forwarded.py
 slixmpp/plugins/xep_0297/stanza.py
 slixmpp/plugins/xep_0300/__init__.py
 slixmpp/plugins/xep_0300/hash.py
 slixmpp/plugins/xep_0300/stanza.py
 slixmpp/plugins/xep_0308/__init__.py
@@ -557,26 +521,35 @@
 slixmpp/plugins/xep_0359/stanzaid.py
 slixmpp/plugins/xep_0363/__init__.py
 slixmpp/plugins/xep_0363/http_upload.py
 slixmpp/plugins/xep_0363/stanza.py
 slixmpp/plugins/xep_0369/__init__.py
 slixmpp/plugins/xep_0369/mix_core.py
 slixmpp/plugins/xep_0369/stanza.py
+slixmpp/plugins/xep_0372/__init__.py
+slixmpp/plugins/xep_0372/references.py
+slixmpp/plugins/xep_0372/stanza.py
 slixmpp/plugins/xep_0377/__init__.py
 slixmpp/plugins/xep_0377/spam_reporting.py
 slixmpp/plugins/xep_0377/stanza.py
 slixmpp/plugins/xep_0380/__init__.py
 slixmpp/plugins/xep_0380/eme.py
 slixmpp/plugins/xep_0380/stanza.py
 slixmpp/plugins/xep_0382/__init__.py
 slixmpp/plugins/xep_0382/spoiler.py
 slixmpp/plugins/xep_0382/stanza.py
+slixmpp/plugins/xep_0385/__init__.py
+slixmpp/plugins/xep_0385/sims.py
+slixmpp/plugins/xep_0385/stanza.py
 slixmpp/plugins/xep_0394/__init__.py
 slixmpp/plugins/xep_0394/markup.py
 slixmpp/plugins/xep_0394/stanza.py
+slixmpp/plugins/xep_0402/__init__.py
+slixmpp/plugins/xep_0402/bookmarks.py
+slixmpp/plugins/xep_0402/stanza.py
 slixmpp/plugins/xep_0403/__init__.py
 slixmpp/plugins/xep_0403/mix_presence.py
 slixmpp/plugins/xep_0403/stanza.py
 slixmpp/plugins/xep_0404/__init__.py
 slixmpp/plugins/xep_0404/mix_anon.py
 slixmpp/plugins/xep_0404/stanza.py
 slixmpp/plugins/xep_0405/__init__.py
@@ -605,14 +578,20 @@
 slixmpp/plugins/xep_0439/stanza.py
 slixmpp/plugins/xep_0441/__init__.py
 slixmpp/plugins/xep_0441/mam_prefs.py
 slixmpp/plugins/xep_0441/stanza.py
 slixmpp/plugins/xep_0444/__init__.py
 slixmpp/plugins/xep_0444/reactions.py
 slixmpp/plugins/xep_0444/stanza.py
+slixmpp/plugins/xep_0446/__init__.py
+slixmpp/plugins/xep_0446/file_metadata.py
+slixmpp/plugins/xep_0446/stanza.py
+slixmpp/plugins/xep_0447/__init__.py
+slixmpp/plugins/xep_0447/sfs.py
+slixmpp/plugins/xep_0447/stanza.py
 slixmpp/plugins/xep_0454/__init__.py
 slixmpp/plugins/xep_0461/__init__.py
 slixmpp/plugins/xep_0461/reply.py
 slixmpp/plugins/xep_0461/stanza.py
 slixmpp/roster/__init__.py
 slixmpp/roster/item.py
 slixmpp/roster/multi.py
@@ -623,15 +602,14 @@
 slixmpp/stanza/handshake.py
 slixmpp/stanza/htmlim.py
 slixmpp/stanza/iq.py
 slixmpp/stanza/message.py
 slixmpp/stanza/presence.py
 slixmpp/stanza/rootstanza.py
 slixmpp/stanza/roster.py
-slixmpp/stanza/starttls.py
 slixmpp/stanza/stream_error.py
 slixmpp/stanza/stream_features.py
 slixmpp/test/__init__.py
 slixmpp/test/integration.py
 slixmpp/test/livesocket.py
 slixmpp/test/mocksocket.py
 slixmpp/test/slixtest.py
@@ -692,22 +670,24 @@
 tests/test_stanza_xep_0050.py
 tests/test_stanza_xep_0055.py
 tests/test_stanza_xep_0059.py
 tests/test_stanza_xep_0060.py
 tests/test_stanza_xep_0085.py
 tests/test_stanza_xep_0122.py
 tests/test_stanza_xep_0184.py
+tests/test_stanza_xep_0292.py
 tests/test_stanza_xep_0300.py
 tests/test_stanza_xep_0313.py
 tests/test_stanza_xep_0323.py
 tests/test_stanza_xep_0325.py
 tests/test_stanza_xep_0356.py
 tests/test_stanza_xep_0369.py
 tests/test_stanza_xep_0377.py
 tests/test_stanza_xep_0380.py
+tests/test_stanza_xep_0402.py
 tests/test_stanza_xep_0403.py
 tests/test_stanza_xep_0405.py
 tests/test_stanza_xep_0421.py
 tests/test_stanza_xep_0422.py
 tests/test_stanza_xep_0424.py
 tests/test_stanza_xep_0425.py
 tests/test_stanza_xep_0437.py
@@ -732,11 +712,13 @@
 tests/test_stream_xep_0100.py
 tests/test_stream_xep_0128.py
 tests/test_stream_xep_0249.py
 tests/test_stream_xep_0313.py
 tests/test_stream_xep_0323.py
 tests/test_stream_xep_0325.py
 tests/test_stream_xep_0356.py
+tests/test_stream_xep_0385.py
 tests/test_stream_xep_0405.py
+tests/test_stream_xep_0447.py
 tests/test_stream_xep_0461.py
 tests/test_tostring.py
 tests/test_xep_0454.py
```

### Comparing `slixmpp-1.8.3/slixmpp.egg-info/top_level.txt` & `slixmpp-1.8.4/slixmpp.egg-info/top_level.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 slixmpp
 slixmpp/features
 slixmpp/features/feature_bind
 slixmpp/features/feature_mechanisms
 slixmpp/features/feature_mechanisms/stanza
 slixmpp/features/feature_preapproval
 slixmpp/features/feature_rosterver
-slixmpp/features/feature_sasl2mechanisms
-slixmpp/features/feature_sasl2mechanisms/stanza
 slixmpp/features/feature_session
 slixmpp/features/feature_starttls
 slixmpp/plugins
 slixmpp/plugins/google
 slixmpp/plugins/google/auth
 slixmpp/plugins/google/gmail
 slixmpp/plugins/google/nosave
@@ -70,21 +68,23 @@
 slixmpp/plugins/xep_0198
 slixmpp/plugins/xep_0199
 slixmpp/plugins/xep_0202
 slixmpp/plugins/xep_0203
 slixmpp/plugins/xep_0221
 slixmpp/plugins/xep_0224
 slixmpp/plugins/xep_0231
+slixmpp/plugins/xep_0234
 slixmpp/plugins/xep_0235
 slixmpp/plugins/xep_0249
 slixmpp/plugins/xep_0256
 slixmpp/plugins/xep_0257
 slixmpp/plugins/xep_0258
 slixmpp/plugins/xep_0279
 slixmpp/plugins/xep_0280
+slixmpp/plugins/xep_0292
 slixmpp/plugins/xep_0297
 slixmpp/plugins/xep_0300
 slixmpp/plugins/xep_0308
 slixmpp/plugins/xep_0313
 slixmpp/plugins/xep_0319
 slixmpp/plugins/xep_0323
 slixmpp/plugins/xep_0323/stanza
@@ -97,30 +97,35 @@
 slixmpp/plugins/xep_0335
 slixmpp/plugins/xep_0352
 slixmpp/plugins/xep_0353
 slixmpp/plugins/xep_0356
 slixmpp/plugins/xep_0359
 slixmpp/plugins/xep_0363
 slixmpp/plugins/xep_0369
+slixmpp/plugins/xep_0372
 slixmpp/plugins/xep_0377
 slixmpp/plugins/xep_0380
 slixmpp/plugins/xep_0382
+slixmpp/plugins/xep_0385
 slixmpp/plugins/xep_0394
+slixmpp/plugins/xep_0402
 slixmpp/plugins/xep_0403
 slixmpp/plugins/xep_0404
 slixmpp/plugins/xep_0405
 slixmpp/plugins/xep_0421
 slixmpp/plugins/xep_0422
 slixmpp/plugins/xep_0424
 slixmpp/plugins/xep_0425
 slixmpp/plugins/xep_0428
 slixmpp/plugins/xep_0437
 slixmpp/plugins/xep_0439
 slixmpp/plugins/xep_0441
 slixmpp/plugins/xep_0444
+slixmpp/plugins/xep_0446
+slixmpp/plugins/xep_0447
 slixmpp/plugins/xep_0454
 slixmpp/plugins/xep_0461
 slixmpp/roster
 slixmpp/stanza
 slixmpp/test
 slixmpp/thirdparty
 slixmpp/util
```

### Comparing `slixmpp-1.8.3/tests/live_multiple_streams.py` & `slixmpp-1.8.4/tests/live_multiple_streams.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/live_test.py` & `slixmpp-1.8.4/tests/live_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 
 
 class TestLiveStream(SlixTest):
     """
     Test that we can test a live stanza stream.
     """
 
-    def tearDown(self):
-        self.stream_close()
-
     def testClientConnection(self):
         """Test that we can interact with a live ClientXMPP instance."""
         self.stream_start(mode='client',
                           socket='live',
                           skip=False,
                           jid='user@localhost/test',
                           password='user')
```

### Comparing `slixmpp-1.8.3/tests/test_cache.py` & `slixmpp-1.8.4/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_events.py` & `slixmpp-1.8.4/tests/test_events.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 
 
 class TestEvents(SlixTest):
 
     def setUp(self):
         self.stream_start()
 
-    def tearDown(self):
-        self.stream_close()
-
     def testEventHappening(self):
         """Test handler working"""
         happened = []
 
         def handletestevent(event):
             happened.append(True)
```

### Comparing `slixmpp-1.8.3/tests/test_jid.py` & `slixmpp-1.8.4/tests/test_jid.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_plugins.py` & `slixmpp-1.8.4/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_base.py` & `slixmpp-1.8.4/tests/test_stanza_base.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_element.py` & `slixmpp-1.8.4/tests/test_stanza_element.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_error.py` & `slixmpp-1.8.4/tests/test_stanza_error.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_gmail.py` & `slixmpp-1.8.4/tests/test_stanza_gmail.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_iq.py` & `slixmpp-1.8.4/tests/test_stanza_iq.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 import unittest
 from slixmpp.test import SlixTest
 from slixmpp.xmlstream.stanzabase import ET
 
 
 class TestIqStanzas(SlixTest):
 
-    def tearDown(self):
-        """Shutdown the XML stream after testing."""
-        self.stream_close()
-
     def testSetup(self):
         """Test initializing default Iq values."""
         iq = self.Iq()
         self.check(iq, """
           <iq id="0" />
         """)
```

### Comparing `slixmpp-1.8.3/tests/test_stanza_message.py` & `slixmpp-1.8.4/tests/test_stanza_message.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_presence.py` & `slixmpp-1.8.4/tests/test_stanza_presence.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_roster.py` & `slixmpp-1.8.4/tests/test_stanza_roster.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0004.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0004.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0009.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0009.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0030.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0030.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0033.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0033.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0045.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0045.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0047.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0047.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0050.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0050.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0055.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0055.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0059.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0059.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0060.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0060.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0085.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0085.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0122.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0122.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0184.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0184.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0300.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0300.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0313.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0313.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0323.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0323.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0325.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0325.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0356.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0356.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0369.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0369.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0377.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0377.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,38 +19,34 @@
             xep_0377.Text,
         )
 
     def testCreateReport(self):
         report = """
           <iq type="set">
             <block xmlns="urn:xmpp:blocking">
-                <report xmlns="urn:xmpp:reporting:0">
-                    <spam/>
-                </report>
+                <report xmlns="urn:xmpp:reporting:1" reason="urn:xmpp:reporting:spam"/>
             </block>
           </iq>
         """
 
         iq = self.Iq()
         iq['type'] = 'set'
-        iq['block']['report']['spam'] = True
+        iq['block']['report']['reason'] = xep_0377.XEP_0377.SPAM
 
-        self.check(iq, report)
+        self.check(iq, report, use_values=False)
 
     def testEnforceOnlyOneSubElement(self):
         report = """
           <iq type="set">
             <block xmlns="urn:xmpp:blocking">
-                <report xmlns="urn:xmpp:reporting:0">
-                    <abuse/>
-                </report>
+                <report xmlns="urn:xmpp:reporting:1" reason="urn:xmpp:reporting:abuse"/>
             </block>
           </iq>
         """
 
         iq = self.Iq()
         iq['type'] = 'set'
-        iq['block']['report']['spam'] = True
-        iq['block']['report']['abuse'] = True
-        self.check(iq, report)
+        iq['block']['report']['reason'] = xep_0377.XEP_0377.SPAM
+        iq['block']['report']['reason'] = xep_0377.XEP_0377.ABUSE
+        self.check(iq, report, use_values=False)
 
 suite = unittest.TestLoader().loadTestsFromTestCase(TestSpamReporting)
```

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0380.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0380.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0403.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0403.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0405.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0405.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0421.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0421.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0422.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0422.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0424.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0424.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0425.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0425.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0437.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0437.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0439.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0439.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0444.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0444.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stanza_xep_0461.py` & `slixmpp-1.8.4/tests/test_stanza_xep_0461.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,26 +23,53 @@
             """,
         )
 
     def testFallback(self):
         message = Message()
         message["body"] = "12345\nrealbody"
         message["feature_fallback"]["for"] = "NS"
-        message["feature_fallback"]["fallback_body"]["start"] = "0"
-        message["feature_fallback"]["fallback_body"]["end"] = "6"
+        message["feature_fallback"]["fallback_body"]["start"] = 0
+        message["feature_fallback"]["fallback_body"]["end"] = 6
 
         self.check(
             message,
             """
             <message xmlns="jabber:client">
               <body>12345\nrealbody</body>
-              <fallback xmlns='urn:xmpp:feature-fallback:0' for='NS'>
+              <fallback xmlns='urn:xmpp:fallback:0' for='NS'>
                 <body start="0" end="6" />
               </fallback>
             </message>
             """,
         )
 
         assert message["feature_fallback"].get_stripped_body() == "realbody"
 
+    def testAddFallBackHelper(self):
+        msg = Message()
+        msg["body"] = "Great"
+        msg["feature_fallback"].add_quoted_fallback("Anna wrote:\nHi, how are you?")
+        # ugly dedent but the test does not pass without it
+        self.check(
+            msg,
+            """
+        <message xmlns="jabber:client" type="normal">
+            <body>> Anna wrote:\n> Hi, how are you?\nGreat</body>
+            <fallback xmlns="urn:xmpp:fallback:0" for="urn:xmpp:reply:0">
+                <body start='0' end='33' />
+            </fallback>
+        </message>
+            """
+        )
+
+    def testGetFallBackBody(self):
+        body = "Anna wrote:\nHi, how are you?"
+        quoted = "> Anna wrote:\n> Hi, how are you?\n"
+
+        msg = Message()
+        msg["body"] = "Great"
+        msg["feature_fallback"].add_quoted_fallback(body)
+        body2 = msg["feature_fallback"].get_fallback_body()
+        self.assertTrue(body2 == quoted, body2)
+
 
 suite = unittest.TestLoader().loadTestsFromTestCase(TestReply)
```

### Comparing `slixmpp-1.8.3/tests/test_stream.py` & `slixmpp-1.8.4/tests/test_stream.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 
 
 class TestStreamTester(SlixTest):
     """
     Test that we can simulate and test a stanza stream.
     """
 
-    def tearDown(self):
-        self.stream_close()
-
     def testClientEcho(self):
         """Test that we can interact with a ClientXMPP instance."""
         self.stream_start(mode='client')
 
         def echo(msg):
             msg.reply('Thanks for sending: %s' % msg['body']).send()
```

### Comparing `slixmpp-1.8.3/tests/test_stream_exceptions.py` & `slixmpp-1.8.4/tests/test_stream_exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,14 @@
 
 
 class TestStreamExceptions(SlixTest):
     """
     Test handling roster updates.
     """
 
-    def tearDown(self):
-        self.stream_close()
-
     def testExceptionContinueWorking(self):
         """Test that Slixmpp continues to respond after an XMPPError is raised."""
 
         def message(msg):
             raise XMPPError(clear=True)
 
         self.stream_start()
```

### Comparing `slixmpp-1.8.3/tests/test_stream_filters.py` & `slixmpp-1.8.4/tests/test_stream_filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,17 +10,14 @@
     """
     Test using incoming and outgoing filters.
     """
 
     def setUp(self):
         self.stream_start()
 
-    def tearDown(self):
-        self.stream_close()
-
     def testIncoming(self):
 
         data = []
 
         def in_filter(stanza):
             if isinstance(stanza, Message):
                 if stanza['body'] == 'testing':
```

### Comparing `slixmpp-1.8.3/tests/test_stream_handlers.py` & `slixmpp-1.8.4/tests/test_stream_handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,14 @@
     """
     Test using handlers and waiters.
     """
 
     def setUp(self):
         self.stream_start()
 
-    def tearDown(self):
-        self.stream_close()
-
     def testCallback(self):
         """Test using stream callback handlers."""
 
         def callback_handler(stanza):
             self.xmpp.send_raw("""
               <message>
                 <body>Success!</body>
```

### Comparing `slixmpp-1.8.3/tests/test_stream_presence.py` & `slixmpp-1.8.4/tests/test_stream_presence.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,14 @@
     """
     Test handling roster updates.
     """
 
     def setUp(self):
         self.stream_start(jid='tester@localhost', plugins=[])
 
-    def tearDown(self):
-        self.stream_close()
-
     def testInitialUnavailablePresences(self):
         """
         Test receiving unavailable presences from JIDs that
         are not online.
         """
         events = set()
```

### Comparing `slixmpp-1.8.3/tests/test_stream_roster.py` & `slixmpp-1.8.4/tests/test_stream_roster.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,14 @@
 
 
 class TestStreamRoster(SlixTest):
     """
     Test handling roster updates.
     """
 
-    def tearDown(self):
-        self.stream_close()
-
     def testGetRoster(self):
         """Test handling roster requests."""
         self.stream_start(mode='client', jid='tester@localhost')
 
         roster_updates = []
 
         self.xmpp.add_event_handler('roster_update', roster_updates.append)
```

### Comparing `slixmpp-1.8.3/tests/test_stream_xep_0030.py` & `slixmpp-1.8.4/tests/test_stream_xep_0030.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,14 @@
 
 class TestStreamDisco(SlixTest):
 
     """
     Test using the XEP-0030 plugin.
     """
 
-    def tearDown(self):
-        self.stream_close()
-
     def testInfoEmptyDefaultNode(self):
         """
         Info query result from an entity MUST have at least one identity
         and feature, namely http://jabber.org/protocol/disco#info.
 
         Since the XEP-0030 plugin is loaded, a disco response should
         be generated and not an error result.
```

### Comparing `slixmpp-1.8.3/tests/test_stream_xep_0047.py` & `slixmpp-1.8.4/tests/test_stream_xep_0047.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,14 @@
 
 
 class TestInBandByteStreams(SlixTest):
 
     def setUp(self):
         self.stream_start(plugins=['xep_0047', 'xep_0030'])
 
-    def tearDown(self):
-        self.stream_close()
-
     def testOpenStream(self):
         """Test requesting a stream, successfully"""
 
         events = []
 
         def on_stream_start(stream):
             events.append('ibb_stream_start')
```

### Comparing `slixmpp-1.8.3/tests/test_stream_xep_0050.py` & `slixmpp-1.8.4/tests/test_stream_xep_0050.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,17 +12,14 @@
         self.stream_start(mode='client',
                           plugins=['xep_0030', 'xep_0004', 'xep_0050'])
 
         # Real session IDs don't make for nice tests, so use
         # a dummy value.
         self.xmpp['xep_0050'].new_session = lambda: '_sessionid_'
 
-    def tearDown(self):
-        self.stream_close()
-
     def testInitialPayloadCommand(self):
         """Test a command with an initial payload."""
 
         class TestPayload(ElementBase):
             name = 'foo'
             namespace = 'test'
             interfaces = {'bar'}
```

### Comparing `slixmpp-1.8.3/tests/test_stream_xep_0055.py` & `slixmpp-1.8.4/tests/test_stream_xep_0055.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,14 @@
             },
             jid="characters.shakespeare.lit",
             plugins={"xep_0055"}
         )
         self.xmpp["xep_0055"].api.register(get_results, "search_query")
         self.xmpp["xep_0055"].api.register(get_results, "search_query")
 
-    def tearDown(self):
-        self.stream_close()
-
     def testRequestingSearchFields(self):
         self.recv(
             """
             <iq type='get'
                 from='juliet@capulet.com/balcony'
                 to='characters.shakespeare.lit'
                 id='search3'
```

### Comparing `slixmpp-1.8.3/tests/test_stream_xep_0060.py` & `slixmpp-1.8.4/tests/test_stream_xep_0060.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,14 @@
     """
     Test using the XEP-0030 plugin.
     """
 
     def setUp(self):
         self.stream_start()
 
-    def tearDown(self):
-        self.stream_close()
-
     def testCreateInstantNode(self):
         """Test creating an instant node"""
         self.xmpp['xep_0060'].create_node('pubsub.example.com', None)
 
         self.send("""
           <iq type="set" id="1" to="pubsub.example.com">
             <pubsub xmlns="http://jabber.org/protocol/pubsub">
```

### Comparing `slixmpp-1.8.3/tests/test_stream_xep_0066.py` & `slixmpp-1.8.4/tests/test_stream_xep_0066.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 
 import unittest
 from slixmpp.test import SlixTest
 
 
 class TestOOB(SlixTest):
 
-    def tearDown(self):
-        self.stream_close()
-
     def testSendOOB(self):
         """Test sending an OOB transfer request."""
         self.stream_start(plugins=['xep_0066', 'xep_0030'])
 
         url = 'http://github.com/fritzy/Slixmpp/blob/master/README'
 
         self.xmpp['xep_0066'].send_oob('user@example.com', url,
```

### Comparing `slixmpp-1.8.3/tests/test_stream_xep_0077.py` & `slixmpp-1.8.4/tests/test_stream_xep_0077.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stream_xep_0085.py` & `slixmpp-1.8.4/tests/test_stream_xep_0085.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 
 import unittest
 from slixmpp.test import SlixTest
 
 
 class TestStreamChatStates(SlixTest):
 
-    def tearDown(self):
-        self.stream_close()
-
     def testChatStates(self):
         self.stream_start(mode='client', plugins=['xep_0030', 'xep_0085'])
 
         results = []
 
         def handle_state(msg):
             results.append(msg['chat_state'])
```

### Comparing `slixmpp-1.8.3/tests/test_stream_xep_0092.py` & `slixmpp-1.8.4/tests/test_stream_xep_0092.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 
 import unittest
 from slixmpp.test import SlixTest
 
 
 class TestStreamSet(SlixTest):
 
-    def tearDown(self):
-        self.stream_close()
-
     def testHandleSoftwareVersionRequest(self):
         self.stream_start(mode='client', plugins=['xep_0030', 'xep_0092'])
 
         self.xmpp['xep_0092'].name = 'Slixmpp'
         self.xmpp['xep_0092'].version = 'dev'
         self.xmpp['xep_0092'].os = 'Linux'
```

### Comparing `slixmpp-1.8.3/tests/test_stream_xep_0100.py` & `slixmpp-1.8.4/tests/test_stream_xep_0100.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
             plugins=["xep_0077", "xep_0100"],
             jid="aim.shakespeare.lit",
             server="shakespeare.lit",
             plugin_config={
                 "xep_0100": {"component_name": "AIM Gateway", "type": "aim"}
             },
         )
+        self.xmpp._fix_error_ns()
 
     def next_sent(self):
         self.wait_for_send_queue()
         sent = self.xmpp.socket.next_sent(timeout=0.5)
         if sent is None:
             return None
         xml = self.parse_xml(sent)
@@ -156,26 +157,25 @@
             <query xmlns='jabber:iq:register'>
                 <username>RomeoMyRomeo</username>
                 <password>ILoveJuliet</password>
             </query>
             </iq>
             """
         )
-        # xmlns="jabber:client" in error substanza, bug in XEP-0077 plugin or OK?
         self.send(
             """
             <iq type='error'
                 from='aim.shakespeare.lit'
                 to='romeo@montague.lit/orchard'
                 id='reg2'>
             <query xmlns='jabber:iq:register'>
                 <username>RomeoMyRomeo</username>
                 <password>ILoveJuliet</password>
             </query>
-            <error code='406' type='modify' xmlns="jabber:client">
+            <error code='406' type='modify'>
                 <not-acceptable
                     xmlns='urn:ietf:params:xml:ns:xmpp-stanzas'/>
                 <text xmlns="urn:ietf:params:xml:ns:xmpp-stanzas">Not good</text>
             </error>
             </iq>
             """,
             use_values=False,
```

### Comparing `slixmpp-1.8.3/tests/test_stream_xep_0128.py` & `slixmpp-1.8.4/tests/test_stream_xep_0128.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 
 class TestStreamExtendedDisco(SlixTest):
 
     """
     Test using the XEP-0128 plugin.
     """
 
-    def tearDown(self):
-        self.stream_close()
-
     def testUsingExtendedInfo(self):
         self.stream_start(mode='client',
                           jid='tester@localhost',
                           plugins=['xep_0030',
                                    'xep_0004',
                                    'xep_0128'])
```

### Comparing `slixmpp-1.8.3/tests/test_stream_xep_0249.py` & `slixmpp-1.8.4/tests/test_stream_xep_0249.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,17 +6,14 @@
 
 class TestStreamDirectInvite(SlixTest):
 
     """
     Test using the XEP-0249 plugin.
     """
 
-    def tearDown(self):
-        self.stream_close()
-
     def testReceiveInvite(self):
         self.stream_start(mode='client',
                           plugins=['xep_0030',
                                    'xep_0249'])
 
         events = []
```

### Comparing `slixmpp-1.8.3/tests/test_stream_xep_0313.py` & `slixmpp-1.8.4/tests/test_stream_xep_0313.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 
 
 class TestMAM(SlixTest):
 
     def setUp(self):
         self.stream_start(plugins=['xep_0313'])
 
-    def tearDown(self):
-        self.stream_close()
-
     def testRetrieveSimple(self):
         """Test requesting MAM messages without RSM"""
 
         msgs = []
 
         async def test():
             iq = await self.xmpp['xep_0313'].retrieve()
```

### Comparing `slixmpp-1.8.3/tests/test_stream_xep_0323.py` & `slixmpp-1.8.4/tests/test_stream_xep_0323.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,14 @@
     """
     def setUp(self):
         pass
 
     def _time_now(self):
         return datetime.datetime.now().replace(microsecond=0).isoformat()
 
-    def tearDown(self):
-        self.stream_close()
-
     def testRequestAccept(self):
         self.stream_start(mode='component',
                           plugins=['xep_0030',
                                    'xep_0323'])
 
         myDevice = Device("Device22")
         myDevice._add_field(name="Temperature", typename="numeric", unit="°C")
```

### Comparing `slixmpp-1.8.3/tests/test_stream_xep_0325.py` & `slixmpp-1.8.4/tests/test_stream_xep_0325.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,17 +26,14 @@
     """
     def setUp(self):
         pass
 
     def _time_now(self):
         return datetime.datetime.now().replace(microsecond=0).isoformat()
 
-    def tearDown(self):
-        self.stream_close()
-
     def testRequestSetOk(self):
         self.stream_start(mode='component',
                           plugins=['xep_0030',
                                    'xep_0325'])
 
         myDevice = Device("Device22")
         myDevice._add_control_field(name="Temperature", typename="int", value="15")
```

### Comparing `slixmpp-1.8.3/tests/test_stream_xep_0356.py` & `slixmpp-1.8.4/tests/test_stream_xep_0356.py`

 * *Files identical despite different names*

### Comparing `slixmpp-1.8.3/tests/test_stream_xep_0405.py` & `slixmpp-1.8.4/tests/test_stream_xep_0405.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 
 
 class TestMIXPAM(SlixTest):
 
     def setUp(self):
         self.stream_start(plugins=['xep_0405'])
 
-    def tearDown(self):
-        self.stream_close()
-
     def testGetRosterEmpty(self):
         """Test requesting an empty annotated roster"""
 
         fut = self.xmpp.wrap(self.xmpp['xep_0405'].get_mix_roster())
 
         self.wait_()
         self.send("""
```

### Comparing `slixmpp-1.8.3/tests/test_stream_xep_0461.py` & `slixmpp-1.8.4/tests/test_stream_xep_0461.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,17 +3,14 @@
 from slixmpp.test import SlixTest
 
 
 class TestReply(SlixTest):
     def setUp(self):
         self.stream_start(plugins=["xep_0461"])
 
-    def tearDown(self):
-        self.stream_close()
-
     def testFallBackBody(self):
         async def on_reply(msg):
             start = msg["feature_fallback"]["fallback_body"]["start"]
             end = msg["feature_fallback"]["fallback_body"]["end"]
             self.xmpp["xep_0461"].send_reply(
                 reply_to=msg.get_from(),
                 reply_id=msg.get_id(),
@@ -24,15 +21,15 @@
         self.xmpp.add_event_handler("message_reply", on_reply)
 
         self.recv(
             """
             <message id="other-id" from="from@from.com/res">
               <reply xmlns="urn:xmpp:reply:0" id="some-id" />
               <body>&gt; quoted\nsome-body</body>
-                <fallback xmlns='urn:xmpp:feature-fallback:0' for='urn:xmpp:reply:0'>
+                <fallback xmlns='urn:xmpp:fallback:0' for='urn:xmpp:reply:0'>
                    <body start="0" end="8" />
                 </fallback>
             </message>
             """
         )
         self.send(
             """
```

### Comparing `slixmpp-1.8.3/tests/test_tostring.py` & `slixmpp-1.8.4/tests/test_tostring.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,14 @@
 
 class TestToString(SlixTest):
 
     """
     Test the implementation of slixmpp.xmlstream.tostring
     """
 
-    def tearDown(self):
-        self.stream_close()
-
     def tryTostring(self, original='', expected=None, message='', **kwargs):
         """
         Compare the result of calling tostring against an
         expected result.
         """
         if not expected:
             expected=original
```

### Comparing `slixmpp-1.8.3/tests/test_xep_0454.py` & `slixmpp-1.8.4/tests/test_xep_0454.py`

 * *Files identical despite different names*

