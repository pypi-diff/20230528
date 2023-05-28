# Comparing `tmp/parce-0.8.5.tar.gz` & `tmp/parce-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/parce-0.8.5.tar", last modified: Sat Apr 25 05:52:50 2020, max compression
+gzip compressed data, was "dist/parce-0.9.0.tar", last modified: Mon May  4 16:18:18 2020, max compression
```

## Comparing `parce-0.8.5.tar` & `parce-0.9.0.tar`

### file list

```diff
@@ -1,138 +1,157 @@
-drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-04-25 05:52:50.000000 parce-0.8.5/
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     4045 2020-04-25 05:50:29.000000 parce-0.8.5/ChangeLog
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    35366 2020-04-12 05:36:23.000000 parce-0.8.5/LICENSE
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      112 2020-04-24 18:05:20.000000 parce-0.8.5/MANIFEST.in
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     2204 2020-04-25 05:52:50.000000 parce-0.8.5/PKG-INFO
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     1455 2020-03-20 07:29:11.000000 parce-0.8.5/README.rst
-drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-04-25 05:52:50.000000 parce-0.8.5/docs/
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      871 2020-03-18 18:58:49.000000 parce-0.8.5/docs/Makefile
-drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-04-25 05:52:50.000000 parce-0.8.5/docs/source/
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)       16 2020-04-24 14:11:35.000000 parce-0.8.5/docs/source/.gitignore
-drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-04-25 05:52:50.000000 parce-0.8.5/docs/source/_static/
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      952 2020-03-28 06:50:44.000000 parce-0.8.5/docs/source/_static/custom.css
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    33571 2020-03-14 18:38:09.000000 parce-0.8.5/docs/source/_static/parce-logo.png
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      124 2020-01-24 05:40:38.000000 parce-0.8.5/docs/source/action.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     6058 2020-04-06 19:45:06.000000 parce-0.8.5/docs/source/building.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)       39 2020-03-19 14:36:22.000000 parce-0.8.5/docs/source/changelog.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     7016 2020-03-27 17:22:21.000000 parce-0.8.5/docs/source/conf.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      115 2020-02-01 19:31:48.000000 parce-0.8.5/docs/source/css.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    16370 2020-04-10 21:41:37.000000 parce-0.8.5/docs/source/deflanguage.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     5289 2020-02-14 19:42:06.000000 parce-0.8.5/docs/source/doc.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      212 2020-01-25 19:31:44.000000 parce-0.8.5/docs/source/document.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      133 2020-02-11 10:22:52.000000 parce-0.8.5/docs/source/formatter.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     7240 2020-03-19 09:18:00.000000 parce-0.8.5/docs/source/gettingstarted.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      403 2020-03-27 15:16:17.000000 parce-0.8.5/docs/source/index.rst
-drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-04-25 05:52:50.000000 parce-0.8.5/docs/source/lang/
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     2286 2020-04-25 05:46:07.000000 parce-0.8.5/docs/source/lang/css.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     7550 2020-04-25 05:46:08.000000 parce-0.8.5/docs/source/lang/html.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     2926 2020-04-25 05:46:08.000000 parce-0.8.5/docs/source/lang/ini.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    20532 2020-04-25 05:46:08.000000 parce-0.8.5/docs/source/lang/json.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     2679 2020-04-25 05:46:08.000000 parce-0.8.5/docs/source/lang/lilypond.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     3457 2020-04-25 05:46:08.000000 parce-0.8.5/docs/source/lang/python.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     3850 2020-04-25 05:46:08.000000 parce-0.8.5/docs/source/lang/scheme.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     7852 2020-04-25 05:46:08.000000 parce-0.8.5/docs/source/lang/tex.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    11277 2020-04-25 05:46:08.000000 parce-0.8.5/docs/source/lang/toml.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     8948 2020-04-25 05:46:08.000000 parce-0.8.5/docs/source/lang/xml.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      960 2020-04-25 05:46:08.000000 parce-0.8.5/docs/source/langs.inc
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      568 2020-04-10 06:47:11.000000 parce-0.8.5/docs/source/langs.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      130 2020-01-24 08:26:25.000000 parce-0.8.5/docs/source/language.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      121 2020-02-25 19:42:43.000000 parce-0.8.5/docs/source/lexer.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      127 2020-02-09 17:22:12.000000 parce-0.8.5/docs/source/lexicon.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      112 2020-04-12 05:36:23.000000 parce-0.8.5/docs/source/license.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      422 2020-04-09 05:32:52.000000 parce-0.8.5/docs/source/modoverview.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     3477 2020-03-19 14:05:36.000000 parce-0.8.5/docs/source/overview.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      124 2020-02-11 16:15:37.000000 parce-0.8.5/docs/source/parce.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      127 2020-01-24 05:40:38.000000 parce-0.8.5/docs/source/pattern.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      127 2020-01-24 08:26:38.000000 parce-0.8.5/docs/source/pkginfo.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      211 2020-02-14 09:02:48.000000 parce-0.8.5/docs/source/query.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      121 2020-02-01 19:30:59.000000 parce-0.8.5/docs/source/regex.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      130 2020-04-09 05:32:40.000000 parce-0.8.5/docs/source/registry.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      118 2020-03-02 05:41:16.000000 parce-0.8.5/docs/source/rule.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      524 2020-04-15 06:24:02.000000 parce-0.8.5/docs/source/stdactions.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      124 2020-02-25 19:42:33.000000 parce-0.8.5/docs/source/target.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      121 2020-02-05 13:17:35.000000 parce-0.8.5/docs/source/theme.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      124 2020-02-05 13:17:35.000000 parce-0.8.5/docs/source/themes.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      118 2020-01-24 08:27:05.000000 parce-0.8.5/docs/source/tree.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      139 2020-01-24 08:27:16.000000 parce-0.8.5/docs/source/treebuilder.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      151 2020-04-01 15:35:19.000000 parce-0.8.5/docs/source/treebuilderutil.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      142 2020-01-24 08:27:25.000000 parce-0.8.5/docs/source/treedocument.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    12719 2020-03-31 10:17:12.000000 parce-0.8.5/docs/source/treestructure.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      118 2020-01-25 20:38:10.000000 parce-0.8.5/docs/source/util.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      129 2020-01-24 08:27:37.000000 parce-0.8.5/docs/source/validate.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     3398 2020-04-24 17:35:45.000000 parce-0.8.5/docs/update_languages.py
-drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-04-25 05:52:50.000000 parce-0.8.5/parce/
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    17761 2020-04-18 06:17:31.000000 parce-0.8.5/parce/__init__.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     6758 2020-04-14 21:32:31.000000 parce-0.8.5/parce/action.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    37518 2020-04-15 10:06:17.000000 parce-0.8.5/parce/css.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    16121 2020-04-18 15:45:09.000000 parce-0.8.5/parce/document.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     6810 2020-04-18 18:57:39.000000 parce-0.8.5/parce/formatter.py
-drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-04-25 05:52:50.000000 parce-0.8.5/parce/lang/
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      786 2020-03-17 15:39:22.000000 parce-0.8.5/parce/lang/__init__.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     4463 2020-04-24 12:56:41.000000 parce-0.8.5/parce/lang/_registry.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     9226 2020-04-16 07:19:20.000000 parce-0.8.5/parce/lang/css.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    18293 2020-04-17 16:15:55.000000 parce-0.8.5/parce/lang/css_words.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     2981 2020-04-11 05:37:27.000000 parce-0.8.5/parce/lang/html.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     2082 2020-04-15 06:13:09.000000 parce-0.8.5/parce/lang/ini.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     2276 2020-03-19 06:23:35.000000 parce-0.8.5/parce/lang/json.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    18888 2020-04-18 16:01:52.000000 parce-0.8.5/parce/lang/lilypond.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    43382 2020-03-31 08:10:46.000000 parce-0.8.5/parce/lang/lilypond_words.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    12361 2020-04-18 10:31:55.000000 parce-0.8.5/parce/lang/python.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     3239 2020-04-13 16:03:19.000000 parce-0.8.5/parce/lang/python_words.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     3491 2020-04-18 20:47:09.000000 parce-0.8.5/parce/lang/scheme.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    29384 2020-01-27 08:04:15.000000 parce-0.8.5/parce/lang/scheme_words.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     3891 2020-04-10 05:18:58.000000 parce-0.8.5/parce/lang/tex.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     5525 2020-04-24 12:49:26.000000 parce-0.8.5/parce/lang/toml.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     6986 2020-04-17 09:37:30.000000 parce-0.8.5/parce/lang/xml.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     4491 2020-04-24 18:48:44.000000 parce-0.8.5/parce/language.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     7136 2020-03-25 12:38:40.000000 parce-0.8.5/parce/lexer.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    15044 2020-04-07 16:11:52.000000 parce-0.8.5/parce/lexicon.py
-drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-04-25 05:52:50.000000 parce-0.8.5/parce/out/
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      836 2020-02-11 14:04:35.000000 parce-0.8.5/parce/out/__init__.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     2102 2020-02-11 14:04:35.000000 parce-0.8.5/parce/out/html.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     4029 2020-03-24 08:59:05.000000 parce-0.8.5/parce/pattern.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     1562 2020-04-15 21:37:11.000000 parce-0.8.5/parce/pkginfo.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    20851 2020-04-11 15:16:03.000000 parce-0.8.5/parce/query.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    12458 2020-03-19 11:04:49.000000 parce-0.8.5/parce/regex.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     7983 2020-04-13 11:14:10.000000 parce-0.8.5/parce/registry.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     7540 2020-04-02 13:32:04.000000 parce-0.8.5/parce/rule.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     4020 2020-04-24 05:02:07.000000 parce-0.8.5/parce/stdactions.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     3186 2020-02-25 19:50:18.000000 parce-0.8.5/parce/target.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    23684 2020-04-18 18:51:08.000000 parce-0.8.5/parce/theme.py
-drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-04-25 05:52:50.000000 parce-0.8.5/parce/themes/
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     1682 2020-03-19 17:02:32.000000 parce-0.8.5/parce/themes/__init__.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     2436 2020-04-24 18:08:01.000000 parce-0.8.5/parce/themes/_template.css
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     3372 2020-04-24 18:42:54.000000 parce-0.8.5/parce/themes/dark.css
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     3578 2020-04-24 18:22:32.000000 parce-0.8.5/parce/themes/default.css
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     3162 2020-04-24 18:44:23.000000 parce-0.8.5/parce/themes/terminal.css
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    30155 2020-04-12 05:36:23.000000 parce-0.8.5/parce/tree.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    28118 2020-04-16 20:14:32.000000 parce-0.8.5/parce/treebuilder.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     8531 2020-04-12 12:23:33.000000 parce-0.8.5/parce/treebuilderutil.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     3464 2020-04-04 13:10:20.000000 parce-0.8.5/parce/treedocument.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     8445 2020-04-06 19:49:31.000000 parce-0.8.5/parce/util.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     7638 2020-04-16 13:29:09.000000 parce-0.8.5/parce/validate.py
-drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-04-25 05:52:50.000000 parce-0.8.5/parce.egg-info/
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     2204 2020-04-25 05:52:50.000000 parce-0.8.5/parce.egg-info/PKG-INFO
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     2771 2020-04-25 05:52:50.000000 parce-0.8.5/parce.egg-info/SOURCES.txt
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)        1 2020-04-25 05:52:50.000000 parce-0.8.5/parce.egg-info/dependency_links.txt
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)        6 2020-04-25 05:52:50.000000 parce-0.8.5/parce.egg-info/top_level.txt
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)       38 2020-04-25 05:52:50.000000 parce-0.8.5/setup.cfg
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     2156 2020-04-14 05:26:31.000000 parce-0.8.5/setup.py
-drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-04-25 05:52:50.000000 parce-0.8.5/tests/
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      963 2020-03-19 08:27:38.000000 parce-0.8.5/tests/__init__.py
-drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-04-25 05:52:50.000000 parce-0.8.5/tests/lang/
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      879 2020-04-24 17:46:33.000000 parce-0.8.5/tests/lang/__init__.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)       81 2020-04-24 14:01:52.000000 parce-0.8.5/tests/lang/example.css
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      286 2020-04-24 14:02:18.000000 parce-0.8.5/tests/lang/example.html
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      230 2020-04-24 14:02:47.000000 parce-0.8.5/tests/lang/example.ini
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      486 2020-04-24 14:03:20.000000 parce-0.8.5/tests/lang/example.json
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      115 2020-04-24 14:03:41.000000 parce-0.8.5/tests/lang/example.ly
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      183 2020-04-24 16:42:27.000000 parce-0.8.5/tests/lang/example.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      195 2020-04-24 14:04:07.000000 parce-0.8.5/tests/lang/example.scm
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      309 2020-04-24 14:04:24.000000 parce-0.8.5/tests/lang/example.tex
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      599 2020-04-24 14:05:00.000000 parce-0.8.5/tests/lang/example.toml
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      222 2020-04-24 14:05:38.000000 parce-0.8.5/tests/lang/example.xml
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     1090 2020-03-24 09:01:33.000000 parce-0.8.5/tests/test_all_languages.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     1591 2020-04-17 09:45:37.000000 parce-0.8.5/tests/test_css.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     1559 2020-04-24 17:42:35.000000 parce-0.8.5/tests/test_lang_examples.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     1499 2020-03-24 09:01:01.000000 parce-0.8.5/tests/test_lexicon_derivate.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     1174 2020-04-11 15:13:21.000000 parce-0.8.5/tests/test_recursion_proof.py
+drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-05-04 16:18:18.000000 parce-0.9.0/
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     4741 2020-05-04 14:31:06.000000 parce-0.9.0/ChangeLog
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    35366 2020-04-12 05:36:23.000000 parce-0.9.0/LICENSE
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      118 2020-05-04 16:15:08.000000 parce-0.9.0/MANIFEST.in
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     2200 2020-05-04 16:18:18.000000 parce-0.9.0/PKG-INFO
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     1451 2020-04-25 12:08:07.000000 parce-0.9.0/README.rst
+drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-05-04 16:18:18.000000 parce-0.9.0/docs/
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      871 2020-03-18 18:58:49.000000 parce-0.9.0/docs/Makefile
+drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-05-04 16:18:18.000000 parce-0.9.0/docs/source/
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)       16 2020-04-24 14:11:35.000000 parce-0.9.0/docs/source/.gitignore
+drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-05-04 16:18:18.000000 parce-0.9.0/docs/source/_static/
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      952 2020-03-28 06:50:44.000000 parce-0.9.0/docs/source/_static/custom.css
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    33571 2020-03-14 18:38:09.000000 parce-0.9.0/docs/source/_static/parce-logo.png
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     4286 2020-04-27 15:29:58.000000 parce-0.9.0/docs/source/_static/parce.ico
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)   305741 2020-04-27 14:10:13.000000 parce-0.9.0/docs/source/_static/parceqt.png
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      124 2020-01-24 05:40:38.000000 parce-0.9.0/docs/source/action.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     6058 2020-04-06 19:45:06.000000 parce-0.9.0/docs/source/building.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)       39 2020-03-19 14:36:22.000000 parce-0.9.0/docs/source/changelog.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     7052 2020-04-27 15:30:47.000000 parce-0.9.0/docs/source/conf.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      115 2020-02-01 19:31:48.000000 parce-0.9.0/docs/source/css.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    16356 2020-04-29 12:21:43.000000 parce-0.9.0/docs/source/deflanguage.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     5289 2020-02-14 19:42:06.000000 parce-0.9.0/docs/source/doc.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      212 2020-01-25 19:31:44.000000 parce-0.9.0/docs/source/document.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      133 2020-02-11 10:22:52.000000 parce-0.9.0/docs/source/formatter.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     7240 2020-03-19 09:18:00.000000 parce-0.9.0/docs/source/gettingstarted.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      493 2020-04-27 14:11:17.000000 parce-0.9.0/docs/source/index.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      136 2020-04-27 13:40:34.000000 parce-0.9.0/docs/source/introspect.rst
+drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-05-04 16:18:18.000000 parce-0.9.0/docs/source/lang/
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     2286 2020-05-04 11:04:00.000000 parce-0.9.0/docs/source/lang/css.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     7550 2020-05-04 11:04:00.000000 parce-0.9.0/docs/source/lang/html.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     2920 2020-05-04 11:04:00.000000 parce-0.9.0/docs/source/lang/ini.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      119 2020-05-04 11:04:00.000000 parce-0.9.0/docs/source/lang/javascript.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    20532 2020-05-04 11:04:00.000000 parce-0.9.0/docs/source/lang/json.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     2679 2020-05-04 11:04:00.000000 parce-0.9.0/docs/source/lang/lilypond.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     3457 2020-05-04 11:04:00.000000 parce-0.9.0/docs/source/lang/python.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     3850 2020-05-04 11:04:00.000000 parce-0.9.0/docs/source/lang/scheme.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     7851 2020-05-04 11:04:00.000000 parce-0.9.0/docs/source/lang/tex.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     4995 2020-05-04 11:04:00.000000 parce-0.9.0/docs/source/lang/texinfo.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    11268 2020-05-04 11:04:00.000000 parce-0.9.0/docs/source/lang/toml.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     5755 2020-05-04 11:04:00.000000 parce-0.9.0/docs/source/lang/troff.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     8945 2020-05-04 11:04:00.000000 parce-0.9.0/docs/source/lang/xml.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     1243 2020-05-04 11:04:00.000000 parce-0.9.0/docs/source/langs.inc
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      568 2020-04-10 06:47:11.000000 parce-0.9.0/docs/source/langs.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      130 2020-01-24 08:26:25.000000 parce-0.9.0/docs/source/language.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      121 2020-02-25 19:42:43.000000 parce-0.9.0/docs/source/lexer.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      158 2020-04-26 14:49:06.000000 parce-0.9.0/docs/source/lexicon.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      112 2020-04-12 05:36:23.000000 parce-0.9.0/docs/source/license.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      477 2020-05-01 13:57:48.000000 parce-0.9.0/docs/source/modoverview.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     3470 2020-04-25 12:12:31.000000 parce-0.9.0/docs/source/overview.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      124 2020-02-11 16:15:37.000000 parce-0.9.0/docs/source/parce.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      127 2020-01-24 05:40:38.000000 parce-0.9.0/docs/source/pattern.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      127 2020-01-24 08:26:38.000000 parce-0.9.0/docs/source/pkginfo.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      211 2020-02-14 09:02:48.000000 parce-0.9.0/docs/source/query.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      121 2020-02-01 19:30:59.000000 parce-0.9.0/docs/source/regex.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      130 2020-04-09 05:32:40.000000 parce-0.9.0/docs/source/registry.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      118 2020-03-02 05:41:16.000000 parce-0.9.0/docs/source/rule.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      524 2020-04-15 06:24:02.000000 parce-0.9.0/docs/source/stdactions.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      124 2020-02-25 19:42:33.000000 parce-0.9.0/docs/source/target.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      121 2020-02-05 13:17:35.000000 parce-0.9.0/docs/source/theme.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      124 2020-02-05 13:17:35.000000 parce-0.9.0/docs/source/themes.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      133 2020-05-01 13:57:40.000000 parce-0.9.0/docs/source/transform.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      118 2020-01-24 08:27:05.000000 parce-0.9.0/docs/source/tree.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      139 2020-01-24 08:27:16.000000 parce-0.9.0/docs/source/treebuilder.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      151 2020-04-01 15:35:19.000000 parce-0.9.0/docs/source/treebuilderutil.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      142 2020-01-24 08:27:25.000000 parce-0.9.0/docs/source/treedocument.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    12719 2020-03-31 10:17:12.000000 parce-0.9.0/docs/source/treestructure.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      142 2020-04-30 10:15:47.000000 parce-0.9.0/docs/source/unicharclass.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      118 2020-01-25 20:38:10.000000 parce-0.9.0/docs/source/util.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      129 2020-01-24 08:27:37.000000 parce-0.9.0/docs/source/validate.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     3398 2020-04-24 17:35:45.000000 parce-0.9.0/docs/update_languages.py
+drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-05-04 16:18:18.000000 parce-0.9.0/parce/
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    18402 2020-05-01 06:46:59.000000 parce-0.9.0/parce/__init__.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     7646 2020-04-29 20:09:16.000000 parce-0.9.0/parce/action.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    37504 2020-04-27 10:20:31.000000 parce-0.9.0/parce/css.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    16109 2020-04-27 10:23:26.000000 parce-0.9.0/parce/document.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     6810 2020-04-18 18:57:39.000000 parce-0.9.0/parce/formatter.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     2739 2020-04-27 13:35:42.000000 parce-0.9.0/parce/introspect.py
+drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-05-04 16:18:18.000000 parce-0.9.0/parce/lang/
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      786 2020-03-17 15:39:22.000000 parce-0.9.0/parce/lang/__init__.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     5463 2020-04-30 06:12:01.000000 parce-0.9.0/parce/lang/_registry.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     9226 2020-04-16 07:19:20.000000 parce-0.9.0/parce/lang/css.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    18293 2020-04-17 16:15:55.000000 parce-0.9.0/parce/lang/css_words.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     3425 2020-05-04 14:57:34.000000 parce-0.9.0/parce/lang/html.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     2082 2020-04-15 06:13:09.000000 parce-0.9.0/parce/lang/ini.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     5676 2020-05-04 14:28:12.000000 parce-0.9.0/parce/lang/javascript.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     2309 2020-04-30 06:42:40.000000 parce-0.9.0/parce/lang/javascript_words.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     4229 2020-05-02 14:27:49.000000 parce-0.9.0/parce/lang/json.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    18890 2020-04-27 13:53:32.000000 parce-0.9.0/parce/lang/lilypond.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    43382 2020-03-31 08:10:46.000000 parce-0.9.0/parce/lang/lilypond_words.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    12883 2020-04-28 20:23:44.000000 parce-0.9.0/parce/lang/python.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     3239 2020-04-13 16:03:19.000000 parce-0.9.0/parce/lang/python_words.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     3495 2020-04-27 13:54:23.000000 parce-0.9.0/parce/lang/scheme.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    29384 2020-01-27 08:04:15.000000 parce-0.9.0/parce/lang/scheme_words.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     3891 2020-04-10 05:18:58.000000 parce-0.9.0/parce/lang/tex.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     2818 2020-04-29 20:25:58.000000 parce-0.9.0/parce/lang/texinfo.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     5525 2020-04-24 12:49:26.000000 parce-0.9.0/parce/lang/toml.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     3715 2020-04-29 20:12:33.000000 parce-0.9.0/parce/lang/troff.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     7037 2020-04-25 12:32:23.000000 parce-0.9.0/parce/lang/xml.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     3175 2020-05-01 06:47:14.000000 parce-0.9.0/parce/language.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     7136 2020-04-28 10:57:54.000000 parce-0.9.0/parce/lexer.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    16268 2020-05-01 20:49:39.000000 parce-0.9.0/parce/lexicon.py
+drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-05-04 16:18:18.000000 parce-0.9.0/parce/out/
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      836 2020-02-11 14:04:35.000000 parce-0.9.0/parce/out/__init__.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     2102 2020-02-11 14:04:35.000000 parce-0.9.0/parce/out/html.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     4521 2020-04-30 08:53:11.000000 parce-0.9.0/parce/pattern.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     1562 2020-05-04 11:03:38.000000 parce-0.9.0/parce/pkginfo.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    20851 2020-04-11 15:16:03.000000 parce-0.9.0/parce/query.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    12583 2020-04-30 08:49:44.000000 parce-0.9.0/parce/regex.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     7983 2020-04-13 11:14:10.000000 parce-0.9.0/parce/registry.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     8264 2020-04-27 10:43:45.000000 parce-0.9.0/parce/rule.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     4035 2020-04-28 20:15:39.000000 parce-0.9.0/parce/stdactions.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     3186 2020-04-26 20:18:24.000000 parce-0.9.0/parce/target.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    23684 2020-04-18 18:51:08.000000 parce-0.9.0/parce/theme.py
+drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-05-04 16:18:18.000000 parce-0.9.0/parce/themes/
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     1682 2020-03-19 17:02:32.000000 parce-0.9.0/parce/themes/__init__.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     2457 2020-04-28 20:24:54.000000 parce-0.9.0/parce/themes/_template.css
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     3393 2020-04-28 20:24:51.000000 parce-0.9.0/parce/themes/dark.css
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     3599 2020-04-28 20:24:53.000000 parce-0.9.0/parce/themes/default.css
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     3183 2020-04-28 20:24:56.000000 parce-0.9.0/parce/themes/terminal.css
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     7625 2020-05-02 15:33:04.000000 parce-0.9.0/parce/transform.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    30685 2020-05-02 12:56:09.000000 parce-0.9.0/parce/tree.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    28043 2020-05-04 06:38:49.000000 parce-0.9.0/parce/treebuilder.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     8939 2020-04-28 14:27:47.000000 parce-0.9.0/parce/treebuilderutil.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     3464 2020-04-04 13:10:20.000000 parce-0.9.0/parce/treedocument.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    63795 2020-05-03 20:51:03.000000 parce-0.9.0/parce/unicharclass.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    15482 2020-05-04 13:25:24.000000 parce-0.9.0/parce/util.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     7528 2020-04-27 10:22:16.000000 parce-0.9.0/parce/validate.py
+drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-05-04 16:18:18.000000 parce-0.9.0/parce.egg-info/
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     2200 2020-05-04 16:18:18.000000 parce-0.9.0/parce.egg-info/PKG-INFO
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     3255 2020-05-04 16:18:18.000000 parce-0.9.0/parce.egg-info/SOURCES.txt
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)        1 2020-05-04 16:18:18.000000 parce-0.9.0/parce.egg-info/dependency_links.txt
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)        6 2020-05-04 16:18:18.000000 parce-0.9.0/parce.egg-info/top_level.txt
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)       38 2020-05-04 16:18:18.000000 parce-0.9.0/setup.cfg
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     2156 2020-04-14 05:26:31.000000 parce-0.9.0/setup.py
+drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-05-04 16:18:18.000000 parce-0.9.0/tests/
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      963 2020-03-19 08:27:38.000000 parce-0.9.0/tests/__init__.py
+drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-05-04 16:18:18.000000 parce-0.9.0/tests/lang/
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      879 2020-04-24 17:46:33.000000 parce-0.9.0/tests/lang/__init__.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      358 2020-04-28 15:40:52.000000 parce-0.9.0/tests/lang/example.1
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)       81 2020-04-24 14:01:52.000000 parce-0.9.0/tests/lang/example.css
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      273 2020-04-25 05:45:55.000000 parce-0.9.0/tests/lang/example.dtd
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      286 2020-04-24 14:02:18.000000 parce-0.9.0/tests/lang/example.html
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      230 2020-04-24 14:02:47.000000 parce-0.9.0/tests/lang/example.ini
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      134 2020-05-04 15:55:11.000000 parce-0.9.0/tests/lang/example.js
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      486 2020-04-24 14:03:20.000000 parce-0.9.0/tests/lang/example.json
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      115 2020-04-24 14:03:41.000000 parce-0.9.0/tests/lang/example.ly
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      183 2020-04-24 16:42:27.000000 parce-0.9.0/tests/lang/example.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      195 2020-04-24 14:04:07.000000 parce-0.9.0/tests/lang/example.scm
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      309 2020-04-24 14:04:24.000000 parce-0.9.0/tests/lang/example.tex
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      988 2020-04-29 13:48:54.000000 parce-0.9.0/tests/lang/example.texinfo
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      599 2020-04-24 14:05:00.000000 parce-0.9.0/tests/lang/example.toml
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      222 2020-04-24 14:05:38.000000 parce-0.9.0/tests/lang/example.xml
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     1090 2020-03-24 09:01:33.000000 parce-0.9.0/tests/test_all_languages.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     1591 2020-04-17 09:45:37.000000 parce-0.9.0/tests/test_css.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     1559 2020-04-24 17:42:35.000000 parce-0.9.0/tests/test_lang_examples.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     1499 2020-03-24 09:01:01.000000 parce-0.9.0/tests/test_lexicon_derivate.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     1174 2020-04-11 15:13:21.000000 parce-0.9.0/tests/test_recursion_proof.py
```

### Comparing `parce-0.8.5/ChangeLog` & `parce-0.9.0/ChangeLog`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 ChangeLog
 =========
 
 
+2020-05-04: parce-0.9.0
+
+- initial version of a transform module, that can transform a parce tree
+  to any structure you want using a Transform class, potentionally using
+  caching on contexts
+- added util.Observable, and use it in TreeBuilder to emit events
+- added unicharclass module
+- added using(), like in Pygments, it lexes a match with another lexicon
+- added JavaScript parser
+- added Python console session parser (with prompts)
+- added basic GNU Texinfo parser
+- added groff/troff parser, even includes LilyPond (as per the groff manual!)
+- fixed parsing resume when first part of a match was skipped or not used
+  (e.g. r'( )(")', bygroup(skip, String) or r' (")', bygroup(String))
+
+
 2020-04-25: parce-0.8.5
 
 - restructured standard actions, easier to combine actions
 - improved default styles, added a template for new CSS styles
 - added oldfashioned terminal CSS style (see parce/themes)
 - parce is now fully recursion proof, there is no limit on the depth of a tree
 - added toml parser
```

### Comparing `parce-0.8.5/LICENSE` & `parce-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/PKG-INFO` & `parce-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: parce
-Version: 0.8.5
+Version: 0.9.0
 Summary: The parce lexer
 Home-page: https://parce.info/
 Maintainer: Wilbert Berendsen
 Maintainer-email: info@wilbertberendsen.nl
 License: GPL
 Description: The parce module
         ================
@@ -15,20 +15,20 @@
         
         `Homepage       <https://parce.info>`_                          •
         `Development    <https://github.com/wbsoft/parce>`_             •
         `Download       <https://pypi.org/project/parce/>`_             •
         `Documentation  <https://parce.info>`_                          •
         `License        <https://www.gnu.org/licenses/gpl-3.0>`_
         
-        This Python package, `parce`, can be used for parsing text into tokens using
+        This Python package, `parce`, can be used for lexing text into tokens using
         one of the supplied language definitions in the ``lang`` directory, or
-        building your own language definitions and parse text using them.
+        building your own language definitions and lex text using them.
         
         The `parce` module is designed to be very fast, while being written in pure
-        Python, using native data structures as much as possible. Parsing can be done
+        Python, using native data structures as much as possible. Lexing can be done
         in a background thread.
         
         A powerful feature of parce is that you can retokenize only modified parts of a
         text if you already have tokenized it. This makes parce suitable for text
         editors etc. that need to keep a tokenized structure of the text up-to-date
         e.g. to support syntax highlighting as you type.
```

### Comparing `parce-0.8.5/README.rst` & `parce-0.9.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 
 `Homepage       <https://parce.info>`_                          •
 `Development    <https://github.com/wbsoft/parce>`_             •
 `Download       <https://pypi.org/project/parce/>`_             •
 `Documentation  <https://parce.info>`_                          •
 `License        <https://www.gnu.org/licenses/gpl-3.0>`_
 
-This Python package, `parce`, can be used for parsing text into tokens using
+This Python package, `parce`, can be used for lexing text into tokens using
 one of the supplied language definitions in the ``lang`` directory, or
-building your own language definitions and parse text using them.
+building your own language definitions and lex text using them.
 
 The `parce` module is designed to be very fast, while being written in pure
-Python, using native data structures as much as possible. Parsing can be done
+Python, using native data structures as much as possible. Lexing can be done
 in a background thread.
 
 A powerful feature of parce is that you can retokenize only modified parts of a
 text if you already have tokenized it. This makes parce suitable for text
 editors etc. that need to keep a tokenized structure of the text up-to-date
 e.g. to support syntax highlighting as you type.
```

### Comparing `parce-0.8.5/docs/Makefile` & `parce-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/docs/source/_static/custom.css` & `parce-0.9.0/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/docs/source/_static/parce-logo.png` & `parce-0.9.0/docs/source/_static/parce-logo.png`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/docs/source/building.rst` & `parce-0.9.0/docs/source/building.rst`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/docs/source/conf.py` & `parce-0.9.0/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,16 @@
 }
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
 
+html_favicon = "_static/parce.ico"
+
 # Custom sidebar templates, must be a dictionary that maps document names
 # to template names.
 #
 # This is required for the alabaster theme
 # refs: http://alabaster.readthedocs.io/en/latest/installation.html#sidebars
 html_sidebars = {
     '**': [
```

### Comparing `parce-0.8.5/docs/source/deflanguage.rst` & `parce-0.9.0/docs/source/deflanguage.rst`

 * *Files 4% similar despite different names*

```diff
@@ -177,19 +177,19 @@
 too difficult or cumbersome. You can also construct the regular expression in
 your lexicon code body, just before yielding it, but the advantage of a Pattern
 object is that is is only created when the lexicon is used for parsing for the
 first time.
 
 There are convenient functions for creating some types of Pattern instances:
 
-    .. autofunction:: parce.words
-        :noindex:
+.. autofunction:: parce.words
+    :noindex:
 
-    .. autofunction:: parce.char
-        :noindex:
+.. autofunction:: parce.char
+    :noindex:
 
 See for more information about Pattern objects the documentation of the
 :mod:`~parce.pattern` module.
 
 
 Dynamic actions and targets
 ---------------------------
@@ -202,50 +202,50 @@
 given itemlists (lists or tuples which can contain zero or more items).
 
 So one dynamic rule item can yield multiple items, for example an action and a
 target. Dynamic items can be nested.
 
 There are a few convenient functions to create dynamic actions and/or targets:
 
-    .. autofunction:: parce.bymatch
-        :noindex:
+.. autofunction:: parce.bymatch
+    :noindex:
 
-    .. autofunction:: parce.bytext
-        :noindex:
+.. autofunction:: parce.bytext
+    :noindex:
 
 (You might wonder why the predicate functions used by :func:`~parce.bymatch`
 and :func:`~parce.bytext` would not directly return the action or target(s).
 This is done to be able to know all actions and/or targets beforehand, and to
 be able to translate actions using a mapping before parsing, and not each time
 when parsing a document. So the actions are not hardwired even if they appear
 verbatim in the lexicon's rules.)
 
 The following functions all use the same mechanism under the hood, but they
 also create the predicate function for you:
 
-    .. autofunction:: parce.ifgroup
-        :noindex:
+.. autofunction:: parce.ifgroup
+    :noindex:
 
-    .. autofunction:: parce.ifmember
-        :noindex:
+.. autofunction:: parce.ifmember
+    :noindex:
 
-    .. autofunction:: parce.ifgroupmember
-        :noindex:
+.. autofunction:: parce.ifgroupmember
+    :noindex:
 
-    .. autofunction:: parce.maptext
-        :noindex:
+.. autofunction:: parce.maptext
+    :noindex:
 
-    .. autofunction:: parce.mapgroup
-        :noindex:
+.. autofunction:: parce.mapgroup
+    :noindex:
 
-    .. autofunction:: parce.mapmember
-        :noindex:
+.. autofunction:: parce.mapmember
+    :noindex:
 
-    .. autofunction:: parce.mapgroupmember
-        :noindex:
+.. autofunction:: parce.mapgroupmember
+    :noindex:
 
 Instead of a list or tuple of items, a single action or target item can also be
 given. These functions can also be used for mapping an action *and* target
 based on the text or match object at the same time. So instead of::
 
     predicate = lambda m: m.group() in some_list
     yield "pattern", bymatch(predicate, action1, action2), bymatch(predicate, target1, target2)
@@ -265,16 +265,22 @@
 Besides the general dynamic rule items, there is a special category of dynamic
 actions, which only create actions, and in this way influence the number of
 tokens generated from a single regular expression match.
 
 The function :func:`~parce.bygroup` can be used to yield zero or more actions,
 yielding a token for every non-empty match in a group:
 
-    .. autofunction:: parce.bygroup
-        :noindex:
+.. autofunction:: parce.bygroup
+    :noindex:
+
+The function :func:`~parce.using` can be used to lex the matched text with
+another lexicon:
+
+.. autofunction:: parce.using
+    :noindex:
 
 Finally, there exists a special :class:`~parce.action.DynamicAction` in the
 ``skip`` object, it's an instance of :class:`~parce.action.SkipAction` and it
 yields no actions, so in effect creating no tokens. Use it if you want to match
 text, but do not need the tokens. See for more information the documentation of
 the :mod:`~parce.action` module.
 
@@ -351,43 +357,43 @@
 would obfuscate the possibility to access all rule items, actions and targets
 etcetera beforehand, before parsing, which would break all language validation
 possibilities and future logic to replace items in rules before parsing.)
 
 There are two helper functions that create the Pattern based on the contents
 of the lexicon argument:
 
-    .. autofunction:: parce.arg
-        :noindex:
+.. autofunction:: parce.arg
+    :noindex:
 
-    .. autofunction:: parce.ifarg
-        :noindex:
+.. autofunction:: parce.ifarg
+    :noindex:
 
 There are three helper functions that create a target lexicon using an
 argument:
 
-    .. autofunction:: parce.withgroup
-        :noindex:
+.. autofunction:: parce.withgroup
+    :noindex:
 
-    .. autofunction:: parce.withtext
-        :noindex:
+.. autofunction:: parce.withtext
+    :noindex:
 
-    .. autofunction:: parce.witharg
-        :noindex:
+.. autofunction:: parce.witharg
+    :noindex:
 
 And there is a helper function that calls a predicate with the lexicon argument
 to choose rule items:
 
-    .. autofunction:: parce.byarg
-        :noindex:
+.. autofunction:: parce.byarg
+    :noindex:
 
 And a function that chooses rule items from a dictionary the lexicon argument
 is looked up in:
 
-    .. autofunction:: parce.maparg
-        :noindex:
+.. autofunction:: parce.maparg
+    :noindex:
 
 
 Of course it is also possible to target a lexicon with an argument directly::
 
     class MyLang(Language):
         @lexicon
         def root(cls):
```

### Comparing `parce-0.8.5/docs/source/doc.rst` & `parce-0.9.0/docs/source/doc.rst`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/docs/source/gettingstarted.rst` & `parce-0.9.0/docs/source/gettingstarted.rst`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/docs/source/lang/css.rst` & `parce-0.9.0/docs/source/lang/css.rst`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/docs/source/lang/html.rst` & `parce-0.9.0/docs/source/lang/html.rst`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/docs/source/lang/ini.rst` & `parce-0.9.0/docs/source/lang/ini.rst`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     <Context Ini.root at 0-229 (25 children)>
      ├╴<Token ';' at 0:1 (Comment)>
      ├╴<Context Ini.comment at 1-13 (1 child)>
      │  ╰╴<Token ' ini example' at 1:13 (Comment)>
      ├╴<Token ';' at 14:15 (Comment)>
      ├╴<Context Ini.comment at 15-54 (1 child)>
-     │  ╰╴<Token ' last modified 1 April 2001 '... at 15:54 (Comment)>
+     │  ╰╴<Token ' last modifi...1 by John Doe' at 15:54 (Comment)>
      ├╴<Token '[' at 55:56 (Delimiter.Section)>
      ├╴<Context Ini.section at 56-62 (2 children)>
      │  ├╴<Token 'owner' at 56:61 (Name.Namespace.Section)>
      │  ╰╴<Token ']' at 61:62 (Delimiter.Section)>
      ├╴<Context Ini.key at 63-67 (1 child)>
      │  ╰╴<Token 'name' at 63:67 (Name.Identifier)>
      ├╴<Token '=' at 67:68 (Delimiter.Operator.Assignment)>
@@ -50,15 +50,15 @@
      │  ╰╴<Token 'Acme Widgets Inc.' at 90:107 (Literal.Data)>
      ├╴<Token '[' at 109:110 (Delimiter.Section)>
      ├╴<Context Ini.section at 110-119 (2 children)>
      │  ├╴<Token 'database' at 110:118 (Name.Namespace.Section)>
      │  ╰╴<Token ']' at 118:119 (Delimiter.Section)>
      ├╴<Token ';' at 120:121 (Comment)>
      ├╴<Context Ini.comment at 121-183 (1 child)>
-     │  ╰╴<Token ' use IP address in case netw'... at 121:183 (Comment)>
+     │  ╰╴<Token ' use IP addr...s not working' at 121:183 (Comment)>
      ├╴<Context Ini.key at 184-190 (1 child)>
      │  ╰╴<Token 'server' at 184:190 (Name.Identifier)>
      ├╴<Token '=' at 190:191 (Delimiter.Operator.Assignment)>
      ├╴<Context Ini.value at 191-201 (1 child)>
      │  ╰╴<Token '192.0.2.62' at 191:201 (Literal.Data)>
      ├╴<Context Ini.key at 202-206 (1 child)>
      │  ╰╴<Token 'port' at 202:206 (Name.Identifier)>
```

### Comparing `parce-0.8.5/docs/source/lang/json.rst` & `parce-0.9.0/docs/source/lang/json.rst`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/docs/source/lang/lilypond.rst` & `parce-0.9.0/docs/source/lang/lilypond.rst`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/docs/source/lang/python.rst` & `parce-0.9.0/docs/source/lang/python.rst`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/docs/source/lang/scheme.rst` & `parce-0.9.0/docs/source/lang/scheme.rst`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/docs/source/lang/tex.rst` & `parce-0.9.0/docs/source/lang/tex.rst`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     \end{document} % End of document
 
 Result tree::
 
     <Context Latex.root at 0-309 (24 children)>
      ├╴<Token '%' at 0:1 (Comment)>
      ├╴<Context Latex.comment at 1-30 (1 child)>
-     │  ╰╴<Token ' Latex example from wikipedia' at 1:30 (Comment)>
+     │  ╰╴<Token ' Latex examp...rom wikipedia' at 1:30 (Comment)>
      ├╴<Token '\n' at 30:31 (Text)>
      ├╴<Token '\\documentclass' at 31:45 (Name.Command)>
      ├╴<Token '[' at 45:46 (Delimiter.Bracket)>
      ├╴<Context Latex.option at 46-54 (2 children)>
      │  ├╴<Token 'a4paper' at 46:53 (Pseudo)>
      │  ╰╴<Token ']' at 53:54 (Delimiter.Bracket)>
      ├╴<Token '{' at 54:55 (Delimiter.Brace)>
```

### Comparing `parce-0.8.5/docs/source/lang/toml.rst` & `parce-0.9.0/docs/source/lang/toml.rst`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 Result tree::
 
     <Context Toml.root at 0-598 (47 children)>
      ├╴<Token '#' at 0:1 (Comment)>
      ├╴<Context Toml.comment at 1-53 (2 children)>
      │  ├╴<Token ' toml example from ' at 1:20 (Comment)>
-     │  ╰╴<Token 'https://github.com/toml-lang'... at 20:53 (Comment.Url)>
+     │  ╰╴<Token 'https://gith...oml-lang/toml' at 20:53 (Comment.Url)>
      ├╴<Token '#' at 54:55 (Comment)>
      ├╴<Context Toml.comment at 55-80 (1 child)>
      │  ╰╴<Token ' This is a TOML document.' at 55:80 (Comment)>
      ├╴<Context Toml.key at 82-89 (2 children)>
      │  ├╴<Token 'title' at 82:87 (Name.Variable)>
      │  ╰╴<Token '=' at 88:89 (Delimiter.Operator.Assignment)>
      ├╴<Context Toml.value at 90-104 (2 children)>
@@ -122,15 +122,15 @@
      │  ╰╴<Token 'true' at 290:294 (Name.Constant)>
      ├╴<Token '[' at 296:297 (Delimiter.Bracket)>
      ├╴<Context Toml.table at 297-305 (2 children)>
      │  ├╴<Token 'servers' at 297:304 (Name.Variable)>
      │  ╰╴<Token ']' at 304:305 (Delimiter.Bracket)>
      ├╴<Token '#' at 309:310 (Comment)>
      ├╴<Context Toml.comment at 310-371 (1 child)>
-     │  ╰╴<Token ' Indentation (tabs and/or sp'... at 310:371 (Comment)>
+     │  ╰╴<Token ' Indentation... not required' at 310:371 (Comment)>
      ├╴<Token '[' at 374:375 (Delimiter.Bracket)>
      ├╴<Context Toml.table at 375-389 (4 children)>
      │  ├╴<Token 'servers' at 375:382 (Name.Variable)>
      │  ├╴<Token '.' at 382:383 (Delimiter.Dot)>
      │  ├╴<Token 'alpha' at 383:388 (Name.Variable)>
      │  ╰╴<Token ']' at 388:389 (Delimiter.Bracket)>
      ├╴<Context Toml.key at 392-396 (2 children)>
@@ -199,15 +199,15 @@
      │     │  ├╴<Token '1' at 517:518 (Literal.Number)>
      │     │  ├╴<Token ',' at 518:519 (Delimiter.Separator)>
      │     │  ├╴<Token '2' at 520:521 (Literal.Number)>
      │     │  ╰╴<Token ']' at 521:522 (Delimiter.Bracket)>
      │     ╰╴<Token ']' at 523:524 (Delimiter.Bracket)>
      ├╴<Token '#' at 526:527 (Comment)>
      ├╴<Context Toml.comment at 527-565 (1 child)>
-     │  ╰╴<Token ' Line breaks are OK when ins'... at 527:565 (Comment)>
+     │  ╰╴<Token ' Line breaks...inside arrays' at 527:565 (Comment)>
      ├╴<Context Toml.key at 566-573 (2 children)>
      │  ├╴<Token 'hosts' at 566:571 (Name.Variable)>
      │  ╰╴<Token '=' at 572:573 (Delimiter.Operator.Assignment)>
      ╰╴<Context Toml.value at 574-598 (2 children)>
         ├╴<Token '[' at 574:575 (Delimiter.Bracket)>
         ╰╴<Context Toml.array at 578-598 (6 children)>
            ├╴<Token '"' at 578:579 (Literal.String)>
```

### Comparing `parce-0.8.5/docs/source/lang/xml.rst` & `parce-0.9.0/docs/source/lang/xml.rst`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     >
 
 Result tree::
 
     <Context Dtd.root at 0-272 (22 children)>
      ├╴<Token '<!--' at 0:4 (Comment.Start)>
      ├╴<Context Dtd.comment at 4-41 (2 children)>
-     │  ├╴<Token ' example doctype definition '... at 4:38 (Comment)>
+     │  ├╴<Token ' example doc...nition (dtd) ' at 4:38 (Comment)>
      │  ╰╴<Token '-->' at 38:41 (Comment.End)>
      ├╴<Token '<!' at 42:44 (Delimiter)>
      ├╴<Token 'ELEMENT' at 44:51 (Keyword)>
      ├╴<Token 'book' at 52:56 (Name.Element.Definition)>
      ├╴<Context Dtd.element at 57-68 (4 children)>
      │  ├╴<Token '(' at 57:58 (Delimiter.Bracket)>
      │  ├╴<Context Dtd.element_contents at 58-66 (2 children)>
```

### Comparing `parce-0.8.5/docs/source/langs.inc` & `parce-0.9.0/docs/source/langs.inc`

 * *Files 13% similar despite different names*

```diff
@@ -13,28 +13,37 @@
 
    * - :mod:`~parce.lang.html`
      - :class:`~parce.lang.html.XHtml`, :class:`~parce.lang.html.Html`
 
    * - :mod:`~parce.lang.ini`
      - :class:`~parce.lang.ini.Ini`
 
+   * - :mod:`~parce.lang.javascript`
+     - :class:`~parce.lang.javascript.JavaScript`
+
    * - :mod:`~parce.lang.json`
      - :class:`~parce.lang.json.Json`
 
    * - :mod:`~parce.lang.lilypond`
      - :class:`~parce.lang.lilypond.LilyPond`
 
    * - :mod:`~parce.lang.python`
-     - :class:`~parce.lang.python.Python`
+     - :class:`~parce.lang.python.Python`, :class:`~parce.lang.python.PythonConsole`
 
    * - :mod:`~parce.lang.scheme`
      - :class:`~parce.lang.scheme.Scheme`, :class:`~parce.lang.scheme.SchemeLily`
 
    * - :mod:`~parce.lang.tex`
      - :class:`~parce.lang.tex.Latex`
 
+   * - :mod:`~parce.lang.texinfo`
+     - :class:`~parce.lang.texinfo.Texinfo`
+
    * - :mod:`~parce.lang.toml`
      - :class:`~parce.lang.toml.Toml`
 
+   * - :mod:`~parce.lang.troff`
+     - :class:`~parce.lang.troff.Troff`
+
    * - :mod:`~parce.lang.xml`
      - :class:`~parce.lang.xml.Xml`, :class:`~parce.lang.xml.Dtd`
```

### Comparing `parce-0.8.5/docs/source/langs.rst` & `parce-0.9.0/docs/source/langs.rst`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/docs/source/overview.rst` & `parce-0.9.0/docs/source/overview.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 Overview
 ========
 
-The `parce` module consists of a parser that can build a tree structure of
-`tokens` from a text, using regular expression patterns. Parsing happens by a
+The `parce` module consists of a lexer that can build a tree structure of
+`tokens` from a text, using regular expression patterns. Lexing happens by a
 `lexicon`, which is a set of rules with patterns to look for. Tokens can be
 given a meaning (`action`) and a rule can, if its pattern matches, also
 move parsing to another lexicon, "opening a new context", so to say.
 
 Lexicons are grouped together defining a language. Some language definitions
 are already bundled, in the ``lang`` directory. But it is also very easy to
 build your own language definitions or inherit from existing definitions and
 taylor them to your own needs. This documentation helps you going, see
 :doc:`gettingstarted`.
 
 Features
 ^^^^^^^^
 
-* parse text to a stream of `events` or a tree structure of `tokens`, according
+* lex text to a stream of `events` or a tree structure of `tokens`, according
   to a language definition
 * examine and query the generated tree structure
 * apply changes to the text, and only update the needed part of a tree
 * provides a Document (mutable string) that can be modified and that keeps
   its tokenized tree up-to-date automatically
 * parsing and tokenizing can be done in a background thread
 * map the `action` of a token to CSS classes for highlighting based on CSS
 
-You can parse a text once and examine the generated tree structure of tokens,
+You can lex a text once and examine the generated tree structure of tokens,
 but, and this is a key point of `parce`, you can also use a Document which
 keeps its text contents tokenized automatically, and if you change part of
 the text, only updates the tokens that need to, leaving the rest in place.
 
 The Document exactly tells the region that needs to be updated, and an
 application could use the type of the tokens (action) to determine the text
 format to highlight every type of text in a special way.
 
 Using some programming you can integrate Document with a structure that
 represents a text document in a GUI editor, and implement syntax highlighting
 as you type. And because the token tree stucture has very powerful search and
 query features, you can quickly provide the user with much feedback about the
 type of the text that is entered/edited.
 
-There is already a package `parceqt <https://github.com/wbsoft/parceqt>`__
+There is already a package `parceqt <https://github.com/wbsoft/parceqt>`_
 that does this for applications based on the Qt5 library (using PyQt5).
 
 A difference with a beautiful package like `pygments` is that emphasis in
 `parce` lies on live updating and interactive usage of the token tree, which
 means that parsing is always sequential. For example, it is not supported that
 first a large chunk of text is matched by one, and then tokenized by another
 lexer. But is is very easy to switch language, because lexicons are not tied to
```

### Comparing `parce-0.8.5/docs/source/stdactions.rst` & `parce-0.9.0/docs/source/stdactions.rst`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/docs/source/treestructure.rst` & `parce-0.9.0/docs/source/treestructure.rst`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/docs/update_languages.py` & `parce-0.9.0/docs/update_languages.py`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/parce/__init__.py` & `parce-0.9.0/parce/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,16 @@
 Besides the classes and functions below, a large amount of *standard actions* is
 also available in the ``parce`` module namespace. See for the full list
 :doc:`stdactions`.
 
 """
 
 
-from . import action, document, lexer, pattern, rule, treebuilder, treedocument
+from . import (
+    action, document, lexer, pattern, rule, treebuilder, treedocument, util)
 from . import lexicon as lexicon_
 from .document import Cursor
 from .language import Language
 from .pkginfo import version, version_string
 from .stdactions import *
 
 
@@ -426,14 +427,30 @@
     If this rule matches, it generates two tokens, one for "url" and the other
     for the opening parenthesis, each with their own action.
 
     """
     return action.SubgroupAction(*actions)
 
 
+def using(lexicon):
+    r"""Return a :class:`~parce.action.DelegateAction` that yields tokens
+    using the specified lexicon.
+
+    All tokens are yielded as one group, flattened, ignoring the tree
+    structure, so this is not efficient for large portions of text, as the
+    whole region is parsed again on every modification.
+
+    But it can be useful when you want to match a not too large text blob first
+    that's difficult to capture otherwise, and then lex it with a lexicon that
+    does (almost) not enter other lexicons.
+
+    """
+    return action.DelegateAction(lexicon)
+
+
 def withgroup(n, lexicon, mapping=None):
     r"""Return a :class:`~parce.rule.LexiconMatchItem` rule item that calls
     the ``lexicon`` with the matched text from group ``n``.
 
     Calling a Lexicon creates a derived Lexicon, i.e. one that has the same set
     of rules and the same name, but the patterns and/or rules may differ by
     using ArgRuleItem instances in the rule, which base their replacement
@@ -516,14 +533,14 @@
 def theme_from_file(filename):
     """Return a Theme loaded from the specified CSS filename."""
     from .theme import Theme
     return Theme(filename)
 
 
 # these can be used in rules where a pattern is expected
-default_action = object()   #: denotes a default action for unmatched text
-default_target = object()   #: denotes a default target when no text matches
+default_action = util.Symbol("default_action")   #: denotes a default action for unmatched text
+default_target = util.Symbol("default_target")   #: denotes a default target when no text matches
 
 
 #: used to suppress generating a token
 skip = action.SkipAction()
```

### Comparing `parce-0.8.5/parce/action.py` & `parce-0.9.0/parce/action.py`

 * *Files 14% similar despite different names*

```diff
@@ -203,14 +203,38 @@
 
     """
     def replace(self, lexer, pos, text, match):
         for i, action in enumerate(self.itemlists[0], match.lastindex + 1):
             yield from lexer.filter_actions(action, match.start(i), match.group(i), match)
 
 
+class DelegateAction(DynamicAction):
+    """This action uses a lexicon to parse the text.
+
+    All tokens are yielded as one group, flattened, ignoring the tree
+    structure, so this is not efficient for large portions of text, as the
+    whole region is parsed again on every modification.
+
+    But it can be useful when you want to match a not too large text blob first
+    that's difficult to capture otherwise, and then lex it with a lexicon that
+    does (almost) not enter other lexicons.
+
+    """
+    def __init__(self, lexicon):
+        super().__init__(lexicon)
+
+    def replace(self, lexer, pos, text, match):
+        """Use our lexicon to parse the matched text."""
+        lexicon = self.itemlists[0][0]
+        sublexer = type(lexer)([lexicon])
+        for e in sublexer.events(text):
+            for p, txt, action in e.tokens:
+                yield pos + p, txt, action
+
+
 class SkipAction(DynamicAction):
     """A DynamicAction that yields nothing.
 
     A SkipAction() is stored in the module variable ``skip`` and causes the rule
     to silently ignore the matched text.
 
     """
```

### Comparing `parce-0.8.5/parce/css.py` & `parce-0.9.0/parce/css.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,15 +433,15 @@
 
     """
     def __bool__(self):
         """Always return True."""
         return True
 
     def __repr__(self):
-        attrs = util.abbreviate_repr(repr(self.get_attributes()))
+        attrs = reprlib.repr(self.get_attributes())
         count = self.get_child_count()
         return "<Element {} {} ({} children)>".format(self.get_name(),
             attrs, count)
 
     def get_name(self):
         """Implement to return the element's name."""
         return ""
```

### Comparing `parce-0.8.5/parce/document.py` & `parce-0.9.0/parce/document.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,20 +35,18 @@
 For tokenized documents, parce inherits from this base class.
 
 """
 
 
 import itertools
 import re
+import reprlib
 import weakref
 
 
-from . import util
-
-
 class AbstractDocument:
     """Base class for a Document.
 
     To make a Document work, you should at least implement:
 
      *   ``text()``
      *   ``_update_contents()``
@@ -78,15 +76,15 @@
 
     def set_text(self, text):
         """Set the text."""
         assert self._edit_context == 0, "can't use set_text() in edit context."
         self[:] = text
 
     def __repr__(self):
-        text = util.abbreviate_repr(self[:31])
+        text = reprlib.repr(self.text())
         return "<{} {}>".format(type(self).__name__, text)
 
     def __str__(self):
         """Return the text."""
         return self.text()
 
     def __format__(self, formatstr):
```

### Comparing `parce-0.8.5/parce/formatter.py` & `parce-0.9.0/parce/formatter.py`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/parce/lang/__init__.py` & `parce-0.9.0/parce/lang/__init__.py`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/parce/lang/_registry.py` & `parce-0.9.0/parce/lang/_registry.py`

 * *Files 11% similar despite different names*

```diff
@@ -57,14 +57,23 @@
     desc = "INI file format",
     aliases = ["config"],
     filenames = [("*.ini", 1), ("*.cfg", 0.6), ("*.conf", 0.6)],
     mimetypes = [("text/plain", 0.1)],
     guesses = [(r'^\s*\[\w+\]', 0.5), (r"^\s*[#;]", 0.1)],
 )
 
+register("parce.lang.javascript.JavaScript.root",
+    name = "JavaScript",
+    desc = "JavaScript programming language",
+    aliases = ["js", "ecmascript"],
+    filenames = [("*.js", 1), ("*.jsm", .8)],
+    mimetypes = [("application/javascript", 1), ("application/x-javascript", 1),
+             ("text/x-javascript", 1), ("text/javascript", 1)],
+)
+
 register("parce.lang.json.Json.root",
     name = "JSON",
     desc = "JavaScript Object Notation format",
     filenames = [("*.json", 1)],
     mimetypes = [("application/json", 1)],
     guesses = [(r'^\s*\{\s*"\w+"\s*:', .7)],
 )
@@ -98,14 +107,31 @@
     name = "Python",
     desc = "Python programming language",
     filenames = [("*.py", 1)],
     mimetypes = [("text/x-python", .8)],
     guesses = [(r'^#!.{,20}python', .8), (r'\bimport\s+[a-z]+\b', .3)],
 )
 
+register("parce.lang.texinfo.Texinfo.root",
+    name = "Texinfo",
+    desc = "GNU Texinfo",
+    filenames = [("*.texi", 1), ("*.texinfo", 1), ("*.txi", .5), ("*.itexi", .3), ("*.tex", .1)],
+    mimetypes = [("application/x-texinfo", 1)],
+    guesses = [(r'^@c\b', .8), (r'^\\input\s+texinfo\b', 1)],
+)
+
+register("parce.lang.troff.Troff.root",
+    name = "Troff",
+    desc = "Troff document processing language",
+    aliases = ["groff", "nroff", "roff", "man"],
+    filenames = [("*.man", .8), ("*.[12345678]", .8)],
+    mimetypes = [("application/x-troff", .8), ("text/troff", .8)],
+    guesses = [(r'^\.', .5), (r'^\.TH\b', 1), (r'^\.\\"', 1)],
+)
+
 register("parce.lang.scheme.Scheme.root",
     name = "Scheme",
     desc = "Scheme programming language",
     aliases = ["guile"],
     filenames = [("*.scm", 1)],
     mimetypes = [("text/x-script.scheme", 1), ("text/x-script.guile", 1)],
     guesses = [(r'^\s*[;(]', .5), (r'\(define\b', .7)],
```

### Comparing `parce-0.8.5/parce/lang/css.py` & `parce-0.9.0/parce/lang/css.py`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/parce/lang/css_words.py` & `parce-0.9.0/parce/lang/css_words.py`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/parce/lang/html.py` & `parce-0.9.0/parce/lang/html.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,54 +26,63 @@
 
 import re
 
 
 from parce import *
 from parce.lang.xml import Xml
 from parce.lang.css import Css
+from parce.lang.javascript import JavaScript
 
 
 # elements that do not start a new tag context
 HTML_VOID_ELEMENTS = (
     "area", "base", "br", "col", "embed", "hr", "img", "input", "link", "meta",
     "param", "source", "track", "wbr", "command", "keygen", "menuitem",
 )
 
 
 class XHtml(Xml):
     """XHtml, is also valid Xml."""
     @lexicon(re_flags=re.IGNORECASE)
     def root(cls):
-        yield r'(<)(style)\b(>|/\s*>)?', bygroup(Delimiter, Name.Tag, Delimiter), \
-            mapgroup(3, {
-                '>': cls.css_style_tag,
-                None: cls.attrs("css"),
+        yield r'(<)(style|script)\b(>|/\s*>)?', bygroup(Delimiter, Name.Tag, Delimiter), \
+            mapgroup(2, {
+                "style": mapgroup(3, {'>': cls.css_style_tag, None: cls.attrs("css")}),
+                "script": mapgroup(3, {'>': cls.script_tag, None: cls.attrs("js")}),
             })  # by default a close tag, stay in the context.
         yield from super().root
 
     @lexicon
     def attrs(cls):
         """Reimplemented to recognize style attributes and switch to style tag."""
         yield r'(style)\s*(=)\s*(")', bygroup(Name.Attribute, Operator, String), \
             cls.css_style_attribute
         yield r'>', Delimiter, -1, maparg({
-            "css": cls.css_style_tag, None: cls.tag})
+            "js": cls.script_tag,
+            "css": cls.css_style_tag,
+            None: cls.tag})
         yield from super().attrs
 
     @lexicon
+    def script_tag(cls):
+        """Stuff between <script> and </script>."""
+        yield r'(<\s*/)\s*(script)\s*(>)', bygroup(Delimiter, Name.Tag, Delimiter), -1
+        yield from JavaScript.root
+
+    @lexicon
     def css_style_tag(cls):
         """Stuff between <style> and </style>."""
         yield r'(<\s*/)\s*(style)\s*(>)', bygroup(Delimiter, Name.Tag, Delimiter), -1
         yield from Css.root
 
     @lexicon
     def css_style_attribute(cls):
         """Stuff inside style=" ... " attrbute."""
-        yield r'"', String, -1
-        yield from Css.inline
+        yield r'([^"]*)(")', bygroup(using(Css.inline), String), -1
+        yield default_target, -1
 
 
 class Html(XHtml):
     """Html, allows certain tags (void elements) not to be closed."""
     @lexicon(re_flags=re.IGNORECASE)
     def root(cls):
         yield words(HTML_VOID_ELEMENTS, prefix=r'(<\s*?/)\s*((?:\w+:)?', suffix=r')\s*(>)'), \
```

### Comparing `parce-0.8.5/parce/lang/ini.py` & `parce-0.9.0/parce/lang/ini.py`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/parce/lang/lilypond.py` & `parce-0.9.0/parce/lang/lilypond.py`

 * *Files 1% similar despite different names*

```diff
@@ -498,15 +498,15 @@
     def get_scheme_target(cls):
         from .scheme import SchemeLily
         return SchemeLily.one_arg
 
     @lexicon
     def schemelily(cls):
         """LilyPond from scheme.SchemeLily #{ #}."""
-        yield r"#}", Delimiter.LilyPond, -1
+        yield r"#}", Bracket.LilyPond.End, -1
         yield from cls.root()
 
     # -------------- String ---------------------
     @lexicon
     def string(cls):
         yield r'"', String, -1
         yield from cls.string_common()
```

### Comparing `parce-0.8.5/parce/lang/lilypond_words.py` & `parce-0.9.0/parce/lang/lilypond_words.py`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/parce/lang/python.py` & `parce-0.9.0/parce/lang/python.py`

 * *Files 3% similar despite different names*

```diff
@@ -336,14 +336,32 @@
     ## ------- comments -------------
     @lexicon(re_flags=re.MULTILINE)
     def comment(cls):
         yield from cls.comment_common()
         yield r'$', Comment, -1
 
 
+class PythonConsole(Python):
+    """Python console input and output with prompt."""
+    @classmethod
+    def common(cls):
+        yield r'(?:(?<=\n)|^)(?:>>>|\.\.\.) ', Literal.Prompt
+        yield from super().common()
+
+    @classmethod
+    def longstring_common(cls):
+        yield r'(?:(?<=\n)|^)\.\.\. ', Literal.Prompt
+        yield from super().longstring_common()
+
+    @classmethod
+    def longbytes_common(cls):
+        yield r'(?:(?<=\n)|^)\.\.\. ', Literal.Prompt
+        yield from super().longbytes_common()
+
+
 def isclassname(text):
     """Return True is text is an uppercased name (skipping starting underscores)."""
     for c in text:
         if c.isupper():
             return True
         elif c is not '_':
             return False
```

### Comparing `parce-0.8.5/parce/lang/python_words.py` & `parce-0.9.0/parce/lang/python_words.py`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/parce/lang/scheme.py` & `parce-0.9.0/parce/lang/scheme.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,10 +104,10 @@
         yield r'\s+', skip
         yield from cls.common(-1)
         yield default_target, -1
 
     @classmethod
     def common(cls, pop=0):
         from . import lilypond
-        yield r"#{", Delimiter.LilyPond, pop, lilypond.LilyPond.schemelily
+        yield r"#{", Bracket.LilyPond.Start, pop, lilypond.LilyPond.schemelily
         yield from super().common(pop)
```

### Comparing `parce-0.8.5/parce/lang/scheme_words.py` & `parce-0.9.0/parce/lang/scheme_words.py`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/parce/lang/tex.py` & `parce-0.9.0/parce/lang/tex.py`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/parce/lang/toml.py` & `parce-0.9.0/parce/lang/toml.py`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/parce/lang/xml.py` & `parce-0.9.0/parce/lang/xml.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     '\xF8-\u02FF\u0370-\u037D\u037F-\u1FFF'
     '\u200C\u200D\u2070-\u218F\u2C00-\u2FEF'
     '\u3001-\uD7FF\uF900-\uFDCF\uFDF0-\uFFFD'
     '\U00010000-\U000EFFFF'
 )
 RE_XML_NAME_CHAR = '-.0-9\xB7\u0300-\u036F\u203F-\u2040' + RE_XML_NAME_START_CHAR
 RE_XML_NAME = _N_ = fr'[{RE_XML_NAME_START_CHAR}][{RE_XML_NAME_CHAR}]*'
-
+RE_XML_NAME_TOKEN = _T_ = fr'[{RE_XML_NAME_CHAR}]*'
 
 class _XmlBase(Language):
     """Common stuff between Xml and Dtd."""
     @lexicon
     def dqstring(cls):
         yield r'&\S*?;', String.Escape
         yield default_action, String.Double
@@ -201,9 +201,9 @@
         ``operators`` is the regexp for the operators, ``nametype`` the action
         for the found names.
 
         """
         yield r'\(', Bracket, 1
         yield r'\)', Bracket, -1
         yield operators, Operator
-        yield _N_, nametype
+        yield _T_, nametype
         yield from cls.common_defs()
```

### Comparing `parce-0.8.5/parce/language.py` & `parce-0.9.0/parce/language.py`

 * *Files 26% similar despite different names*

```diff
@@ -28,17 +28,14 @@
 
 import importlib
 import glob
 import os
 
 import parce
 import parce.lang
-from parce.action import StandardAction
-from parce.rule import DynamicItem
-from parce.lexicon import LexiconDescriptor, Lexicon
 
 
 class Language:
     """A Language represents a set of Lexicons comprising a specific language.
 
     A Language is never instantiated. The class itself serves as a namespace
     and can be inherited from.
@@ -51,63 +48,20 @@
 
         The default implementation highlight TODO, XXX and TEMP
         using Comment.Alert, and highlights URLs and email addresses with the
         Comment.Url and Comment.Email action respectively.
         Most bundled languages use this method for their comment lexicons.
 
         """
-        yield r'\b\w(?:[._%+-]?\w+)*@\w(?:[._-]?\w+)*\b', parce.Comment.Email
-        yield r'(?:https?|ftp):/(?:[\w._~:?/#-]+|\([\w._~:?/#-]*\))+', parce.Comment.Url
+        yield r'\b\w+(?:[._%+-]\w+)*@\w+(?:[._-]\w+)*\b', parce.Comment.Email
+        yield r'(?:(?:https?|ftp):/|\bwww\.)(?:[\w_~:/#-]+([.?=][\w_~:/#-]+)*|\([\w._~:?/#-]*\))+', parce.Comment.Url
         yield r"\b(ALERT|BUG|FIXME|TEMP|TODO|XXX+)\b", parce.Comment.Alert
         yield parce.default_action, parce.Comment
 
 
-def lexicons(lang):
-    """Return a list of all the lexicons on the language."""
-    lexicons = []
-    for key, value in lang.__dict__.items():
-        if isinstance(value, LexiconDescriptor):
-            lexicons.append(getattr(lang, key))
-    return lexicons
-
-
-def rule_items(lang):
-    """Yield all rule items in a language, flattening all DynamicItem instances."""
-    def flatten(items):
-        for i in items:
-            if isinstance(i, DynamicItem):
-                for l in i.itemlists:
-                    yield from flatten(l)
-            else:
-                yield i
-    for lexicon in lexicons(lang):
-        for rule in lexicon:
-            yield from flatten(rule)
-
-
-def standardactions(lang):
-    """Return the set of all the StandardAction instances in the language.
-
-    Does not follow targets to other languages.
-
-    """
-    return set(i for i in rule_items(lang) if isinstance(i, StandardAction))
-
-
-def languages(lang):
-    """Return the set of all languages that this language refers to.
-
-    Does not follow targets from languages that are referred to.
-
-    """
-    return set(i.language
-        for i in rule_items(lang)
-            if isinstance(i, Lexicon) and i.language is not lang)
-
-
 def get_all_modules():
     """Return the sorted list of module names in ``parce.lang``.
 
     Modules that start with an underscore are skipped.
 
     """
     names = []
```

### Comparing `parce-0.8.5/parce/lexer.py` & `parce-0.9.0/parce/lexer.py`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/parce/lexicon.py` & `parce-0.9.0/parce/lexicon.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,24 +28,47 @@
 
 The Lexicon can parse text according to the rules. When parsing for the first
 time, the rules-function is run with the language class as argument, and the
 rules it creates are cached.
 
 This makes it possible to inherit from a Language class and only re-implement
 some lexicons, the others keep working as in the base class.
+
+Every Lexicon has the following attributes: (they are almost never needed, but
+anyway)
+
+``arg``
+    The argument the lexicon was called with (creating a derived Lexicon).
+    None for a normal lexicon.
+``name``
+    The short name (name of the method it was defined with)
+``fullname``
+    The short name with the Language name prepended, like
+    ``'Language.lexicon'``.
+``qualname``
+    The full name with the Language's module prepended, like
+    ``'parce.lang.xml.Xml.root'``.
+``language``
+    The Language class the lexicon belongs to.
+``lexicon``
+    The LexiconDescriptor the Lexicon was created by.
+``re_flags``
+    The ``re_flags`` set by the @lexicon decorator.
+
 """
 
 import itertools
 import re
 import threading
 
 import parce.regex
-from .pattern import Pattern
+from . import util
+from .pattern import ArgPattern, Pattern
 from .target import TargetFactory
-from .rule import Item, ArgItem, DynamicItem, TextItem, variations
+from .rule import Item, ArgItem, DynamicItem, TextItem
 
 
 class LexiconDescriptor:
     """The LexiconDescriptor creates a Lexicon when called via a class."""
     __slots__ = ('rules_func', 'lexicons', '_lock', 're_flags')
 
     def __init__(self, rules_func,
@@ -88,14 +111,17 @@
     This function is created as soon as it is called for the first time.
 
     """
     def __init__(self, lexicon, language, arg=None):
         self.lexicon = lexicon
         self.language = language
         self.arg = arg
+        self.name = lexicon.rules_func.__name__
+        self.fullname = language.__name__ + '.' + self.name
+        self.qualname = language.__module__ + '.' + self.fullname
         self.__doc__ = lexicon.rules_func.__doc__
         self._derived = {}
         # lock is used when creating a derivate and/or the parse() instance function
         self._lock = threading.Lock()
 
     def __call__(self, arg=None):
         """Create a derived Lexicon with argument ``arg``.
@@ -126,38 +152,52 @@
                     lexicon = self._derived[arg] = Lexicon(self.lexicon, self.language, arg)
             return lexicon
 
     def equals(self, other):
         """Return True if we are the same lexicon or a derivate from the same."""
         return self.lexicon is other.lexicon and self.language is other.language
 
-    def __iter__(self):
-        """Yield the rules, replacing the ArgItem instances."""
+    @util.cached_property
+    def _rules(self):
+        """Yield the rules, building the patterns and replacing the ArgItem instances."""
         def replace_arg_items(items):
             """Replace ArgRuleItem instances."""
             for i in items:
                 if isinstance(i, ArgItem):
                     yield from replace_arg_items(i.replace(self.arg))
                 else:
                     if isinstance(i, Item):
                         i.itemlists = [list(replace_arg_items(l)) for l in i.itemlists]
                     yield i
-        for rule in self.lexicon.rules_func(self.language) or ():
-            yield list(replace_arg_items(rule))
+        def rules():
+            for rule in self.lexicon.rules_func(self.language) or ():
+                pattern, *rule = replace_arg_items(rule)
+                while isinstance(pattern, Pattern):
+                    if isinstance(pattern, ArgPattern):
+                        pattern = pattern.build(self.arg)
+                    else:
+                        pattern = pattern.build()
+                yield (pattern, *rule)
+        return tuple(rules())
+
+    def __iter__(self):
+        """Yield the rules.
+
+        Pattern objects are built, and the ArgItem instances replaced when this
+        method is called for the first time.
+
+        """
+        yield from self._rules
 
     def __repr__(self):
-        s = self.name()
+        s = self.fullname
         if self.arg is not None:
             s += '*'
         return s
 
-    def name(self):
-        """Return the 'Language.lexicon' name of this bound lexicon."""
-        return '.'.join((self.language.__name__, self.lexicon.rules_func.__name__))
-
     def __getattr__(self, name):
         """Create certain instance attributes when requested the first time.
 
         Calls :meth:`get_instance_attributes` to get instance attributes needed
         to use the Lexicon. Those attributes then are set in the Lexicon
         instance, so the do not need to be computed again.
 
@@ -190,16 +230,14 @@
         default_action = no_default_action
         default_target = None
 
         make_target = TargetFactory.make
 
         # make lists of pattern, action and possible targets
         for pattern, *rule in self:
-            while isinstance(pattern, Pattern):
-                pattern = pattern.build(self.arg)
             if pattern is parce.default_action:
                 default_action = rule[0]
             elif pattern is parce.default_target:
                 default_target = make_target(self, rule)
             elif rule and pattern is not None and pattern not in patterns:
                 # skip rule when the pattern is None or already seen
                 patterns.append(pattern)
@@ -231,16 +269,16 @@
                 # just quits parsing
                 def parse(text, pos):
                     yield from ()
             return parse
 
         # if there is only one pattern, and no dynamic action or target,
         # see if the pattern is simple enough to just use str.find
-        if len(patterns) == 1 and not any(isinstance(item, Item)
-                                          for item in rules[0]):
+        if len(patterns) == 1 and not self.re_flags & re.IGNORECASE and \
+                not any(isinstance(item, Item) for item in rules[0]):
             needle = parce.regex.to_string(patterns[0])
             if needle:
                 l= len(needle)
                 action, *rule = rules[0]
                 target = make_target(self, rule)
                 if dynamic_default_action:
                     def parse(text, pos):
```

### Comparing `parce-0.8.5/parce/out/__init__.py` & `parce-0.9.0/parce/out/__init__.py`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/parce/out/html.py` & `parce-0.9.0/parce/out/html.py`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/parce/pattern.py` & `parce-0.9.0/parce/pattern.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,39 +21,44 @@
 """
 Helper objects to construct regular expressions.
 
 """
 
 
 import re
+import reprlib
 
 
 class Pattern:
     """Base class for objects that build a regular expression.
 
     The ``build()`` method should return a regular pattern string, or another
-    ``Pattern`` object. The ``arg`` is the lexicon argument, which can be
-    used to customize the pattern.
+    ``Pattern`` object.
 
     If the ``build()`` method returns None, the entire rule is skipped.
 
     """
-    def build(self, arg=None):
+    def build(self):
         """Create and return the regular expression string."""
         raise NotImplementedError
 
+    def __repr__(self):
+        items = ("{}={}".format(name, reprlib.repr(value))
+                    for name, value in self.__dict__.items())
+        return "<{} {}>".format(self.__class__.__name__, ", ".join(items))
+
 
 class Words(Pattern):
     """Creates a regular expression from a list of words."""
     def __init__(self, words, prefix="", suffix=""):
         self.words = words
         self.prefix = prefix
         self.suffix = suffix
 
-    def build(self, arg=None):
+    def build(self):
         """Return an optimized regular expression string from the words list."""
         from . import regex
         expr = regex.words2regexp(self.words)
         if self.prefix or self.suffix:
             return self.prefix + '(?:' + expr + ')' + self.suffix
         return expr
 
@@ -65,22 +70,34 @@
     if it is not in the string.
 
     """
     def __init__(self, chars, positive=True):
         self.chars = chars
         self.positive = positive
 
-    def build(self, arg=None):
+    def build(self):
         """Return an optimized regular expression string for the characters."""
         from . import regex
         negate = "" if self.positive else "^"
-        return '[' + negate + regex.make_charclass(set(self.chars)) + ']'
+        return '[{}{}]'.format(negate, regex.make_charclass(self.chars))
+
+
+class ArgPattern(Pattern):
+    """Abstract Pattern subclass that uses the lexicon argument.
+
+    The :meth:`build` method has changed to accept the Lexicon argument, which
+    can be used to customize the pattern.
+
+    """
+    def build(self, arg):
+        """Create and return the regular expression string, using the lexicon argument."""
+        raise NotImplementedError
 
 
-class Arg(Pattern):
+class Arg(ArgPattern):
     r"""Creates a pattern that contains the argument the current Lexicon was
     called with.
 
     If there is no argument in the current lexicon, this Pattern yields the
     default value, which is by default None, resulting in the rule being
     skipped.
 
@@ -92,32 +109,32 @@
     """
     def __init__(self, escape=True, prefix="", suffix="", default=None):
         self.escape = escape
         self.prefix = prefix
         self.suffix = suffix
         self.default = default
 
-    def build(self, arg=None):
+    def build(self, arg):
         """Return the lexicon argument as regular expression."""
         if isinstance(arg, str):
             if self.escape:
                 arg = re.escape(arg)
             return self.prefix + arg + self.suffix
         return self.default
 
 
-class IfArg(Pattern):
+class IfArg(ArgPattern):
     r"""Pattern that returns the specified regular expression pattern (or
     nested Pattern instance) if the lexicon was called with an argument.
 
     If there is no argument in the current lexicon, ``else_pattern`` is
     yielded, which is None by default, resulting in the rule being skipped.
 
     """
     def __init__(self, pattern, else_pattern=None):
         self.pattern = pattern
         self.else_pattern = else_pattern
 
-    def build(self, arg=None):
+    def build(self, arg):
         return self.pattern if arg is not None else self.else_pattern
```

### Comparing `parce-0.8.5/parce/pkginfo.py` & `parce-0.9.0/parce/pkginfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 
 #: name of the package
 name = "parce"
 
 #: the current version
-version = Version(0, 8, 5)
+version = Version(0, 9, 0)
 version_suffix = ""
 version_string = "{}.{}.{}".format(*version) + version_suffix
 
 #: short description
 description = "The parce lexer"
 
 #: long description
```

### Comparing `parce-0.8.5/parce/query.py` & `parce-0.9.0/parce/query.py`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/parce/regex.py` & `parce-0.9.0/parce/regex.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,19 +50,24 @@
     """Return a string with adjacent characters grouped.
 
     Example::
 
         >>> parce.regex.make_charclass(('a', 'd', 'b', 'f', 'c'))
         'a-df'
 
+    Supplying a string is also supported::
+
+        >>> parce.regex.make_charclass("abcdefghjklmnop")
+        'a-hj-p'
+
     Special characters are properly escaped.
 
     """
     buf = []
-    for c in sorted(map(ord, chars)):
+    for c in sorted(map(ord, set(chars))):
         if buf and buf[-1][1] == c - 1:
             buf[-1][1] = c
         else:
             buf.append([c, c])
     return ''.join(re.escape(chr(a)) if a == b else
                    re.escape(chr(a) + chr(b)) if a == b - 1 else
                    re.escape(chr(a)) + '-' + re.escape(chr(b))
```

### Comparing `parce-0.8.5/parce/registry.py` & `parce-0.9.0/parce/registry.py`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/parce/rule.py` & `parce-0.9.0/parce/rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,25 +202,45 @@
         result = self.predicate(match)
         return self.itemlists[0][0](result),
 
 
 def variations(rule):
     """Yield lists with all possible variations on the rule.
 
-    Every DynamicItem is recursively replaced with all of its alternatives.
-    Note that DynamicAction is an ActionItem subclass, and that is not
-    unfolded.
+    Every DynamicItem and every ArgItem is recursively replaced with all of its
+    alternatives. Note that DynamicAction is an ActionItem subclass, and that
+    is not unfolded.
 
     """
     items = list(rule)
     for i, item in enumerate(items):
-        if isinstance(item, DynamicItem):
+        if isinstance(item, (DynamicItem, ArgItem)):
             prefix = items[:i]
             for suffix in variations(items[i+1:]):
                 for itemlist in item.itemlists:
                     for l in variations(itemlist):
                         yield prefix + l + suffix
             break
     else:
         yield items
 
 
+def variations_tree(rule):
+    """Return a tuple with the tree structure of all possible variations.
+
+    Unlike :func:`variations`, this function unfolds *all* Item instances.
+    Branches (choices) are indicated by a frozenset, which contains
+    one or more tuples.
+
+    A DynamicAction can be recognized as a frozenset with only one member.
+    For the SkipAction that member is an empty tuple.
+
+    """
+    items = tuple(rule)
+    for i, item in enumerate(items):
+        if isinstance(item, Item):
+            return items[:i] + (
+                    frozenset(variations_tree(l) for l in item.itemlists),
+                    *variations_tree(items[i+1:]))
+    else:
+        return items
+
```

### Comparing `parce-0.8.5/parce/stdactions.py` & `parce-0.9.0/parce/stdactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,15 @@
 Literal.Color
 Literal.Email
 Literal.Url
 Literal.Timestamp
 Literal.Input
 Literal.Output
 Literal.Error
+Literal.Prompt
 
 
 # Actions that derive of String:
 
 String.Double
 String.Single
```

### Comparing `parce-0.8.5/parce/target.py` & `parce-0.9.0/parce/target.py`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/parce/theme.py` & `parce-0.9.0/parce/theme.py`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/parce/themes/__init__.py` & `parce-0.9.0/parce/themes/__init__.py`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/parce/themes/_template.css` & `parce-0.9.0/parce/themes/_template.css`

 * *Files 1% similar despite different names*

```diff
@@ -352,14 +352,19 @@
 }
 
 .parce
 .error {
 
 }
 
+.parce
+.prompt {
+
+}
+
 /*
  * String styles
  */
 .parce
 .string.double {
 
 }
```

### Comparing `parce-0.8.5/parce/themes/dark.css` & `parce-0.9.0/parce/themes/dark.css`

 * *Files 2% similar despite different names*

```diff
@@ -359,14 +359,19 @@
 }
 
 .parce
 .error {
 
 }
 
+.parce
+.prompt {
+
+}
+
 /*
  * String styles
  */
 .parce
 .string.double {
 
 }
```

### Comparing `parce-0.8.5/parce/themes/default.css` & `parce-0.9.0/parce/themes/default.css`

 * *Files 1% similar despite different names*

```diff
@@ -365,14 +365,19 @@
 }
 
 .parce
 .error {
 
 }
 
+.parce
+.prompt {
+
+}
+
 /*
  * String styles
  */
 .parce
 .string.double {
 
 }
```

### Comparing `parce-0.8.5/parce/themes/terminal.css` & `parce-0.9.0/parce/themes/terminal.css`

 * *Files 2% similar despite different names*

```diff
@@ -362,14 +362,19 @@
 }
 
 .parce
 .error {
 
 }
 
+.parce
+.prompt {
+
+}
+
 /*
  * String styles
  */
 .parce
 .string.double {
 
 }
```

### Comparing `parce-0.8.5/parce/tree.py` & `parce-0.9.0/parce/tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 
 See also the documentation for Token and Context.
 
 """
 
 
 import itertools
+import reprlib
 
 from parce import util
 from parce import query
 from parce.lexicon import Lexicon
 
 
 DUMP_STYLES = {
@@ -392,15 +393,15 @@
             if c1 is c2:
                 return True
             elif c1.lexicon != c2.lexicon:
                 return False
         return c1.parent is None and c2.parent is None
 
     def __repr__(self):
-        text = util.abbreviate_repr(self.text[:31])
+        text = reprlib.repr(self.text)
         return "<Token {} at {}:{} ({})>".format(text, self.pos, self.end, self.action)
 
     def __eq__(self, other):
         if isinstance(other, str):
             return other == self.text
         return other is self
 
@@ -934,7 +935,25 @@
 
         """
         for token in self.backward():
             if token.group:
                 token = token.group[0]
             return token
 
+
+def make_tokens(event, parent=None):
+    """Factory returning a tuple of one or more Token instances for the event.
+
+    The event is an Event namedtuple defined in the mod:`~parce.lexer` module.
+    If the event contains more than one token, _GroupToken instances are
+    created.
+
+    """
+    if len(event.tokens) > 1:
+        tokens = tuple(_GroupToken(parent, *t) for t in event.tokens)
+        for t in tokens:
+            t.group = tokens
+        return tokens
+    else:
+        return Token(parent, *event.tokens[0]),
+
+
```

### Comparing `parce-0.8.5/parce/treebuilder.py` & `parce-0.9.0/parce/treebuilder.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,47 +41,42 @@
 while processing previous changes.
 
 The :class:`BackgroundTreeBuilder` provides an implementation using Python
 threads.
 
 """
 
-
+import operator
 import threading
 
 from parce.lexer import Lexer
-from parce.tree import Context, Token, _GroupToken
-from parce.util import tokens
+from parce.util import Observable, tokens
 from parce.target import TargetFactory
+from parce.tree import Context, make_tokens
 from parce.treebuilderutil import (
-    BuildResult, ReplaceResult, Changes, find_insert_tokens, get_lexer, new_tree)
+    BuildResult, ReplaceResult, Changes, get_prepared_lexer, new_tree)
 
 
 def build_tree(root_lexicon, text, pos=0):
     """Build and return a tree in one go."""
+    from parce.tree import Context, make_tokens # local is faster
     root = context = Context(root_lexicon, None)
     lexer = Lexer([root_lexicon])
     for e in lexer.events(text, pos):
         if e.target:
             for _ in range(e.target.pop, 0):
                 context = context.parent
             for lexicon in e.target.push:
                 context = Context(lexicon, context)
                 context.parent.append(context)
-        if len(e.tokens) > 1:
-            tokens = tuple(_GroupToken(context, *t) for t in e.tokens)
-            for t in tokens:
-                t.group = tokens
-            context.extend(tokens)
-        else:
-            context.append(Token(context, *e.tokens[0]))
+        context.extend(make_tokens(e, context))
     return root
 
 
-class TreeBuilder:
+class TreeBuilder(Observable):
     """Build a tree from parsing the text.
 
     The root node of the tree is in the ``root`` instance attribute.
     This root context is never replaced, although its lexicon may change and
     of course its children.
 
     Call :meth:`rebuild` to build or rebuild the tree. This method stores the
@@ -109,22 +104,68 @@
         If a tree was rebuilt, and old tail tokens were reused, the lexicons
         variable is not set, meaning that the old value is still valid. If the
         TreeBuilder was not used before, lexicons is an empty tuple.
 
     No other variables or state are kept, so if you don't need the above
     information anymore, you can throw away the TreeBuilder after use.
 
+    During the building process, the TreeBuilder emits certain events you can
+    subscribe to, using the :meth:`~parce.util.Observable.connect` method
+    provided by the :class:`~parce.util.Observable` class that's mixed into
+    this TreeBuilder class.
+
+    The following events are emitted, with following arguments:
+
+    ``"started"``:
+        emitted when a (re)build starts; the handler is called without
+        arguments
+
+    ``"replace"``:
+        emitted just before the tree actually changes (while the new tree is
+        being built, the tree is still unchanged and accessible, but between
+        the ``"replace"`` and ``"finished"`` events the tree is in an
+        inconsistent state)
+
+    ``"finished"``:
+        emitted when a (re)build has finished; the handler is called without
+        arguments
+
+    ``"updated"``:
+        emitted when a (re)build has finished; the handler is called with two
+        arguments: ``start``, ``end``, that denote the updated range
+
+    ``"peek"``:
+        emitted by the default implementation of the :meth:`peek` method,
+        the handler is called with two arguments: ``start``, ``tree``
+
+    ``"invalidate"``:
+        emitted by the default implementation of the :meth:`invalidate_context`
+        method, the handler is called with the Context that needs to be
+        invalidated
+
+    For example, to get notified when a build process starts::
+
+        >>> b = TreeBuilder(MyLang.root)
+        >>> def hi_there():
+        ...     print("started")
+        ...
+        >>> b.connect("started", hi_there)
+        >>> b.rebuild("some boring text")
+        started
+        >>>
+
     """
     start = 0
     end = 0
     lexicons = ()
 
     peek_threshold = 0  #: set to a value > 0 to get :meth:`peek` called during building
 
     def __init__(self, root_lexicon=None):
+        super().__init__()
         self.root = Context(root_lexicon, None)
         self.busy = False
         self.changes = []
 
     def tree(self, text):
         """Convenience method to build a tree and return the root node."""
         self.rebuild(text)
@@ -207,14 +248,16 @@
         preserved.
 
         If ``lexicons`` is None, old tail tokens after ``end`` must be reused,
         and the old list of open lexicons is still relevant. The ``offset`` then
         gives the position change for the tokens that are reused.
 
         """
+        from parce.tree import Context, make_tokens # local is faster
+
         if root_lexicon is not False:
             start, removed, added = 0, 0, len(text)
         else:
             root_lexicon = self.root.lexicon
 
         # manage end, and record if there is text after the modified part (tail)
         end = start + removed
@@ -240,35 +283,32 @@
 
         lowest_start = start
         changes = self.changes
         tree = None
         while True:
             # when restarting, see if we can reuse (part of) the new tree
             if tree:
-                tokens = find_insert_tokens(tree, text, start)
-                if tokens:
+                result = get_prepared_lexer(tree, text, start)
+                if result:
+                    lexer, events, tokens = result
                     t = tokens[0]
                     context = t.parent
-                    lexer = get_lexer(t)
-                    events = lexer.events(text, t.pos)
                     for p, i in t.ancestors_with_index():
                         del p[i+1:]
                     del context[-1]
                 else:
                     tree = None
             # find insertion spot in old tree
             if not tree:
                 start = min(lowest_start, start)
-                tokens = find_insert_tokens(self.root, text, start)
-                if tokens:
+                result = get_prepared_lexer(self.root, text, start)
+                if result:
+                    lexer, events, tokens = result
                     t = tokens[0]
                     context = new_tree(t)
-                    lexer = get_lexer(t)
-                    events = lexer.events(text, t.pos)
-                    next(events) # skip over the first token, we need its target
                     tree = context.root()
                     start = tokens[-1].end
                     lowest_start = min(lowest_start, start)
                 else:
                     tree = context = Context(root_lexicon, None)
                     lexer = Lexer([root_lexicon])
                     events = lexer.events(text)
@@ -278,20 +318,15 @@
             for e in events:
                 if e.target:
                     for _ in range(e.target.pop, 0):
                         context = context.parent
                     for lexicon in e.target.push:
                         context = Context(lexicon, context)
                         context.parent.append(context)
-                if len(e.tokens) > 1:
-                    tokens = tuple(_GroupToken(context, *t) for t in e.tokens)
-                    for t in tokens:
-                        t.group = tokens
-                else:
-                    tokens = Token(context, *e.tokens[0]),
+                tokens = make_tokens(e, context)
                 if tail:
                     # handle tail
                     pos = tokens[0].pos - offset
                     if pos > tail_pos:
                         for tail_token, tail_pos in tail_gen:
                             if tail_pos >= pos:
                                 break
@@ -355,24 +390,28 @@
         In most types of GUI applications, this method should be called in the
         main (GUI) thread.
 
         The changes are delegated to the various ``replace_`` methods, which
         can be reimplemented to get fine-grained monitoring of and control over
         the tree-replacing process.
 
+        Additionally, this method calls :meth:`invalidate_context` with the
+        youghest Context that had children removed or added.
+
         """
         tree, start, end, offset, lexicons = result
 
         if not tree.lexicon or tree.lexicon != self.root.lexicon:
             # whole tree update
             root = self.root
             for n in tree:
                 n.parent = root
             self.replace_nodes(self.root, slice(None), tree)
             self.replace_root_lexicon(tree.lexicon)
+            self.invalidate_context(self.root)
 
         else:
 
             context = self.root
             start_trail = self.root.find_token_left_with_trail(start)[1] if start else []
             end_trail = self.root.find_token_with_trail(end)[1] if lexicons is None else []
 
@@ -425,16 +464,18 @@
                     slice_end = None
                     t = t[0]
                     c = c[i]
                 i = start_trail[-1]
                 for n in t:
                     n.parent = c
                 self.replace_nodes(c, slice(i + 1, slice_end), t)
+                self.invalidate_context(c)
             else:
                 self.replace_nodes(context, slice(slice_end), tree)
+                self.invalidate_context(context)
 
             if offset:
                 for p, i in context.ancestors_with_index():
                     self.replace_pos(p, slice(i + 1, None), offset)
 
         return ReplaceResult(start, end + offset, lexicons)
 
@@ -462,26 +503,54 @@
         This method is called by :meth:`replace_tree`.
         You can reimplement this method to notify others of the change.
 
         """
         for t in tokens(context[slice_]):
             t.pos += offset
 
-    def get_root(self, wait=False, *args, **kwargs):
+    def invalidate_context(self, context):
+        """Called with the younghest Context that had children are removed or
+        added.
+
+        This means that the meaning of this context probably has changed, for
+        example when you want to transform the context to some other data
+        structure, and that the ancestors also need to be invalidated.
+
+        The default implementation of this method emits the ``invalidate``
+        event, see :meth:`~parce.util.Observable.connect`.
+
+        """
+        self.emit("invalidate", context)
+
+    def get_root(self, wait=False, callback=None, args=(), kwargs={}):
         """Return the root element of the completed tree.
 
         This is simply the ``root`` instance attribute, but this method only
         returns the tree when the ``busy`` attribute is False.
 
-        If tree building is busy, returns None or calls :meth:`wait` if
-        ``wait`` is True. The default implementation ignores the other
-        arguments.
+        If wait is True, this call blocks until tokenizing is done, and the
+        full tree is returned. If wait is False, None is returned if the tree
+        is still busy being built.
+
+        If a callback is given and tokenizing is still busy, that callback is
+        called once when tokenizing is ready. If given, args and kwargs are the
+        arguments the callback is called with, defaulting to () and {},
+        respectively.
+
+        Note that, for the lifetime of a TreeBuilder, the root element is always
+        the same. The root element is also accessible in the `root` attribute.
+        But using this method you can be sure that you are dealing with a
+        complete and fully intact tree.
 
         """
         if self.busy:
+            if callback:
+                if args or kwargs:
+                    callback = lambda: callback(*args, **kwargs)
+                self.connect("finished", callback, True)
             if not wait:
                 return
             self.wait()
         return self.root
 
     def get_changes(self):
         """Get and combine the stored change requests in a Changes object.
@@ -530,14 +599,15 @@
         self.lock(True)
         c = self.get_changes()
         while c and c.has_changes():
             self.lock(False)
             yield "build"
             result = self.build_new_tree(c.text, c.root_lexicon, c.start, c.removed, c.added)
             yield "replace"
+            self.emit("replace")
             r = self.replace_tree(result)
             start = r.start if start == -1 else min (start, r.start)
             end = r.end if end == -1 else max(c.new_position(end), r.end)
             if r.lexicons is not None:
                 lexicons = r.lexicons
             self.lock(True)
             c = self.get_changes()
@@ -579,157 +649,82 @@
 
         The tree that is given, is a copy of the current tree. It is safe to
         use it in another thread, although its contents are not valid anymore
         when the build has finished, or when a build is restarted, causing
         peek() to be called a second time. (A build is restarted when there are
         new changes close to the position the build originally started.)
 
-        The default implementation of this method does nothing; the default
-        value of the  ``peek_threshold`` attribute is 0.
+        The default implementation of this method emits the ``peek`` event, see
+        :meth:`~parce.util.Observable.connect`.
 
         """
-        pass
+        self.emit("peek", start, tree)
 
     def lock(self, acquire):
         """Acquire lock (True) or release lock (False). Does nothing by default.
 
         If you want to run the full update and replace jobs in a background
         thread, you may need locking, to prevent changes from going unnoticed.
 
         """
         pass
 
     def process_started(self):
         """Called at the start ot the tree building process.
 
-        Does nothing by default.
+        The default implementation of this method emits the ``started`` event,
+        see :meth:`~parce.util.Observable.connect`.
 
         """
-        pass
+        self.emit("started")
 
     def process_finished(self):
         """Called when tree building is done.
 
-        Does nothing by default.
+        The default implementation of this method emits the ``updated(start,
+        end)`` and ``finished`` events, see
+        :meth:`~parce.util.Observable.connect`.
 
         """
-        pass
+        self.emit("updated", self.start, self.end)
+        self.emit("finished")
 
 
 class BackgroundTreeBuilder(TreeBuilder):
     """A TreeBuilder that can tokenize a text in a Python thread.
 
     In BackgroundTreeBuilder, :meth:`rebuild()` returns immediately, because
     :meth:`start_processing()` has been reimplemented to call itself in a
     background thread.
 
     You can continue adding changes while previous changes are processed;
     the tree builder will immediately adapt to the new changes.
 
-    You can add callbacks to the ``updated_callbacks`` attribute (using
-    ``add_build_updated_callback()``) that are called everytime the whole
-    document is tokenized.
-
-    You can also add callbacks to the ``finished_callbacks`` attribute, using
-    ``add_finished_callback()``; those are called once when all pending changes
-    are processed and then forgotten again.
-
     To be sure you get a completed tree, call ``get_root(True)``.
 
     """
     def __init__(self, root_lexicon=None):
         super().__init__(root_lexicon)
         self.job = None
         self._lock = threading.Lock()
-        self.updated_callbacks = []
-        self.finished_callbacks = []
 
     def lock(self, acquire):
         """Reimplemented to actually lock/unlock."""
         self._lock.acquire() if acquire else self._lock.release()
 
     def start_processing(self):
         """Reimplemented to call start_processing in a background thread."""
         self.job = threading.Thread(target=super().start_processing)
         self.job.start()
 
-    def process_finished(self):
-        """Reimplemented to clear the job attribute and call the callbacks."""
-        self.job = None
-        for cb in self.updated_callbacks:
-            cb(self.start, self.end)
-        while self.finished_callbacks:
-            callback, args, kwargs = self.finished_callbacks.pop()
-            callback(*args, **kwargs)
-
     def wait(self):
         """Reimplemented to await our background thread if active."""
         job = self.job
         if job:
             job.join()
 
-    def get_root(self, wait=False, callback=None, args=None, kwargs=None):
-        """Get the root element of the completed tree.
-
-        If wait is True, this call blocks until tokenizing is done, and the
-        full tree is returned. If wait is False, None is returned if the tree
-        is still busy being built.
-
-        If a callback is given and tokenizing is still busy, that callback is
-        called once when tokenizing is ready. If given, args and kwargs are the
-        arguments the callback is called with, defaulting to () and {},
-        respectively.
-
-        Note that, for the lifetime of a TreeBuilder, the root element is always
-        the same. The root element is also accessible in the `root` attribute.
-        But using this method you can be sure that you are dealing with a
-        complete and fully intact tree.
-
-        """
-        if not self.job:
-            return self.root
-        if callback:
-            self.add_finished_callback(callback, args, kwargs)
-        if wait:
-            self.wait()
-            return self.root
-
-    def add_build_updated_callback(self, callback):
-        """Add a callback to be called when the whole text is tokenized.
-
-        The callback is called with two arguments (start, end) denoting
-        the range in the text that was tokenized again.
+    def process_finished(self):
+        """Reimplemented to clear the job attribute."""
+        self.job = None
+        super().process_finished()
 
-        """
-        if callback not in self.updated_callbacks:
-            self.updated_callbacks.append(callback)
-
-    def remove_build_updated_callback(self, callback):
-        """Remove a previously registered callback to be called when the whole text is tokenized."""
-        if callback in self.updated_callbacks:
-            self.updated_callbacks.remove(callback)
-
-    def add_finished_callback(self, callback, args=None, kwargs=None):
-        """Add a callback to be called when tokenizing finishes.
-
-        This callback will be called once, directly after being called
-        it will be forgotten.
-
-        """
-        if args is None:
-            args = ()
-        if kwargs is None:
-            kwargs = {}
-        cb = (callback, args, kwargs)
-        if cb not in self.finished_callbacks:
-            self.finished_callbacks.append(cb)
-
-    def remove_finished_callback(self, callback, args=None, kwargs=None):
-        """Remove a callback that was registered to be called when tokenizing finishes."""
-        if args is None:
-            args = ()
-        if kwargs is None:
-            kwargs = {}
-        cb = (callback, args, kwargs)
-        if cb in self.finished_callbacks:
-            self.finished_callbacks.remove(cb)
```

### Comparing `parce-0.8.5/parce/treebuilderutil.py` & `parce-0.9.0/parce/treebuilderutil.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 
 #: encapsulates the return values of :meth:`TreeBuilder.build_new_tree`
 BuildResult = collections.namedtuple("BuildResult", "tree start end offset lexicons")
 
 #: encapsulates the return values of :meth:`TreeBuilder.replace_tree`
 ReplaceResult = collections.namedtuple("ReplaceResult", "start end lexicons")
 
+#: encapsulates the return values of :func:`get_prepared_lexer`
+PreparedLexer = collections.namedtuple("PreparedLexer", "lexer events start")
+
 
 class Changes:
     """Store changes that have to be made to a tree.
 
     This object is used by
     :meth:`~parce.treebuilder.TreeBuilder.get_changes()`. Calling
     :meth:`add()` merges new changes with the existing changes.
@@ -111,21 +114,23 @@
         if pos < self.start:
             return pos
         elif pos < self.start + self.removed:
             return self.start + self.added
         return pos - self.removed + self.added
 
 
-def find_insert_tokens(tree, text, start):
-    """Return the token(group) after which new tokens should be inserted.
+def get_prepared_lexer(tree, text, start):
+    """Get a prepared lexer reading from text, positioned at (or before) start.
 
-    Normally this is the last complete tokengroup just before the start
-    position; but in certain cases this can be earlier in the text.
+    Returns the three-tuple (lexer, events, tokens). The events stream is
+    returned seperately because the last Event can be pushed back, so it is
+    yielded again. The tokens are the last tokens group that remained the same.
 
-    If this function returns None, you should start at the beginning.
+    Returns None when no position to start can be found, just start from the
+    beginning in this case.
 
     """
     while start:
         last_token = start_token = find_token_before(tree, start)
         while last_token and last_token.group and last_token.group[-1].end > start:
             last_token = last_token.group[0].previous_token()
         if not last_token:
@@ -141,18 +146,21 @@
         events = lexer.events(text, start)
         # compare the new events with the old tokens; at least one
         # should be the same; if not, go back further if possible
         old_events = events_with_tokens(start_token, last_token)
         prev = None
         for (old, tokens), new in zip(old_events, events):
             if old != new:
+                if prev:
+                    return lexer, itertools.chain((new,), events), prev
                 break
             prev = tokens
-        if prev:
-            return prev
+        else:
+            if prev:
+                return lexer, events, prev
 
 
 def events_with_tokens(start_token, last_token):
     r"""Yield (Event, tokens) tuples for start_token until and including last_token.
 
     Events are yielded together with token groups (or single tokens in a
     1-length tuple).
```

### Comparing `parce-0.8.5/parce/treedocument.py` & `parce-0.9.0/parce/treedocument.py`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/parce/validate.py` & `parce-0.9.0/parce/validate.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
 import collections
 import re
+import reprlib
 
 import parce
 from .lexicon import LexiconDescriptor, Lexicon
 from .pattern import Pattern
 from .rule import Item, variations
-from . import util
 
 
 def validate_language(lang):
     """Validate all lexicons in this language.
 
     Errors and warnings are printed to stdout. If there are errors,
     this function returns False, otherwise True.
@@ -99,22 +99,20 @@
             elif pattern is parce.default_target:
                 if default_tg:
                     self.error("rule #{}: conflicting default targets".format(n))
                 else:
                     default_tg = rule
                     self.check_default_target(default_tg)
             else:
-                while isinstance(pattern, Pattern):
-                    pattern = pattern.build()
                 if pattern is None:
                     self.warning("rule #{}: pattern is None; rule will be skipped".format(n))
                 else:
                     self.validate_pattern(pattern, n)
                     if pattern in patterns:
-                        self.warning("rule #{0}: repeated pattern {1}; will be skipped".format(n, util.abbreviate_repr(pattern)))
+                        self.warning("rule #{0}: repeated pattern {1}; will be skipped".format(n, reprlib.repr(pattern)))
                     patterns.add(pattern)
                 self.validate_rule(rule, n)
 
         if default_act and default_tg:
             self.error("can't have both default_action and default_target")
         return not self.errors
```

### Comparing `parce-0.8.5/parce.egg-info/PKG-INFO` & `parce-0.9.0/parce.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: parce
-Version: 0.8.5
+Version: 0.9.0
 Summary: The parce lexer
 Home-page: https://parce.info/
 Maintainer: Wilbert Berendsen
 Maintainer-email: info@wilbertberendsen.nl
 License: GPL
 Description: The parce module
         ================
@@ -15,20 +15,20 @@
         
         `Homepage       <https://parce.info>`_                          •
         `Development    <https://github.com/wbsoft/parce>`_             •
         `Download       <https://pypi.org/project/parce/>`_             •
         `Documentation  <https://parce.info>`_                          •
         `License        <https://www.gnu.org/licenses/gpl-3.0>`_
         
-        This Python package, `parce`, can be used for parsing text into tokens using
+        This Python package, `parce`, can be used for lexing text into tokens using
         one of the supplied language definitions in the ``lang`` directory, or
-        building your own language definitions and parse text using them.
+        building your own language definitions and lex text using them.
         
         The `parce` module is designed to be very fast, while being written in pure
-        Python, using native data structures as much as possible. Parsing can be done
+        Python, using native data structures as much as possible. Lexing can be done
         in a background thread.
         
         A powerful feature of parce is that you can retokenize only modified parts of a
         text if you already have tokenized it. This makes parce suitable for text
         editors etc. that need to keep a tokenized structure of the text up-to-date
         e.g. to support syntax highlighting as you type.
```

### Comparing `parce-0.8.5/parce.egg-info/SOURCES.txt` & `parce-0.9.0/parce.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 docs/source/css.rst
 docs/source/deflanguage.rst
 docs/source/doc.rst
 docs/source/document.rst
 docs/source/formatter.rst
 docs/source/gettingstarted.rst
 docs/source/index.rst
+docs/source/introspect.rst
 docs/source/langs.inc
 docs/source/langs.rst
 docs/source/language.rst
 docs/source/lexer.rst
 docs/source/lexicon.rst
 docs/source/license.rst
 docs/source/modoverview.rst
@@ -32,75 +33,89 @@
 docs/source/regex.rst
 docs/source/registry.rst
 docs/source/rule.rst
 docs/source/stdactions.rst
 docs/source/target.rst
 docs/source/theme.rst
 docs/source/themes.rst
+docs/source/transform.rst
 docs/source/tree.rst
 docs/source/treebuilder.rst
 docs/source/treebuilderutil.rst
 docs/source/treedocument.rst
 docs/source/treestructure.rst
+docs/source/unicharclass.rst
 docs/source/util.rst
 docs/source/validate.rst
 docs/source/_static/custom.css
 docs/source/_static/parce-logo.png
+docs/source/_static/parce.ico
+docs/source/_static/parceqt.png
 docs/source/lang/css.rst
 docs/source/lang/html.rst
 docs/source/lang/ini.rst
+docs/source/lang/javascript.rst
 docs/source/lang/json.rst
 docs/source/lang/lilypond.rst
 docs/source/lang/python.rst
 docs/source/lang/scheme.rst
 docs/source/lang/tex.rst
+docs/source/lang/texinfo.rst
 docs/source/lang/toml.rst
+docs/source/lang/troff.rst
 docs/source/lang/xml.rst
 parce/__init__.py
 parce/action.py
 parce/css.py
 parce/document.py
 parce/formatter.py
+parce/introspect.py
 parce/language.py
 parce/lexer.py
 parce/lexicon.py
 parce/pattern.py
 parce/pkginfo.py
 parce/query.py
 parce/regex.py
 parce/registry.py
 parce/rule.py
 parce/stdactions.py
 parce/target.py
 parce/theme.py
+parce/transform.py
 parce/tree.py
 parce/treebuilder.py
 parce/treebuilderutil.py
 parce/treedocument.py
+parce/unicharclass.py
 parce/util.py
 parce/validate.py
 parce.egg-info/PKG-INFO
 parce.egg-info/SOURCES.txt
 parce.egg-info/dependency_links.txt
 parce.egg-info/top_level.txt
 parce/lang/__init__.py
 parce/lang/_registry.py
 parce/lang/css.py
 parce/lang/css_words.py
 parce/lang/html.py
 parce/lang/ini.py
+parce/lang/javascript.py
+parce/lang/javascript_words.py
 parce/lang/json.py
 parce/lang/lilypond.py
 parce/lang/lilypond_words.py
 parce/lang/python.py
 parce/lang/python_words.py
 parce/lang/scheme.py
 parce/lang/scheme_words.py
 parce/lang/tex.py
+parce/lang/texinfo.py
 parce/lang/toml.py
+parce/lang/troff.py
 parce/lang/xml.py
 parce/out/__init__.py
 parce/out/html.py
 parce/themes/__init__.py
 parce/themes/_template.css
 parce/themes/dark.css
 parce/themes/default.css
@@ -108,17 +123,21 @@
 tests/__init__.py
 tests/test_all_languages.py
 tests/test_css.py
 tests/test_lang_examples.py
 tests/test_lexicon_derivate.py
 tests/test_recursion_proof.py
 tests/lang/__init__.py
+tests/lang/example.1
 tests/lang/example.css
+tests/lang/example.dtd
 tests/lang/example.html
 tests/lang/example.ini
+tests/lang/example.js
 tests/lang/example.json
 tests/lang/example.ly
 tests/lang/example.py
 tests/lang/example.scm
 tests/lang/example.tex
+tests/lang/example.texinfo
 tests/lang/example.toml
 tests/lang/example.xml
```

### Comparing `parce-0.8.5/setup.py` & `parce-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/tests/__init__.py` & `parce-0.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/tests/lang/__init__.py` & `parce-0.9.0/tests/lang/__init__.py`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/tests/lang/example.toml` & `parce-0.9.0/tests/lang/example.toml`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/tests/test_all_languages.py` & `parce-0.9.0/tests/test_all_languages.py`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/tests/test_css.py` & `parce-0.9.0/tests/test_css.py`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/tests/test_lang_examples.py` & `parce-0.9.0/tests/test_lang_examples.py`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/tests/test_lexicon_derivate.py` & `parce-0.9.0/tests/test_lexicon_derivate.py`

 * *Files identical despite different names*

### Comparing `parce-0.8.5/tests/test_recursion_proof.py` & `parce-0.9.0/tests/test_recursion_proof.py`

 * *Files identical despite different names*

